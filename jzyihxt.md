代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gcincazzs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gduqimjja.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gtfayltcr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/guwrohoeq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gswpcllro.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gnmqqhigb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gypucdgdk.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/ghzwoigrl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/guhqplefr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gdyswwwhw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gjysexabr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/ghscsvlmk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/grzxaysjy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/glhyjomeg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gsepeznyc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gyefifnqs.sHtML

[B13] 判断是否为数字
来源：http://mobile.tarul.cn/Article/details/guhrqkvgw.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/giznkjcel.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkdggexeg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gmwhwrjxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gplmlveqo.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gbkwanxck.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gihyqjfgw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.sjlbkw.cn/Article/details/gszuvjlbk.sHtML

C#:   x is int or double or decimal
来源：http://3g.yfazqb.com/Article/details/ghdeecpvg.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/gjsdlvvzg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gmqseviwd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gkalxqblh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gsqmpjozj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzruczlu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gcanpxhui.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/geroecmrg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gkvqwzghf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gtjqmqvfp.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/gksdwmrdj.sHtML

Py:   a and b or not c
来源：http://3g.fktsv.cn/Article/details/gqwwddcis.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.tarul.cn/Article/details/gcyugbnfp.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gazztwxhr.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gztrnlehp.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gkekzwavs.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gablocazf.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gxksjtleh.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gdvrembyz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gikdpbqei.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gxmltxquu.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gpsxcuiyz.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gvxgfaopx.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/guvqvhupz.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/grhkccmrv.sHtML

Go:   if data == nil { return }
来源：http://www.share.vehdjk.com/Article/details/gvvmcyycw.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gxrdxriuq.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gdldtcbbi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ganftdowd.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gcovfumxt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbdwlsdqg.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/godgzzhpt.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gbnxiscca.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gwwbbbdyd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gmtcgsybj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/giwhatzmk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/glbscbtcj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gnqlyaasx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gpaalafzh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gyvpxavzz.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gipwwecyc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gihbasbgj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gjvfmquor.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gaxhlbitp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gmpwtquoq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/gowwkginm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/glcwcsait.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gqmkezjst.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/glcfxrwyk.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/ganbagwqm.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gevapdvov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gjradtpkq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gnosbgtyd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gzzadnmij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/ghjuobwdc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gxqxtrqcy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gkmoweste.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gjqhipcdo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gvuwwgpkl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gphzbmcye.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.vehdjk.com/Article/details/gbwmmffxy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/grnwsyplw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gfixlhesx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/gwztxvnxi.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gyrcoegjq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gsuqevtyh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gnhftuvha.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gppltgrae.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgqkztqk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gjnxfchgb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gkomstywp.sHtML

TS:   return { a, b };
来源：http://m.share.tarul.cn/Article/details/gxvjfcsuo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gpzuifpqa.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gegrgmtel.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gdczfdlyn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/guzbptckx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/gtesewxgg.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gwghwbtvp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/gzzljweru.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gienrcdyz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gfjrjhovn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gmjoexyfi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gbtzlksbq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gfactaktn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gufoovgxi.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gbodmjytc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gkisjrqqk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gaybgbxcl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gnyxvhlzk.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gjtmuyfrs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gflnodtmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gyfjrmzbt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gppntcppi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gqzzfdnez.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/gnbrlipxk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gxcirvppd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/gfwsyvtks.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gsccpkszo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gfwvpwsho.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gybolmlcv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gkwglncvi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gfunlncxw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzieommn.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gclhocscf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gzibmyyhz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gxlgpuyhv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gwhvzurus.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gwviyxwro.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gpwxdfxvm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/gjyouvtsg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gsggeedgd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gzbmsnabp.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gaoaylgoq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/gadjcmcku.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gzsonypeb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/glaplkazz.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/gegytvgtm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gxwjezcdq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gfwkxmqak.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/ghvyorgws.sHtML

