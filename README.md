#include "SevSeg.h"
SevSeg sevseg;

Void setup()  {
byte numDigits = 1;
byte digitPins[] = {};
byte segmentPins[] = {6, 5, 2, 3, 4, 7, 8, 9};
bool resistorsOnSegment = true;
byte hardwareConfig = COMMON_CATHODE;

sevseg.begin(hardwareConfig, numDigits, digitPins, segmentPins, resistorsOnSegment) ;
sevseg.setBrightness(100) ;
