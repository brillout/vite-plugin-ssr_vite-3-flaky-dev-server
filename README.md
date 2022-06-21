Reproduction showcasing that the dev server of `vite@3.0.0-alpha.9` (purposley using an old Vite version) is flaky.

It's somewhat tricky to explain. The tricky part is that the problem is caused by **both** a Vite change as well as a `vite-plugin-ssr` change.

I plan to fix the situation by reverting the `vite-plugin-ssr` problematic change. But this doesn't really help us: the Vite problematic change would still be around, looming around the corner to haunt us back at some point in the future.

That's said, I'd be up to take a faith of leap and fix the problem on `vite-plugin-ssr`'s side. But I believe that someone familiar with the Vite 3 changes should consider this issue and maybe point us to Vite 3 changes that have potential to be the cause.

Note that the falkines also happens with `vite@3.0.0-alpha.13` but I chose to showcase the flakiness with `vite@3.0.0-alpha.13` to reduce the Vite search space. For example, we know.

On Vite's side, the problem is somwhere [between `v2.9.10` and `v3.0.0-alpha.9`](https://github.com/vitejs/vite/compare/v2.9.10..v3.0.0-alpha.9).

On vite-plugin-ssr's side, the problem is somwhere [between ]().


Note that, even if I 


Vite 3 bug reproduction showing that the Vite 
