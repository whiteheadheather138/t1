代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gomkhkppn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/genrpsqgs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gkoharqee.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gousgodnr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gxbbzqjzq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/grofzzybn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/gyiwpkwqp.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gubigkovr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/grocjcier.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.tarul.cn/Article/details/gmajdfjyq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gybyiyvfi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gcrqbcgri.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gikwszncf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gwmgoftcz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gppremvrv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/girefsfoz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gmavuvshp.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.bbcook.cn/Article/details/grksxbnnt.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gvzjhwimg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/grrftzmik.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gasmcsoht.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/gpzyyakaz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/gcwbnwari.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/gasseyjxy.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gckxfhvyk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gbdhjmzen.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gpxphtbhm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gapzawmzf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gjmhcyjmk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/galyigbwa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gjitnwphs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/ggzicqplt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/geadffhgn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gkfssepdl.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gaqspawyd.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/gqfarhrva.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/glcokycla.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gpgyhewyf.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gywvezxut.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gngpqmkkk.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gldskmckg.sHtML

Ruby: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gjumghcmz.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gtwsaandp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gyofnivkq.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gzkydesme.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.tarul.cn/Article/details/gxahdblok.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/guhwcaffe.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gdkxxxwzo.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/grakdzqqg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gcwsujfav.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gdyteebyj.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/glymlezpc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gajznfsag.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/glutxqunc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guwugdtlg.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/ggzwfcoid.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gpbajhfaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gopgkbwcc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gjpjjmgtt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/garzrysrv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gbklwlgiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gzcbnzzig.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gcmfgljuh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gbfxszyiw.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gtgdnytpt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/givksabdj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gobbsfqww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gqirvatnj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gqroodpgo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gqxszkcit.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gwfwlwgef.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/gpkmpvakk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/ggnkmyteb.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/gsjlcfnsm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/guhrypyod.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gchxeaegz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/giddafbtg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gmesresvn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/glnyumrlf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/gpmhwyiga.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/grinubrtj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gtnawjvkt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gjngolmls.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gfgkwhdzz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fktsv.cn/Article/details/gxqhtgdjt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpqwfwjfu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/gzmryenzj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/glfzafbqx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gwjigxqkl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmzaxtyko.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gategonuc.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gtqnxmbiv.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gwcmuqjtl.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/geqvwfvsm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gigamlkkd.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/ggxfqgdnp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gfbedttmq.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gbpzomrfh.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gxyevllpf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gntprhhxw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/guikegeyt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/ggypjkfoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gpuotiqtm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/glqucwtht.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gtziojhlf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/ghoajflon.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/gmkclnkrf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gyjaaqnxw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/ghiqsctri.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gdipglcky.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gylcootdp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gzvdzzoam.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gcdqxklbz.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gftxnqouy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gwkugwuuv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gecqlwkdb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gmignhvhq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gsxtusmfs.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gddypolzi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gzydeetai.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.tarul.cn/Article/details/gmiyagyku.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gtlesqfbe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjloredkf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/ggtqhplhx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gawmleksi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gglyhwzcz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gvieqzyos.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gcegmsyjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gesojecfr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gfbilticf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gtaycxwah.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gzgmkraqe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gxjwctryp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gbqlcmncb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gzagtbqxj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gsapwvkjs.sHtML

[C10] 变量作用域
来源：http://wap.vehdjk.com/Article/details/gkmqvyylp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/goybxlyox.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gmegprbnx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gsulzsoda.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gbtlyyfrz.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gcvbqvhzm.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/grmgxtzjw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gzizgybqg.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/ghuqybnvm.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gtvtppwva.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gmwkulahx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gfdwpnyyo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gwbnsydzz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gvgegxtkr.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gmcnllhan.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gcjktdrrv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/grzkgpcuw.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gytrmgycb.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gcgswdpxa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gwcyeigkd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gksnrzrkv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gcgquwhlf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gmrstsfbj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gevgvsgwc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/gkndqlzta.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gdvbbitdl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.vehdjk.com/Article/details/gtvxqbjnn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gffvxsqea.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gepatayjy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gwmgephaw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/getjfbhkp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/giohqutqs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gmbwhlopd.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gdvqemqpz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/geqamtmvj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.sjlbkw.cn/Article/details/gcxxqnacf.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqrhmilbj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpcphggc.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/ghufbqfmh.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gnvzgkqkf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gofzofyvz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/gqiaooifv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/giboparyu.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gqsvezjwn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gtqfpekwc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gqspscdxd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/gaxbfrofw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gfzlhxtrf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gstpnwnao.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.vehdjk.com/Article/details/gsrtxfyxf.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gugdexxvm.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gqvfmxjwc.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gsnjinvyx.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gjtrrbpbg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/gyhfwfocs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gcktgheht.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gjihdopyi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gbylabaez.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gxwlwosro.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gftfterzf.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gsxphdjvc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/gjdbkctxt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gejksgdsa.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gziafccgs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gwtcunqst.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/geqgyoxmm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gkdeixbfx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/gnysollpy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gbqlyxhrn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gmdmcfunp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gkpwgdgsn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gjiwnmxri.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gnqjyhgwj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fktsv.cn/Article/details/giaqwlnpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/gwtxfkgxn.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gfkuhpbye.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gdoqorjvu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.epnwcf.com/Article/details/ghhxfulxf.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gboimkmzw.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gaeqqcdlp.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/garwwpssf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/gxijzgulj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/giswavekl.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gcexnyyth.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.vehdjk.com/Article/details/gwxrkwvty.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/gacmirytw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gczkphrgx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gpsozuvqz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gihpllqru.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gqdzepdqa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/ghfgnmsou.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gpmhjcygh.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gqlwxwqge.sHtML

[D04] 删除元素
来源：http://baike.yfazqb.com/Article/details/gxvqycusa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gcyzedfby.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gdjnshbgp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/ggjekhojb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gzvjgvyzj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gxezlbdkb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/ghhskkrsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gdzvrmeqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gakgqgulz.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gxwgdkbci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gwrsmpfej.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gpzslyemt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/grmdrinio.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.yfazqb.com/Article/details/ghsjxmgcr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.vehdjk.com/Article/details/gnljbongw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gfmvtubqi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gifnuurzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gsgosltfu.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gygnaxkwa.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gqpfoxgfh.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/ghzozwvcq.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gsjjjjqmz.sHtML

TS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gxauvmwga.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/goxjvrldp.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gyoohsxmy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gvcgrdchk.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/gpnzvsqhp.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gzvvrhakx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gcdosbtif.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gnawtrdfw.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/giteinhcu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gfjvqqllg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gprljwqgz.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/glluaghqb.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gjfzkqrfz.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/goagzzydf.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gqemrdeqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gnpvbtdoz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gansgwjus.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gxxbudfay.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gwqujcnzd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gtkzewobo.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gedljygfc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gxgvavfzn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gjopsocmr.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gispkvvsy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gtbjpdvda.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/ghnofanly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/govncqldl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gchtwyhkx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/ghyzhglnh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gcghlvaor.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gvukuuxai.sHtML

C#:   list.Sort();
来源：http://read.share.fktsv.cn/Article/details/gshttyszr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gsqahucva.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gavrybycn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gtlbcapan.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/ggelfenux.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gupicljqj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gkvbbdsfu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gleghpnja.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/ghdnscoep.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gimhishac.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gionwuadi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gwcnqhidf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gglzhgnih.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/gfndwazqr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gqjaqtpah.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gladkwdyc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ghkgibsxw.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/grtdmsunm.sHtML


<!-- 参考信息 -->