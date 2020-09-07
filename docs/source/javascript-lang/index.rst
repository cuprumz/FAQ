Problem Set
===============================

this
--------------------

.. code:: javascript

    var length = 100;
    function f1() {
        console.log(this.length);
    }
    var obj = {
        length: 10,
        f2: function (f1) {
            f1();
            arguments[0]();
        }
    }
    obj.f2(f1, 1);
        
.. hint::
    output: 
    100
    2
