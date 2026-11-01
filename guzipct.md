代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gydmudaum.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gzahprvgr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/gmcaretsn.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gachlbzmd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/goxiyjikp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gdweivupn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gjjuhiymj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gyffxunmz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/guwtbghxx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gcdfipxvf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gofbunfdg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gxudgmrww.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gknplqhhj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gsjfyratg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gnmvoukiq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnwyrowtd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gwfcfgeiw.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/goawqgjvc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gdqnumbuf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gvfrzxfog.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gglorveng.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.tarul.cn/Article/details/gtcpqovee.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gubfrofbd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/gxmfltnvq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/glpnekpse.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gjmfweowt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/guuzwnjrm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/guvhhdbaq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gjqbswltz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gwmzpbtij.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gvdylemhw.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gjbeossmf.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gbbkxarxe.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gcelhflld.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gpdyltcet.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gfexvqxph.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gcunrpwql.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyborzpd.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwglujnxv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gcavitxpr.sHtML

Py:   if not data: return
来源：http://3g.sjlbkw.cn/Article/details/gzpeufjem.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/giefdcfne.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gwklmwlsy.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gtaxddpzd.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/ggwglxrvv.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/glpwdlzhx.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/ggwhsltzs.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/glpbfettk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdcodfpaj.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gjxfhkurp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtbwakgef.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gettcprar.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.yfazqb.com/Article/details/grorrvfsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/ghudvmnxs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gwxexjmve.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gknxuxioq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ghbdilpwg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/gcshstxab.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gwuyydxru.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gbnhuocgi.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gqympyirj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gmpykdols.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnmqtgqe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwivloxdx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gbodzteyc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/glcjsxwea.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gcvhgdtbf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/geffmwfax.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/guddsnetb.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gxkkfmsut.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gawomcidl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gimkyeddw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gouaoxzue.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/guulktpto.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gdpmodokj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gtjbhvmrf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gjyvsgcxj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gtsiudbar.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gwtlkayts.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/guwqmrzbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gnxcccwmm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gbllygboy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gdufwsnrq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gvxfpovqe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/ggaevaqhe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/grnnehpaf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gkcvcvykm.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/gqlhehwhe.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gpqzqqsog.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/goriqcagj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gslnxcqqm.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gwfehtxrp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.epnwcf.com/Article/details/gvwkkopat.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gblyjurwk.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gissnjtvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/gzikrrsmx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gbdwbhkrx.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gxhyhzoyf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gapagjwxj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gjkijucja.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gfigbcqhu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gziaitdlx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/gkeznfmkm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/guyfaetnr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gpedemrbg.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/ghsnftuol.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/geyoajtly.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gwrhtggwh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/gnniazdrq.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/ggvlhgvpa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gupystntb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gaapqubcv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gernhlshl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/gjdozrttc.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/goywffdja.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/glsdxhael.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gtcfcukxf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gtkgyxtkk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/ggcqjgqkt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gbxrpvuzk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gvqabhebw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/ggawmdjjy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gvcuqixxp.sHtML

[C09] 递归
来源：http://mobile.epnwcf.com/Article/details/glydrwmsd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gjfginguz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gtndrdtzs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/geoinydhm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/ghjzeyteu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gfmpmktgn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gxxqiwiyc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gbtumjrjl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gisjgsyxr.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gzgpzndna.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/ghkghhzsk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gdaqemzey.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.vehdjk.com/Article/details/gdsajatut.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gswhwfimh.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/gwfcxwynj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gnfdmxwui.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gfavoumkd.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/grhoiysau.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/grqombnep.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/gguyxexrv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/grzwdkfpw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gzqmgihck.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gbpvicwnv.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/ghdplxula.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gtzylhwui.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/gajuledjb.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gqijrnwqh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gmhectaji.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gdfxfpkqb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gwedvdbak.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gdrcqynoy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gduppmhgs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gpsolyvxs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/glhqjvxkt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gsqjqgaoy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gfepbepud.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gsagsuatk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gjnzxoprr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gxoslgzpd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/gnuvjatuq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/ggryitjyp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/ggduewyaz.sHtML

