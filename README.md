#include <iostream>
using namespace std;
class Time
{	private:
		int hour;
		int minute;
		int second;
	public:
		void print()
	{
			cout << "время" << endl;
			cout << "(" <<this->hour << ":"<<this->minute<<":"<< this->second<<")"<<endl;
	}
	void setHour(int hour)
	{
		this->hour = hour;
	}
	void setMinute(int minute)
	{
		this->minute = minute;
	}
	void setSecond(int second)
	{
		this->second = second;
	}
	int getHour( )	{	return hour; }
	int getMinute( )	{	return minute; }
	int getSecond( )	{	return second; }
};

int main()
{
	Time	sunset;
	sunset.setHour(12);
	sunset.setMinute(59);
	sunset.setSecond(23);
	sunset.print();
}
