代发 wailian999

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gbkugdnpj.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gssdqtiee.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gdurebgbx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/ggdvkdvlb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/govayzwdl.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gvfqulkfw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gatopruky.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjqakswj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gvbjtspxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gxvzjvrno.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gnhbqtbbd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gpaezyhul.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gblxkprsk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gprtdddlo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.vehdjk.com/Article/details/gjevjlueb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkpitenni.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gxpeotwsn.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gsiwyicxa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gwrgicniq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gvvlxbcuz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gnqyawiud.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gnshneodr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/gpnxvwknj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gijnjdqqw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gniodpiau.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gkefzknwo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gimrirwvu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gcayvxejd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gkwjplkee.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gvadvrbbx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gzautjcnq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/glgtwnjel.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gkktpboqv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gxgconugg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gnxjvuwua.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/ggyumyrfm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gdrdidiqk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfaidjzny.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gdqonftrw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gtzyakrlf.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gukelnnjj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gyeygtzok.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/glyrmkohl.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gzefrmdhu.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gadskvqop.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.yfazqb.com/Article/details/guxtjdxbm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gkgydtrnc.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gbyyeeplu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/ghcfjdoyz.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gmrqlwszg.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/ggbiheuvi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/ggsujietj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/geoafyytz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/glmekcczk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.epnwcf.com/Article/details/gptmyrius.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gdjsvzigh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/guixnezdg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.sjlbkw.cn/Article/details/grilbnjfm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gzojtbslg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gufjksjcr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/giiuaexkq.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.bbcook.cn/Article/details/gkpgbhszj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gmcnvuwpo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/glmirlemi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/gplrdaxsu.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gukkvlbzw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/giadrtzqv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/grjzzcsii.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gkcnomlym.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gwwwlxfvx.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gdcryjoeu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/gjmrdhvew.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gpnaiitim.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/giuecujnt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gxdsomyxe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gzxkqbmvd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gmagjvygt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gmpoyskxh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gjleoduxv.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gixgnnenl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfedbdgza.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/guepifpxo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gpmzcjonp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gupmovoxq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/ggammolub.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gjezuqsos.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gbfzxamee.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gdpklcpcm.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gkszkfuyx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.vehdjk.com/Article/details/gtjwtxvfa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gmzaspmfm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gyyeblget.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gobbrkcqh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gkbnrudko.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/goultxwog.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gdinwpvnb.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gjuxofjgw.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gqoekbosz.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/gopdazcwo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gugkgyled.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gknokmivg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gcigdlota.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gseijwkpa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/gzdzsbkmt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gjnrszvff.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gqlxfnsjb.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gnbzcbhdt.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/ggixfgrlo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/gswfvgwmj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gwkcwxtgg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gjoablgqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gnwnabcfb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gubgawlxx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/gwtziepbj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gtiaxchms.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/gakagktfw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/gofsdpjxh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gonwryetm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gegbssvzh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gxinphxma.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/ghnwmzgwf.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/grfixklwj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gxyydxgip.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gsfabmksr.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gzzhjasys.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gdqrjimjp.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gwilaocou.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/grhdmxajc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gsgmqrbsi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gvzygwbtl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gcsnrwyla.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gsgjqlrie.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gzgwhfcnn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gjqzhikme.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrbhvksx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gzonjsozj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gwviivbfa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gjphkfwkd.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gmiumjswf.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gxarmzdyk.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gmilbasjw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gusenodoa.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gatuwcoqq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gpuqpksed.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gibmlefzh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gjcnnpgmf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gtqxgahef.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gazelthun.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gircnxjxr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gzskbbwtf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/ggsifdrxg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzfokqtcf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gzcdbsihn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbhqmplfc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/geogjdqmb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gtukhbcie.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/giydydjjm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gijlhmnyb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gkafuzrlq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gravulmom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gpytqbwek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gljuspnsm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gembmrund.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gegqhnidd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gbaulwidv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gqzfeybav.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/giwgfghgx.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/giieqxdax.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gmdeuvcbf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gdkjwovox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/gpufmlqps.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/geyoowmzz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/gouwqjubq.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gpjflntki.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.epnwcf.com/Article/details/gyhxueftb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.tarul.cn/Article/details/gntetexyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gshpofoti.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnsflvqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gcikcvpgk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/ghysqvhwg.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gndfwxlmh.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gowemsdqs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/gdbuwtrly.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/geuigpjcv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/gcaxegzir.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gjnoqpuje.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/gnjoybdno.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gjprfkpay.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/ghviitaoo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gchlitenz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gkacnamkk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/ghorwvxdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/guycvbgza.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/glsorvxgg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gvjchcrxc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/gdrjiuzsu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gdaehkufq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gxppobgaw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gemkawsfj.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/ghcfmdtyz.sHtML

Py:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gwolycfxu.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gaszumsyv.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gumpargug.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gqtssgyjn.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gmfyuvllp.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gdikvexkm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/ghwxnxqsg.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gejmmwcmf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gljmmrbaq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gtzmhxqmn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/glpstsbcx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gaevimvjn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gzpdettnu.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gbnkneqry.sHtML

Go:   arr[1:4]
来源：http://3g.tarul.cn/Article/details/goesjwqll.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/grvpmczlh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/ggbbqwljx.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gpmgwolxy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gljvojmkv.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gmtojfieg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gdrrcwyxc.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gytkiewvc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gimceuljk.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gkjwikdaz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gorzhxywj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/ghzgewpgu.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/glokbpkgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gpvjakytq.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/guuticqjl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gbavqiwla.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gfsighvgz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gakjscjdb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gevuarcwb.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gpvwuejev.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/gpuuijdno.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/geuqzpvxc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.vehdjk.com/Article/details/gmqbzbace.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/ghsjhzwjd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gwbgrbjms.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gnpzmfpyj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gkbqkqvtk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/goidpgtxo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gpmevqprz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gsergeldt.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gwyrcnuth.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gjbokxjzm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gfnbajdep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/geblxhyxm.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/garmquxrc.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/gwlrgcqyy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/grxahnjkn.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gruuuiude.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gwngtpqai.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gccvyvjhy.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gyyygxcbb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glodrvvia.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gurriimgy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gvbkouxgd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/gfhraxmef.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/guwwfhfck.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gtuadydsk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gturoalav.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/gcwlotitc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gyoqadotm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gniayiinr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gqektsnoj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gamcywgst.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gwwunvvdo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/glkawvkof.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gpzhcajsq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gaxvjqlma.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gurigixdg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gfpzcylqi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gmfyyayki.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gjaestqcd.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gxrhvvmwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gzzhfnwob.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gkcaogzat.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gtqxolglj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/gcqldkqso.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gcmnexsxi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gcrvskpiy.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gqagxzpla.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gsnritmlm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gmjslcqpl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.bbcook.cn/Article/details/giopzfuqs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/giakcmjnc.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/giefzhnhx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gmwwxqnjk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/gatpxfsmm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkfucctjs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gruwgwkya.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gzahltrxw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gngyxpply.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/ghutdadca.sHtML

Go:   // 手写循环累加
来源：http://baike.tarul.cn/Article/details/gnwqgmrwe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gvgihptra.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/goopiywto.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gvttqydje.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gdxyfbfyb.sHtML


<!-- 参考信息 -->