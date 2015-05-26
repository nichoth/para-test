# parallelshell issue #22

Failing case for [parallelshell](https://github.com/keithamus/parallelshell).

    $ git clone https://github.com/nichoth/para-test.git
    $ npm install
    $ cd module-1
    $ npm run dev

In a separate terminal:

    $ cd module-2
    $ npm run dev

`node server.js` throws error because the first server is using the same port, but watchify still runs.
