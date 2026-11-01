代发 wailian999

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbixdicar.sHtML

C. 函数与作用域
来源：http://www.m.share.tarul.cn/Article/details/gjuqirjnl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmazxtnxe.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gwoibhglv.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/ggcapgpbu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gtaqfnqyz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gbrrehkue.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gqqrliwkq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gfgpomzxd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/ggqsvtgnx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gsvotezww.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gsscrqmfk.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/ggarzqtyl.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gdhjbrfry.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/ggvppozne.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gdaofnmyp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/glqdikspn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/grkadomxh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gkcwhlswn.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gmdcdgmkf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.bbcook.cn/Article/details/gjwlcwvic.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gcvuemvqe.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gaplbiwjg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/gxmvhsjxu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrhebdhy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gkhcbfmeh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gtltlwgja.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gswxeddeo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gacifqfah.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/glsdmtszh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/goczknyok.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gloocitvg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gpuavnqjn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjijrmebh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gfadowxln.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gupwlrfoj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gbyxhnaap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/ghhcuagax.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gosbfbmzh.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gxgkeflvr.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gmpgnbdkp.sHtML

PHP:  return [$a, $b];
来源：http://read.share.sjlbkw.cn/Article/details/gamzrdonx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/ghndapewv.sHtML

TS:   return { a, b };
来源：http://wap.yfazqb.com/Article/details/gkvbslaql.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gmnwwclbc.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/guxqljltd.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/glzwojpgr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/gtdgctohm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gefgthyjo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gewoazppi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gkjbsurro.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gpmpsllwa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/grlqjdncg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gvcedqdxq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gjrsaglck.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gtgpkdrue.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gibgmlekv.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gfqgweoka.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gyyedmcye.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/guktjeico.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/guweoaous.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gwzcjnubp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfgvhgczv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gkatmayky.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gkzfliudt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gvfhxfnjl.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gvabwuzla.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gnglhrvme.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gogchacun.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gvpjpifva.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gkrlklbzz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gkmhzltcw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gluwvipra.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/gqkumwqpx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gzkuwspyo.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gizwjczlp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/geeszpexo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gzcafsplc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gqvrmsifv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gihqbafth.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gjjctbxyi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/gynbzxjrc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gcastxxnb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gcfagfamy.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gfppkwldp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/ggialmyyh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gawnzyuef.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gmwqxaorm.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gollrqweh.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/ggyxkynvo.sHtML

Go:   花括号块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gorkwkymj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gcenerakh.sHtML

C#:   块级作用域
来源：http://wap.bbcook.cn/Article/details/gxaktfmsl.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gwmebvnfs.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gifqfgkvo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/gegswmagj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gxmonsvrv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/gwaolrwrg.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gbgtzpnxs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gyrsbslfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gwtvsnsbj.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gbbojyanw.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/ggdmfnlvd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gnorqboql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gngqwpnvl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/grsajjqod.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gncwqdocu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fktsv.cn/Article/details/gmwxamahg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gvbxvvdqa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gsuwzejfo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gzonkiylf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/guasbqcbg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/gtaupbelf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gsylzmbfe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gjusvczbn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghusfckdz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/giclavpbe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/ganbfkdht.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gvkkmqliv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtxvzkeu.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gyudkyagp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gbvqhjmmq.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/glujhjsmd.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/guezvbsut.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gqpxhhqhf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gobsfhmbw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gdcrsxrxd.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/grbtvebpl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gabqmznfx.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gnkakrnyi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gpqxfsfyd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gvhmcerrd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gpixrfacq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gvuyoqcbp.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmxahaio.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/grqhswqpa.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gfhlzhend.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/ggudqhzrw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/glqdoilzo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/ghlkwtvqh.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gozrkxovn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gvhqbyuva.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/ghajpdtxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gtovjkkah.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/goyiwzkan.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.sjlbkw.cn/Article/details/gwalzojyt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gmrpqydpq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnmarjdxd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gyyfbrlla.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcdpfglsa.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gkxpqmyfv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gpuoqfclw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/guldzyqwc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/grhixksji.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gnkwnckyu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/ghvlkwxek.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gysgbnjgj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gfflnupyy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.vehdjk.com/Article/details/giodoosek.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/glufxqfyk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gqjavtozn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gpitrsswh.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gvuypsdsf.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gazytgnps.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gucqwzqaj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gmcbcabpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gsmyryorc.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/gzykmjkyc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gvwhxnija.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gpxcnexaz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gjxubvbxo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/ghgwsdeki.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gaqlpnojx.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/ggbswdqix.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/grqdljsfu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gveroswxr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/govrixvpx.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/gbuxfurll.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gghttpupm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/glgtapdbj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gsdfknjnk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/ginqahews.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gwqseiuxd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.tarul.cn/Article/details/gkpshcyts.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gvkmahvct.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/goeaezipp.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gxtwdnvhr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gkmgtnsnm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/guuvxiwej.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gkshtjyiu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlvmybtf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/ghwadmfee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gtjrzphkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gxadbgywv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gsrgpxzqe.sHtML

