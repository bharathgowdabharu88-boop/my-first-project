 #include<stdio.h>
int main()
{
    char a[9]={' ',' ',' ',' ',' ',' ',' ',' ',' '};
    char move='X';
    int pos;
    for(int i=1;i<=9;i++)
    {
        printf("Enter your pos:");
        scanf("%d",&pos);
        a[pos]=move;
        printf("\t%c|%c|%c\n",a[0],a[1],a[2]);
        printf("\t-+-+-\n");
        printf("\t%c|%c|%c\n",a[3],a[4],a[5]);
        printf("\t-+-+-\n");
        printf("\t%c|%c|%c\n",a[6],a[7],a[8]);
        
    
    
        if((a[0]=='X'&&a[1]=='X'&&a[2]=='X')||(a[3]=='X'&&a[4]=='X'&&a[5]=='X')||(a[6]=='X'&&a[7]=='X'&&a[8]=='X')||(a[0]=='X'&&a[3]=='X'&&a[6]=='X')||(a[1]=='X'&&a[4]=='X'&&a[7]=='X')||(a[2]=='X'&&a[5]=='X'&&a[8]=='X')||(a[0]=='X'&&a[4]=='X'&&a[8]=='X')||(a[2]=='X'&&a[4]=='X'&&a[6]=='X'))
       {
           printf("X wins!\n");
           break;
       }
        else if((a[0]=='O'&&a[1]=='O'&&a[2]=='O')||(a[3]=='O'&&a[4]=='O'&&a[5]=='O')||(a[6]=='O'&&a[7]=='O'&&a[8]=='O')||(a[0]=='O'&&a[3]=='O'&&a[6]=='O')||(a[1]=='O'&&a[4]=='O'&&a[7]=='O')||(a[2]=='O'&&a[5]=='O'&&a[8]=='O')||(a[0]=='O'&&a[4]=='O'&&a[8]=='O')||(a[2]=='O'&&a[4]=='O'&&a[6]=='O'))
        {
            printf("O wins!\n");
            break;
            }
            else
            printf("Tie");
            
             if(move=='X')
         move='O';
         else
         move='X';
    }   
    
         return 0;
        
    
}
