PAYBOX_API_KEY=your_actual_api_key
PAYBOX_SIGNING_KEY=your_actual_signing_key
DEMO_MODE=false
import { PayboxClient } from "@paybox-sh/sdk";

const paybox = PayboxClient.fromConfig();

const services = await paybox.discoverServices("weather api");

console.log(services);
