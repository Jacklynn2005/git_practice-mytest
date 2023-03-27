**Welcome to the git_practice repo!**   
**This is the repo to test if you can fluently use Git & Github!**

# git_practice
First fork this repo, and follow the instructions to finish the practice

# Here are the things you need to do:
1. Fork this repo and clone it in your own work space.  
   **All of the following steps are executed in your own repo!**
2. Run the "main.cpp" file. It will be compiled as an executable binary file and output "Hello World!".
3. Create a new branch called "test" from "master" branch, and go to that "test". Add a new cpp hearder file called "algo.hpp" under the "include" folder.
   Paste the following code in "algo.hpp" file:
    ```c++
    #ifndef _ALGO_H_
    #define _ALGO_H_

    /**
     * @brief           find the Greatest Common Divisor
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of gcd
     */
    extern int gcd(int a, int b);

    #endif
    ```

4. Add a new cpp source file called "algo.cpp" under the "src" folder.  
Paste the following code in your new file:
   ```c++
   #include "../include/algo.hpp"

    /**
     * @brief           find the Greatest Common Divisor
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of gcd
     */
    int gcd(int a, int b);

    /**
     * @brief           find the Greatest Common Divisor
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of gcd
     */
    int gcd(int a, int b) {
        int r;
        while (a%b!=0)
        {
            r=a%b;
            a=b;
            b=r;    
        }
        return b; 
    }
   ```
   Upload to GitHub.
5. Create a new branch called "dev" from the "test" branch, and go to that "dev". Delete the branch "test" and update the branch status to Github. In "algo.cpp" file, add the following code after the declaration ``int gcd(int a, int b);``:
   ```c++
    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcm(int a,int b);
   ```
   Add the following code after the end of "algo.cpp" file:
   ```c++
    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcm(int a, int b)
    {
            return a/gcd(a,b)*b;
    }
   ```
   Upload to GitHub.  
6. Create a branch called "modify_algo" from "dev" branch, and go to the "modify_algo" branch. Rollback to the previous version.  
   In "algo.cpp" file, add the following code after the declaration ``int gcd(int a, int b);``:
   ```c++
    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcmm(int a,int b);
   ```
   Add the following code after the end of "algo.cpp" file:
   ```c++
    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcmm(int a, int b)
    {
            return a/gcd(a,b)*b;
    }
    // code from "modify_algo"
   ```
   Upload to GitHub.  
7. At github, create the Pull Request from branch "dev" to branch "master". And then merge it. **Do not delete this branch!**
8. At github, create the Pull Request from branch "modify_algo" to branch "master". And then merge it. Assume the code that existed in "master" is the right one. **Do not delete this branch!**
9. At local, go to branch "master", add a new cpp hearder file called "algo.hpp" under the "include" folder.
10. Add a new cpp source file called "algo.cpp" under the "src" folder.  
    Paste the following code into your new file:
    ```c++
    #include "../include/algo.hpp"
    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcm(int a,int b);

    /**
     * @brief           find the Least Common Multiple
     * @param[in]       a: one of the integer
     * @param[in]       b: one of the integer
     * @return          int
     * @retval          the result of lcm
     */
    int lcm(int a, int b)
    {
            return a/gcd(a,b)*b;
    }
    ```
11. create a function to output "hello world" at the end of "algo.cpp". 
Upload to Github with your own understanding. 