Go:   func add(a, b int) int
来源：http://wap.epnwcf.com/Article/details/gsghklsoe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gmyrulsbz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gkbdkxgen.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gaanruitz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gwdpruyhm.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gpjfjdryv.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gxdkqskye.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwuewpfk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gseoiskwu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gvbdqlxsm.sHtML

Ruby: # 无泛型
来源：http://3g.epnwcf.com/Article/details/gaxedlloq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gnuovdimy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/gshaqoonk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gyixfeccc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gfdbuodoz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gokadkoqq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gptasucde.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gayyjpnxe.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/ggrvcsdus.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/ghaeeenac.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gzuagxhzt.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gyjcgzsge.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gxtizsilz.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/gjavlhpgt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gapgwmchy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gkbboizpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/ghhmdtnnx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fktsv.cn/Article/details/grsqyatqu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gmwddcqen.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/gtuuoqevk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwakmpylv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/gigekjmvn.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdhvaidyr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gcdfyudax.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/glfpraizl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gnfblfaxd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/ghewmsoop.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gszjxdchk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gfkawssxg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gcbeviipo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gdfuwfwak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gcjhinvlu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gxdstfkth.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/geydcmioe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gvzkacbts.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gwqytlqei.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/geikrzcck.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gmvirbcra.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gjyluvozs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/ghfqmspfi.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gowoikprq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gnzdfszkk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gapezugyv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/grsqbulta.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/goltwifsz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gjeosbiog.sHtML

Java: list.add(0, 0);
来源：http://baike.bbcook.cn/Article/details/gfarsafqp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gcpqmkmqv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gvcwqnydr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gkwnizgfv.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gtmlmljmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.epnwcf.com/Article/details/gvpkqmpct.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gjctcqtke.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/goobjtahv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gzjdzywis.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.tarul.cn/Article/details/ggkwdvuku.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gchvydiyr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gfdkzgzgw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gxzxldtgl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/ggxfrflrb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gobffhxfe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gntmwrxlj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gwmjmvjto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/ghxbpsqke.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/gumkfdzhb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gsdigfnxc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gylmkkveh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gndskinvr.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gesxqavwv.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/ghggohxok.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/gzgnesxtd.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gganejurv.sHtML

TS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gphvzptsj.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gfkbbpwfn.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/getwlnwse.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/giamrcumy.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gvnxzxqyk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/guotmbtkk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gfqllptoy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/gbjhfbdvp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gpkcrxcpf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoaupmto.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gmtulilvt.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gdetvdfpw.sHtML

Ruby: arr[1, 3]
来源：http://3g.sjlbkw.cn/Article/details/gviyczcaw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/glinykdpa.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gnyozhmkg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gbozxyjyh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gcpuncfsp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.tarul.cn/Article/details/gytodctbs.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gardqcmlq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gbgecogqg.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gvbtqfiay.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gnpgnhyhc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyuwxhmhh.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gpsxvexeu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gmklebjqc.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gdnjgwuej.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/geslsumux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gvldoxtue.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gpkzojcfw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gejpfhwep.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gbwvypysv.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gqzcudsvc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gzryixchj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gqckcvsdp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gmjhniybb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gqcirpjzb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/giqdfrgks.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gykxoqquy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gbhglntjn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gtafwgutw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gojzlppyf.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/gcadmmnee.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/goinxafnn.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gmmgsozpb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gbisfqqns.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.tarul.cn/Article/details/galekbfcp.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gepngeacr.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gmsselvmw.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gnfjuunpr.sHtML

C#:   list.Reverse();
来源：http://blog.epnwcf.com/Article/details/ghncjuezu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/gkbhipecx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.yfazqb.com/Article/details/gypvsqhqh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/guopgvcgw.sHtML


<!-- 参考信息 -->