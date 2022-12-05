# Usage

***Note: install the **[solana wallet adapter](https://github.com/solana-labs/wallet-adapter)*****.

```
import { 
    PhantomWalletAdapter, 
    GlowWalletAdapter,
    SolflareWalletAdapter
} from '@solana/wallet-adapter-wallets';

import { E2EWallet } from 'e2e-solana-wallet';

...
const wallets = useMemo(
    () => [

        new PhantomWalletAdapter(),
        new GlowWalletAdapter(),
        new SolflareWalletAdapter(),
        new E2EWallet(),
    ],
    // eslint-disable-next-line react-hooks/exhaustive-deps
    [network]
);
...
```