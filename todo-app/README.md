# To-Do List Application

A beautiful, responsive to-do list application with local storage functionality. Manage your tasks efficiently with a clean and intuitive interface.

## Features

✨ **Core Features**
- ➕ Add new tasks
- ✅ Mark tasks as completed
- 🗑️ Delete tasks
- 📊 Task counter showing active and completed tasks
- 🔍 Filter tasks (All, Active, Completed)
- 🧹 Clear all completed tasks at once

💾 **Storage**
- 💾 Persistent local storage - your tasks are saved automatically
- 📱 Works offline - no internet connection needed
- 🔄 Data persists across browser sessions

🎨 **User Interface**
- 🌈 Modern gradient design with purple theme
- 📱 Fully responsive - works on desktop, tablet, and mobile
- ⚡ Smooth animations and transitions
- 🎯 Intuitive and easy-to-use interface
- 🌙 Clean, minimalist design

## How to Use

1. **Add a Task**: Type your task in the input field and click "Add" or press Enter
2. **Complete a Task**: Click the checkbox next to a task to mark it as completed
3. **Delete a Task**: Click the "Delete" button to remove a task
4. **Filter Tasks**: Use the filter buttons to view All, Active, or Completed tasks
5. **Clear Completed**: Click "Clear Completed" to remove all finished tasks at once

## File Structure

```
todo-app/
├── index.html      # HTML structure
├── styles.css      # Styling and animations
├── script.js       # JavaScript functionality
└── README.md       # Documentation
```

## Technical Details

### Local Storage
- Tasks are automatically saved to browser's localStorage
- Data persists even after closing the browser
- Storage key: `todoAppData`

### Data Structure
Each todo item contains:
```javascript
{
  id: timestamp,           // Unique identifier
  text: "task text",       // Task description
  completed: false,        // Completion status
  createdAt: "date/time"  // Creation timestamp
}
```

### Browser Support
- Chrome 4+
- Firefox 3.5+
- Safari 4+
- Edge (all versions)
- Mobile browsers

## Features Explained

### Filter System
- **All**: Shows all tasks regardless of status
- **Active**: Shows only uncompleted tasks
- **Completed**: Shows only completed tasks

### Task Counter
Displays the count based on current filter:
- Shows total tasks when "All" is selected
- Shows active tasks when "Active" is selected
- Shows completed tasks when "Completed" is selected

### Data Validation
- Tasks must not be empty
- Maximum 100 characters per task
- Duplicate tasks are allowed (in case you need to do the same thing twice)

## Tips & Tricks

💡 **Productivity Tips**
- Use specific, actionable task descriptions
- Break large tasks into smaller subtasks
- Regularly clear completed tasks to stay focused
- Use the filter feature to focus on active tasks

🎯 **Keyboard Shortcuts**
- `Enter` key: Add task (when input is focused)
- `Tab`: Navigate through elements

## Customization

You can easily customize:
- **Colors**: Change the gradient colors in `styles.css`
- **Storage**: Modify the storage key in `script.js`
- **Task limit**: Update the character limit in the `addTodo()` method
- **Animations**: Adjust timing and effects in the CSS

## Performance

- Lightweight: < 10KB total size
- Fast: No external dependencies
- Efficient: Uses native localStorage API
- Smooth animations: CSS transitions only

## Known Limitations

- Storage is limited to ~5MB per domain
- localStorage is domain-specific (not shared across domains)
- No cloud sync (data is local only)
- No task categories or tags

## Future Enhancements

Potential features to add:
- 📅 Due dates and reminders
- 🏷️ Task categories/tags
- 🔄 Task priority levels
- 📤 Export/Import functionality
- 🌙 Dark mode toggle
- 🔔 Browser notifications
- ☁️ Cloud sync with authentication

## Troubleshooting

**Tasks not saving?**
- Check if localStorage is enabled in your browser
- Check browser's storage quota
- Clear browser cache and try again

**Tasks disappeared?**
- Check if you cleared browser data
- Disable browser extensions that might clear storage
- Try using incognito/private mode to test

**Styling looks off?**
- Clear browser cache (Ctrl+F5 / Cmd+Shift+R)
- Make sure CSS file is loaded
- Check browser console for errors

## License

This project is free to use and modify for personal or commercial purposes.

## Support

For issues or suggestions, feel free to open an issue or create a pull request!

---

**Made with ❤️ by RGautam2005**
