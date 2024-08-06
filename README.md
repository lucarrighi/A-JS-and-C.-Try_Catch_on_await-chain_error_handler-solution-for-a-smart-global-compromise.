# A-JS-and-C.-Try_Catch_on_await-chain_error_handler-solution-for-a-smart-global-compromise.
Unavoidably, the await instance, as well as any async function, requires try/catch blocks for a better error handling. Here, a modular and global compromise/solution for your website,  able to  keep order in your code.

The here solution is offered by:
1) a ChainErrorHandler_CustomErrorLauncher(): that creates and returns a custom error object with additional debugging information.
2) a Try / Catch block: (which I will present both integrally and into its DRY version) that handles: (if) EITHER the propagation of the error launced by the Previous ring of the chain in case of its detection, OR (else), the launch of a new Error via ChainErrorHandler_CustomErrorLauncher(), including the report of the original error not to lose the stack trace.

Essentially: the usage of this module in each ring of the chain, will allow you to see launched and propagated untill the surface the most rooted error, via a system ab
