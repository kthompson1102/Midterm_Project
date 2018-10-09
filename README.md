# Midterm_Project
#include <iostream>
#include <string>
#include <iomanip>
using namespace std;

void createSchools();
void outOfState();
void projSalary();
void recomYears();
void testScores();
void acceptRate();


struct College{
 string name;
 string major1, major2, major3, major4, major5, major6, major7, major8, major9, major10;
 double istate_tuition;
 double ostate_tuition;
 double proj_salary;
 int recom_years;
 int ssat, esat, sact, eact;
 int acceptance;
 string campusLife;
};
const int MAX = 10;
College list[MAX];

int main() {
 createSchools();
 cout << "Name:\t\t\t Instate Tuition:\t Campus Life:\t" << endl;
 for(int i = 0; i < MAX; i++){
  cout << setw(0) << list[i].name << "\t\t\t" << list[i].istate_tuition << setw(20) << list[i].campusLife << endl;
 }
 string more_info;
 cout << "Would you like any other information on the schools?"<< endl;
 getline(cin,more_info);
 while (more_info != "no"){
  if (more_info = "out of state tuition"){
  outOfState();
  }
  if (more_info = "projected salary") {
  
 }
}

void createSchools(){
 College Spelman = {"Spelman College", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 28181, 28181, 46800, 4, 980, 1170, 22, 26, 36, "A-"};
 list[0] = Spelman;
 College MorganState = {"Morgan State University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 7766, 17832, 39200, 4, 810, 990, 16, 20, 60, "B-"};
 list[1] = MorganState;
 College Howard = {"Howard University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 24122, 24122, 46800, 4, 1040, 1240, 22, 28, 30, "B+"};
 list[2] = Howard;
 College Hampton = {"Hampton University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 25441, 25441, 41700, 4, 860, 1040, 19, 24, 65, "B-"};
 list[3] = Hampton;
 College Tuskeegee = {"Tuskeegee University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 22170, 22170, 35300, 4, 890, 1110, 21, 22, 50, "B-"};
 list[4] = Tuskeegee;
 College Morehouse = {"Morehouse College", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 27278, 27278, 42500, 4, 860, 1095, 19, 24, 66, "B"};
 list[5] = Morehouse;
 College Xavier = {"Xavier University of Louisianna", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 23606, 23606, 47900, 4, 890, 1110, 20, 26, 62, "B+"};
 list[6] = Xavier;
 College FloridaAM = {"Florida A&M University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 5785, 17725, 35800, 4, 900, 1080, 19, 24, 31, "B+"};
 list[7] = FloridaAM;
 College NorthCarolinaCentr = {"North Carolina Central University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 6399, 19106, 32200, 4, 810, 940, 17, 19, 67, "B-"};
 list[8] = NorthCarolinaCentr;
 College NorthCarolinaAT = {"North Carolina A&T State University", "Social Sciences", "Psychology", "Biological and Biomedical Sciences", "English", "Math and Statistics", "Engineering", "Health Professions", "Business", "Visual and Performing Arts", "Protective Services, Linguistics", 6526, 19416, 33100, 4, 850, 1010, 18, 22, 54, "B"};
 list[9] = NorthCarolinaAT;

}

void outOfState(){
for(int i = 0; i < 10; i++){
   cout << setw(0) << list[i].name << "\t\t\t $" << list[i].ostate_tuition << setw(20) << endl;
   }  
}

void projSalary(){
for(int i = 0; i < 10; i++){
   cout << setw(0) << list[i].name << "\t\t\t $" << list[i].proj_salary << setw(20) << endl;
   }  
}

void recomYears(){
for(int i = 0; i < 10; i++){
   cout << setw(0) << list[i].name << "\t\t\t" << list[i].recom_years << setw(20) << endl;
   }  
}

void testScores(){
for(int i = 0; i < 10; i++){
   cout << setw(0) << list[i].name << "\t\t\t SAT:" << list[i].ssat<< "-" << list[i].esat << "  ACT:" << list[i].sact << "-" << list[i].eact << setw(20) << endl;
   }  
}

void acceptRate(){
for(int i = 0; i < 10; i++){
   cout << setw(0) << list[i].name << "\t\t\t" << list[i].acceptance << "%" << setw(20) << endl;
   }  
}
