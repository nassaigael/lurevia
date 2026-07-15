Parfait ! Je vois que tu utilises une structure **Next.js classique avec le dossier `app/`** à la racine, sans le dossier `src/`. Je vais te donner l'arborescence exacte qui correspond à ta structure actuelle.

---

```
lurevia/
│
├── .next/
├── node_modules/
├── public/
│   ├── favicon.ico
│   ├── images/
│   │   ├── hero/
│   │   ├── categories/
│   │   ├── products/
│   │   └── blog/
│   └── icons/
│       └── payment/
│
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   ├── globals.css
│   ├── providers.tsx
│   │
│   ├── (auth)/
│   │   ├── login/
│   │   │   └── page.tsx
│   │   ├── register/
│   │   │   └── page.tsx
│   │   └── forgot-password/
│   │       └── page.tsx
│   │
│   ├── (dashboard)/
│   │   └── account/
│   │       ├── page.tsx
│   │       ├── orders/
│   │       │   └── page.tsx
│   │       ├── wishlist/
│   │       │   └── page.tsx
│   │       └── profile/
│   │           └── page.tsx
│   │
│   ├── (shop)/
│   │   ├── products/
│   │   │   ├── page.tsx
│   │   │   └── [slug]/
│   │   │       └── page.tsx
│   │   ├── categories/
│   │   │   ├── maison/
│   │   │   │   └── page.tsx
│   │   │   ├── cuisine/
│   │   │   │   └── page.tsx
│   │   │   ├── salle-de-bain/
│   │   │   │   └── page.tsx
│   │   │   ├── animaux/
│   │   │   │   └── page.tsx
│   │   │   ├── bureau/
│   │   │   │   └── page.tsx
│   │   │   └── voyage/
│   │   │       └── page.tsx
│   │   ├── cart/
│   │   │   └── page.tsx
│   │   ├── checkout/
│   │   │   └── page.tsx
│   │   └── search/
│   │       └── page.tsx
│   │
│   ├── (info)/
│   │   ├── about/
│   │   │   └── page.tsx
│   │   ├── blog/
│   │   │   ├── page.tsx
│   │   │   └── [slug]/
│   │   │       └── page.tsx
│   │   ├── faq/
│   │   │   └── page.tsx
│   │   ├── contact/
│   │   │   └── page.tsx
│   │   ├── shipping/
│   │   │   └── page.tsx
│   │   ├── returns/
│   │   │   └── page.tsx
│   │   └── track-order/
│   │       └── page.tsx
│   │
│   ├── (legal)/
│   │   ├── cgv/
│   │   │   └── page.tsx
│   │   ├── privacy/
│   │   │   └── page.tsx
│   │   └── legal-notice/
│   │       └── page.tsx
│   │
│   └── api/
│       ├── auth/
│       │   └── [...nextauth]/
│       │       └── route.ts
│       ├── products/
│       │   └── route.ts
│       ├── cart/
│       │   └── route.ts
│       └── orders/
│           └── route.ts
│
├── components/
│   ├── ui/
│   │   ├── Button/
│   │   │   ├── Button.tsx
│   │   │   └── index.ts
│   │   ├── Input/
│   │   │   ├── Input.tsx
│   │   │   └── index.ts
│   │   ├── Select/
│   │   │   ├── Select.tsx
│   │   │   └── index.ts
│   │   ├── Card/
│   │   │   ├── Card.tsx
│   │   │   └── index.ts
│   │   ├── Modal/
│   │   │   ├── Modal.tsx
│   │   │   └── index.ts
│   │   ├── Badge/
│   │   │   ├── Badge.tsx
│   │   │   └── index.ts
│   │   ├── Skeleton/
│   │   │   ├── Skeleton.tsx
│   │   │   └── index.ts
│   │   ├── Loading/
│   │   │   ├── Loading.tsx
│   │   │   └── index.ts
│   │   ├── Container/
│   │   │   ├── Container.tsx
│   │   │   └── index.ts
│   │   └── Section/
│   │       ├── Section.tsx
│   │       └── index.ts
│   │
│   ├── layout/
│   │   ├── Header/
│   │   │   ├── Header.tsx
│   │   │   ├── HeaderMobile.tsx
│   │   │   ├── Navigation.tsx
│   │   │   ├── SearchBar.tsx
│   │   │   └── index.ts
│   │   ├── Footer/
│   │   │   ├── Footer.tsx
│   │   │   ├── FooterLinks.tsx
│   │   │   ├── FooterNewsletter.tsx
│   │   │   └── index.ts
│   │   └── Sidebar/
│   │       ├── Sidebar.tsx
│   │       └── index.ts
│   │
│   ├── home/
│   │   ├── Hero/
│   │   │   ├── Hero.tsx
│   │   │   └── index.ts
│   │   ├── Categories/
│   │   │   ├── Categories.tsx
│   │   │   ├── CategoryCard.tsx
│   │   │   └── index.ts
│   │   ├── FeaturedProducts/
│   │   │   ├── FeaturedProducts.tsx
│   │   │   ├── ProductCard.tsx
│   │   │   └── index.ts
│   │   ├── NewArrivals/
│   │   │   ├── NewArrivals.tsx
│   │   │   └── index.ts
│   │   ├── PromoBanner/
│   │   │   ├── PromoBanner.tsx
│   │   │   └── index.ts
│   │   ├── Testimonials/
│   │   │   ├── Testimonials.tsx
│   │   │   └── index.ts
│   │   └── Newsletter/
│   │       ├── Newsletter.tsx
│   │       └── index.ts
│   │
│   ├── products/
│   │   ├── ProductGrid/
│   │   │   ├── ProductGrid.tsx
│   │   │   └── index.ts
│   │   ├── ProductFilters/
│   │   │   ├── ProductFilters.tsx
│   │   │   ├── FilterSidebar.tsx
│   │   │   ├── FilterSort.tsx
│   │   │   └── index.ts
│   │   ├── ProductDetail/
│   │   │   ├── ProductDetail.tsx
│   │   │   ├── ProductGallery.tsx
│   │   │   ├── ProductInfo.tsx
│   │   │   ├── ProductActions.tsx
│   │   │   ├── ProductReviews.tsx
│   │   │   └── index.ts
│   │   └── ProductCard/
│   │       ├── ProductCard.tsx
│   │       └── index.ts
│   │
│   ├── cart/
│   │   ├── CartDrawer/
│   │   │   ├── CartDrawer.tsx
│   │   │   ├── CartItem.tsx
│   │   │   └── index.ts
│   │   ├── CartPage/
│   │   │   ├── CartPage.tsx
│   │   │   ├── CartSummary.tsx
│   │   │   └── index.ts
│   │   └── CartIcon/
│   │       ├── CartIcon.tsx
│   │       └── index.ts
│   │
│   ├── checkout/
│   │   ├── CheckoutForm/
│   │   │   ├── CheckoutForm.tsx
│   │   │   ├── ShippingForm.tsx
│   │   │   ├── PaymentForm.tsx
│   │   │   ├── OrderSummary.tsx
│   │   │   └── index.ts
│   │   └── CheckoutSuccess/
│   │       ├── CheckoutSuccess.tsx
│   │       └── index.ts
│   │
│   ├── blog/
│   │   ├── BlogGrid/
│   │   │   ├── BlogGrid.tsx
│   │   │   └── index.ts
│   │   ├── BlogCard/
│   │   │   ├── BlogCard.tsx
│   │   │   └── index.ts
│   │   └── BlogDetail/
│   │       ├── BlogDetail.tsx
│   │       └── index.ts
│   │
│   ├── account/
│   │   ├── OrderHistory/
│   │   │   ├── OrderHistory.tsx
│   │   │   ├── OrderCard.tsx
│   │   │   └── index.ts
│   │   ├── Wishlist/
│   │   │   ├── Wishlist.tsx
│   │   │   └── index.ts
│   │   └── ProfileForm/
│   │       ├── ProfileForm.tsx
│   │       └── index.ts
│   │
│   └── shared/
│       ├── Breadcrumb/
│       │   ├── Breadcrumb.tsx
│       │   └── index.ts
│       ├── Pagination/
│       │   ├── Pagination.tsx
│       │   └── index.ts
│       ├── StarRating/
│       │   ├── StarRating.tsx
│       │   └── index.ts
│       └── Price/
│           ├── Price.tsx
│           └── index.ts
│
├── hooks/
│   ├── useCart.ts
│   ├── useAuth.ts
│   ├── useWishlist.ts
│   ├── useFilters.ts
│   ├── usePagination.ts
│   ├── useMediaQuery.ts
│   ├── useScroll.ts
│   ├── useOutsideClick.ts
│   └── index.ts
│
├── lib/
│   ├── api/
│   │   ├── client.ts
│   │   ├── products.ts
│   │   ├── categories.ts
│   │   ├── auth.ts
│   │   ├── cart.ts
│   │   ├── orders.ts
│   │   └── blog.ts
│   │
│   ├── utils/
│   │   ├── formatPrice.ts
│   │   ├── formatDate.ts
│   │   ├── slugify.ts
│   │   ├── truncateText.ts
│   │   ├── validateEmail.ts
│   │   ├── validatePhone.ts
│   │   └── index.ts
│   │
│   ├── constants/
│   │   ├── navigation.ts
│   │   ├── categories.ts
│   │   ├── colors.ts
│   │   ├── payment.ts
│   │   └── index.ts
│   │
│   ├── animations/
│   │   ├── fadeIn.ts
│   │   ├── slideIn.ts
│   │   ├── scaleIn.ts
│   │   ├── stagger.ts
│   │   └── index.ts
│   │
│   └── types/
│       ├── product.ts
│       ├── category.ts
│       ├── user.ts
│       ├── order.ts
│       ├── cart.ts
│       ├── blog.ts
│       ├── api.ts
│       └── index.ts
│
├── store/
│   ├── cartStore.ts
│   ├── authStore.ts
│   ├── wishlistStore.ts
│   ├── filterStore.ts
│   └── index.ts
│
├── providers/
│   ├── ThemeProvider.tsx
│   ├── AuthProvider.tsx
│   ├── CartProvider.tsx
│   └── index.ts
│
├── styles/
│   ├── globals.css
│   └── animations.css
│
├── middleware.ts
│
├── .gitignore
├── AGENTS.md
├── CLAUDE.md
├── eslint.config.mjs
├── next-env.d.ts
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── README.md
├── tailwind.config.ts
└── tsconfig.json
```

---

## Structure des dossiers avec Next.js App Router

| Dossier | Description |
|---------|-------------|
| `app/` | Routes Next.js avec App Router |
| `app/(auth)/` | Routes d'authentification (layout spécifique sans header/footer) |
| `app/(dashboard)/` | Espace client protégé |
| `app/(shop)/` | Routes principales du e-commerce |
| `app/(info)/` | Pages informatives |
| `app/(legal)/` | Pages légales |
| `app/api/` | API Routes Next.js |
| `components/` | Composants React réutilisables |
| `hooks/` | Custom hooks |
| `lib/` | Utilitaires, API, types, constantes, animations |
| `store/` | Stores Zustand |
| `providers/` | Context providers |
| `styles/` | Fichiers CSS globaux |
| `public/` | Assets statiques |

---

## Fichiers de configuration à vérifier

```
tailwind.config.ts
next.config.ts
postcss.config.mjs
eslint.config.mjs
tsconfig.json
```

---

Tu veux que je te génère le contenu d'un dossier spécifique ou d'un fichier en particulier ?