# OTPPSCORCH
##JUST MODULES FOR POWERSHELL

ÿþ
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 #         C o p y r i g h t   ( c )   M i c r o s o f t .   A l l   r i g h t s   r e s e r v e d . 
 
 #         T h i s   c o d e   i s   l i c e n s e d   u n d e r   t h e   M i c r o s o f t   P u b l i c   L i c e n s e . 
 
 #         T H I S   C O D E   I S   P R O V I D E D   * A S   I S *   W I T H O U T   W A R R A N T Y   O F 
 
 #         A N Y   K I N D ,   E I T H E R   E X P R E S S   O R   I M P L I E D ,   I N C L U D I N G   A N Y 
 
 #         I M P L I E D   W A R R A N T I E S   O F   F I T N E S S   F O R   A   P A R T I C U L A R 
 
 #         P U R P O S E ,   M E R C H A N T A B I L I T Y ,   O R   N O N - I N F R I N G E M E N T . 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
   
 
 < # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 M o d i f i e d   -   D a v i d   W a l l i s   -   1 9 / 0 1 / 2 0 1 5 
 
 
 
 A d d e d   A d d i t i o n a l   F u n c t i o n a l i t y : 
 
 
 
 W a i t F o r R u n b o o k 
 
 G e t - R e t u r n e d D a t a 
 
 E x e c u t e R u n b o o k 
 
 N e w - P a r a m e t e r V a l u e 
 
 	 
 
 0 9 / 0 2 / 2 0 1 5   -   F i x e d   B u g   i n   g e t R u n b o o k O b j e c t   s o   t h a t 
 
 s e n d H t t p G e t R e q u e s t   p a s s e s   c r e d e n t i a l s 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # > 
 
 
 
 A d d - T y p e   - A s s e m b l y N a m e   S y s t e m . W e b 
 
 # [ r e f l e c t i o n . a s s e m b l y ] : : l o a d w i t h p a r t i a l n a m e ( " s y s t e m . w e b " ) 
 
   
 
 
 
 #   W e b   s e r v i c e   r e s o u r c e   r e c o r d s   p e r   p a g e 
 
 [ i n t ]   $ c _ R e c o r d s P e r P a g e   =   5 0 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r S e r v i c e U r l 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r S e r v i c e U r l 
 
         # 
 
         #   C r e a t e   a   c o m p l e t e   U R L   f o r   t h e   O r c h e s t r a t o r   w e b   s e r v i c e . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r S e r v i c e U r l   - S e r v e r   < s t r i n g >   [ - P o r t   < s t r i n g > ]   [ - V e r s i o n   < s t r i n g > ]   [ - Q u e r y   < s t r i n g > ]   [ - U s e S S L ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S t r i n g ]   $ S e r v e r , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S t r i n g ]   $ P o r t   =   " 8 1 " , 
 
                                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S t r i n g ]   $ V e r s i o n   =   " O r c h e s t r a t o r 2 0 1 2 " ,   
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S t r i n g ]   $ Q u e r y   =   " " , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S w i t c h ]   $ U s e S S L 
 
         ) 
 
         
 
         # d e t e r m i n e   t h e   p r o t o c o l 
 
         $ p r o t o c o l   =   $ (   i f   ( $ U s e S S L )   { " h t t p s " }   e l s e   { " h t t p " }   ) 
 
                 
 
         i f   ( $ Q u e r y   - n e   " " ) 
 
         { 
 
                 # a s s u r e   $ Q u e r y   d o e s n ' t   s t a r t   w i t h   / 
 
                 $ Q u e r y   =   $ Q u e r y . T r i m ( ) 
 
                 i f   ( $ Q u e r y . S t a r t s W i t h ( ' / ' )   - o r   $ Q u e r y . S t a r t s W i t h ( ' \ ' ) )   { $ Q u e r y   =   $ Q u e r y . S u b s t r i n g ( 1 ) }   
 
         } 
 
 
 
         r e t u r n   - j o i n   ( $ p r o t o c o l , " : / / " , $ S e r v e r , " : " , $ P o r t , " / " , $ V e r s i o n , " / O r c h e s t r a t o r . s v c / " , $ Q u e r y ) 
 
 } 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r J o b 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r J o b 
 
         # 
 
         #   G e t   a   J o b   o r   c o l l e c t i o n   o f   J o b s . 
 
         #   E a c h   J o b   i s   a   c u s t o m   P S   o b j e c t   t h a t   r e p r e s e n t s   a   J o b   e n t i t y . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r J o b   - S e r v i c e U r l   < s t r i n g >   [ - J o b I d   < g u i d > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ]   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         #       G e t - O r c h e s t r a t o r J o b   - S e r v i c e U r l   < s t r i n g >   [ - S e r v e r I d   < g u i d > ]   [ - S t a t u s   < c s v   s t r i n g > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ]   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         #       G e t - O r c h e s t r a t o r J o b   - S e r v i c e U r l   < s t r i n g >   [ - R u n b o o k I d   < g u i d > ]   [ - S t a t u s   < c s v   s t r i n g > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ]   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         #       G e t - O r c h e s t r a t o r J o b   - S e r v i c e U r l   < s t r i n g >   [ - S t a t u s   < c s v   s t r i n g > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ]   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ S t r i n g ]   $ S e r v i c e U r l , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . G u i d ]   $ J o b I d , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . G u i d ]   $ R u n b o o k I d , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . G u i d ]   $ S e r v e r I d , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S t r i n g ]   $ S t a t u s , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ I n t ]   $ P a g e   =   0 , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ I n t ]   $ M a x P a g e s   =   1 0 
 
         ) 
 
         
 
         #   C r e a t e   t h e   S t a t u s   p a r t   o f   t h e   q u e r y 
 
         $ s t a t u s q u e r y   =   " " 
 
         i f   ( - n o t   [ s t r i n g ] : : I s N u l l O r E m p t y ( $ S t a t u s ) )   { 
 
                 $ t e m p a r r a y   =   $ S t a t u s   - s p l i t   " , " 
 
                 
 
                 f o r   ( $ i   =   0 ;   $ i   - l t   $ t e m p a r r a y . C o u n t ;   $ i + + )   { 
 
                         i f   ( $ i   - g t   0 )   {   $ s t a t u s q u e r y   + =   " % 2 0 o r % 2 0 " } 
 
                         $ s t a t u s q u e r y   + =   " S t a t u s % 2 0 e q % 2 0 ' "   +   $ t e m p a r r a y [ $ i ]   +   " ' " 
 
                 } 
 
         } 
 
         
 
         #   C r e a t e   t h e   f u l l   q u e r y 
 
         i f   ( $ J o b I d   - n e   $ n u l l ) 
 
         { 
 
                 #   g e t   a   s p e c i f i c   J o b 
 
                 $ q u e r y   =   - j o i n   ( " J o b s ( g u i d ' " , $ J o b I d . T o S t r i n g ( ) , " ' ) " ) 
 
         } 
 
         e l s e i f   ( $ S e r v e r I d   - n e   $ n u l l ) 
 
         { 
 
                 #   g e t   a l l   J o b s   o n   a   s p e c i f i c   r u n b o o k   s e r v e r   [ w i t h   s p e c i f i c   s t a t u s ] 
 
                 $ q u e r y   =   - j o i n   ( " J o b s ( ) ? ` $ f i l t e r = R u n b o o k S e r v e r I d % 2 0 e q % 2 0 g u i d ' " , $ S e r v e r I d . T o S t r i n g ( ) , " ' " ) 
 
                 i f   ( - n o t   [ s t r i n g ] : : I s N u l l O r E m p t y ( $ s t a t u s q u e r y ) )   { 
 
                         $ q u e r y   =   - j o i n   ( $ q u e r y , " % 2 0 a n d % 2 0 ( " , $ s t a t u s q u e r y , " ) " ) 
 
                 } 
 
         } 
 
         e l s e i f   ( $ R u n b o o k I d   - n e   $ n u l l ) 
 
         { 
 
                 #   g e t   a l l   J o b s   f o r   a   s p e c i f i c   r u n b o o k   [ w i t h   s p e c i f i c   s t a t u s ] 
 
                 $ q u e r y   =   - j o i n   ( " J o b s ( ) ? ` $ f i l t e r = R u n b o o k I d % 2 0 e q % 2 0 g u i d ' " , $ R u n b o o k I d . T o S t r i n g ( ) , " ' " ) 
 
                 i f   ( - n o t   [ s t r i n g ] : : I s N u l l O r E m p t y ( $ s t a t u s q u e r y ) )   { 
 
                         $ q u e r y   =   - j o i n   ( $ q u e r y , " % 2 0 a n d % 2 0 ( " , $ s t a t u s q u e r y , " ) " ) 
 
                 } 
 
         } 
 
         e l s e 
 
         { 
 
                 #   g e t   a l l   J o b s   i n   t h e   s y s t e m   [ w i t h   s p e c i f i c   s t a t u s ] 
 
                 $ q u e r y   =   " J o b s ( ) " 
 
                 i f   ( - n o t   [ s t r i n g ] : : I s N u l l O r E m p t y ( $ s t a t u s q u e r y ) )   { 
 
                         $ q u e r y   =   - j o i n   ( $ q u e r y , " ? ` $ f i l t e r = " , $ s t a t u s q u e r y ) 
 
                 } 
 
         } 
 
         
 
         #   C r e a t e   t h e   f u l l   u r l 
 
         $ u r l   =   $ S e r v i c e U r l   +   $ q u e r y 
 
         
 
         $ j o b a r r a y   =   $ n u l l 
 
         i f   ( $ P a g e   - e q   0 ) 
 
         { 
 
                 #   G e t   J o b s   i n   a l l   p a g e s   u p   t o   M a x P a g e s 
 
                 f o r   ( $ p g   =   1 ;   $ p g   - l e   $ M a x P a g e s ;   $ p g + + ) 
 
                 { 
 
                         $ a   =   g e t O r c h e s t r a t o r J o b P a g e   - U r l   $ u r l   - P a g e   $ p g   - C r e d e n t i a l s   $ C r e d e n t i a l s 
 
                         $ j o b a r r a y   + =   $ a [ 0 ] 
 
                         $ m a x j o b s   =   $ a [ 1 ] 
 
 
 
                         $ l a s t R e c o r d   =   $ p g   *   $ c _ R e c o r d s P e r P a g e 
 
                         i f   ( $ l a s t R e c o r d   - g e   $ m a x j o b s )   {   b r e a k ;   }   #   N o   m o r e   j o b s   t o   g e t ,   s o   e x i t   t h e   f o r   l o o p 
 
                 } 
 
                 
 
         } 
 
         e l s e i f   ( $ P a g e   - g e   1 ) 
 
         { 
 
                 #   G e t   J o b s   i n   a   s p e c i f i c   p a g e 
 
                 $ a   =   g e t O r c h e s t r a t o r J o b P a g e   - U r l   $ u r l   - P a g e   $ P a g e   - C r e d e n t i a l s   $ C r e d e n t i a l s 
 
                 $ j o b a r r a y   =   $ a [ 0 ] 
 
         } 
 
         
 
         #   R e t u r n   t h e   a r r a y   o f   J o b   o b j e c t s 
 
         r e t u r n   $ j o b a r r a y 
 
 } 
 
 
 
 f u n c t i o n   g e t O r c h e s t r a t o r J o b P a g e 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t O r c h e s t r a t o r J o b P a g e 
 
         # 
 
         #   G e t   a   J o b   o r   c o l l e c t i o n   o f   J o b s   f o r   t h e   p a r t i c u l a r   p a g e . 
 
         # 
 
         #   U s a g e : 
 
         #       g e t O r c h e s t r a t o r J o b P a g e   - U r l   < s t r i n g >   - P a g e   < i n t >   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ S t r i n g ]   $ U r l , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ I n t ]   $ P a g e , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
 
 
         #   I s   t h i s   r e q u e s t   f o r   s i n g l e   j o b ? 
 
         [ b o o l ]   $ i s S i n g l e J o b   =   $ U r l . C o n t a i n s ( " J o b s ( g u i d " ) 
 
 
 
         i f   ( - n o t   $ i s S i n g l e J o b ) 
 
         { 
 
                 #   A d d   t h e   p a g e   q u e r y   t o   t h e   u r l 
 
                 $ j o i n c h a r   =   $ (   i f   ( $ U r l . E n d s W i t h ( " J o b s ( ) " ) )   { " ? " }   e l s e   { " & " }   ) 
 
                 $ U r l   =   - j o i n   ( $ U r l , $ j o i n c h a r , $ ( g e t P a g e Q u e r y   $ P a g e ) ) 
 
         } 
 
         
 
         #   C a l l   t h e   s e r v i c e   a n d   g e t   t h e   x m l   d o c   w i t h   J o b   i n f o r m a t i o n 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - U r l   $ U r l   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
         
 
         #   H o w   m a n y   t o t a l   j o b s   a r e   t h e r e   ( a l l   p a g e s ) 
 
         $ j o b s c o u n t t o t a l   =   $ (   i f   ( $ i s S i n g l e J o b )   { 1 }   e l s e   { g e t R e s o u r c e C o u n t ( $ x m l D o c ) }   ) 
 
         
 
         $ j o b a r r a y   =   $ n u l l 
 
         i f   (   ( ( ( $ P a g e   -   1 )   *   $ c _ R e c o r d s P e r P a g e )   - l t   $ j o b s c o u n t t o t a l )   - o r   ( $ i s S i n g l e J o b ) ) 
 
         { 
 
                 #   T h i s   p a g e   i s   w i t h i n   r a n g e 
 
                 
 
                 #   G e t   t h e   c o l l e c t i o n   o f   J o b   n o d e s 
 
                 $ j o b n o d e s   =   g e t E n t r y N o d e s   $ x m l D o c 
 
                 
 
                 #   C r e a t e   a   c u s t o m   P S O b j e c t   f o r   e a c h   J o b   a n d   a d d   e a c h   J o b   t o   a n   a r r a y 
 
                 $ j o b a r r a y   =   @ ( ) 
 
                 f o r e a c h   ( $ j o b n o d e   i n   $ j o b n o d e s ) 
 
                 { 
 
                         #   C r e a t e   a   J o b   o b j e c t   a n d   a d d   i t   t o   t h e   a r r a y 
 
                         $ j o b a r r a y   + =   g e t J o b O b j e c t   - J o b N o d e   $ j o b n o d e 
 
                 } 
 
                 i f   ( $ j o b a r r a y . L e n g t h   - e q   0 )   {   $ j o b a r r a y   =   $ n u l l   } 
 
         } 
 
         
 
         #   R e t u r n   t h e   a r r a y   o f   J o b   o b j e c t s   a n d   t h e   c o u n t   o f   t o t a l   J o b   o b j e c t s   p o s s i b l e   f o r   a l l   p a g e s 
 
         r e t u r n   @ ( $ j o b a r r a y , $ j o b s c o u n t t o t a l ) 
 
 } 
 
 
 
 f u n c t i o n   g e t J o b O b j e c t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t J o b O b j e c t 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   f o r   a   J o b   c o n s t r u c t   a   P S   c u s t o m   o b j e c t 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ J o b N o d e 
 
         ) 
 
         
 
         #   G e t   t h e   l i n k s   t o   r e l a t e d   e n t i t i e s 
 
         $ s e r v i c e b a s e u r l   =   g e t B a s e S e r v i c e U r l   $ J o b N o d e 
 
         $ l i n k n o d e s   =   $ J o b N o d e . l i n k 
 
         f o r e a c h   ( $ l i n k n o d e   i n   $ l i n k n o d e s ) 
 
         { 
 
                 s w i t c h ( $ l i n k n o d e . t i t l e ) 
 
                 { 
 
                         " R u n b o o k "   { $ r u n b o o k u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " I n s t a n c e s "   { $ i n s t a n c e s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " R u n b o o k S e r v e r "   { $ r u n b o o k s e r v e r u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                 } 
 
         } 
 
         
 
         #   G e t   t h e   r u n b o o k   p a r a m e t e r s 
 
         t r y 
 
         { 
 
                 $ p a r a m e t e r s x m l   =   [ x m l ]   $ J o b N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : P a r a m e t e r s " ) . I n n e r T e x t 
 
                 $ p a r a m e t e r n o d e s   =   $ p a r a m e t e r s x m l . I t e m ( " D a t a " ) . S e l e c t N o d e s ( " P a r a m e t e r " ) 
 
                 $ p a r a m e t e r a r r a y   =   @ ( ) 
 
                 
 
                 f o r e a c h ( $ p n   i n   $ p a r a m e t e r n o d e s ) 
 
                 { 
 
                         $ i d   =   $ p n . I t e m ( " I D " ) . I n n e r T e x t 
 
                         
 
                         $ p r o p s   =   @ { 
 
                                 ' N a m e '   =   $ p n . I t e m ( " N a m e " ) . I n n e r T e x t 
 
                                 ' I d '   =   $ i d . S u b S t r i n g ( 1 , $ i d . L e n g t h   -   2 ) 
 
                                 ' V a l u e '   =   $ p n . I t e m ( " V a l u e " ) . I n n e r T e x t 
 
                         } 
 
 
 
                         $ p a r a m e t e r a r r a y   + =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p s 
 
                 } 
 
         } 
 
         c a t c h 
 
         { 
 
                 $ p a r a m e t e r a r r a y   =   $ n u l l 
 
         } 
 
         
 
         #   C r e a t e   t h e   p r o p e r t i e s 
 
         $ p r o p n o d e   =   $ J o b N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) 
 
         $ p r o p e r t i e s   =   @ { 
 
                 ' U r l _ S e r v i c e '   =   $ s e r v i c e b a s e u r l 
 
                 ' P a r a m e t e r s '   =   $ p a r a m e t e r a r r a y 
 
                 ' U r l _ R u n b o o k '   =   $ r u n b o o k u r l 
 
                 ' U r l _ R u n b o o k I n s t a n c e s '   =   $ i n s t a n c e s u r l 
 
                 ' U r l _ R u n b o o k S e r v e r '   =   $ r u n b o o k s e r v e r u r l 
 
                 ' U r l '   =   $ J o b N o d e . i d 
 
                 ' P u b l i s h e d '   =   $ J o b N o d e . p u b l i s h e d 
 
                 ' U p d a t e d '   =   $ J o b N o d e . u p d a t e d 
 
                 ' C a t e g o r y '   =   $ J o b N o d e . c a t e g o r y . t e r m 
 
                 ' I d '   =   $ p r o p n o d e . I t e m ( " d : I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k S e r v e r s '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k S e r v e r s " ) . I n n e r T e x t 
 
                 ' R u n b o o k S e r v e r I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k S e r v e r I d " ) . I n n e r T e x t 
 
                 ' S t a t u s '   =   $ p r o p n o d e . I t e m ( " d : S t a t u s " ) . I n n e r T e x t 
 
                 ' P a r e n t I d '   =   $ p r o p n o d e . I t e m ( " d : P a r e n t I d " ) . I n n e r T e x t 
 
                 ' P a r e n t I s W a i t i n g '   =   [ b o o l ] $ p r o p n o d e . I t e m ( " d : P a r e n t I s W a i t i n g " ) . I n n e r T e x t 
 
                 ' C r e a t e d B y '   =   $ p r o p n o d e . I t e m ( " d : C r e a t e d B y " ) . I n n e r T e x t 
 
                 ' C r e a t i o n T i m e '   =   $ p r o p n o d e . I t e m ( " d : C r e a t i o n T i m e " ) . I n n e r T e x t 
 
                 ' L a s t M o d i f i e d B y '   =   $ p r o p n o d e . I t e m ( " d : L a s t M o d i f i e d B y " ) . I n n e r T e x t 
 
                 ' L a s t M o d i f i e d T i m e '   =   $ p r o p n o d e . I t e m ( " d : L a s t M o d i f i e d T i m e " ) . I n n e r T e x t                         
 
         } 
 
 
 
         #   R e t u r n   t h e   J o b   o b j e c t 
 
         $ j o b o b j e c t   =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
         r e t u r n   $ j o b o b j e c t 
 
 } 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e 
 
         # 
 
         #   G e t   a   R u n b o o k I n s t a n c e   o r   c o l l e c t i o n   o f   R u n b o o k I n s t a n c e   a s s o c i a t e d   w i t h   a   J o b . 
 
         #   T h e   R u n b o o k I n s t a n c e   i s   a   c u s t o m   P S   o b j e c t   t h a t   r e p r e s e n t s   a   R u n b o o k I n s t a n c e   r e s o u r c e . 
 
         # 
 
         #   N o t e :   N o   p a g i n g   e n a b l e d ;   s o   g e t   u p   t o   5 0   i n s t a n c e s   ( t h e   w e b   s e r v i c e   l i m i t   p e r   p a g e ) . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e   - J o b   < P S O b j e c t >   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ P S O b j e c t ]   $ J o b , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
 
 
         #   C a l l   t h e   s e r v i c e   a n d   g e t   t h e   x m l   d o c   w i t h   R u n b o o k I n s t a n c e   i n f o r m a t i o n 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - u r l   $ J o b . U r l _ R u n b o o k I n s t a n c e s   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
         
 
         #   G e t   t h e   c o l l e c t i o n   o f   R u n b o o k I n s t a n c e   n o d e s 
 
         $ i n s t a n c e n o d e s   =   g e t E n t r y N o d e s   $ x m l D o c 
 
         
 
         i f   ( $ i n s t a n c e n o d e s   - n e   $ n u l l ) 
 
         {                 
 
                 #   C r e a t e   a   c u s t o m   P S O b j e c t   f o r   e a c h   R u n b o o k I n s t a n c e   a n d   a d d   e a c h   t o   a n   a r r a y 
 
                 $ i n s t a n c e a r r a y   =   @ ( ) 
 
                 f o r e a c h   ( $ i n s t a n c e n o d e   i n   $ i n s t a n c e n o d e s ) 
 
                 { 
 
                         #   C r e a t e   a   J o b   o b j e c t   a n d   a d d   i t   t o   t h e   a r r a y 
 
                         $ i n s t a n c e a r r a y   + =   g e t R u n b o o k I n s t a n c e O b j e c t   - I n s t a n c e N o d e   $ i n s t a n c e n o d e 
 
                 } 
 
               
 
                 #   R e t u r n   t h e   a r r a y   o f   I n s t a n c e   o b j e c t s 
 
                 i f   ( $ i n s t a n c e a r r a y . L e n g t h   - e q   0 )   {   $ i n s t a n c e a r r a y   =   $ n u l l   } 
 
                 r e t u r n   $ i n s t a n c e a r r a y 
 
         } 
 
         e l s e 
 
         { 
 
                 #   T h e r e   a r e   n o   I n s t a n c e s 
 
                 r e t u r n   $ n u l l 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   g e t R u n b o o k I n s t a n c e O b j e c t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R u n b o o k I n s t a n c e O b j e c t 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   f o r   a   R u n b o o k I n s t a n c e   c o n s t r u c t   a   P S   c u s t o m   o b j e c t 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ I n s t a n c e N o d e 
 
         ) 
 
         
 
         #   G e t   t h e   l i n k s   t o   r e l a t e d   e n t i t i e s 
 
         $ u r l _ s e r v i c e   =   g e t B a s e S e r v i c e U r l   $ I n s t a n c e N o d e 
 
         $ l i n k n o d e s   =   $ I n s t a n c e N o d e . l i n k 
 
         f o r e a c h   ( $ l i n k n o d e   i n   $ l i n k n o d e s ) 
 
         { 
 
                 s w i t c h ( $ l i n k n o d e . t i t l e ) 
 
                 { 
 
                         " R u n b o o k "   { $ u r l _ r u n b o o k   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " J o b "   { $ u r l _ j o b   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " P a r a m e t e r s "   { $ u r l _ p a r a m e t e r s   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " A c t i v i t y I n s t a n c e s "   { $ u r l _ a c t i v i t y i n s t a n c e s   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " R u n b o o k S e r v e r "   { $ u r l _ r u n b o o k s e r v e r   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                 } 
 
         } 
 
         
 
         #   C r e a t e   t h e   p r o p e r t i e s 
 
         $ p r o p n o d e   =   $ I n s t a n c e N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) 
 
         $ p r o p e r t i e s   =   @ { 
 
                 ' U r l _ S e r v i c e '   =   $ u r l _ s e r v i c e 
 
                 ' U r l _ R u n b o o k '   =   $ u r l _ r u n b o o k 
 
                 ' U r l _ J o b '   =   $ u r l _ j o b 
 
                 ' U r l _ P a r a m e t e r s '   =   $ u r l _ p a r a m e t e r s 
 
                 ' U r l _ A c t i v i t y I n s t a n c e s '   =   $ u r l _ a c t i v i t y i n s t a n c e s 
 
                 ' U r l _ R u n b o o k S e r v e r '   =   $ u r l _ r u n b o o k s e r v e r 
 
                 ' U r l '   =   $ I n s t a n c e N o d e . i d 
 
                 ' P u b l i s h e d '   =   $ I n s t a n c e N o d e . p u b l i s h e d 
 
                 ' U p d a t e d '   =   $ I n s t a n c e N o d e . u p d a t e d 
 
                 ' C a t e g o r y '   =   $ I n s t a n c e N o d e . c a t e g o r y . t e r m 
 
                 ' I d '   =   $ p r o p n o d e . I t e m ( " d : I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k I d " ) . I n n e r T e x t 
 
                 ' J o b I d '   =   $ p r o p n o d e . I t e m ( " d : J o b I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k S e r v e r I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k S e r v e r I d " ) . I n n e r T e x t 
 
                 ' S t a t u s '   =   $ p r o p n o d e . I t e m ( " d : S t a t u s " ) . I n n e r T e x t 
 
                 ' C r e a t i o n T i m e '   =   $ p r o p n o d e . I t e m ( " d : C r e a t i o n T i m e " ) . I n n e r T e x t 
 
                 ' C o m p l e t i o n T i m e '   =   $ p r o p n o d e . I t e m ( " d : C o m p l e t i o n T i m e " ) . I n n e r T e x t                         
 
         } 
 
 
 
         #   R e t u r n   t h e   I n s t a n c e   o b j e c t 
 
         $ i n s t a n c e o b j e c t   =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
         r e t u r n   $ i n s t a n c e o b j e c t 
 
 } 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e P a r a m e t e r 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e P a r a m e t e r 
 
         # 
 
         #   G e t   a   R u n b o o k I n s t a n c e P a r a m e t e r   o r   c o l l e c t i o n   o f   R u n b o o k I n s t a n c e P a r a m e t e r   a s s o c i a t e d   w i t h   a   R u n b o o k I n s t a n c e . 
 
         #   T h e   R u n b o o k I n s t a n c e P a r a m e t e r   i s   a   c u s t o m   P S   o b j e c t   t h a t   r e p r e s e n t s   a   R u n b o o k I n s t a n c e P a r a m e t e r   r e s o u r c e . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e P a r a m e t e r   - R u n b o o k I n s t a n c e   < P S O b j e c t >   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ P S O b j e c t ]   $ R u n b o o k I n s t a n c e , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
 
 
         #   C a l l   t h e   s e r v i c e   a n d   g e t   t h e   x m l   d o c   w i t h   R u n b o o k I n s t a n c e   i n f o r m a t i o n 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - u r l   $ R u n b o o k I n s t a n c e . U r l _ P a r a m e t e r s   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
         
 
         #   G e t   t h e   c o l l e c t i o n   o f   R u n b o o k I n s t a n c e P a r a m e t e r   n o d e s 
 
         $ p a r a m n o d e s   =   g e t E n t r y N o d e s   $ x m l D o c 
 
         
 
         i f   ( $ p a r a m n o d e s   - n e   $ n u l l ) 
 
         {                 
 
                 #   C r e a t e   a   c u s t o m   P S O b j e c t   f o r   e a c h   R u n b o o k I n s t a n c e   a n d   a d d   e a c h   t o   a n   a r r a y 
 
                 $ p a r a m a r r a y   =   @ ( ) 
 
                 f o r e a c h   ( $ p a r a m n o d e   i n   $ p a r a m n o d e s ) 
 
                 { 
 
                         #   C r e a t e   a   J o b   o b j e c t   a n d   a d d   i t   t o   t h e   a r r a y 
 
                         $ p a r a m a r r a y   + =   g e t R u n b o o k I n s t a n c e P a r a m e t e r O b j e c t   - I n s t a n c e P a r a m e t e r N o d e   $ p a r a m n o d e 
 
                 } 
 
               
 
                 #   R e t u r n   t h e   a r r a y   o f   R u n b o o k I n s t a n c e P a r a m e t e r   o b j e c t s 
 
                 i f   ( $ p a r a m a r r a y . L e n g t h   - e q   0 )   {   $ p a r a m a r r a y   =   $ n u l l   } 
 
                 r e t u r n   $ p a r a m a r r a y 
 
         } 
 
         e l s e 
 
         { 
 
                 #   T h e r e   a r e   n o   R u n b o o k I n s t a n c e P a r a m e t e r 
 
                 r e t u r n   $ n u l l 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   g e t R u n b o o k I n s t a n c e P a r a m e t e r O b j e c t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R u n b o o k I n s t a n c e P a r a m e t e r O b j e c t 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   f o r   a   R u n b o o k I n s t a n c e P a r a m e t e r   c o n s t r u c t   a   P S   c u s t o m   o b j e c t 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ I n s t a n c e P a r a m e t e r N o d e 
 
         ) 
 
         
 
         #   G e t   t h e   l i n k s   t o   r e l a t e d   e n t i t i e s 
 
         $ u r l _ s e r v i c e   =   g e t B a s e S e r v i c e U r l   $ I n s t a n c e P a r a m e t e r N o d e 
 
         $ l i n k n o d e s   =   $ I n s t a n c e P a r a m e t e r N o d e . l i n k 
 
         f o r e a c h   ( $ l i n k n o d e   i n   $ l i n k n o d e s ) 
 
         { 
 
                 s w i t c h ( $ l i n k n o d e . t i t l e ) 
 
                 { 
 
                         " R u n b o o k I n s t a n c e "   { $ u r l _ r u n b o o k i n s t a n c e   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " R u n b o o k P a r a m e t e r "   { $ u r l _ r u n b o o k p a r a m e t e r   =   $ u r l _ s e r v i c e   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                 } 
 
         } 
 
         
 
         #   C r e a t e   t h e   p r o p e r t i e s 
 
         $ p r o p n o d e   =   $ I n s t a n c e P a r a m e t e r N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) 
 
         $ p r o p e r t i e s   =   @ { 
 
                 ' U r l _ S e r v i c e '   =   $ u r l _ s e r v i c e 
 
                 ' U r l _ R u n b o o k I n s t a n c e '   =   $ u r l _ r u n b o o k i n s t a n c e 
 
                 ' U r l _ R u n b o o k P a r a m e t e r '   =   $ u r l _ r u n b o o k p a r a m e t e r 
 
                 ' U r l '   =   $ I n s t a n c e P a r a m e t e r N o d e . i d 
 
                 ' U p d a t e d '   =   $ I n s t a n c e P a r a m e t e r N o d e . u p d a t e d 
 
                 ' C a t e g o r y '   =   $ I n s t a n c e P a r a m e t e r N o d e . c a t e g o r y . t e r m 
 
                 ' I d '   =   $ p r o p n o d e . I t e m ( " d : I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k I n s t a n c e I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k I n s t a n c e I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k P a r a m e t e r I d '   =   $ p r o p n o d e . I t e m ( " d : R u n b o o k P a r a m e t e r I d " ) . I n n e r T e x t 
 
                 ' N a m e '   =   $ p r o p n o d e . I t e m ( " d : N a m e " ) . I n n e r T e x t 
 
                 ' V a l u e '   =   $ p r o p n o d e . I t e m ( " d : V a l u e " ) . I n n e r T e x t 
 
                 ' D i r e c t i o n '   =   $ p r o p n o d e . I t e m ( " d : D i r e c t i o n " ) . I n n e r T e x t 
 
                 ' G r o u p I d '   =   $ p r o p n o d e . I t e m ( " d : G r o u p I d " ) . I n n e r T e x t                         
 
         } 
 
 
 
         #   R e t u r n   t h e   I n s t a n c e   o b j e c t 
 
         $ i n s t a n c e o b j e c t   =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
         r e t u r n   $ i n s t a n c e o b j e c t 
 
 } 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r R u n b o o k 
 
         # 
 
         #   G e t   a   R u n b o o k   o r   c o l l e c t i o n   o f   R u n b o o k s . 
 
         #   E a c h   R u n b o o k   i s   a   c u s t o m   P S   o b j e c t   t h a t   r e p r e s e n t s   a   R u n b o o k   e n t i t y . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r R u n b o o k   - S e r v i c e U r l   < s t r i n g >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ]   [ - R u n b o o k I d   < g u i d > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ] 
 
         #       G e t - O r c h e s t r a t o r R u n b o o k   - S e r v i c e U r l   < s t r i n g >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ]   [ - R u n b o o k P a t h   < s t r i n g > ]   [ - P a g e   < i n t > ]   [ - M a x P a g e s   < i n t > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S t r i n g ]   $ S e r v i c e U r l , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . G u i d ]   $ R u n b o o k I d , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S t r i n g ]   $ R u n b o o k P a t h , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ I n t ]   $ P a g e   =   0 , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ I n t ]   $ M a x P a g e s   =   1 0                         
 
         ) 
 
         
 
         #   F o r m   f u l l   U R L 
 
         i f   ( $ R u n b o o k I d   - n e   $ n u l l ) 
 
         { 
 
                 #   U r l   f o r   g e t t i n g   a   s i n g l e   r u n b o o k   b y   i t s   i d 
 
                 $ u r l   =   - j o i n   ( $ S e r v i c e U r l , " R u n b o o k s ( g u i d ' " , $ R u n b o o k I d . T o S t r i n g ( ) , " ' ) " ) 
 
                 
 
                 #   P a g e   w i l l   b e   1 
 
                 $ P a g e   =   1 
 
         } 
 
         e l s e i f   ( ( $ R u n b o o k P a t h   - n e   $ n u l l )   - a n d   ( $ R u n b o o k P a t h . L e n g t h   - g t   0 ) ) 
 
         { 
 
                 #   F o r m   t h e   q u e r y 
 
                 $ q u e r y   =   - j o i n   ( " ` $ f i l t e r = s t a r t s w i t h ( P a t h , ' " , $ R u n b o o k P a t h . T o S t r i n g ( ) , " ' ) " ) 
 
                 # $ q u e r y   =   - j o i n   ( " ` $ f i l t e r = P a t h   e q   ' " , $ R u n b o o k P a t h . T o S t r i n g ( ) , " ' " ) 
 
                 $ q u e r y   =   [ S y s t e m . W e b . H t t p U t i l i t y ] : : U r l P a t h E n c o d e ( $ q u e r y ) 
 
                 
 
                 
 
                 #   U r l   f o r   g e t t i n g   o n e   o r   m o r e   r u n b o o k s   b y   p a t h 
 
                 $ u r l   =   - j o i n   ( $ S e r v i c e U r l , " R u n b o o k s ( ) ? " , $ q u e r y )                 
 
         } 
 
         e l s e 
 
         { 
 
                 #   U r l   f o r   a l l   r u n b o o k s 
 
                 $ u r l   =   $ S e r v i c e U r l   +   " R u n b o o k s ( ) " 
 
         } 
 
         
 
         # # #   H a n d l e   p a g i n g 
 
         $ r b a r r a y   =   $ n u l l 
 
         i f   ( $ P a g e   - e q   0 ) 
 
         { 
 
                 #   G e t   R u n b o o k s   i n   a l l   p a g e s   u p   t o   M a x P a g e s 
 
                 f o r   ( $ p g   =   1 ;   $ p g   - l e   $ M a x P a g e s ;   $ p g + + ) 
 
                 { 
 
                         $ a   =   g e t O r c h e s t r a t o r R u n b o o k P a g e   - U r l   $ u r l   - P a g e   $ p g   - C r e d e n t i a l s   $ C r e d e n t i a l s 
 
 	 	 	 $ r b a r r a y   + =   $ a [ 0 ] 
 
                         $ m a x r b s   =   $ a [ 1 ] 
 
 
 
                         $ l a s t R e c o r d   =   $ p g   *   $ c _ R e c o r d s P e r P a g e 
 
                         i f   ( $ l a s t R e c o r d   - g e   $ m a x r b s )   {   b r e a k ;   }   #   N o   m o r e   j o b s   t o   g e t ,   s o   e x i t   t h e   f o r   l o o p 
 
                 }   
 
         } 
 
         e l s e i f   ( $ P a g e   - g e   1 ) 
 
         { 
 
                 #   G e t   R u n b o o k s   i n   a   s p e c i f i c   p a g e 
 
                 $ a   =   g e t O r c h e s t r a t o r R u n b o o k P a g e   - U r l   $ u r l   - P a g e   $ P a g e   - C r e d e n t i a l s   $ C r e d e n t i a l s 	 
 
                 $ r b a r r a y   =   $ a [ 0 ] 
 
         } 
 
         #   R e t u r n   t h e   a r r a y   o f   R u n b o o k   o b j e c t s 
 
         r e t u r n   $ r b a r r a y 
 
 } 
 
 
 
 f u n c t i o n   g e t O r c h e s t r a t o r R u n b o o k P a g e 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t O r c h e s t r a t o r R u n b o o k P a g e 
 
         # 
 
         #   G e t   a   R u n b o o k   o r   c o l l e c t i o n   o f   R u n b o o k s   f o r   a   p a r t i c u l a r   p a g e 
 
         # 
 
         #   U s a g e : 
 
         #       g e t O r c h e s t r a t o r R u n b o o k P a g e   - U r l   < s t r i n g >   - P a g e   < i n t >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ S t r i n g ]   $ U r l , 
 
 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ I n t ]   $ P a g e , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
 
 
         #   I s   t h i s   r e q u e s t   f o r   s i n g l e   r u n b o o k ? 
 
         $ i s S i n g l e R u n b o o k   =   $ U r l . C o n t a i n s ( " R u n b o o k s ( g u i d " ) 
 
 
 
         i f   ( - n o t   $ i s S i n g l e R u n b o o k ) 
 
         { 
 
                 #   A d d   t h e   p a g e   q u e r y   t o   t h e   u r l 
 
                 $ j o i n c h a r   =   $ (   i f   ( $ U r l . E n d s W i t h ( " R u n b o o k s ( ) " ) )   { " ? " }   e l s e   { " & " }   ) 
 
                 $ U r l   =   - j o i n   ( $ U r l , $ j o i n c h a r , $ ( g e t P a g e Q u e r y   $ P a g e ) ) 
 
         } 
 
         
 
         #   C a l l   t h e   s e r v i c e   a n d   g e t   t h e   x m l   d o c   w i t h   R u n b o o k   r e c o r d s 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - u r l   $ U r l   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
         
 
 	 i f   ( $ x m l D o c   - e q   $ n u l l ) { 
 
 	 	 W r i t e - D e b u g   ' $ x m l D o c   i s   $ n u l l   f r o m   s e n d H t t p G e t R e q u e s t   w i t h i n   g e t O r c h e s t r a t o r R u n b o o k P a g e ' 
 
 	 	 w r i t e - v e r b o s e   " N o   D a t a   R e t u r n e d   f r o m   s e n d H t t p G e t R e q u e s t " 
 
 	 	 #   t h r o w   " N o   R e s p o n s e   f r o m   s e n d H t t p G e t R e q u e s t " 
 
 	 } 
 
 	 
 
 	 
 
         #   H o w   m a n y   t o t a l   r u n b o o k s   a r e   t h e r e   ( a l l   p a g e s ) 
 
         $ r b c o u n t t o t a l   =   $ (   i f ( $ i s S i n g l e R u n b o o k )   { 1 }   e l s e   { g e t R e s o u r c e C o u n t ( $ x m l D o c ) }   ) 
 
 
 
         $ r b a r r a y   =   $ n u l l 
 
         i f   (   ( ( ( $ P a g e   -   1 )   *   $ c _ R e c o r d s P e r P a g e )   - l t   $ r b c o u n t t o t a l )   - o r   $ i s S i n g l e R u n b o o k   ) 
 
         { 
 
                 #   T h i s   p a g e   i s   w i t h i n   r a n g e 
 
                 
 
                 #   G e t   t h e   R u n b o o k   n o d e s 
 
                 $ r b n o d e s   =   g e t E n t r y N o d e s   $ x m l D o c 
 
                 
 
                 #   C r e a t e   a   c u s t o m   P S O b j e c t   f o r   e a c h   R u n b o o k   a n d   a d d   e a c h   R u n b o o k   t o   a n   a r r a y 
 
                 $ r b a r r a y   =   @ ( ) 
 
                 f o r e a c h   ( $ r b n o d e   i n   $ r b n o d e s ) 
 
                 { 
 
                         #   C r e a t e   a   R u n b o o k   o b j e c t   a n d   a d d   i t   t o   t h e   a r r a y 
 
                         $ r b a r r a y   + =   g e t R u n b o o k O b j e c t   $ r b n o d e 
 
                 } 
 
                 
 
                 i f   ( $ r b a r r a y . L e n g t h   - e q   0 )   {   $ r b a r r a y   =   $ n u l l   } 
 
         } 
 
         
 
         #   R e t u r n   t h e   a r r a y   o f   R u n b o o k   o b j e c t s   a n d   t h e   c o u n t   o f   t o t a l   R u n b o o k   o b j e c t s   p o s s i b l e   f o r   a l l   p a g e s 
 
         r e t u r n   @ ( $ r b a r r a y , $ r b c o u n t t o t a l ) 
 
 } 
 
 
 
 f u n c t i o n   g e t R u n b o o k O b j e c t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R u n b o o k O b j e c t 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   f o r   a   R u n b o o k   c o n s t r u c t   a   P S   c u s t o m   o b j e c t 
 
         # 
 
         #   U s a g e : 
 
         #       g e t R u n b o o k O b j e c t   - R b N o d e   < x m l e l e m e n t > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ R b N o d e 
 
         ) 
 
         
 
         #   G e t   t h e   l i n k s   t o   r e l a t e d   e n t i t i e s 
 
         $ s e r v i c e b a s e u r l   =   g e t B a s e S e r v i c e U r l   $ R b N o d e 
 
         $ l i n k n o d e s   =   $ R b N o d e . l i n k 
 
         f o r e a c h   ( $ l i n k n o d e   i n   $ l i n k n o d e s ) 
 
         { 
 
                 s w i t c h ( $ l i n k n o d e . t i t l e ) 
 
                 { 
 
                         " F o l d e r "   { $ f o l d e r u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " P a r a m e t e r s "   { $ p a r a m e t e r s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " A c t i v i t i e s "   { $ a c t i v i t i e s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " J o b s "   { $ j o b s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " I n s t a n c e s "   { $ i n s t a n c e s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " D i a g r a m "   { $ d i a g r a m u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                 } 
 
         } 
 
         
 
         #   G e t   t h e   r u n b o o k   p a r a m e t e r s   ( N a m e ,   I d ,   T y p e ,   D e s c r i p t i o n ) 
 
         # 
 
         #   C a l l   t h e   s e r v i c e   t o   g e t   P a r a m e t e r s   i n f o   f o r   t h i s   r u n b o o k 
 
         $ p m u r l   =   $ p a r a m e t e r s u r l 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - u r l   $ p m u r l   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
 
 
         #   G e t   t h e   P a r a m e t e r   n o d e s 
 
         $ p m n o d e s   =   g e t E n t r y N o d e s   $ x m l D o c 
 
 
 
         #   I f   t h e r e   a r e   p a r a m e t e r s   t h e n   g e t   t h e   i n f o 
 
         i f   ( $ p m n o d e s   - n e   $ n u l l ) 
 
         { 
 
                 $ p a r a m e t e r a r r a y   =   @ ( ) 
 
                 f o r e a c h ( $ p n   i n   $ p m n o d e s ) 
 
                 { 
 
                         $ p a r a m e t e r a r r a y   + =   g e t R u n b o o k P a r a m e t e r O b j e c t   $ p n 
 
                 } 
 
         } 
 
         e l s e 
 
         { 
 
                 #   N o   p a r a m e t e r s ,   s o   s e t   t o   n u l l 
 
                 $ p a r a m e t e r a r r a y   =   $ n u l l 
 
         } 
 
         
 
         $ p r o p n o d e   =   $ R b N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) 
 
         $ p r o p e r t i e s   =   @ { 
 
                 ' U r l _ S e r v i c e '   =   $ s e r v i c e b a s e u r l 
 
                 ' P a r a m e t e r s '   =   $ p a r a m e t e r a r r a y 
 
                 ' U r l _ F o l d e r '   =   $ f o l d e r u r l 
 
                 ' U r l _ P a r a m e t e r s '   =   $ p a r a m e t e r s u r l 
 
                 ' U r l _ A c t i v i t i e s '   =   $ a c t i v i t i e s u r l 
 
                 ' U r l _ J o b s '   =   $ j o b s u r l 
 
                 ' U r l _ I n s t a n c e s '   =   $ i n s t a n c e s u r l 
 
                 ' U r l _ D i a g r a m '   =   $ d i a g r a m u r l 
 
                 ' U r l '   =   $ R b N o d e . i d 
 
                 ' P u b l i s h e d '   =   $ R b N o d e . p u b l i s h e d 
 
                 ' U p d a t e d '   =   $ R b N o d e . u p d a t e d 
 
                 ' C a t e g o r y '   =   $ R b N o d e . c a t e g o r y . t e r m 
 
                 ' N a m e '   =   $ p r o p n o d e . I t e m ( " d : N a m e " ) . I n n e r T e x t 
 
                 ' I d '   =   $ p r o p n o d e . I t e m ( " d : I d " ) . I n n e r T e x t 
 
                 ' F o l d e r I d '   =   $ p r o p n o d e . I t e m ( " d : F o l d e r I d " ) . I n n e r T e x t 
 
                 ' D e s c r i p t i o n '   =   $ p r o p n o d e . I t e m ( " d : D e s c r i p t i o n " ) . I n n e r T e x t 
 
                 ' C r e a t e d B y '   =   $ p r o p n o d e . I t e m ( " d : C r e a t e d B y " ) . I n n e r T e x t 
 
                 ' C r e a t i o n T i m e '   =   $ p r o p n o d e . I t e m ( " d : C r e a t i o n T i m e " ) . I n n e r T e x t 
 
                 ' L a s t M o d i f i e d B y '   =   $ p r o p n o d e . I t e m ( " d : L a s t M o d i f i e d B y " ) . I n n e r T e x t 
 
                 ' L a s t M o d i f i e d T i m e '   =   $ p r o p n o d e . I t e m ( " d : L a s t M o d i f i e d T i m e " ) . I n n e r T e x t 
 
                 ' I s M o n i t o r '   =   [ S y s t e m . C o n v e r t ] : : T o B o o l e a n ( $ p r o p n o d e . I t e m ( " d : I s M o n i t o r " ) . I n n e r T e x t ) 
 
                 ' P a t h '   =   $ p r o p n o d e . I t e m ( " d : P a t h " ) . I n n e r T e x t 
 
                 ' C h e c k e d O u t B y '   =   $ p r o p n o d e . I t e m ( " d : C h e c k e d O u t B y " ) . I n n e r T e x t 
 
                 ' C h e c k e d O u t T i m e '   =   $ p r o p n o d e . I t e m ( " d : C h e c k e d O u t T i m e " ) . I n n e r T e x t 
 
         } 
 
         
 
         $ r b o b j e c t   =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
         r e t u r n   $ r b o b j e c t 
 
 } 
 
 
 
 f u n c t i o n   g e t R u n b o o k P a r a m e t e r O b j e c t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R u n b o o k P a r a m e t e r O b j e c t 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   f o r   a   R u n b o o k   P a r a m e t e r   c o n s t r u c t   a   P S   c u s t o m   o b j e c t 
 
         # 
 
         #   U s a g e : 
 
         #       g e t R u n b o o k P a r a m e t e r O b j e c t   - R b P a r a m N o d e   < x m l e l e m e n t > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ R b P a r a m N o d e 
 
         ) 
 
         
 
         #   G e t   t h e   l i n k s   t o   r e l a t e d   e n t i t i e s 
 
         $ s e r v i c e b a s e u r l   =   g e t B a s e S e r v i c e U r l   $ R b P a r a m N o d e 
 
         $ l i n k n o d e s   =   $ R b P a r a m N o d e . l i n k 
 
         f o r e a c h   ( $ l i n k n o d e   i n   $ l i n k n o d e s ) 
 
         { 
 
                 s w i t c h ( $ l i n k n o d e . t i t l e ) 
 
                 { 
 
                         " R u n b o o k "   { $ r u n b o o k u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                         " I n s t a n c e s "   { $ i n s t a n c e s u r l   =   $ s e r v i c e b a s e u r l   +   $ l i n k n o d e . h r e f ;   b r e a k } 
 
                 } 
 
         } 
 
                 
 
         #   C r e a t e   t h e   p r o p e r t i e s 
 
         $ p r o p e r t i e s   =   @ { 
 
                 ' R u n b o o k U r l '   =   $ r u n b o o k u r l 
 
                 ' I n s t a n c e s U r l '   =   $ i n s t a n c e s u r l 
 
                 ' U r l '   =   $ R b P a r a m N o d e . i d 
 
                 ' U p d a t e d '   =   $ R b P a r a m N o d e . u p d a t e d 
 
                 ' C a t e g o r y '   =   $ R b P a r a m N o d e . c a t e g o r y . t e r m 
 
                 ' I d '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : I d " ) . I n n e r T e x t 
 
                 ' R u n b o o k I d '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : R u n b o o k I d " ) . I n n e r T e x t 
 
                 ' N a m e '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : N a m e " ) . I n n e r T e x t 
 
                 ' T y p e '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : T y p e " ) . I n n e r T e x t 
 
                 ' D e s c r i p t i o n '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : D e s c r i p t i o n " ) . I n n e r T e x t 
 
                 ' D i r e c t i o n '   =   $ R b P a r a m N o d e . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : D i r e c t i o n " ) . I n n e r T e x t                         
 
         } 
 
 
 
         #   R e t u r n   t h e   R u n b o o k P a r a m e t e r   o b j e c t 
 
         $ r b p o b j e c t   =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
         r e t u r n   $ r b p o b j e c t 
 
 } 
 
 
 
 f u n c t i o n   S t o p - O r c h e s t r a t o r J o b 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   S t o p - O r c h e s t r a t o r J o b 
 
         # 
 
         #   S t o p   a   J o b 
 
         # 
 
         #   U s a g e : 
 
         #       S t o p - O r c h e s t r a t o r J o b   - J o b   < j o b >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ P S O b j e c t ]   $ J o b , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
 
 
         p r o c e s s 
 
         { 
 
                 #   C o n t i n u e   o n l y   i f   t h e   J o b   i s   n o t   a l r e a d y   s t o p p e d 
 
                 i f   ( - n o t   (   ( $ J o b . S t a t u s   - e q   " P e n d i n g " )   - o r   ( $ J o b . S t a t u s   - e q   " R u n n i n g " )   )   ) 
 
                 { 
 
                         r e t u r n   $ f a l s e 
 
                 } 
 
         
 
                 # 
 
                 #   C r e a t e   t h e   r e q u e s t   o b j e c t 
 
                 # 
 
                 $ r e q u e s t   =   [ S y s t e m . N e t . H t t p W e b R e q u e s t ] : : C r e a t e ( $ J o b . U r l ) 
 
 
 
                 #   S e t   t h e   c r e d e n t i a l s 
 
                 i f   ( $ C r e d e n t i a l s   - e q   $ n u l l ) 
 
                 { 
 
                         $ r e q u e s t . U s e D e f a u l t C r e d e n t i a l s   =   $ t r u e 
 
                 } 
 
                 e l s e 
 
                 { 
 
                         $ r e q u e s t . C r e d e n t i a l s   =   $ C r e d e n t i a l s 
 
                 } 
 
 
 
                 $ r e q u e s t . T i m e o u t   =   3 6 0 0 0 
 
 
 
                 #   B u i l d   t h e   r e q u e s t   h e a d e r 
 
                 $ r e q u e s t . M e t h o d   =   " P O S T " 
 
                 $ r e q u e s t . U s e r A g e n t   =   g e t U s e r A g e n t 
 
                 $ r e q u e s t . A c c e p t   =   " a p p l i c a t i o n / a t o m + x m l , a p p l i c a t i o n / x m l " 
 
                 $ r e q u e s t . C o n t e n t T y p e   =   " a p p l i c a t i o n / a t o m + x m l " 
 
                 $ r e q u e s t . K e e p A l i v e   =   $ t r u e 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " A c c e p t - E n c o d i n g " , " i d e n t i t y " ) 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " A c c e p t - L a n g u a g e " , " e n - U S " ) 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " D a t a S e r v i c e V e r s i o n " , " 1 . 0 ; N e t F x " ) 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " M a x D a t a S e r v i c e V e r s i o n " , " 3 . 0 ; N e t F x " ) 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " P r a g m a " , " n o - c a c h e " ) 
 
                 
 
                 #   A d d   h e a d e r   p r o p e r t i e s   s p e c i f i c   f o r   S t o p   J o b 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " X - H T T P - M e t h o d " , " M E R G E " ) 
 
                 #   t h i s   i s   t h e   L a s t M o d i f i e d T i m e 
 
                 $ l a s t m o d i f i e d t i m e   =   $ J o b . L a s t M o d i f i e d T i m e 
 
                 #   c h a n g e   " : "   t o   " % 3 A " 
 
                 $ l m t i m e   =   $ l a s t m o d i f i e d t i m e . R e p l a c e ( " : " , " % 3 A " ) 
 
                 $ t e m p s t r i n g   =   - j o i n   ( " W / "   ,   ' " '   ,   " d a t e t i m e ' "   ,   $ l m t i m e   ,   " ' "   ,   ' " ' ) 
 
                 $ r e q u e s t . H e a d e r s . A d d ( " I f - M a t c h " , $ t e m p s t r i n g ) 
 
 
 
                 # 
 
                 #   B u i l d   t h e   r e q u e s t   b o d y 
 
                 # 
 
                 #   F i r s t   r e q u e s t   t h e   j o b   f r o m   t h e   O r c h e s t r a t o r   s e r v i c e   a n d   g e t   t h e   r a w   r e s p o n s e   t h a t   w e   w i l l   m o d i f y 
 
                 #   C a l l   t h e   s e r v i c e   a n d   g e t   t h e   x m l   d o c   w i t h   J o b   i n f o r m a t i o n 
 
                 [ x m l ]   $ j o b x m l   =   s e n d H t t p G e t R e q u e s t   - u r l   $ J o b . U r l   - c r e d e n t i a l s   $ c r e d e n t i a l s         
 
                 
 
                 #   S e t   < p u b l i s h e d >   t o   C r e a t i o n T i m e 
 
                 $ j o b x m l . D o c u m e n t E l e m e n t . I t e m ( " p u b l i s h e d " ) . I n n e r T e x t   =   $ J o b . C r e a t i o n T i m e   +   " Z " 
 
                 
 
                 #   S e t   < u p d a t e d >   t o   L a s t M o d i f i e d T i m e 
 
                 $ j o b x m l . D o c u m e n t E l e m e n t . I t e m ( " u p d a t e d " ) . I n n e r T e x t   =   $ J o b . L a s t M o d i f i e d T i m e     +   " Z " 
 
                 
 
                 #   S e t   < d : S t a t u s >   t o   " C a n c e l e d "   ( t h i s   i s   w h a t   s t o p s   t h e   J o b ) 
 
                 $ j o b x m l . D o c u m e n t E l e m e n t . I t e m ( " c o n t e n t " ) . I t e m ( " m : p r o p e r t i e s " ) . I t e m ( " d : S t a t u s " ) . I n n e r T e x t   =   " C a n c e l e d " 
 
                 
 
                 #   R e m o v e   t h e   < l i n k >   n o d e s 
 
                 $ l i n k n o d e   =   $ j o b x m l . D o c u m e n t E l e m e n t . I t e m ( " l i n k " ) 
 
                 w h i l e   ( $ l i n k n o d e   - n e   $ n u l l ) 
 
                 { 
 
                         $ j o b x m l . D o c u m e n t E l e m e n t . R e m o v e C h i l d ( $ l i n k n o d e ) 
 
                         $ l i n k n o d e   =   $ j o b x m l . D o c u m e n t E l e m e n t . I t e m ( " l i n k " ) 
 
                 } 
 
 
 
                 #   E x e c u t e   t h e   s e r v i c e   r e q u e s t   a n d   g e t   t h e   r e s p o n s e 
 
                 [ S y s t e m . N e t . H t t p W e b R e s p o n s e ] $ r e s p o n s e   =   s e n d H t t p P o s t R e q u e s t   - R e q u e s t   $ r e q u e s t   - R e q u e s t B o d y   $ j o b x m l . g e t _ o u t e r x m l ( ) 
 
 
 
                 r e t u r n   ( $ r e s p o n s e . S t a t u s C o d e   - e q   " N o C o n t e n t " ) 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   S t a r t - O r c h e s t r a t o r R u n b o o k 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   S t a r t - O r c h e s t r a t o r R u n b o o k 
 
         # 
 
         #   S t a r t   a n   i n s t a n c e   o f   a   r u n b o o k 
 
         # 
 
         #   U s a g e : 
 
         #       S t a r t - O r c h e s t r a t o r R u n b o o k   - R u n b o o k   < r u n b o o k >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ]   [ - P a r a m e t e r s   < h a s h t a b l e > ]   [ - R u n b o o k S e r v e r s   < c s v   s t r i n g > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ P S O b j e c t ]   $ R u n b o o k , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ S t r i n g ]   $ R u n b o o k S e r v e r s , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                         [ h a s h t a b l e ]   $ P a r a m e t e r s                   
 
         ) 
 
         #   I f   t h i s   i s   m o n i t o r   r u n b o o k ,   a s s u r e   i t   d o e s   n o t   a l r e a d y   h a v e   a   j o b 
 
         i f   ( $ R u n b o o k . I s M o n i t o r ) 
 
         { 
 
                 W r i t e - H o s t   " R u n b o o k . I s M o n i t o r   =   "   $ R u n b o o k . I s M o n i t o r 
 
                 
 
                 $ m o n j o b   =   G e t - O r c h e s t r a t o r J o b   - r u n b o o k i d   $ R u n b o o k . I d   - s t a t u s   " R u n n i n g , P e n d i n g "   - s e r v i c e u r l   $ R u n b o o k . U r l _ S e r v i c e   - c r e d e n t i a l s   $ C r e d e n t i a l s   
 
                 i f   ( $ m o n j o b   - n e   $ n u l l ) 
 
                 { 
 
                         W r i t e - H o s t   " M o n i t o r   a l r e a d y   h a s   r u n n i n g   j o b :   "   $ m o n j o b . I d 
 
                         r e t u r n   $ n u l l 
 
                 }                 
 
         } 
 
 
 
         #   C r e a t e   t h e   r e q u e s t   o b j e c t 
 
         $ r e q u e s t   =   [ S y s t e m . N e t . H t t p W e b R e q u e s t ] : : C r e a t e ( $ R u n b o o k . U r l _ S e r v i c e   +   " J o b s " ) 
 
 
 
         #   S e t   t h e   c r e d e n t i a l s 
 
         i f   ( $ C r e d e n t i a l s   - e q   $ n u l l ) 
 
         { 
 
                 $ r e q u e s t . U s e D e f a u l t C r e d e n t i a l s   =   $ t r u e 
 
         } 
 
         e l s e 
 
         { 
 
                 $ r e q u e s t . C r e d e n t i a l s   =   $ C r e d e n t i a l s 
 
         } 
 
 
 
         $ r e q u e s t . T i m e o u t   =   3 6 0 0 0 
 
 
 
         #   B u i l d   t h e   r e q u e s t   h e a d e r 
 
         $ r e q u e s t . M e t h o d   =   " P O S T " 
 
         $ r e q u e s t . U s e r A g e n t   =   g e t U s e r A g e n t 
 
         $ r e q u e s t . A c c e p t   =   " a p p l i c a t i o n / a t o m + x m l , a p p l i c a t i o n / x m l " 
 
         $ r e q u e s t . C o n t e n t T y p e   =   " a p p l i c a t i o n / a t o m + x m l " 
 
         $ r e q u e s t . K e e p A l i v e   =   $ t r u e 
 
         $ r e q u e s t . H e a d e r s . A d d ( " A c c e p t - E n c o d i n g " , " i d e n t i t y " ) 
 
         $ r e q u e s t . H e a d e r s . A d d ( " A c c e p t - L a n g u a g e " , " e n - U S " ) 
 
         $ r e q u e s t . H e a d e r s . A d d ( " D a t a S e r v i c e V e r s i o n " , " 1 . 0 ; N e t F x " ) 
 
         $ r e q u e s t . H e a d e r s . A d d ( " M a x D a t a S e r v i c e V e r s i o n " , " 2 . 0 ; N e t F x " ) 
 
         $ r e q u e s t . H e a d e r s . A d d ( " P r a g m a " , " n o - c a c h e " ) 
 
 
 
         #   G e t   t h e   R u n b o o k I d 
 
         $ r b i d   =   $ R u n b o o k . I d 
 
         
 
         #   F o r m a t   t h e   R u n b o o k S e r v e r s   s t r i n g ,   i f   a n y 
 
         $ r b s e r v e r s t r i n g   =   " " 
 
         i f   ( - n o t   [ s t r i n g ] : : I s N u l l O r E m p t y ( $ R u n b o o k S e r v e r s ) )   { 
 
                 $ r b s e r v e r s t r i n g   =   - j o i n   ( " < d : R u n b o o k S e r v e r s > " , $ R u n b o o k S e r v e r s , " < / d : R u n b o o k S e r v e r s > " ) 
 
         } 
 
 	 
 
         #   F o r m a t   t h e   R u n b o o k   p a r a m e t e r s ,   i f   a n y 
 
         $ r b p a r a m s t r i n g   =   " " 
 
         i f   ( $ P a r a m e t e r s   - n e   $ n u l l )   { 
 
                 #   F o r m a t   t h e   p a r a m   s t r i n g   f r o m   t h e   P a r a m e t e r s   h a s h t a b l e 
 
                 $ r b p a r a m s t r i n g   =   " < d : P a r a m e t e r s > & l t ; D a t a & g t ; " 
 
                 f o r e a c h   ( $ p   i n   $ P a r a m e t e r s . G e t E n u m e r a t o r ( ) ) 
 
                 { 
 
                         $ r b p a r a m s t r i n g   =   - j o i n   ( $ r b p a r a m s t r i n g , " & l t ; P a r a m e t e r & g t ; & l t ; I D & g t ; { " , $ p . k e y , " } & l t ; / I D & g t ; & l t ; V a l u e & g t ; " , $ p . v a l u e , " & l t ; / V a l u e & g t ; & l t ; / P a r a m e t e r & g t ; " ) 
 
                 } 
 
                 $ r b p a r a m s t r i n g   + =   " & l t ; / D a t a & g t ; < / d : P a r a m e t e r s > " 
 
         } 
 
         
 
         #   B u i l d   t h e   r e q u e s t   b o d y 
 
         $ r e q u e s t B o d y   =   @ " 
 
 < ? x m l   v e r s i o n = " 1 . 0 "   e n c o d i n g = " u t f - 8 "   s t a n d a l o n e = " y e s " ? > 
 
 < e n t r y   x m l n s : d = " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s "   x m l n s : m = " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s / m e t a d a t a "   x m l n s = " h t t p : / / w w w . w 3 . o r g / 2 0 0 5 / A t o m " > 
 
         < c o n t e n t   t y p e = " a p p l i c a t i o n / x m l " > 
 
                 < m : p r o p e r t i e s > 
 
                         < d : R u n b o o k I d   m : t y p e = " E d m . G u i d " > $ r b i d < / d : R u n b o o k I d > 
 
                         $ r b s e r v e r s t r i n g 
 
                         $ r b p a r a m s t r i n g 
 
                 < / m : p r o p e r t i e s > 
 
         < / c o n t e n t > 
 
 < / e n t r y > 
 
 " @ 
 
   
 
 	 #   E x e c u t e   t h e   s e r v i c e   r e q u e s t   a n d   g e t   t h e   r e s p o n s e 
 
         $ r e s p o n s e   =   s e n d H t t p P o s t R e q u e s t   - R e q u e s t   $ r e q u e s t   - R e q u e s t B o d y   $ r e q u e s t B o d y 
 
 
 
         $ j o b   =   $ n u l l 
 
         i f   ( $ r e s p o n s e   - n e   $ n u l l ) 
 
         { 
 
                 #   G e t   t h e   r e s p o n s e   x m l   w i t h   t h e   J o b   n o d e 
 
               
 
                 $ r e s p o n s e X m l   =   g e t R e s p o n s e X m l   $ r e s p o n s e 
 
                 $ r e s p o n s e . C l o s e ( ) 
 
                 $ j o b n o d e   =   g e t E n t r y N o d e s   $ r e s p o n s e X m l 
 
                 
 
                 #   R e t u r n   t h e   J o b   t h a t   w a s   c r e a t e d 
 
                 $ j o b   =   g e t J o b O b j e c t   $ j o b n o d e 
 
         } 
 
         
 
         r e t u r n   $ j o b 
 
 } 
 
 
 
 f u n c t i o n   G e t - O r c h e s t r a t o r C o l l e c t i o n 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   G e t - O r c h e s t r a t o r C o l l e c t i o n 
 
         # 
 
         #   G e t   a n   a r r a y   l i s t   w i t h   a l l   o f   t h e   c o l l e c t i o n s   e x p o s e d   b y   t h e   O r c h e s t r a t o r   O D a t a   w e b   s e r v i c e . 
 
         #   E a c h   c o l l e c t i o n   o b j e c t   c o n t a i n s   t h e   T i t l e   a n d   U r l   p r o p e r t i e s . 
 
         # 
 
         #   U s a g e : 
 
         #       G e t - O r c h e s t r a t o r C o l l e c t i o n   - S e r v i c e U r l   < s t r i n g >   [ - C r e d e n t i a l s   < c r e d e n t i a l s > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ s t r i n g ]   $ S e r v i c e U r l , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
 	 ) 
 
         
 
         #   G e t   t h e   s e r v i c e   p a g e   x m l   d o c u m e n t   f r o m   t h e   s e r v i c e 
 
         [ x m l ]   $ x m l D o c   =   s e n d H t t p G e t R e q u e s t   - u r l   $ S e r v i c e U r l   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
 
 
         #   G e t   t h e   " c o l l e c t i o n "   x m l   n o d e s   ( / s e r v i c e / w o r k s p a c e / c o l l e c t i o n ) 
 
         $ c o l l e c t i o n n o d e s   =   $ x m l D o c . s e r v i c e . w o r k s p a c e . c o l l e c t i o n 
 
         
 
         i f   ( $ c o l l e c t i o n n o d e s   - n e   $ n u l l ) 
 
         { 
 
                 #   C r e a t e   a n   a r r a y   t h a t   w i l l   h o l d   a l l   t h e   x m l   c o l l e c t i o n   n o d e s 
 
                 $ c o l l e c t i o n a r r a y   =   @ ( ) 
 
 
 
                 #   C r e a t e   a   c u s t o m   P S O b j e c t   f o r   e a c h   c o l l e c t i o n   a n d   a d d   e a c h   t o   t h e   a r r a y 
 
                 f o r e a c h   ( $ c o l l e c t i o n n o d e   i n   $ c o l l e c t i o n n o d e s ) 
 
                 { 
 
                         $ p r o p e r t i e s   =   @ { 
 
                                 ' T i t l e '   =   $ c o l l e c t i o n n o d e . t i t l e 
 
                                 ' U r l '   =   $ S e r v i c e U r l   +   $ c o l l e c t i o n n o d e . h r e f 
 
                         } 
 
                         
 
                         $ c o l l e c t i o n a r r a y   + =   N e w - O b j e c t   P S O b j e c t   - P r o p e r t y   $ p r o p e r t i e s 
 
                 } 
 
               
 
                 #   R e t u r n   t h e   a r r a y   o f   c o l l e c t i o n   o b j e c t s 
 
                 r e t u r n   $ c o l l e c t i o n a r r a y 
 
         } 
 
         e l s e 
 
         { 
 
                 #   N o   c o l l e c t i o n s ,   s o   r e t u r n   n u l l 
 
                 r e t u r n   $ n u l l 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   G e t - C r e d e n t i a l s 
 
 { 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ s t r i n g ]   $ D o m a i n , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ s t r i n g ]   $ U s e r n a m e , 
 
                                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ s t r i n g ]   $ P a s s w o r d 
 
 	 ) 
 
         
 
         i f   ( - n o t ( [ s t r i n g ] : : I s N u l l O r E m p t y ( $ P a s s w o r d ) ) ) 
 
         { 
 
                 r e t u r n   N e w - O b j e c t   S y s t e m . N e t . N e t w o r k C r e d e n t i a l ( $ U s e r n a m e , $ P a s s w o r d , $ D o m a i n )     
 
         } 
 
         e l s e 
 
         { 
 
                 $ c r e d e n t i a l   =   $ D o m a i n   +   " \ "   +   $ U s e r n a m e 
 
                 r e t u r n   G e t - C r e d e n t i a l   - C r e d e n t i a l   $ c r e d e n t i a l 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   g e t E n t r y N o d e s 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t E n t r y N o d e s 
 
         # 
 
         #   G e t   t h e   " e n t r y "   X m l E l e m e n t   o r   c o l l e c t i o n   o f   X m l E l e m e n t   f r o m   t h e   X M L   d o c   r e t u r n e d   b y   t h e   O r c h e s t r a t o r   O D a t a   w e b   s e r v i c e 
 
         #   R e t u r n s   n u l l   i f   n o   n o d e s   a r e   f o u n d 
 
         # 
 
         #   U s a g e : 
 
         #       g e t E n t r y N o d e s   - X m l D o c   < x m l d o c > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ x m l ]   $ X m l D o c 
 
 	 ) 
 
         
 
         $ n s   =   N e w - O b j e c t   X m l . X m l N a m e s p a c e M a n a g e r   $ X m l D o c . N a m e T a b l e 
 
         $ n s . A d d N a m e s p a c e (   " a " ,   " h t t p : / / w w w . w 3 . o r g / 2 0 0 5 / A t o m " ) 
 
         $ n s . A d d N a m e s p a c e (   " d " ,   " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s " ) 
 
         $ n s . A d d N a m e s p a c e (   " m " ,   " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s / m e t a d a t a " ) 
 
         
 
         $ e n t r y N o d e s   =   $ X m l D o c . S e l e c t N o d e s ( " / / a : e n t r y " , $ n s ) 
 
 
 
         r e t u r n   $ e n t r y N o d e s 
 
 } 
 
 
 
 f u n c t i o n   g e t U s e r A g e n t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t U s e r A g e n t 
 
         # 
 
         #   U s a g e : 
 
         #       g e t U s e r A g e n t 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         $ U s e r A g e n t   =   " P o w e r S h e l l   A P I   C l i e n t " 
 
         r e t u r n   $ (       
 
                 " { 0 }   ( P o w e r S h e l l   { 1 } ;   . N E T   C L R   { 2 } ;   { 3 } ) "   - f   $ U s e r A g e n t ,   $ ( i f ( $ H o s t . V e r s i o n ) { $ H o s t . V e r s i o n } e l s e { " 1 . 0 " } ) ,     
 
                 [ E n v i r o n m e n t ] : : V e r s i o n ,     
 
                 [ E n v i r o n m e n t ] : : O S V e r s i o n . T o S t r i n g ( ) . R e p l a c e ( " M i c r o s o f t   W i n d o w s   " ,   " W i n " )     
 
         ) 
 
 } 
 
 
 
 f u n c t i o n   s e n d H t t p G e t R e q u e s t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   s e n d H t t p G e t R e q u e s t 
 
         # 
 
         #   M a k e   a n   H T T P   G e t   r e q u e s t   t o   a   w e b   s i t e . 
 
         # 
 
         #   U s a g e : 
 
         #       s e n d H t t p G e t R e q u e s t   - U r l s t r i n g   < s t r i n g >   [ - C r e d e n t i a l s   < c r e d e n t i a l > ] 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 P A R A M   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S t r i n g ]   $ U r l s t r i n g , 
 
                 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
 	 ) 
 
 	 W r i t e - D e b u g   " H T T P   G e t   F r o m   $ ( $ u r l s t r i n g ) " 
 
         #   C r e a t e   a   r e q u e s t   o b j e c t 
 
         $ r e q u e s t   =   [ S y s t e m . N e t . H t t p W e b R e q u e s t ] : : C r e a t e ( $ U r l s t r i n g )       
 
 
 
         #   S e t   t h e   c r e d e n t i a l s 
 
         i f   ( $ C r e d e n t i a l s   - e q   $ n u l l ) 
 
         { 
 
                 $ r e q u e s t . U s e D e f a u l t C r e d e n t i a l s   =   $ t r u e 
 
         } 
 
         e l s e 
 
         { 
 
                 $ r e q u e s t . C r e d e n t i a l s   =   $ C r e d e n t i a l s 
 
         } 
 
 
 
         #   B u i l d   t h e   U s e r   A g e n t 
 
         $ r e q u e s t . U s e r A g e n t   =   g e t U s e r A g e n t 
 
         
 
         t r y 
 
         { 
 
                 $ r e s p o n s e   =   [ S y s t e m . N e t . H t t p W e b R e s p o n s e ]   $ R e q u e s t . G e t R e s p o n s e ( ) 
 
         } 
 
         c a t c h   [ S y s t e m . N e t . W e b E x c e p t i o n ] 
 
         { 
 
 	 	 W r i t e - E r r o r   " E x c e p t i o n   o c c u r r e d   i n   $ ( $ M y I n v o c a t i o n . M y C o m m a n d ) :   $ ( $ _ . E x c e p t i o n . M e s s a g e ) "   - E r r o r A c t i o n   S t o p 
 
                 # W r i t e - O u t p u t   " R e s p o n s e   =   " 
 
                 $ r e s p o n s e   =   $ ( $ _ . E x c e p t i o n . R e s p o n s e ) 
 
                 
 
                 #   S h o w   t h e   r e s p o n s e   w i t h   t h e   e r r o r   i n f o r m a t i o n 
 
                 i f   ( $ r e s p o n s e . C o n t e n t L e n g t h   - g t   0 ) 
 
                 { 
 
                         $ r e a d e r   =   [ I O . S t r e a m R e a d e r ]   $ r e s p o n s e . G e t R e s p o n s e S t r e a m ( )     
 
                         $ o u t p u t   =   $ r e a d e r . R e a d T o E n d ( )     
 
                         $ r e a d e r . C l o s e ( ) 
 
                         # W r i t e - H o s t   $ o u t p u t 
 
                         # W r i t e - H o s t   " " 
 
 	 	 	 
 
 	 	 	 # R e t u r n   $ O u t p u t 
 
 	 	 	 # $ o u t p u t 
 
                 } 
 
                 $ r e s p o n s e   =   $ n u l l 
 
         } 
 
         f i n a l l y 
 
         { 
 
                 $ o u t p u t   =   $ n u l l 
 
                 i f   ( ( $ r e s p o n s e   - n e   $ n u l l )   - a n d   ( $ r e s p o n s e . C o n t e n t L e n g t h   - g t   0 ) ) 
 
                 { 
 
                         $ r e a d e r   =   [ I O . S t r e a m R e a d e r ]   $ r e s p o n s e . G e t R e s p o n s e S t r e a m ( )     
 
                         $ o u t p u t   =   $ r e a d e r . R e a d T o E n d ( )     
 
                         [ x m l ] $ o u t p u t   =   $ o u t p u t 
 
                         $ r e a d e r . C l o s e ( ) 
 
 	 	 	 $ r e s p o n s e . C l o s e ( ) 
 
                 } 
 
 
 
 	 	 #   T O D O :   t h i s   c a u s e d   a n   e x c e p t i o n   w h e n   w e   g o t   a   " u n a b l e   t o   c o n n e c t   t o   t h e   r e m o t e   s e r v e r "   e r r o r 
 
 	 	 #   I   b e l i e v e   i t   w a n t s   t o   m o v e   a b o v e   s o   C o m m e n t e d   i t   o u t   a n d   m o v e d   u n d e r   r e a d e r . c l o s e   a b o v e . 
 
 	 	 #   N e e d   t o   c h e c k   w e   s t i l l   h a n d l e   a   4 0 1   ( r u n b o o k   c h e c k e d   o u t ) 
 
                 #   $ r e s p o n s e . C l o s e ( ) 
 
 	 	 
 
                 # R e t u r n   R e s p o n s e 
 
                 $ o u t p u t 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   s e n d H t t p P o s t R e q u e s t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   s e n d H t t p P o s t R e q u e s t 
 
         # 
 
         #   U s a g e : 
 
         #       s e n d H t t p P o s t R e q u e s t   - R e q u e s t   < H t t p W e b R e q u e s t >   - R e q u e s t B o d y   < s t r i n g > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ S y s t e m . N e t . H t t p W e b R e q u e s t ]   $ R e q u e s t , 
 
                         
 
                         [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                         [ s t r i n g ]   $ R e q u e s t B o d y 
 
         ) 
 
                                                 
 
         #   A d d   t h e   b o d y   t o   t h e   r e q u e s t 
 
         $ r e q u e s t s t r e a m   =   n e w - o b j e c t   S y s t e m . I O . S t r e a m W r i t e r   $ R e q u e s t . G e t R e q u e s t S t r e a m ( ) 
 
         
 
         #   T h e   W r i t e   m e t h o d   s e n d s   t h e   r e q u e s t 
 
         $ r e q u e s t s t r e a m . W r i t e ( $ R e q u e s t B o d y ) 
 
         $ r e q u e s t s t r e a m . F l u s h ( ) 
 
         $ r e q u e s t s t r e a m . C l o s e ( ) 
 
         
 
         t r y 
 
         { 
 
                 [ S y s t e m . N e t . H t t p W e b R e s p o n s e ]   $ r e s p o n s e   =   [ S y s t e m . N e t . H t t p W e b R e s p o n s e ]   $ R e q u e s t . G e t R e s p o n s e ( ) 
 
         } 
 
         c a t c h   [ S y s t e m . N e t . W e b E x c e p t i o n ] 
 
         { 
 
                 i f   ( $ r e s p o n s e . C o n t e n t L e n g t h   - e q   0 ) { W r i t e - E r r o r   " E x c e p t i o n   o c c u r r e d   i n   $ ( $ M y I n v o c a t i o n . M y C o m m a n d ) :   $ ( $ _ . E x c e p t i o n . M e s s a g e ) " } 
 
                 $ r e s p o n s e   =   $ ( $ _ . E x c e p t i o n . R e s p o n s e ) 
 
 
 
                 i f   ( $ r e s p o n s e . C o n t e n t L e n g t h   - g t   0 ) 
 
                 { 
 
                         $ r e a d e r   =   [ I O . S t r e a m R e a d e r ]   $ r e s p o n s e . G e t R e s p o n s e S t r e a m ( )     
 
                         $ o u t p u t   =   $ r e a d e r . R e a d T o E n d ( )     
 
                         $ r e a d e r . C l o s e ( ) 
 
 	 	 	 $ m e s s a g e   =   ( [ x m l ] $ o u t p u t ) 
 
 	 	 	 #   D i s p l a y   t h e   c o n t e n t s   o f   t h e   m e s s a g e . 
 
 	 	 	 W r i t e - E r r o r   $ ( $ m e s s a g e . e r r o r . i n n e r t e x t )   - E r r o r A c t i o n   S t o p 
 
                 } 
 
 
 
                 $ r e s p o n s e . C l o s e ( ) 
 
                 $ r e s p o n s e   =   $ n u l l 
 
         } 
 
         f i n a l l y 
 
         { 
 
                 W r i t e - O u t p u t   $ r e s p o n s e 
 
         } 
 
 } 
 
 
 
 f u n c t i o n   g e t R e s p o n s e X m l 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R e s p o n s e X m l 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . N e t . H t t p W e b R e s p o n s e ]   $ R e s p o n s e 
 
 	 ) 
 
         
 
         #   W r i t e   t h e   H t t p W e b R e s p o n s e   t o   S t r i n g 
 
         $ r e s p o n s e S t r e a m   =   $ R e s p o n s e . G e t R e s p o n s e S t r e a m ( ) 
 
         $ r e a d S t r e a m   =   n e w - o b j e c t   S y s t e m . I O . S t r e a m R e a d e r   $ r e s p o n s e S t r e a m 
 
         $ r e s p o n s e S t r i n g   =   $ r e a d S t r e a m . R e a d T o E n d ( ) 
 
         
 
         #   C l o s e   t h e   s t r e a m s 
 
         $ r e a d S t r e a m . C l o s e ( ) 
 
         $ r e s p o n s e S t r e a m . C l o s e ( ) 
 
 
 
         #   R e t u r n   t h e   r e s p o n s e   a s   x m l 
 
         r e t u r n   [ x m l ]   $ r e s p o n s e S t r i n g 
 
 } 
 
 
 
 f u n c t i o n   g e t R e s o u r c e C o u n t 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t R e s o u r c e C o u n t 
 
         # 
 
         #   G e t   t h e   c o u n t   o f   t o t a l   r e s o u r c e s   f r o m   t h e   X M L   d o c   r e t u r n e d   b y   t h e   O r c h e s t r a t o r   O D a t a   w e b   s e r v i c e 
 
         #   R e t u r n s   n u l l   i f   n o   c o u n t   n o d e   i s   f o u n d 
 
         # 
 
         #   U s a g e : 
 
         #       g e t R e s o u r c e C o u n t   - X m l D o c   < x m l d o c > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m   ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ x m l ]   $ X m l D o c 
 
 	 ) 
 
 
 
         $ n s   =   N e w - O b j e c t   X m l . X m l N a m e s p a c e M a n a g e r   $ X m l D o c . N a m e T a b l e 
 
         $ n s . A d d N a m e s p a c e (   " a " ,   " h t t p : / / w w w . w 3 . o r g / 2 0 0 5 / A t o m " ) 
 
         $ n s . A d d N a m e s p a c e (   " d " ,   " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s " ) 
 
         $ n s . A d d N a m e s p a c e (   " m " ,   " h t t p : / / s c h e m a s . m i c r o s o f t . c o m / a d o / 2 0 0 7 / 0 8 / d a t a s e r v i c e s / m e t a d a t a " ) 
 
         
 
         $ c o u n t N o d e   =   $ X m l D o c . S e l e c t S i n g l e N o d e ( " / / m : c o u n t " , $ n s ) 
 
 
 
         $ c o u n t   =   $ n u l l 
 
         i f   ( $ c o u n t N o d e   - n e   $ n u l l ) 
 
         { 
 
                 $ c o u n t   =   $ c o u n t N o d e . I n n e r T e x t 
 
         } 
 
         
 
         W r i t e - d e b u g   " G e t R e s o u c e C o u n t   c o u n t   =   $ ( $ c o u n t ) " 
 
         
 
         r e t u r n   $ c o u n t 
 
 } 
 
 
 
 f u n c t i o n   g e t B a s e S e r v i c e U r l 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t B a s e S e r v i c e U r l 
 
         # 
 
         #   F r o m   a n   " e n t r y "   n o d e   g e t   t h e   b a s e   s e r v i c e   U R L 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . X m l . X m l E l e m e n t ]   $ E n t r y N o d e 
 
         ) 
 
         
 
         $ b a s e u r l   =   $ J o b N o d e . b a s e 
 
         i f   ( $ b a s e u r l   - e q   $ n u l l ) 
 
         { 
 
                 $ s   =   " O r c h e s t r a t o r . s v c / " 
 
                 $ b a s e u r l   =   $ E n t r y N o d e . i d 
 
                 $ i n d e x   =   $ b a s e u r l . I n d e x O f ( $ s ) 
 
                 $ b a s e u r l   =   $ b a s e u r l . s u b s t r i n g ( 0 , $ i n d e x   +   $ s . L e n g t h ) 
 
         } 
 
         
 
         r e t u r n   $ b a s e u r l 
 
 } 
 
 
 
 f u n c t i o n   g e t P a g e Q u e r y 
 
 { 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
         #   g e t P a g e Q u e r y 
 
         # 
 
         #   G e t   a   q u e r y   s t r i n g   f o r   a   p a r t i c u l a r   p a g e 
 
         # 
 
         #   U s a g e : 
 
         #       g e t P a g e Q u e r y   - P a g e   < i n t > 
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ I n t ]   $ P a g e 
 
         ) 
 
         
 
         #   C r e a t e   t h e   p a g e   q u e r y 
 
         i f   ( $ P a g e   - l e   0 )   { $ P a g e   =   1 } 
 
         $ s k i p c o u n t   =   ( $ P a g e   -   1 )   *   $ c _ R e c o r d s P e r P a g e 
 
         
 
         r e t u r n   - j o i n   ( " ` $ s k i p = " , $ s k i p c o u n t , " & ` $ t o p = " , $ c _ R e c o r d s P e r P a g e , " & ` $ i n l i n e c o u n t = a l l p a g e s " ) 
 
 } 
 
 
 
 f u n c t i o n   W a i t F o r R u n b o o k 
 
 { 
 
 	 < # 
 
 	 . S Y N O P S I S 
 
 	 	 W a i t ' s   f o r   a   r u n b o o k s   e x e c u t i o n   t o   c o m p l e t e 
 
 	 . D E S C R I P T I O N 
 
 	 	 W a i t s   f o r   a   r u n b o o k   e x e c u t i o n   t o   c o m p l e t e . 
 
 	 . P A R A M E T E R     J o b 
 
 	 	 J o b   t o   w a u t   f o r 
 
 	 . P A R A M E T E R     C r e d e n t i a l s 
 
 	 	 C r e d e n t i a l s 
 
 	 . E X A M P L E 
 
 	 	 P S   C : \ >   W a i t F o r R u n b o o k   - J o b   $ j o b   - C r e d e n t i a l s   $ c r e d e n t i a l s 
 
 	 # > 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ O b j e c t ] $ j o b , 
 
 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ] $ C r e d e n t i a l s , 
 
 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . I n t 3 2 ] $ t i m e o u t = 0 , 
 
 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ S y s t e m . I n t 3 2 ] $ P o l l I n t e r v a l 
 
         ) 
 
 
 
 
 
 	 #   T i m e o u t   p a r a m e t e r   s p e c i f i e d ,   s o   s t a r t   a   s t o p   w a t c h   t o   m e a s u r e   t h e   p o l l i n g   d u r a t i o n 
 
 	 i f   ( $ t i m e o u t   - g t   0 ) { 
 
 	 	 $ t i m e o u t 1   =   n e w - t i m e s p a n   - S e c o n d s   $ T i m e o u t 
 
 	 	 $ s t o p w a t c h   =   [ d i a g n o s t i c s . s t o p w a t c h ] : : S t a r t N e w ( ) 
 
 	 } 
 
 	 
 
         w h i l e (   ( $ j o b . S t a t u s   - e q   " R u n n i n g " )   - o r   ( $ j o b . S t a t u s   - e q   " P e n d i n g " )   ) 
 
         { 
 
 	 	 w r i t e - v e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   $ ( $ j o b . S t a t u s ) " 
 
                 S t a r t - S l e e p   - s   $ P o l l I n t e r v a l 
 
                 $ j o b   =   G e t - O r c h e s t r a t o r J o b   - j o b i d   $ j o b . I d   - s e r v i c e u r l   $ j o b . U r l _ S e r v i c e   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
 	 	 i f   (   ( $ s t o p w a t c h . e l a p s e d   - g e   $ t i m e o u t 1 )   - a n d   ( $ t i m e o u t   - g t   0 )   )   { 
 
 	 	 	 #   T i m e o u t   e n a b l e d   a n d   s t o p w a t c h   e l a p s e d 
 
 	 	 	 w r i t e - v e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   S c r i p t   T i m e o u t " 
 
 	 	 	 r e t u r n   " S c r i p t   T i m e o u t " 
 
 	 	 } 
 
         } 
 
 	 w r i t e - v e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   $ ( $ j o b . S t a t u s ) " 
 
         
 
         
 
         r e t u r n   $ ( $ j o b . S t a t u s ) 
 
 } 
 
 
 
 f u n c t i o n   G e t - R e t u r n e d D a t a 
 
 { 
 
 	 < # 
 
 	 . S Y N O P S I S 
 
 	 	 G e t s   a   r u n b o o k s   r e t u r n e d   d a t a 
 
 	 . D E S C R I P T I O N 
 
 	 	 G e t s   t h e   r e t u r n e d   d a t a   f o r   a   s p e c i f i c   j o b 
 
 	 . P A R A M E T E R     J o b 
 
 	 	 J o b   t o   c o l l e c t   t h e   p a r a m e t e r s   f o r 
 
 	 . P A R A M E T E R     C r e d e n t i a l s 
 
 	 	 C r e d e n t i a l s 
 
 	 . E X A M P L E 
 
 	 	 P S   C : \ >   G e t - R e t u r n e d D a t a   - J o b   $ j o b   - C r e d e n t i a l s   $ c r e d e n t i a l s 
 
 	 # > 
 
         [ C m d l e t B i n d i n g ( ) ] 
 
         p a r a m   
 
         ( 
 
                 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
                 [ O b j e c t ] $ j o b , 
 
 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
                 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ]   $ C r e d e n t i a l s 
 
         ) 
 
         $ i n s t a n c e   =   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e   - j o b   $ j o b   - c r e d e n t i a l s   $ C r e d e n t i a l s 
 
         $ i n s t p a r a m s   =   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e P a r a m e t e r   - R u n b o o k I n s t a n c e   $ i n s t a n c e   - C r e d e n t i a l s   $ C r e d e n t i a l s 
 
 	               
 
 	 i f   ( $ i n s t p a r a m s   - n e   $ n u l l )   
 
 	 {   
 
 	 	 $ R e t u r n e d D a t a   = @ ( ) 
 
                 f o r e a c h   ( $ i n s t p a r a m   i n   $ i n s t p a r a m s )   {   
 
                     i f   ( $ i n s t p a r a m . D i r e c t i o n   - e q   " O u t " )   
 
                     {   
 
 	 	 	 $ R u n b o o k D e t a i l   =   N e w - O b j e c t   P S O b j e c t 
 
 	 	 	 $ R u n b o o k D e t a i l   |   A d d - M e m b e r   - N a m e   " P a r a m e t e r N a m e "   - M e m b e r T y p e   N o t e P r o p e r t y   - V a l u e   $ ( $ i n s t p a r a m . N a m e ) 
 
 	 	 	 $ R u n b o o k D e t a i l   |   A d d - M e m b e r   - N a m e   " V a l u e "   - M e m b e r T y p e   N o t e P r o p e r t y   - V a l u e   $ ( $ i n s t p a r a m . V a l u e ) 
 
 	 	 	 $ R u n b o o k D e t a i l   |   A d d - M e m b e r   - N a m e   " G u i d "   - M e m b e r T y p e   N o t e P r o p e r t y   - V a l u e   $ ( $ i n s t p a r a m . I d ) 	 
 
 	 	 	 $ R e t u r n e d D a t a   + =   $ R u n b o o k D e t a i l 	 
 
                     }   
 
       	 	 } 
 
 	 	 r e t u r n   $ R e t u r n e d D a t a 
 
 	 } 
 
 	 e l s e 
 
 	 { 
 
 	 	 r e t u r n   $ n u l l 
 
 	 } 
 
 } 
 
 
 
 f u n c t i o n   E x e c u t e R u n b o o k 
 
 { 
 
 	 < # 
 
 	 	 . S Y N O P S I S 
 
 	 	 	 E x e c u t e s   a   r u n b o o k 
 
 	 	 . D E S C R I P T I O N 
 
 	 	 	 E x e c u t e s   a   r u n b o o k   a n d   o p t i o n a l l y   w a i t s   f o r   t h e   e x e c u t i o n   t o   c o m p l e t e . 
 
 	 	 	 I f   w a i t i n g   f o r   c o m p l e t i o n   i t   w i l l   a l s o   c o l l e c t   t h e   r e t u r n e d   d a t a . 
 
 	 	 . P A R A M E T E R     N a m e 
 
 	 	 	 R u n b o o k   N a m e 
 
 	 	 . P A R A M E T E R     P a r a m e t e r s 
 
 	 	 	 H a s h t a b l e   c o n t a i n i n g   n a m e   v a l u e   p a i r s 	 	 	 
 
 	 	 . P A R A M E T E R     W a i t 
 
 	 	 	 S p e c i f y   w h e t h e r   t o   w a i t   f o r   r u n b o o k   e x e c u t i o n   t o   c o m p l e t e 	 	 	 
 
 	 	 . P A R A M E T E R     O r c h e s t r a t o r S e r v e r 
 
 	 	 	 O r c h e s t r a t o r   S e r v e r   N a m e 	 	 
 
 	 	 . P A R A M E T E R     C r e d e n t i a l s 
 
 	 	 	 C r e d e n t i a l s 
 
 	 	 . E X A M P L E 
 
 	 	 	 P S   C : \ >   E x e c u t e R u n b o o k   - N a m e   ' R u n b o o k 1 '   - O r c h e s t r a t o r S e r v e r   ' s e r v e r . b l a h . l o c a l '   - W a i t   - V e r b o s e 
 
 
 
 	 # > 
 
 	 [ C m d l e t B i n d i n g ( ) ] 
 
 	 p a r a m ( 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ t r u e ) ] 
 
 	 	 [ S y s t e m . S t r i n g ] $ N a m e , 
 
 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
 	 	 #   T O D O :   S t r o n g l y   T y p e d 
 
 	 	 $ P a r a m e t e r s , 
 
 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ F a l s e ) ] 
 
 	 	 [ s w i t c h ] $ W a i t , 
 
 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ F a l s e ) ] 
 
 	 	 [ s t r i n g ] $ O r c h e s t r a t o r S e r v e r = " " , 
 
 	 	 	 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
 	 	 [ S y s t e m . N e t . N e t w o r k C r e d e n t i a l ] $ c r e d e n t i a l s , 
 
 
 
 	 	 [ P a r a m e t e r ( M a n d a t o r y = $ f a l s e ) ] 
 
 	 	 [ S y s t e m . I n t 3 2 ] $ P o l l I n t e r v a l = 2 
 
 	 ) 
 
         #   c r e a t e   t h e   b a s e   u r l   t o   t h e   s e r v i c e 
 
         $ u r l   =   G e t - O r c h e s t r a t o r S e r v i c e U r l   - s e r v e r   $ O r c h e s t r a t o r S e r v e r 
 
 	 
 
 	 #   D W :   Q u i c k   b o d g e   t o   t r y   a n d   m a s k   t h e   i n t e r m i t t e n t   i s s u e s   w h e n   t r y i n g   t o   c a l l   r u n b o o k s 
 
 	 #   S o   f a r   u n a b l e   t o   r e l i a b l y   r e c r e a t e   t h e   i s s u e ,   i n   o r d e r   t o   f i x . 
 
 	 
 
 	 $ S t o p l o o p   =   $ f a l s e 
 
 	 [ i n t ] $ R e t r y c o u n t   =   1 
 
 	 
 
 	 d o   { 
 
 	 	 $ r u n b o o k   =   G e t - O r c h e s t r a t o r R u n b o o k   - S e r v i c e U r l   $ u r l   - c r e d e n t i a l s   $ c r e d e n t i a l s   - r u n b o o k p a t h   $ N a m e 
 
 	 	 #   E x i t   i f   w e   g e t   a   r u n b o o k . . 
 
 	 	 i f   ( $ r u n b o o k   - n e   $ n u l l ) { 
 
 	 	 	 w r i t e - v e r b o s e   " G o t   R u n b o o k   $ ( $ N a m e ) " 
 
 	 	 	 $ S t o p l o o p   =   $ t r u e 
 
 	 	 } 
 
 	 	 
 
 	 	 #   C h e c k   r e t r y   c o u n t 	 
 
 	 	 i f   ( $ R e t r y c o u n t   - g e   3 ) { 
 
 	 	 	 w r i t e - e r r o r   " R u n b o o k   n o t   f o u n d   a f t e r   $ ( $ R e t r y c o u n t )   a t t e m p t s ,   I n v a l i d   R u n b o o k   N a m e ? "   - E r r o r A c t i o n   S t o p 
 
 	 	 } 
 
 	 	 
 
 	 	 #   I f   w e   a r e   e x i t i n g   o n   t h i s   l o o p   d o n t   r u n   t h i s   s e c t i o n 
 
 	 	 i f   ( $ S t o p l o o p   - e q   $ f a l s e ) { 
 
 	 	 	 #   D e l a y   b e f o r e   a t t e m p t i n g   a g a i n . 
 
 	 	 	 w r i t e - w a r n i n g   " G e t - O r c h e s t r a t o r R u n b o o k   r e t u r n e d   N u l l ,   r e t r y i n g   i n   3 0   s e c o n d s " 
 
 	 	 	 S t a r t - S l e e p   - S e c o n d s   3 0 
 
 	 	 	 $ R e t r y c o u n t   =   $ R e t r y c o u n t   +   1 
 
 	 	 } 
 
 	 } 
 
 	 W h i l e   ( $ S t o p l o o p   - e q   $ f a l s e ) 
 
 	 
 
 	 #   S o r t   R u n b o o k   P a r a m e t e r s 
 
 	 $ P a r a m s W i t h V a l u e s   =   $ n u l l 
 
 	 	 
 
 	 i f   ( $ P a r a m e t e r s   - n e   $ n u l l ) { 
 
 	 	 W r i t e - V e r b o s e   " P a r a m e t e r s   s u p p l i e d   f o r   R u n b o o k :   $ ( $ r u n b o o k . N a m e )   $ ( $ r u n b o o k . I d ) " 
 
 	 	 #   C r e a t e   E m p t y   H a s h t a b l e 
 
 	 	 $ P a r a m s W i t h V a l u e s   =   @ { } 
 
 
 
 	 	 #   L o o p   t h r o u g h   R u n b o o k   P a r a m e t e r s   a d d i n g   v a l u e s   w h e r e   w e   h a v e   t h e m . 
 
 	 	 f o r e a c h   ( $ P a r a m e t e r   i n   $ r u n b o o k . P a r a m e t e r s )   { 
 
 	 	 	 i f   ( $ P a r a m e t e r . D i r e c t i o n   - e q   " I n " ) { 
 
 	 	 	 	 W r i t e - D e b u g   " P a r a m e t e r   N a m e :   $ ( $ P a r a m e t e r . N a m e ) " 
 
 	 	 	 	 #   A d d   t o   h a s h t a b l e   s o   w e   h a v e   a n   e n t r y   f o r   e a c h   r u n b o o k   p a r a m ,   r e g a r d l e s s   o f   w h e t h e r   w e   h a v e   a   v a l u e . 
 
 	 	 	 	 $ P a r a m s W i t h V a l u e s . A d d ( $ P a r a m e t e r . I D ,   $ n u l l ) 	 
 
 	 	 	 	 #   N o w   l o o k   t h r o u g h   p a s s e d   p a r a m ' s   a n d   a d d   a   v a l u e   w h e r e   w e   h a v e   o n e . . 
 
 	 	 	 	 f o r e a c h   ( $ i t e m   i n   $ P a r a m e t e r s ) { 
 
 	 	 	 	 	 W r i t e - D e b u g   " I t e m :   $ ( $ i t e m . N a m e )   P a r a m   N a m e :   $ ( $ P a r a m e t e r . N a m e ) " 
 
 	 	 	 	 	 i f   ( $ i t e m . N a m e   - e q   $ P a r a m e t e r . N a m e )   { 
 
 	 	 	 	 	 	 W r i t e - V e r b o s e   " P r o c e s s i n g   S u p p l i e d   P a r a m e t e r :   $ ( $ P a r a m e t e r . N a m e )   I D :   $ ( $ P a r a m e t e r . I d ) " 
 
 	 	 	 	 	 	 #   T h e y   b o t h   m a t c h   s o   a d d   t h e   p a r a m   v a l u e 
 
 	 	 	 	 	 	 $ P a r a m s W i t h V a l u e s . S e t _ I t e m ( $ P a r a m e t e r . I d ,   $ i t e m . V a l u e ) 
 
 	 	 	 	 	 	 #   E x i t   F o r   E a c h . . .   n o   n e e d   t o   c o n t i n u e   w i t h i n   t h i s   l o o p 
 
 	 	 	 	 	 	 b r e a k 
 
 	 	 	 	 	 } 
 
 	 	 	 	 } 
 
 	 	 	 } 
 
 	 	 } 
 
 	 } 
 
 	 	 
 
 	 #   S t a r t   T h e   R u n b o o k 
 
 	 w r i t e - v e r b o s e   " S t a r t i n g   R u n b o o k :   $ ( $ r u n b o o k . N a m e )   $ ( $ r u n b o o k . I d ) " 
 
 	 
 
 	 $ j o b   =   S t a r t - O r c h e s t r a t o r R u n b o o k   - r u n b o o k   $ r u n b o o k   - c r e d e n t i a l s   $ c r e d e n t i a l s   - P a r a m e t e r s   $ P a r a m s W i t h V a l u e s   
 
 	 
 
 	 #   E n s u r e   a   j o b   h a s   b e e n   c r e a t e d   b e f o r e   c o n t i n u i n g 
 
 	 i f   ( $ j o b   - e q   $ n u l l ) 
 
 	 { 
 
 	 	 W r i t e - D e b u g   " N o   J o b   O b j e c t   w a s   r e t u r n e d   f r o m   S t a r t - O r c h e s t r a t o r R u n b o o k " 
 
 	 	 t h r o w   " E R R O R :   N o   j o b   w a s   c r e a t e d " 
 
 	 } e l s e 
 
 	 { 
 
 	 	 W r i t e - V e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   C r e a t e d " 
 
 	 } 
 
 	 
 
 	 $ R e t u r n e d D a t a   =   $ n u l l 
 
 	 i f   ( $ W a i t   - e q   $ t r u e ) { 
 
 	 	 #   M o n i t o r   j o b   ( R u n b o o k )   s t a t u s   
 
 	 	 W r i t e - V e r b o s e   " J o b :   $ ( $ j o b . i d )   W a i t i n g   f o r   e x e c u t i o n ,   p l e a s e   w a i t " 
 
 	 	 $ j o b S t a t u s   =   W a i t F o r R u n b o o k   - J o b   $ j o b   - c r e d e n t i a l s   $ c r e d e n t i a l s   - P o l l I n t e r v a l   $ P o l l I n t e r v a l 
 
 	 	 
 
 	 	 #   T O D O :   I m p l e m e n t   t h i s   f u n c t i o n a l i t y . 
 
 	 	 I f   ( $ j o b S t a t u s   - e q   " T i m e d o u t " ) { 
 
 	 	 	 W r i t e - V e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   T i m e o u t   w h i l s t   p o l l i n g   r u n b o o k   s t a t u s " 
 
 	 	 	 T h r o w   " T i m e o u t   w a i t i n g   f o r   j o b   t o   c o m p l e t e .   T h e   j o b   w i l l   c o n t i n u e   t o   r u n   o n   t h e   s e r v e r . " 
 
 	 	 } 
 
 	 	 
 
 	 	 #   g e t   R e t u r n e d D a t a   i f   t h e r e   i s   a n y . 
 
 	 	 W r i t e - V e r b o s e   " J o b :   $ ( $ j o b . i d )   S t a t u s :   G e t t i n g   r e t u r n e d   d a t a " 
 
 	 	 $ R e t u r n e d D a t a   =   G e t - R e t u r n e d D a t a   - J o b   $ j o b   - C r e d e n t i a l s   $ c r e d e n t i a l s 
 
 
 
 	 	 i f   ( $ R e t u r n e d D a t a   - n e   $ n u l l ) { 
 
 	 	 	 W r i t e - v e r b o s e   " J o b :   $ ( $ j o b . I d )   S t a t u s :   R e t r i e v e d   r e t u r n e d   d a t a " 
 
 	 	 } e l s e { 
 
 	 	 	 $ R e t u r n e d D a t a   =   " N o t h i n g   t o   r e t u r n " 
 
 	 	 } 
 
 	 } e l s e { 
 
 	 	 W r i t e - V e r b o s e   " J o b :   $ ( $ j o b . I d )   S t a t u s :   N o t   w a i t i n g   f o r   r u n b o o k   e x e c u t i o n   t o   c o m p l e t e . " 
 
 	 	 $ R e t u r n e d D a t a   =   " R u n b o o k   S t a r t e d " 
 
 	 } 
 
 	 W r i t e - V e r b o s e   " F i n i s h e d   e x e c u t i n g   R u n b o o k :   $ ( $ r u n b o o k . N a m e )   R u n b o o k :   $ ( $ r u n b o o k . I d )   J o b :   $ ( $ j o b . i d )   " 
 
 	 
 
 	 #   R e t u r n   D a t a 
 
 	 r e t u r n   $ R e t u r n e d D a t a 
 
 } 
 
 
 
 F u n c t i o n   N e w - P a r a m e t e r V a l u e   { 
 
 	 < # 
 
 	 	 . S Y N O P S I S 
 
 	 	 	 U s e d   f o r   c r e a t i n g   r u n b o o k   p a r a m e t e r s   ' n e a t l y ' 
 
 	 	 . D E S C R I P T I O N 
 
 	 	 	 U s e d   f o r   c r e a t i n g   t h e   r u n b o o k   p a r a m e t e r s   i n   a   ' n e a t '   w a y   o n   o n e   l i n e 
 
 	 	 . P A R A M E T E R     N a m e 
 
 	 	 	 R u n b o o k   P a r a m e t e r   N a m e 
 
 	 	 . P A R A M E T E R     V a l u e 
 
 	 	 	 R u n b o o k   P a r a m e t e r   V a l u e 	 	 	 
 
 	 	 . E X A M P L E 
 
 	 	 	 P S   C : \ > 	 $ R u n b o o k P a r a m A r r a y   + =   N e w - P a r a m e t e r V a l u e   - n a m e   " U s e r n a m e "   - V a l u e   " J o e   B l o g g s " 
 
 	 # > 
 
         [ C m d l e t B i n d i n g ( ) ]   
 
         p a r a m   ( 
 
                 [ p a r a m e t e r ( M a n d a t o r y = $ t r u e ,   P o s i t i o n = 0 ) ]   
 
                 [ V a l i d a t e N o t N u l l ( ) ]   
 
 	 	 [ s t r i n g ] $ N a m e , 
 
                 
 
                 [ p a r a m e t e r ( M a n d a t o r y = $ f a l s e ,   P o s i t i o n = 1 ) ]   
 
 	 	 [ A l l o w E m p t y S t r i n g ( ) ] 
 
 	 	 [ s t r i n g ] $ V a l u e 
 
         )   
 
 
 
 	 $ V a r i a b l e   =   N e w - O b j e c t   p s o b j e c t   - P r o p e r t y   @ { N a m e = $ N a m e ; V a l u e = $ V a l u e } 
 
         r e t u r n   $ V a r i a b l e   
 
 } 
 
 
 
 # #   E x p o r t   t h e   f u n c t i o n s 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r S e r v i c e U r l 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r C o l l e c t i o n 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r J o b 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - O r c h e s t r a t o r R u n b o o k I n s t a n c e P a r a m e t e r 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   S t o p - O r c h e s t r a t o r J o b 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   S t a r t - O r c h e s t r a t o r R u n b o o k 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - C r e d e n t i a l s 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   W a i t F o r R u n b o o k 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   G e t - R e t u r n e d D a t a 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   E x e c u t e R u n b o o k 
 
 E x p o r t - M o d u l e M e m b e r   - F u n c t i o n   N e w - P a r a m e t e r V a l u e 
