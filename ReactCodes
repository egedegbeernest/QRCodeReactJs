import React from "react";
import QRCode from "react-qr-code";

import { useState } from "react";

function QrCodeInfo() {
  const [wifiName, setWifiName] = useState("");
  const [password, setPassword] = useState("");
  const [qrCodeVisible, setQrCodeVisible] = useState(false);

  const clickButton = () => {
    let qrimage = password;
    setQrCodeVisible(!!qrimage);
  };

  return (
    <div className="center">
      <div className=" center card shadow">
        <div className="flex">
          <form>
            <div className="user-details">
              <div className="input-box">
                <span className="details">WifiName</span>
                <input
                  type="text"
                  placeholder="Enter your WifiName"
                  value={wifiName}
                  onChange={(event) => setWifiName(event.target.value)}
                  required
                />
              </div>
              <div className="input-box">
                <span className="details">Password</span>
                <input
                  type="text"
                  placeholder="Enter your Password"
                  value={password}
                  onChange={(event) => setPassword(event.target.value)}
                  required
                />
              </div>
            </div>
            <div className="center">
              <button type="button" className="center" onClick={clickButton}>
                Submit
              </button>
            </div>
          </form>
          <div>
            <h1>{wifiName}</h1>
            {qrCodeVisible && <QRCode value={password} />}
          </div>
        </div>
      </div>
    </div>
  );
}

export default QrCodeInfo;
