#include <stdio.h>
#include <stdlib.h>
#include <string.h>

const int NUMBER_OF_GRADES = 9;
const int SCORES[NUMBER_OF_GRADES] = {95, 90, 85, 80, 75, 70, 65, 60, 0};
const char *GRADES[NUMBER_OF_GRADES] = {"A+", "A", "B+", "B", "C+", "C", "D+", "D", "F"};

int main(void)
{
    printf("학점 프로그램\n");
    printf("종료를 원하면 \"999"\ 를 입력\n");
    printf("점수 : 95    90    85    80    75    70    65    60    0\n");
    printf("학점 : A+    A    B+    B    C+    C    D+    D    F\n");
    
    int grade = -1;
    for (int i = 0; i < NUMBER_OF_GRADES; i++)
    {
        if (grade[i] >= 0 && grade[i] <= 100)
        {
            continue;
        }
        else
        {
            printf("성적을 올바르게 입력하세요. 범위는 0 ~ 100입니다.\n")
            return -1;
        }
    }
}

int score = -1;
{
    printf("성적을 입력하세요 (0 ~ 100) : ");
    scanf("%d", score);
    
    if(score >= 95)
        printf("학점은 A+입니다.");
    else if(score >= 90)
        printf("학점은 A입니다.");
    else if(score >= 85)
        printf("학점은 B+입니다.");
    else if(score >= 80)
        printf("학점은 B입니다.");
    else if(score >= 75)
        printf("학점은 C+입니다.");
    else if(score >= 70)
        printf("학점은 C입니다.");
    else if(score >= 65)
        printf("학점은 D+입니다.");
    else if(score >= 60)
        printf("학점은 D입니다.");
    else
        printf("학점은 F입니다.");
        
    return score;
}
