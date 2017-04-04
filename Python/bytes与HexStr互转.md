## bytes��HexStr��ת

``` python
def ByteToHex( bins ):

    """
    Convert a byte string to it's hex string representation e.g. for output.
    """
    return ''.join(["%02X" % x for x in bins]).strip()
    

def HexToByte( hexStr ):

    """
    Convert a string hex byte values into a byte string. The Hex Byte values may
    or may not be space separated.
    """
    return bytes.fromhex(hexStr)
```