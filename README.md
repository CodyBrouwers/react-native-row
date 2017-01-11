# react-native-row

A wrapper around the react-native View component enabling concise assignment of flexbox properties

## installation (not yet!)

    npm install react-native-row

## usage

    import { View, Row } from react-native-row
    
    <Row dial={5}>
      <View style={{width: 50, height: 50, backgroundColor: 'powderblue'}} />
      <View style={{width: 50, height: 50, backgroundColor: 'skyblue'}} />
      <View style={{width: 50, height: 50, backgroundColor: 'steelblue'}} />
    </Row>
    
## result

the child components of `Row` are centered and horizontally aligned 

    <View style={{flex:1, flexDirection:"row", justifyContent:"center" alignItems:"center"}}>   
      <View style={{width: 50, height: 50, backgroundColor: 'powderblue'}} />
      <View style={{width: 50, height: 50, backgroundColor: 'skyblue'}} />
      <View style={{width: 50, height: 50, backgroundColor: 'steelblue'}} />
    </View>
    
## concept

Simple. Use `dial` to set the position of the children with a number that corresponds to the position of the number on a phone keypad.

![example](example1.jpg)

Use `Row` for horizontally-aligned children. Optionally import `View` from this package instead of from `react-native` and all of your `View` components can use dial as well.
