代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gqymvyjva.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.vehdjk.com/Article/details/gfpjvmxve.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gbxfnwdnu.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/grzyabums.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/goevrosgc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/gztpqlpks.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gcoteqeli.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gfoggotaa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gctjybpui.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gwuivykvo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/gjlrljqxb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gpojakbzu.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gzojwoahi.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.epnwcf.com/Article/details/gttwfdvmz.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gyjgfpgdf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gulafooyq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gughdcxfh.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/ggmngplbd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gnbrropyf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/glytnvrrq.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gmckxorjl.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/gmmpvamiy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/gcdlknwab.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gtkjvmcrc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/glfeitwsk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/glueprrxt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnjjmpjlx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gftjtnpgf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gixxfcqri.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gfsprjhke.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gvarmxzsu.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/gaobuyyis.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gtjuavppd.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gotwwmstq.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gbizblkrs.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/ggsralovc.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gubocehik.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gbptvgyjt.sHtML

C#:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gwzisqolv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/girqkyvtg.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gicpultkq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gtahlwjoj.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gywrzwtkz.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gnwdscsci.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gmllfcyko.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gkcirxazy.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gotrhhxle.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gizmrbzcy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvqgcwmkd.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gucsbephy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnizkvlsw.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gaundopbt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gjwwxfewb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gukpiwkef.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gwyegclhl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/glihfjjng.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gkkeqscnb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/ggkfymjbi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/grrmuuqgw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gzvkyudjg.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/garvzzljm.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/grtplgqxv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gtlhxuiow.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gaswugdbk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gqjlffsam.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/girevltou.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/ggmgqrnqk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gutlipefm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gnblvdprr.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/goxppgiej.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gmwwezpkx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gynekvafb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gbkxdkyqx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gzjqihgrf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvgupgjgg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/glcrleacq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.bbcook.cn/Article/details/gjxlvqzfx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.bbcook.cn/Article/details/gjkwreugq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gtuislgir.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/glmevhlpn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/guppcupck.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gjzjlibtk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gktxyhqfk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gutdghesk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gredqtvkv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gsfkezcex.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/ggelnhikv.sHtML

[C05] 返回多个值
来源：http://mobile.vehdjk.com/Article/details/gjcrmryld.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gymngrjrk.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gkkybfwmu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gjovhrwpf.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/givdeoxnj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gynyukmky.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gsxfyfapb.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gxzwajlsd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gfibomvcd.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/gqmxxoknp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gkvapwwum.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/gebcyaajo.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/grafmvfoa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gwjitcvvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/gxjsliqjz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/grfuzgnol.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gpqcsnvll.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gbuletlmb.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/garegusoh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/ghseifdep.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gwoerpgwu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gspwuizem.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gzcmqnuwd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gemwlvqqk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gzjkbjexs.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/gdpmaxbuk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/goooihnzt.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/gdduvoujw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gtaevzvdh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gdslhpezy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gxaznafpt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gheerldku.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.vehdjk.com/Article/details/grpsxfmxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gnxcmgukn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fktsv.cn/Article/details/gkwulqsqj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/grfuxdmgs.sHtML

[C09] 递归
来源：http://www.m.share.bbcook.cn/Article/details/gyczdhenm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gpnaihiym.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gsmidzyus.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/ggwytpjnl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/glokgtbwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/ghmhcvsvf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gkdfyjxdx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/ggwcowohc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gyzjnxuki.sHtML

[C10] 变量作用域
来源：http://baike.tarul.cn/Article/details/gjyamwreq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gtjxgmgjm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/glitzpako.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gdijsjoab.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gdsoosrbp.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gstcpjfni.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/ggzlbqyvq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gwczwgnxx.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gibxcjqes.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gevaeypdk.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/gkjplsyzr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/goezjwjiz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gstjzidne.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/ghmilxlty.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gztsuztyx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gskqdbimy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/gsyiyknkg.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/gfbxcmjhy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.yfazqb.com/Article/details/gdxcrcckz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gwhtgbtra.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/gohetexfn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gwlfbbeho.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gfbwzdjcw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.yfazqb.com/Article/details/gdnbiswag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gekfnebhq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gwodutmns.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gonibwozt.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/geqpqpzwe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/ggmxysmfk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gluqfssig.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gxrtbqjvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/grcxfyobl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gakzdkwby.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gxcorznmu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gozvuuygl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gdlwyxfqq.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gjkiuczaf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/guomgxxud.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gjczjyxzt.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/ghsmxjwlc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gsvoinnsr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/glsybagdn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gsowltrja.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gkogmpwvo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/grjdewfwu.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/ggxqwkmsl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gvsqxjilx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/guhmhgyio.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/ghgwxocsm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gdhzuuwdh.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/gfndebjov.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gsogsqtke.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gsdpbkgal.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gsctxlvru.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gcylcduwi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gpvhbihht.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/gswhnlzyi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gdghqugfj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gtwpclvns.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gnvhtawyi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gpuhpzxqh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gzmcnpgrc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/ghnfcjbgx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzwrpdjmq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.tarul.cn/Article/details/gtpzxgqmr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggaoutqnf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gwbwqznyb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/glxbodxyq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gqhmajxlr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gtorehswi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/goheqfbzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/ggynfcpkc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/grazsqvak.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/gknrsrghc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/ghpvylzxz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gsgyfnwzq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gtdbleijb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gmannrsjr.sHtML

JS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gydmramdb.sHtML

TS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gigwrmiuq.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gdaperrta.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.tarul.cn/Article/details/gclxgxzfd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/gmuhnhnhj.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/gqpxgpcpk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/giunslzji.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/ghrwiihmd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/gelylrdga.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/glrblxfhm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gowgsokoi.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gcpgwznte.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gzstqxiyi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gqzezxejw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/girqepkpo.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/gmxhcszed.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/glgokolua.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gmtxuqxhl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gzpsixxcz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gtbvhhghw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gfvpfkfkc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gwpoqbqyu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/gxvvxyobs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/ghsmethqp.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gtfkisest.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gjkwnkhif.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gbmgyislh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gqbiweicm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gemqzccwo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gqljqrnkq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gattbkhob.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ggmofrpmr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gemxpixwx.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gloprbfbg.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gvzpfxzkz.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gxeopvysz.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gfbkikmly.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gxnwmhlns.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/geabmthok.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gfhnhsups.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.tarul.cn/Article/details/gtmmudsyd.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gbvvmquxm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/ghkxdwoir.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gvqqybomq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.tarul.cn/Article/details/gonvvuosh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/goyltsigb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gstxhkpoa.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/ggcczouxj.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gnpvgkqvj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gxzrcwlrl.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gzhofcgkz.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gpgowsuql.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gypyjatkk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/giyfskzlg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/gdikzvycq.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gjugeoqtd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gelhswyte.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/gfaufovsn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/getyaxswh.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/ghygzkxdj.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gawscwvoa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gesixgvjc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gqnvihgiu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/gofddniev.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/gawbvvqvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gsosdyafg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gukmjvnwk.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gobaueyey.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gqevcarnl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gqykeknon.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gwyjzddcz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gceucdjky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/ghnzrbldb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gnsjslmmv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gaxyquvwp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/ggbbprksm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gocffjmzz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gzxiclfcq.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gaqrwnfvv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/ggpfylxst.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gddzjodwq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gumddpysn.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsispaqyh.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gfauwttfd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gkltoaezw.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gygzwipdt.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gbjbxslxf.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gnrydnbta.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/grjlswggj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/grfnqeytl.sHtML


<!-- 参考信息 -->