# SafeCoin: user-granularity safety on top of the Libra Blockchain

SafeCoin is a module built on top of the Libray Blockchain the move IR language
that grants users a set of capabilities. It also defines a module that acts as a transferrable currency (SafeCoin) and a set of methods through an API that allows a user to access and store SafeCoin. Right now, SafeCoin works with a whitelist and blacklist capability, where one can send SafeCoins to a user iff the user is on the whitelist, as well as not on the blacklist.  

SafeCoin is built on top of a malleable framework that could allow for many powerful extensions to it's core architecture - it was just a whim to begin with a whitelisting/blacklisting set of capabilities.

Currently, Libra doesn't allow modules to be published, which is why the source code for SafeCoin is run as a test.

## Try and Run the Test
* Clone the Libra repository
* Follow the Libra `README` for how to compile and install it.
* Clone this repository
* Copy the SafeCoin source code located at `src/SafeCoin.mvir` in this repository, 
  to the test folder in the Libra repository located at `language/functional_tests/tests/testsuite/module/`
* Execute the following command somewhere in the Libra repository: `cargo test -p functional_tests SafeCoin`