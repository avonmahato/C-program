#include <stdio.h>

int main() {
    float cost_price, selling_price, profit_or_loss, profit_or_loss_percent;
 printf(" program to determine how much profit or loss is incurred in percentage\n");
    printf("Author name:Avon Mahato\n");

    printf("Enter the cost price and selling price of the item: ");
    scanf("%f %f", &cost_price, &selling_price);
    if (selling_price > cost_price) {
        profit_or_loss = selling_price - cost_price;
        profit_or_loss_percent = (profit_or_loss / cost_price) * 100;
        printf("The seller has made a profit of %.2f rupees (%.2f%%).\n", profit_or_loss, profit_or_loss_percent);
    }
    else if (selling_price < cost_price) {
        profit_or_loss = cost_price - selling_price;
        profit_or_loss_percent = (profit_or_loss / cost_price) * 100;
        printf("The seller has incurred a loss of %.2f rupees (%.2f%%).\n", profit_or_loss, profit_or_loss_percent);
    }
    else {
        printf("The seller neither incurs a loss nor makes a profit.\n");
    }
    return 0;
}
