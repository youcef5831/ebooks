<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <base target="_self">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر الكتب الإلكترونية</title>
    <meta name="description" content="متجر متخصص لبيع الكتب الإلكترونية بصيغة PDF">
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: "#4F46E5",
                        secondary: "#10B981"
                    },
                    fontFamily: {
                        'sans': ['Tajawal', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700&display=swap');
        body {
            font-family: 'Tajawal', sans-serif;
        }
    </style>
</head>
<body class="min-h-screen bg-gray-50">
    <!-- Header -->
    <header class="bg-white shadow-md">
        <div class="container mx-auto px-4 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-2 space-x-reverse">
                    <i class="fas fa-book-open text-2xl text-primary"></i>
                    <h1 class="text-xl font-bold text-gray-800">متجر الكتب</h1>
                </div>
                
                <nav class="hidden md:flex space-x-6 space-x-reverse">
                    <a href="#" class="text-gray-700 hover:text-primary font-medium">الرئيسية</a>
                    <a href="#" class="text-gray-700 hover:text-primary font-medium">المكتبة</a>
                    <a href="#" class="text-gray-700 hover:text-primary font-medium">من نحن</a>
                    <a href="#" class="text-gray-700 hover:text-primary font-medium">اتصل بنا</a>
                </nav>
                
                <div class="flex items-center space-x-4 space-x-reverse">
                    <a href="#" class="text-gray-700 hover:text-primary">
                        <i class="fas fa-shopping-cart"></i>
                    </a>
                    <a href="#" class="text-gray-700 hover:text-primary">
                        <i class="fas fa-user"></i>
                    </a>
                    <button class="md:hidden text-gray-700">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="bg-gradient-to-l from-primary to-secondary text-white py-16">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-4">اكتشف عالم المعرفة مع كتبنا الإلكترونية</h2>
            <p class="text-lg mb-8">أكثر من 1000 كتاب إلكتروني متاح للتحميل الفوري بصيغة PDF</p>
            <div class="max-w-md mx-auto relative">
                <input type="text" placeholder="ابحث عن كتاب..." class="w-full py-3 px-4 rounded-full text-gray-800 focus:outline-none">
                <button class="absolute left-3 top-1/2 transform -translate-y-1/2 bg-primary text-white p-2 rounded-full">
                    <i class="fas fa-search"></i>
                </button>
            </div>
        </div>
    </section>

    <!-- Featured Books -->
    <section class="py-12">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-2xl font-bold text-gray-800">أحدث الكتب</h2>
                <a href="#" class="text-primary hover:underline">عرض الكل</a>
            </div>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <!-- Book 1 -->
                <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow">
                    <img src="https://picsum.photos/300/400?random=1" alt="غلاف كتاب تطوير الذات" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">فن اللامبالاة</h3>
                        <p class="text-gray-600 text-sm mb-3">مارك مانسون</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold text-primary">$9.99</span>
                            <button class="bg-primary text-white px-3 py-1 rounded hover:bg-primary-dark transition">شراء</button>
                        </div>
                    </div>
                </div>
                
                <!-- Book 2 -->
                <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow">
                    <img src="https://picsum.photos/300/400?random=2" alt="غلاف كتاب ريادة الأعمال" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">الأب الغني والأب الفقير</h3>
                        <p class="text-gray-600 text-sm mb-3">روبرت كيوساكي</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold text-primary">$12.99</span>
                            <button class="bg-primary text-white px-3 py-1 rounded hover:bg-primary-dark transition">شراء</button>
                        </div>
                    </div>
                </div>
                
                <!-- Book 3 -->
                <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow">
                    <img src="https://picsum.photos/300/400?random=3" alt="غلاف كتاب البرمجة" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">تعلم JavaScript في 30 يوم</h3>
                        <p class="text-gray-600 text-sm mb-3">أحمد محمد</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold text-primary">$14.99</span>
                            <button class="bg-primary text-white px-3 py-1 rounded hover:bg-primary-dark transition">شراء</button>
                        </div>
                    </div>
                </div>
                
                <!-- Book 4 -->
                <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow">
                    <img src="https://picsum.photos/300/400?random=4" alt="غلاف كتاب التاريخ" class="w-full h-48 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">تاريخ العالم في 100 صفحة</h3>
                        <p class="text-gray-600 text-sm mb-3">سارة أحمد</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold text-primary">$8.99</span>
                            <button class="bg-primary text-white px-3 py-1 rounded hover:bg-primary-dark transition">شراء</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Categories -->
    <section class="py-12 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-bold text-gray-800 mb-8">تصفح حسب التصنيف</h2>
            
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4">
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-brain text-2xl mb-2"></i>
                    <p>تطوير الذات</p>
                </a>
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-chart-line text-2xl mb-2"></i>
                    <p>ريادة الأعمال</p>
                </a>
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-laptop-code text-2xl mb-2"></i>
                    <p>البرمجة</p>
                </a>
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-book text-2xl mb-2"></i>
                    <p>الأدب</p>
                </a>
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-history text-2xl mb-2"></i>
                    <p>التاريخ</p>
                </a>
                <a href="#" class="bg-white rounded-lg shadow p-4 text-center hover:bg-primary hover:text-white transition">
                    <i class="fas fa-flask text-2xl mb-2"></i>
                    <p>العلوم</p>
                </a>
            </div>
        </div>
    </section>

    <!-- How it Works -->
    <section class="py-12">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-bold text-gray-800 mb-8 text-center">كيف يعمل متجرنا</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="text-center">
                    <div class="bg-primary text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-search text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">ابحث عن الكتاب</h3>
                    <p class="text-gray-600">ابحث عن الكتاب الذي تريده باستخدام محرك البحث أو تصفح التصنيفات</p>
                </div>
                
                <div class="text-center">
                    <div class="bg-primary text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-shopping-cart text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">أضف إلى السلة</h3>
                    <p class="text-gray-600">أضف الكتاب إلى سلة التسوق واكمل عملية الدفع</p>
                </div>
                
                <div class="text-center">
                    <div class="bg-primary text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-download text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">حمل الكتاب</h3>
                    <p class="text-gray-600">بعد الدفع، يمكنك تحميل الكتاب مباشرة بصيغة PDF</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">متجر الكتب</h3>
                    <p class="text-gray-400">أكبر متجر لبيع الكتب الإلكترونية في العالم العربي</p>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">روابط سريعة</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">الرئيسية</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">المكتبة</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">من نحن</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">اتصل بنا</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">التصنيفات</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">تطوير الذات</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">ريادة الأعمال</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">البرمجة</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">الأدب</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">تواصل معنا</h4>
                    <div class="flex space-x-4 space-x-reverse mb-4">
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                    <p class="text-gray-400">البريد الإلكتروني: info@ebookstore.com</p>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>© 2023 متجر الكتب. جميع الحقوق محفوظة.</p>
            </div>
        </div>
    </footer>

    <!-- Shopping Cart Modal -->
    <div class="fixed inset-0 bg-black bg-opacity-50 z-50 hidden" id="cartModal">
        <div class="absolute left-0 top-0 h-full w-full md:w-96 bg-white shadow-lg overflow-y-auto">
            <div class="p-4 border-b">
                <div class="flex justify-between items-center">
                    <h3 class="text-lg font-bold">سلة التسوق</h3>
                    <button onclick="closeCart()" class="text-gray-500 hover:text-gray-700">
                        <i class="fas fa-times"></i>
                    </button>
                </div>
            </div>
            
            <div class="p-4 space-y-4" id="cartItems">
                <!-- Cart items will be added here dynamically -->
                <div class="text-center py-8 text-gray-500">
                    <i class="fas fa-shopping-cart text-4xl mb-2"></i>
                    <p>سلة التسوق فارغة</p>
                </div>
            </div>
            
            <div class="p-4 border-t">
                <div class="flex justify-between mb-4">
                    <span class="font-bold">المجموع:</span>
                    <span class="font-bold" id="cartTotal">$0.00</span>
                </div>
                <button class="w-full bg-primary text-white py-2 rounded hover:bg-primary-dark transition">
                    اتمام الشراء
                </button>
            </div>
        </div>
    </div>

    <script>
        // Sample book data
        const books = [
            {
                "id": 1,
                "title": "فن اللامبالاة",
                "author": "مارك مانسون",
                "price": 9.99,
                "image": "https://picsum.photos/300/400?random=1"
            },
            {
                "id": 2,
                "title": "الأب الغني والأب الفقير",
                "author": "روبرت كيوساكي",
                "price": 12.99,
                "image": "https://picsum.photos/300/400?random=2"
            },
            {
                "id": 3,
                "title": "تعلم JavaScript في 30 يوم",
                "author": "أحمد محمد",
                "price": 14.99,
                "image": "https://picsum.photos/300/400?random=3"
            },
            {
                "id": 4,
                "title": "تاريخ العالم في 100 صفحة",
                "author": "سارة أحمد",
                "price": 8.99,
                "image": "https://picsum.photos/300/400?random=4"
            }
        ];

        // Shopping cart functionality
        let cart = [];

        function addToCart(bookId) {
            const book = books.find(b => b.id === bookId);
            if (book) {
                cart.push(book);
                updateCart();
                alert(`تمت إضافة "${book.title}" إلى سلة التسوق`);
            }
        }

        function updateCart() {
            const cartItems = document.getElementById('cartItems');
            const cartTotal = document.getElementById('cartTotal');
            
            if (cart.length === 0) {
                cartItems.innerHTML = `
                    <div class="text-center py-8 text-gray-500">
                        <i class="fas fa-shopping-cart text-4xl mb-2"></i>
                        <p>سلة التسوق فارغة</p>
                    </div>
                `;
                cartTotal.textContent = "$0.00";
                return;
            }
            
            let itemsHTML = '';
            let total = 0;
            
            cart.forEach(item => {
                total += item.price;
                itemsHTML += `
                    <div class="flex justify-between items-center border-b pb-4">
                        <div class="flex items-center space-x-4 space-x-reverse">
                            <img src="${item.image}" alt="${item.title}" class="w-16 h-16 object-cover rounded">
                            <div>
                                <h4 class="font-medium">${item.title}</h4>
                                <p class="text-sm text-gray-500">${item.author}</p>
                            </div>
                        </div>
                        <div>
                            <span class="font-bold">$${item.price.toFixed(2)}</span>
                        </div>
                    </div>
                `;
            });
            
            cartItems.innerHTML = itemsHTML;
            cartTotal.textContent = `$${total.toFixed(2)}`;
        }

        function openCart() {
            document.getElementById('cartModal').classList.remove('hidden');
        }

        function closeCart() {
            document.getElementById('cartModal').classList.add('hidden');
        }

        // Initialize event listeners
        document.addEventListener('DOMContentLoaded', function() {
            // Add click events to all "Add to Cart" buttons
            document.querySelectorAll('[onclick^="addToCart"]').forEach(button => {
                const bookId = parseInt(button.getAttribute('onclick').match(/\d+/)[0]);
                button.addEventListener('click', () => addToCart(bookId));
            });
            
            // Cart icon click event
            document.querySelector('.fa-shopping-cart').closest('a').addEventListener('click', function(e) {
                e.preventDefault();
                openCart();
            });
            
            // Close modal when clicking outside
            document.getElementById('cartModal').addEventListener('click', function(e) {
                if (e.target === this) {
                    closeCart();
                }
            });
        });

        // Prevent default behavior for all anchor tags
        document.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', function(e) {
                if (this.getAttribute('href') === '#') {
                    e.preventDefault();
                }
            });
        });
    </script>
</body>
</html>
