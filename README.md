# Flutter Navigation App

This is a simple Flutter app demonstrating navigation and routing using a bottom navigation bar.

### Running the App

1. Clone this repository:

   ```bash
   git clone https://github.com/OlimovAlibek/HW3.git


   Project Structure

lib/main.dart: Entry point of the app.
lib/screens/: Contains individual screens.
lib/screens/home_screen.dart: Home screen of the app.
lib/screens/about_screen.dart: About screen.
lib/screens/team_screen.dart: Team screen.
lib/screens/contact_screen.dart: Contact screen.
lib/screens/settings_screen.dart: Settings screen.
lib/screens/new_screen.dart: Example of a new screen added.
Navigation

The app uses a bottom navigation bar for navigation between screens. Each screen can also navigate to a new screen using Navigator.push().

ElevatedButton(
  onPressed: () {
    Navigator.push(
      context,
      MaterialPageRoute(builder: (context) => NewScreen()),
    );
  },
  child: Text('Go to New Screen'),
),


Data Passing

Data can be passed between screens using the Navigator.pushNamed() or Navigator.push() method.

// Passing data from HomeScreen to AboutScreen
final result = await Navigator.pushNamed(context, '/about', arguments: 'Data from HomeScreen');

// Sending back a result from AboutScreen to HomeScreen
Navigator.pop(context, 'Result from AboutScreen');