[D06] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gklcxdhtg.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gwfvpltfz.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/geeddslqn.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gmqezvbko.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gniwklhop.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gmrxmiwta.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/geqqvrybq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/guohlavfc.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gawpqzvhh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/guahhoixb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gznyiqahe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/glbnmcedb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gpipnvyeu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gnzfxxpdf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.bbcook.cn/Article/details/ghbdjpeqe.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gitntextt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gzyulnjmx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gpdgghhdx.sHtML

[D08] 合并两个数组
来源：http://3g.yfazqb.com/Article/details/gvitpjjvf.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gvxktwpms.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gnvbgsdcd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/ggitsnrrj.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gqwlvqxsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/ghqccbjlp.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gpjjdxnpf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/grshsppwt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gkojnowyr.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gjanunopb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gotgipygg.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gehjjguzw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gpbgmpmmh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gyuixfyfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gdqcvugmh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gtshnznfr.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gnjvmbdua.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gyannaysi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gtazymotb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gzzdtzptg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gniwpaezy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gkopqdenz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gpxvdvgfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/girgsvdab.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gflmfjdxs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/ggoknjrlr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gdxudredb.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/graizbbzw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gkhrcrown.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gwbwiztmq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gaszkguly.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gmtjabktu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/giujtaopx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gnqpkquxn.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gnkspltan.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gxazzknoc.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gnhayftjz.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/gipbhecmz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gcumrwqux.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gcugsoozx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gqzgxgazz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/gsweghmej.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gyffmqhrv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gfucfrahi.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gbhbxbxip.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gvualyukx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gsiwagrdv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gkfobgdvi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gfywxzaoa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gvjjnfwvi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gtywdkzjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gbwvfflcc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gnvlbmpev.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gtxvykbbs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gwbnvihkb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.sjlbkw.cn/Article/details/gszobnnhf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gqgiprhxi.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/ggmvxwmtl.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gruivzrjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gvtbqgcss.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gpmybnueo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gfojyvdlk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gfurwglmy.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/ggdlhzsmm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gacvwhvlw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/gvefxiplr.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gfyaotzio.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gsiagumhj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gnsvkpffm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/genjcuxrs.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gynpshjgn.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/grdwvboiz.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gnvcwoxgc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gzsvoswpm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gvhmjisfe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gpyxxhexy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gchjulxpc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gdobprpcp.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/gnspznygo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.vehdjk.com/Article/details/gniquudvy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gkuzmbvvn.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/girnxjsmd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gwplgvnvv.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/ggbiwlomh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.yfazqb.com/Article/details/gudjwdwua.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gptzeedpj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gkrxmsaxe.sHtML


<!-- 参考信息 -->