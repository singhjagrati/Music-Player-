Mume Music App
A fully-functional React Native music streaming app featuring tabbed navigation, artist grids, song sorting, favorites, and 10+ interactive song actions. Built with pixel-perfect UI for iOS/Android.

✨ Features
Tabbed Navigation: Suggested, Songs, Artists (85+), Albums, Folders

Interactive Song List: Album art, artist info, favorite toggle, 3-dot menu

Artist Grid: 85+ artists with circular images, album/song counts

Bottom Sheet Menus: 10+ actions (Play Next, Add to Playlist/Queue, Share, Delete)

Sorting: Ascending/Descending, Artist, Album, Year, Date Added/Modified, Composer

Dark Theme: Production-ready dark UI matching Mume design

State Management: Persistent favorites, blacklist using React hooks

Navigation: Stack navigation to PlayerScreen, Albums, Artists

Responsive: SafeAreaView, keyboard handling, accessible touch targets

🛠️ Tech Stack
text
Frontend: React Native 0.74, Expo 51, TypeScript
UI: Ionicons, FlatList virtualization, Modal animations
Navigation: @react-navigation/native, @react-navigation/bottom-tabs
Data: DummySongs.ts (20+ songs/artists/albums)
State: React hooks (useState for favorites/blacklist)
🚀 Quick Start
bash
# Clone repo
git clone <your-repo-url>
cd mume-music-app

# Install dependencies
npx expo install

# Run on iOS/Android
npx expo start --clear

# Development build
eas build --profile development --platform all
📁 Project Structure
text
src/
├── screens/tabs/
│   ├── SongsScreen.tsx        # Song list + 10-action menu
│   ├── ArtistsScreen.tsx      # 85+ artist grid + popup
│   ├── SuggestedScreen.tsx    # Tab navigation hub
│   └── PlayerScreen.tsx       # Now playing
├── data/
│   └── dummySongs.ts          # 20+ songs/artists/albums
├── components/
│   └── SongCard.tsx           # Reusable song row
└── navigation/
    └── BottomTabs.tsx         # Tab navigator
🎯 Key Features Implemented
Interactive Song Menu (10 Actions)
text
✅ Play Next → PlayerScreen navigation
✅ Add to Playing Queue → Alert feedback
✅ Add to Playlist → Alert feedback  
✅ Go to Album/Artist → Tab navigation
✅ Details → Song info dialog
✅ Set as Ringtone → Confirmation
✅ Add to Blacklist → State management
✅ Share → Share sheet
✅ Delete from Device → Confirmation dialog
✅ Favorite heart toggle → Persistent state
Advanced UI Challenges Solved
text
✅ Modal z-index overlaps (presentationStyle="overFullScreen")
✅ SafeAreaView + statusBarTranslucent
✅ FlatList virtualization (560+ songs)
✅ Bottom sheet animations (slide/fade)
✅ Dark theme hardcoded colors
✅ hitSlop for accessible touch targets
Production Optimizations
text
✅ TypeScript interfaces (Song, Artist, Album)
✅ Error-free Image loading (optional chaining)
✅ KeyboardShouldPersistTaps handling
✅ ActiveOpacity + haptic feedback
✅ Shadow/elevation cross-platform
🔮 Future Enhancements
Real audio playback (Expo AV)

Offline storage (AsyncStorage)

Search functionality

Queue management

Playlist creation

Real API integration

📄 License
MIT License

text
Built with ❤️ for React Native developers
👨‍💻 Author: Jagrati Singh
📧 Contact: [jagratisingh1212@gmail.com] | | [GitHub]