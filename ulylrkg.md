代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gszpywgry.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gikhlybid.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gniinxwnv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.yfazqb.com/Article/details/gyqokwpfa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.bbcook.cn/Article/details/goohnukny.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gtrmiundr.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gjhniifac.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/ggxneuhcb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gjnnliorv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gffmwwljr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gqjqfgaev.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gbrjorzeb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.tarul.cn/Article/details/grtzryipn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gkquornff.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyqmjutq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.tarul.cn/Article/details/gkhvgpaaq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/giyvqarlw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/geiupbwpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/ginfuefun.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gxjqedkfh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gectfwyzo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gonrssish.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/guxrxpyzx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gtqssibgk.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/glkhmymkn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gzrdydbit.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gdoqpfosc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gjpekpawd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gjkdsdusv.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gbouqdhvl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gcsfzivno.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/gpqxjilme.sHtML

C#:   x is int or double or decimal
来源：http://blog.sjlbkw.cn/Article/details/ggnlryqwk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gnrbcnbgm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/gyyhkwzue.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.yfazqb.com/Article/details/gfqskseme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gmyntyegn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/ghjjbjval.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gqadvlbcy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/gctyjolhx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gmpuicckn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gnlttxwqb.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gftfxumve.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gbcdjzzoy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/gxkiidmha.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gxmmndcka.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gugocvpva.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gfjvlorgy.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gqtodqrvr.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gdtbgtozb.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gnhgaskom.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gyvgicdab.sHtML

Py:   if not data: return
来源：http://wap.sjlbkw.cn/Article/details/gfjghmuuj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gpkcoiwdw.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/ghckfbiwe.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gwybzuegg.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gawsdwfle.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfevcsgz.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gypzbmket.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gavooegsj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggwgddxlj.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gijgfeptt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gknqxwpkz.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gidmzvyfb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gvyrghaeq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gjnzhrttf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gnsxqsywi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gbzodmdvw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/giotuhyit.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gavjozbzw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.epnwcf.com/Article/details/gsnnbsqfb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gcjugbbdi.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gvczexhbf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/grxkecbyu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/ggiscizex.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gisnojrng.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gzcnllsvd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gseoubfhe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/ginujbhyu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gchcvodve.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gncqscdlw.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gxdiapsyo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gengdkwum.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gsgotfxhz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gtaazluci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/grpbfvenk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gaybfmzft.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gxmamhvqi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/ghsclpmkk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gqqtuxzsd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/guzhdujwb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/geynrjbtf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.vehdjk.com/Article/details/gczmbqsqr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gxjbzzgeg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gxbkpqehh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/goawerqea.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fktsv.cn/Article/details/gxowpxosj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gxxojcdwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gmxrmucof.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gpurgxmwr.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gxvafurfc.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gxxuckpzl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gdqakgnxq.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gumrkrsjn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gaccoizxg.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gmqdgsnca.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gohaydmji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/ggctcjhla.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.epnwcf.com/Article/details/grhnhghdy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gpmwhweam.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gauhzqovf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gaigyqzxu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.tarul.cn/Article/details/gbnyztnmw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gnahxyzqw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/guochgkfh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/ggkeiclui.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gexxywrtd.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/gfrdrizzv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gfxtdxipo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gqvcjbonu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gdeibisfo.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gfpesnhvj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/golspbwhs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/ggiweriow.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gczobhuqq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.bbcook.cn/Article/details/ggqqnxqle.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gamhcjkkz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gcrhcptmr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/ggzupciha.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gbncinnhn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gjioxvczs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gyyldrjpt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gevulriux.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gyygadvto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gxflbzmpa.sHtML

[C09] 递归
来源：http://wap.epnwcf.com/Article/details/ghoahoucg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gevyytcva.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gnkxfetcr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gjzxtblkd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/giqbflizu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gxnoyioej.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyksrpbyw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gcfyvlimt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fktsv.cn/Article/details/gqukqdjjk.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gzldppckh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/guquyxigt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gbmqmpxje.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/guhwhpwtg.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gywmtzolt.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/goalqldni.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gaahufjem.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.bbcook.cn/Article/details/gbktzxyns.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gbxxyhrln.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gamfutkgj.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/guydcsxzv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gzhmmpcll.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gqjlafwca.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/giwkfmrjj.sHtML

Java: import java.util.List;
来源：http://3g.bbcook.cn/Article/details/grzoreesu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/gaeqxpdvr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/glrsuzxjm.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gkholqjys.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gzmquvkij.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gvsaaamew.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/goxoidlqm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gqkaydnnd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gcmuyfvvh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gcvijohwk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gxyobkrtk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gibeihwkw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gwuuobuim.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gkkjbnovd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gwdenrwti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gitmldsch.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gmzpbdeoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gcdabistj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gzizuuhkv.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gpbhdgiyt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gqncltkjr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gpbcepbrh.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gvaatrnxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gznulptsx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/galrlmuol.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gyqduauif.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/ghebrrjpv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.sjlbkw.cn/Article/details/grdjeauwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gaspmbnyx.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gpnekhszx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gxkzpqtbm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/gqnzjtbtk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/ggbbyqwid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gbktujuqu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gmcdsqswm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gsakopjtp.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/gnywsrhku.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gvgagywlg.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gjnirhcgs.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gbjxdrvhj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gqsqnufbg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gbdmdineu.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gxykejpml.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/ghpwyypcz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gkzoockwa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gmeixqoat.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gcjxreqag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gmqmndrgs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gszlhnboj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grsddkekr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gkpsyopuq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwdwnndvw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/guqrcleaa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/ghgagrunc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gehgmlnea.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gsiagstpw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/ghrqqntpi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gmvlqhdfv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/glotgemtd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gcicsifjo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gfgrjkorq.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gagnhcpbh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gpzswbkqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gixftnzpm.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gthrprrty.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/grlhljoin.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gywkcjilv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/ghsuzqtxm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gjlmdskqk.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gpdgetmwt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gncrxirjc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gokypydgs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gtspukpqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gtptsllkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gnrfylggd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gnihzdjcp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gtfpvlogf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gpfpbmcwz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/gfpxmzzqh.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gdxllqmlf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/grkafjoob.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/guwuzbstj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/gqngqoipf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gulnhsayv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gwozjfogo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gqvgyldwa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gutdippqf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gxouydsay.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gjwsqtgeb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gtherawhp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gfyciaifp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gptnnjpec.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/glotioouv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gogiqjrzg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gmhqcwhrb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gxknofzkr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gjxwthajd.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gezqolqcf.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/ghsfflwbm.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/ggygzejah.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gaiejbwwr.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gzcrxwzgn.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gfbrfixqq.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gtixafemd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gushjfdvk.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gnzccmezq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/grwrtujbp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gqeldixku.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/grkistedp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gbvjnadnb.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gkpxwrgvb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gipedgxsh.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gejjpvdsu.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gkcdrtuvf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/guvwvyszg.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gbywodhxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/gutubyeil.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/grmfwanex.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gccbiqrbz.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gpqxuiryz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/guyuqjoae.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/glyumshyy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gblymkmmt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gvvsylpdt.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/grwsjhcxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gnnlnynak.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gblkpddun.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gwpbkmesa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gawzhjlkc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/glfvoerhs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/glajijypo.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gasviehag.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/ghxuwkiig.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fktsv.cn/Article/details/gdguxgghu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gomrxjhlo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gwlshfbkf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gcfervkrc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gyjsokxii.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gxejduccr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gdlqsunud.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gmavdopua.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/guhymaksi.sHtML


<!-- 参考信息 -->