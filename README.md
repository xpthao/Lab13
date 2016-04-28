# Lab13
Assignment 13 

#include <iostream>
#include <string>
using namespace std;

class BlogEntry
{
private:

	string entryTxt;
		string date;
			string username;
				int userID;

				public:
					

						BlogEntry();
							BlogEntry(string txt, string d, string un, int uID);

								
									void setEntryTxt(string txt)
										{
												entryTxt = txt;
													}

														void setDate(string d)
															{
																	date = d;
																		}

																			void setUserName(string un)
																				{
																						username = un;
																							}

																								void setUserID(int uid)
																									{
																											userID = uid;
																												}




																													string getEntryText()
																														{
																																return entryTxt;
																																	}

																																		string getDate()
																																			{
																																					return date;
																																						}

																																							string getUsername()
																																								{
																																										return username;
																																											}

																																												int getuserID()
																																													{
																																															return userID;
																																																}

																																																	string getInfo()
																																																		{
																																																				string temID = userID + " "; 
																																																						string info = "UserID " + temID + "Entry Text: " + entryTxt + "Date: " + date + "User Name: " + username;
																																																								return info;
																																																									}
																																																									};

																																																									int main()

																																																									{

																																																										BlogEntry listOfBlogsEntries[4];
																																																											string tempTextEntry, tempDate, tempUserName;
																																																												int tempUserID;

																																																													for (int i = 0; i < 2; i++)
																																																														{
																																																																cout << "Enter TextEntry: ";
																																																																		getline(cin, tempTextEntry);
																																																																				cout << "Enter Date: ";
																																																																						getline(cin, tempDate);
																																																																								cout << "Enter userName: ";
																																																																										getline(cin, tempUserName);
																																																																												cout << "Enter UserID: ";
																																																																														cin >> tempUserID;
																																																																																cout << endl;

																																																																																		cin.ignore();


																																																																																				listOfBlogsEntries[i].setEntryTxt(tempTextEntry);
																																																																																						listOfBlogsEntries[i].setDate(tempDate);
																																																																																								listOfBlogsEntries[i].setUserName(tempUserName);
																																																																																										listOfBlogsEntries[i].setUserID(tempUserID);

																																																																																											}


																																																																																												for (int count = 0; count < 4; count++)
																																																																																													{
																																																																																															cout << listOfBlogsEntries[count].getInfo() << endl;
																																																																																																}

																																																																																																}

