#include <stdio.h>
#include <math.h>

int main() {
    int T;
    scanf("%d", &T);

    for (int caseNumber = 1; caseNumber <= T; caseNumber++) {
        long long S;
        scanf("%lld", &S);
        long long N = ceil(sqrt(S));
        long long square = N * N;
        long long diff = square - S;

        long long x, y;
        if (n%2 == 0) {
            if (diff<n) {
                x = n;
                y =diff+1;
            }
            else {
                x = n-(diff-N + 1);
                y = n;
            }
        } else
        {
            if (diff <n)
                {
                x = diff + 1;
                y = n;
            } else
            {
                x = n;
                y=n-(diff-n+ 1);
            }
        }
printf("Case %d: %lld %lld\n", caseNumber, x, y);
    }
    return 0;
}