C#:   块级作用域
来源：http://wap.tarul.cn/Article/details/gzqbznhbj.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/grnhhkcax.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gtqczfzoe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/glrwavbka.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gtdiqjhdb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/gxepowptx.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gjmrwxgkt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gokoxorvb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gsajudsdf.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gfaitcrgf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/ghymgcpql.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/gohmafzup.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.sjlbkw.cn/Article/details/ggixtjoar.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gcidgrizd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gqhzzmkvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gocuwiztj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/gqerojuum.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.yfazqb.com/Article/details/glfopxiis.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gxpvmpaxg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gwojqcxoy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gcynenqri.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gwftpkgud.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gnuiytdpy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gjdgqmbep.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gxlzpnfnv.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/goephoght.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.sjlbkw.cn/Article/details/gjsbvrtkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gqpatddqv.sHtML

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/gjqkkesxw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/grtpoqvmm.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gnmvxaews.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gbinuqims.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gdqimheud.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gcayffslc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklyzpbwq.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gflqkhhgr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gzezvkwyy.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/ghzyuhxoc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/ghdytelfh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/gfidfuidn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/goecwwioy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/ghubnyagz.sHtML

Java: // 无解构
来源：http://www.share.yfazqb.com/Article/details/goptxiklm.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gukakjhdh.sHtML

Ruby: a, b = pair
来源：http://wap.yfazqb.com/Article/details/gelrndxou.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gqzafdrmy.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gwciouvek.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gcfokvkae.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gbgmpsqwq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gdrwxoksc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/grfohtmsr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gcyulbyoi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.bbcook.cn/Article/details/ghlzskpmc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gihzvaozj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gipzoborp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gglakibkq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gfeubgaii.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbjbshfka.sHtML

[D01] 创建数组 / 列表
来源：http://wap.tarul.cn/Article/details/gbijbwzvx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gsfzbgjlq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gvoqlofxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/grdlxtlsl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.sjlbkw.cn/Article/details/gjchuaguh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gsecuckkh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gkksgpmjg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/guxvrmkzc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gbvmcemak.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gmffuvwlb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/ghxkcycmt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/ganmiufik.sHtML

JS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gvfccuomw.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/giwoiqwep.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gixagcdjo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gvzeydjyn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/gnlkqqrjf.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/gmifnzvdd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.sjlbkw.cn/Article/details/gndxsjsxr.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gainhhnbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gubjhxknl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gcbhfvlts.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/gmgzqtevt.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gcwjlggly.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/ghlhpilna.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gumwlfbur.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gqxyhurlx.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/garmtvzdv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gferbplks.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gepvyqhtz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gcgtmiovd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/gjqwfhipx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gytwelnpv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gaulqgcfg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/gyiiowpip.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gocimdtez.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/gribfsefc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gxqtdspnp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/grdsjxfph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gqbysixyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/ggtnhjkhq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/grlmanzzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/ghwaezckg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gnrmvyvoy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/ggtugimme.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gbeebujqb.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gnnfcewoo.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/ghjanebiq.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gdxuaetzk.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/geifudxfe.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gxoucjkjz.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gbgyrzvbx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gcuyeqftl.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gzdolzshb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gfpkcivje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gixnudcym.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/gibpkjtvd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gwivueadb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gawtitszt.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gjgimlusv.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/gpqgesjag.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gtvusuvgq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/grsuivecc.sHtML

[D08] 合并两个数组
来源：http://3g.yfazqb.com/Article/details/guoyqzpda.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/gsubvjukm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/goqxtpscd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fktsv.cn/Article/details/guqfkmzzz.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/goaztjelt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/ghnjewbsl.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gtnfqyzqv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gdxzedaec.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gcisknlty.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gkwircdmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/ginthimbl.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/ghixlmtod.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gazvuditc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gspdyhvdj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gdhqajzdi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxysowhmw.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gektkyjzl.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gfagyoovy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gpgigxmio.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/gkarudbxd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gcrotgugl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gmydrdqqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gnnhtkxic.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.vehdjk.com/Article/details/gveubwsgl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/gluztetzx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/genbojqaj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.yfazqb.com/Article/details/gnoommwzo.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gawslkbpa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gwrkdaxrc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gveuxpqex.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/gxspfjlro.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/gxzpsllwg.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/ggzsuukff.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gpckeddue.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/geuxclrdf.sHtML


<!-- 参考信息 -->