---
layout: page
title: Experiments
---

<script src="scripts/jquery-1.4.1.min.js"></script>
<script src="scripts/VBAMcode.js"></script>
<script src="scripts/clock.js"></script>
<link rel="stylesheet" href="/css/VBAM.css?_={{site.time | date: '%s%N'}}">

On this page you can see random projects and tinkerings I have made over the years.
<br>
<br>

### Mirrorless Edge (Mini Ludum Dare Entry, March 2014)
This is a little game I made with my friend Steven back in March 2014. 
We used typescript for this *(because it is **awesome**)*. The game is a simple endless runner but can still be quite addictive.

[![Alt text](images/mirrorlessedge.jpg)](https://github.com/edwin-jones/LDMINI50)

<br />

### Virtual Binary Adding Machine
This is an 8 bit/single byte binary adding machine designed to demonstrate simple
binary logic. This machine can perform basic operations on any two unsigned 8 bit
binary integers and output the result in binary as an unsigned integer.

Please note that input two is the subtrahend in subtraction operations.

<div id="input1" class="center">
    <table class="textcenter">
        <tr>
            <td></td>
            <td>128
            </td>
            <td>64
            </td>
            <td>32
            </td>
            <td>16
            </td>
            <td>8
            </td>
            <td>4
            </td>
            <td>2
            </td>
            <td>1
            </td>
        </tr>
        <tr>
            <td colspan="9">
                <b></b>
            </td>
        </tr>
        <tr>
            <td colspan="9">
                <b>Input One</b>
            </td>
        </tr>
        <tr>
            <td>0
            </td>
            <td>
                <input type="radio" name="inputOneBit7" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit6" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit5" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit4" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit3" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit2" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit1" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputOneBit0" value="0" checked="checked" />
            </td>
        </tr>
        <tr>
            <td>1
            </td>
            <td>
                <input type="radio" name="inputOneBit7" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit6" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit5" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit4" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit3" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit2" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit1" value="1" />
            </td>
            <td>
                <input type="radio" name="inputOneBit0" value="1" />
            </td>
        </tr>
        <tr>
            <td colspan="9">
                <b></b>
            </td>
        </tr>
        <tr>
            <td colspan="9">
                <b>Input Two</b>
            </td>
        </tr>
        <tr>
            <td>0
            </td>
            <td>
                <input type="radio" name="inputTwoBit7" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit6" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit5" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit4" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit3" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit2" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit1" value="0" checked="checked" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit0" value="0" checked="checked" />
            </td>
        </tr>
        <tr>
            <td>1
            </td>
            <td>
                <input type="radio" name="inputTwoBit7" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit6" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit5" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit4" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit3" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit2" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit1" value="1" />
            </td>
            <td>
                <input type="radio" name="inputTwoBit0" value="1" />
            </td>
        </tr>
    </table>
</div>
<div class="textcenter">
    <p>
        <button class="btn btn-primary" class="btn btn-primary" onclick="Calculate('add')">Add</button>
        <button class="btn btn-primary" class="btn btn-primary" onclick="Calculate('subtract')">Subtract</button>
    </p>
</div>
<h4 id="output" class="textcenter">ERROR
</h4>
<br>

### Digital Clock
<p>
    This is a simple digital clock that allows you to check the time in different cities
    across the world. It uses your system clock, so if your system time is incorrect
    it will also be wrong.
</p>
<p id="Clock" class="textcenter" style="font-size: 3.0em;">
</p>
<div class="textcenter">
    <input type="radio" name="City" value="-8" />San Francisco&nbsp;
    <input type="radio" name="City" value="-5" />New York&nbsp;
    <input type="radio" name="City" value="0" checked="checked" />London&nbsp;
    <input type="radio" name="City" value="3" />Moscow&nbsp;
    <input type="radio" name="City" value="9" />Tokyo&nbsp;
</div>

<!-- call start at end of document -->
<script type="text/javascript">Start();</script>