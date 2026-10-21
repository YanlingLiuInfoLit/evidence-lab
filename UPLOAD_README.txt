CORE SCORING LOOKUP FIX

Upload all files to repository root.

Commit:
Fix scoring lookup for Practice and Capstone

Root cause:
Protected scoring records were stored in an array but looked up by string case_id.
The game now creates a case_id-keyed scoring map.

After deployment:
1. Start Practice.
2. Open at least one evidence item.
3. Select an answer and evidence.
4. Click Submit investigation.
5. Confirm the score/feedback screen appears.
6. Repeat once in Capstone.
