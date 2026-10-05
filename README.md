import 'package:flutter/material.dart';
import 'package:animated_text_kit/animated_text_kit.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text("Animated Text"),
          backgroundColor: Colors.blue,
        ),

        body: Center(
          child: AnimatedTextKit(
            animatedTexts: [
              TypewriterAnimatedText(
                'Welcome to Flutter',
                speed: const Duration(milliseconds: 100),
              ),

              FadeAnimatedText(
                'Learn Flutter Easily',
                ),
            ],
            repeatForever: true,
          ),
        ),
      ),
    ),
  );
}
