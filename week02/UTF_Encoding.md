### String 转 Buffer

function UTF8_Encoding(str ) {
        let length =  str.length,
                strIndex = -1,
                strEnd = length - 1,
                bytes = new Uint8Array(length),
                index = 0;
        while (strIndex++ < strEnd) {
                bytes[index] = str.charCodeAt(strIndex) & 0xFF;
                index++;
        }
        return bytes;
}

### 字节流文件转String

function UTF8_Decoding(bytes) {
        let str = "",
                bytesIndex = -1,
                bytesEnd = bytes.length - 1;
        while (bytesIndex ++ <  bytesEnd) {
                str += String.fromCharCode(bytes[bytesIndex]);
        }
        return str;
}