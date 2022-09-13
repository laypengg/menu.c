
#include<stdlib.h>
#pragma warning(disable:4996)
#define A001_ 165.00
#define A002_ 125.00
#define A003_ 144.00
#define B001_ 110.00
#define B002_ 125.00
#define B003_ 144.00
#define C001_ 163.00
#define C002_ 89.00
#define C003_ 112.00

int menuBookfield();
int menuWeb();
int menuSoftware();
int menuMobile();
void menuOrderbook();
int booklist();
int bookselect();
int quantity();

void main()
{
	int option;

	do {
		printf("=====Menu=====\n");
		printf("Select an option > \n");
		printf("1.Book field\n");
		printf("2.Order Book\n");
		printf("0.Exit from program\n");
		printf("Select an option --> \n");
		scanf_s("%d",&option);

		switch (option) {
		case 1:menuBookfield(); break;
		case 2:menuOrderbook(); break;
		case 0:break;
		default:printf("Invalid option!\n");
		}
	} while (option != 0);
	return option;
}
int menuBookfield()
{
	int choice;
	do {
		printf("=====Select a field to view=====\n");
		printf("||1.Web Programming Field      ||\n");
		printf("||2.Software Programming Field ||\n");
		printf("||3.Mobile Programming Field   ||\n");
		printf("||0.Return to Menu             ||\n");
		printf("=====Enter your choice --> =====\n");
		scanf_s("%d", &choice);

		switch (choice) {
		case 1:menuWeb(); break;
		case 2:menuSoftware(); break;
		case 3:menuMobile(); break;
		case 0:break;
		default:printf("Invalid choice! Please enter 1-2 or 3\n");
		}
	} while (choice != 0);
	return choice;
}
int menuWeb()
{
	int web;
	do {
		printf("1.Web Design with HTML, CSS, JavaScript and jQuery Set --> RM165.00\n");
		printf("2.Full Stack web development For Beginners --> RM125.00");
		printf("3.Learning Web App Development --> RM144.00\n");
		printf("0.Return to Menu\n");
		printf("Enter your choice --> \n");
		printf("%d", &web);

		switch (web) {
		case 1:printf("A two-book set for web design and development by learning the structure of a web by using HTML, step-by-step guide to design your own website using CSS and use Javasript to determine how your website works suitable for beginners to start their journey and master to become a web developer.\n"); break;
		case 2:printf("A book written for beginners who wants to become a full stack developer that  contains HTML5, CSS, JavaScript, Bootstrap, PHP including professional knowledge, guides and examples .\n"); break;
		case 3:printf("Here's the intro\n"); break;
		case 0:break;
		default:printf("Invalid Choice! Please enter by select 1-2 or 3\n");
		}
	} while (web != 0);
	return web;
}
int menuSoftware()
{
	int software;
	do {
		printf("4.The Digital Guide To Software Development by Misc, 1990 --> RM110.00\n");
		printf("5.Full Stack web development For Beginners --> RM125.00");
		printf("6.Learning Web App Development --> RM144.00\n");
		printf("0.Return to Menu\n");
		printf("Enter your choice --> \n");
		printf("%d", &software);

		switch (software) {
		case 1:printf("A two-book set for web design and development by learning the structure of a web by using HTML, step-by-step guide to design your own website using CSS and use Javasript to determine how your website works suitable for beginners to start their journey and master to become a web developer.\n"); break;
		case 2:printf("A book written for beginners who wants to become a full stack developer that  contains HTML5, CSS, JavaScript, Bootstrap, PHP including professional knowledge, guides and examples .\n"); break;
		case 3:printf("Here's the intro\n"); break;
		case 0:break;
		default:printf("Invalid Choice! Please enter by select 1-2 or 3\n");
		}
	} while (software != 0);
	return software;
}
int menuMobile() {
	int mobile;
	do {
		printf("7.Designing Mobile Interfaces --> RM163.00\n");
		printf("8.Android App Development For Dummies --> RM89.00");
		printf("9.Mobile Design and Development --> RM112.00\n");
		printf("0.Return to Menu\n");
		printf("Enter your choice --> \n");
		printf("%d", &mobile);

		switch (mobile) {
		case 1:printf("A two-book set for web design and development by learning the structure of a web by using HTML, step-by-step guide to design your own website using CSS and use Javasript to determine how your website works suitable for beginners to start their journey and master to become a web developer.\n"); break;
		case 2:printf("A book written for beginners who wants to become a full stack developer that  contains HTML5, CSS, JavaScript, Bootstrap, PHP including professional knowledge, guides and examples .\n"); break;
		case 3:printf("Here's the intro\n"); break;
		case 0:break;
		default:printf("Invalid Choice! Please enter by select 1-2 or 3\n");
		}
	} while (mobile != 0);
	return mobile;
}
