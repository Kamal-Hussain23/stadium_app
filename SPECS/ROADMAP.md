# Roadmap

## Current State

- ✅ Phase 1: Mock backend with in-memory data
- 🔄 Phase 2: SQLite data layer (in progress)

## Next Steps

### Phase 2: SQLite Data Layer
- [ ] Implement `data_layer.py` with parameterized SQL
- [ ] Create tables: `stadium_entries`, `people`
- [ ] Wire backend routes to data layer
- [ ] Verify data persists across restarts

### Phase 3: Frontend Integration
- [ ] Connect dashboard to SQLite-backed endpoints
- [ ] Add gate filtering (A, B, C, D)
- [ ] Show entry count and person details

### Phase 4: Polish
- [ ] Handle database errors gracefully in UI
- [ ] Add loading states
- [ ] Clean up code and add comments
