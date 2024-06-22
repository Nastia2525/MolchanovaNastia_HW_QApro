let x=prompt("Insert x (numbers only) = ", '');
let n=prompt("Insert n (numbers only) = ", '');


//pow(x,n);


if (n % 1==0) {
    pow(x, n)
}
else {
    console.log(`Fractional number n is not supported`);
}




function pow(x, n) {
    let answer;
    if (x==0) {
        answer=0
    }
    if (n==0) {
        answer=1
    }
    else {
        answer=x;
        if (n<0) {
            n=-n;
            for (let i=1; i<n; i++) {
                answer=answer*x
            }
            answer=1/answer
        }
        else {
            for (let i=1; i<n; i++) {
                answer=answer*x
            }
        }
    }


    console.log(answer)
}