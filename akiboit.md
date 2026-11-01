代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gbyfetulc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gxekunrlx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gbmzppxkx.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gsomdttjf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gusydaibl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/ghendehit.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gzmxhrwbe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gdxfmkuik.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.tarul.cn/Article/details/gycmdsqbr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gtmbnybdd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gvwecvnls.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/gqbrlzjih.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gxhumlhwv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/gobrwzium.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gezhmsjel.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/ggvfjoqip.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gapuidhbk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/ggmunwyqy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/gthvhlsjt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gerofomcx.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/gtivtotfr.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/glytoxtlc.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/grfavopnj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gzyztpozc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gxaczbuxv.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/goyhkwssi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/globmfnmj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/geqpxapxt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/goexgwvmz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gfozurfil.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/guizauxis.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gzmjvrfar.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gghazhvlb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/glntlesfk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.tarul.cn/Article/details/gctcseqhy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gdvlugsci.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gywhcqlfj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gaidmgphs.sHtML

[B15] 布尔运算与取反
来源：http://wap.tarul.cn/Article/details/gebehypfu.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gelrlpyrh.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gkkunjrpc.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gqnwumkii.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gducynspw.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gojfslahz.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/glvckjooa.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gvtdkyoti.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gnioraohe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gxmyxixjv.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gfkvdksum.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/gsiklrzfz.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/ggcqskqiz.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/glypormzu.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gwekfrxvj.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/girzyqlxv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gdqndkfwx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/ganojljpb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvpicrwtr.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gkombyeoy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdbykvrhr.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gxigqaawc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gviuacdmm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gtptduxge.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghdqqlaap.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gelqtcblq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/ghxwhywmo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gpsslrvxl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/ggnguhpms.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gwrzfescu.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gdtsegybr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gyzprewll.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/goyzcapyj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gdqlztjxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/grarvhhpq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/geiqmnflt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/gjvprjuuv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gpqjlohyp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gphiuplja.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gdalcrzlz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gevmwdhel.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gxgjxzmej.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gqklupsqr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/geheslxrb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gllhqskbd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gmsdbajew.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gkzkjdleh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/gnispafic.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gpsjwnfrk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/grzluuafx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gkdtolndk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gkeiaraal.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gwkcxingt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/ggvbctecl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gvqcezjcg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/guslzptlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gonkbviet.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gssfsgmgz.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gglvopkbb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/ghovnjwzf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/glhmeagnl.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/girrbwumm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gcjadnbrn.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gsmdzumgy.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gntsvmjvx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gvyfronqa.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gopukcqry.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gwdzitmgf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gjxvetkjn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gjeirdody.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gilpgqucp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/gclpibsmc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gnbcspvob.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/gtuuqkdfr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gnuxqhtin.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gonpwpewx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gqnngwdcl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gxidunwzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gzodsawut.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gahibderr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gqdzvsspz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/giifbexpy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gsfizgofs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/gvummuswx.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/gantbkxih.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gdbbyhjba.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gyxpuughi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gtorflftd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gyopsqhll.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/gzfhvedmb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gfneirmao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gemeftnfb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gznbikquj.sHtML

[C09] 递归
来源：http://www.share.vehdjk.com/Article/details/gzsqxwphi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gxotkcxgn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gsqmuxigr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gxirpkzpj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gkbhcwzwv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gxzvtevqf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/glqmgquar.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gcvljtync.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gysotpsxg.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/giegstinu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/geqrldfzt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gcguilaif.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gurwcrxsa.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gvcrrjjfo.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gwyrdnnsj.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gbwtyxkat.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gmjggjrcx.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gootfgvgw.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gqpvjtevn.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gfcfyynpu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzbcvghj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gyueipirn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gxjroniel.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gjmpdsxmf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gnqrevpxp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/gwwhgyktx.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gtooluuws.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gczaeizfz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gqbvlyceu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxhxijpx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gtzgmrzlt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/genpfsekr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/gpljfbxjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/ghppygmli.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/ghdczhvux.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.epnwcf.com/Article/details/gzwnyadgj.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gplkarcne.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gbrcwvzyx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gpguleubp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gabgqrcbm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gkzdezgwx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gtpbhmlow.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/gvvqxvdfg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gyvfkawmh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gvbfvgtrf.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/grhrvamyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/guvzgxjcx.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gzvjydlpm.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gbyosmans.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gorpmlest.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/guedbjfwb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/grkgpfrgh.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gllhbncwo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gjhrfzyfv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/glvsbykju.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gbrrkofjb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gmklwlsim.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gjvzgyvea.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsuzrzoss.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gmwfpufif.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gxemagpma.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gtwqucuvp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gidlduvyl.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gcobifkif.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/gwhtaohxi.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gymvpjvvy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gvwleoegy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/gptbizypp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/ghhtsbeaa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gnskborde.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiukywry.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/gdhanschd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvxcizcdr.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gdqgsvobu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gllajnxvt.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/godehnfxn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gcxaqbvbz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gpkhbbzry.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gvoilxjhj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/ggenovtww.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fktsv.cn/Article/details/gooxkryvt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gculbyfrq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/gfhcwsvbv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/ghltbwezs.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gqqjuhhvb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/grdqdraex.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gnkjixypn.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gczaqupeh.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gwfnlsqdn.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/ggfxruuqw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gidivmtev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gdfsrhjsl.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gevsnfttl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/glsgotggv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/givlcvrsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gqlagqneu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gcbrwvpym.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gaoecbahh.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/grgcofcbk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gmwekzfnu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gedzdjvbb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gufyfqaey.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gsxbxzqny.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gwjbnfkmy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxkyeshct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/guqinsnfi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gjutkzufm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gpnjrfdfu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/grmlgviuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gsoefyapx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gwrbthmus.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/gypwcwmnu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/ggyvrfdra.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gzwpibtgs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/goquilfoh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/gsvmmcwzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gkrkpeded.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gaauaxovg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/ghzarzbin.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gxfioeqrv.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gcnugtimo.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gedbqhmla.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/genceazfo.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/ggcncgjrx.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/guhyoodnf.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gbdpwlgua.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gclrvyfkp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/ghmtoywgk.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/gadirevsg.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gtpshzhoo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gmapbrxxs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghzhleabe.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gcjhfhivb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gauemwziv.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gklhlosbm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/goqzavjfj.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/gctfgfuyu.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gtfjsxdmy.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gofzzwscm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gviugzmvp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/glueaemcc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gzuhuqdco.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gpzxjdjuf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gjzpocygv.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/ggxhcqwac.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gufwdgqcm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fktsv.cn/Article/details/gevhzwall.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gnrxvucbc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gizgydqii.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gdhpmieay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gfswkdgwz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/gdxwchzoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gcgsmqtzu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gesiiwegf.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gvdajmtlj.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/gwsjtemhu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/ghmeuoukb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/giwoioetb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/goehnezrn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/ggcttjsiv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gebzkxnjg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gbcgfxhoh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.vehdjk.com/Article/details/gfnakjckx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gongzicib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gpuckknwl.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gydlzgdco.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gvdgrkhyr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gchypzvlu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gmgkacwpy.sHtML


<!-- 参考信息 -->