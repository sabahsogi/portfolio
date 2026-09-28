<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Project architecture

- Portfolio projects and their media references live only in `src/data/projects.ts` so new work never requires component changes.
- Shared site navigation and footer wrap every route in the root layout so portfolio pages remain visually consistent.
- Project evidence pairs each future thumbnail with its Instagram URL in `src/data/projects.ts` so primary media and supporting proof stay synchronized.
- Google Doodles and Trust & Safety items are independent projects, never combined parent projects, because each requires its own card, URL, metadata, and project narrative.
- Instagram and YouTube evidence renders as an on-page embed with an original-link fallback; uploaded videos use the native player.
