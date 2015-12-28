# SYNOPSIS

simple monitporing for blog.perl.org

* get logged and check if your profile page is valid

# INSTALL

    sparrow plg install swat-blog-perl-org

# Usage

    sparrow project create blog-perl-org
    sparrow check add blog-perl-org my-account
    sparrow check set blog-perl-org my-account -u http://blogs.perl.org -p swat-blog-perl-org
    

Then you need to setup `user` and `password` variables.


    sparrow check set_swat blog-perl-org my-account

        user=melezhik
        password=*********

That's it! Now just run it:

    sparrow check run blog-perl-org my-account

# Example Output

    /home/vagrant/.swat/.cache/13505/prove/mt/mt-cp.fcgi/00.POST.t ..
    ok 1 - POST http://blogs.perl.org//mt/mt-cp.fcgi succeeded
    # response saved to /home/vagrant/.swat/.cache/13505/prove/Y7bcav3tlg
    ok 2 - output match '200 OK'
    ok 3 - output match 'Edit Profile'
    ok 4 - output match 'Display Name'
    ok 5 - output match 'Email Address'
    ok 6 - output match 'New Password'
    ok 7 - output match 'Confirm Password'
    1..7
    ok
    /home/vagrant/.swat/.cache/13505/prove/00.GET.t .................
    ok 1 - GET http://blogs.perl.org// succeeded
    # response saved to /home/vagrant/.swat/.cache/13505/prove/_eMBUtrctu
    ok 2 - output match 'blogs.perl.org'
    ok 3 - output match 'There's more than one way to blog it.'
    1..3
    ok
    All tests successful.
    Files=2, Tests=10, 13 wallclock secs ( 0.03 usr  0.01 sys +  0.15 cusr  0.02 csys =  0.21 CPU)
    Result: PASS
    
# AUTHOR

Alexey Melezhik


  
