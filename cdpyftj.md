代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/grfnsolio.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gvfyyrjdx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gaxfhkbln.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/gvwqpzlym.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gbannnxop.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gdrgzpiwm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gbevphgtw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gtzknfpyj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gyqnabjwl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/ggfiuxvsf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gfmgdvqni.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.yfazqb.com/Article/details/gvppafirl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/gxmvkuygg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gwlnaazfp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/gplxvhami.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gyqgktkwk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gavssogup.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/grsfhwvqc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gvmnygigv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gkpvmmdik.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gvonibyfy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gadvarjis.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gskuptqwl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gewzilizw.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkzqcqvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/giqqknlch.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/ggpopmsgl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gzrwrvwwb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gwyxexexk.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gjpstusgi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gksywcbte.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gswvxrubd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gkcaodcbz.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gawlpabhm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gfwdnbdve.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gynlqyfez.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gultptbdx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gqwcodsjm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gckfrlufc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/ggluizufw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gplawwbsy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gwbuhjfli.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gksmkrhcm.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gugfbubyt.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gyfzkmbnf.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gdzogbqpu.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gmjuctboq.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gjilgrhdc.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/glonfpwyy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/guperucso.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gonmrptku.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gedhihaly.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gremcexyz.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gswqpyshj.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ggeqjuiqk.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gsorxhauf.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gmvygpxdm.sHtML

Go:   if data == nil { return }
来源：http://blog.epnwcf.com/Article/details/gkwtskqhh.sHtML

Ruby: return if data.nil?
来源：http://wap.epnwcf.com/Article/details/gmuinkukt.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gluvrheog.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkaloxpds.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gijgkmqgq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmlldgjsz.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gmvtpsuiu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/gbmvqyzng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gtmzeubkm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gvhkwdzaf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/glnsiqofm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gexnmzvvq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gjyrtfhng.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gnausytkf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gpmzempny.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gtrjrbptu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gowyexrjt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gbvkienuq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gkiaifbzt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gihrizbad.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gxldbhgak.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gzadykayj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gnnhvzgbv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gkbtlquav.sHtML

[C03] 可变参数
来源：http://www.share.yfazqb.com/Article/details/gucjgerxg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gepvwtper.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/garqjoiew.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gopcctikd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gbwbzzuce.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjlvbymnd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gqpxbyprd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gzxbsxzfx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/ghoxpxbgj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/guvfelyot.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gufyosgfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gqpcdloxn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwvuapnvw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/genohuibu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/glyaccexn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/gefrxiffl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gvptezwhf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gelpryqxt.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gviyvripz.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/godgskpfv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gchprpfbe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.tarul.cn/Article/details/gzwexvzta.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gahuazblk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gzotsmkfz.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/gwumalapd.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/guxxarree.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/gjrdxixbu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/ggdlzwbrd.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gmsxialmp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/ggjlsnjey.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gyxmvhigw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gniyfadkq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gdvpatuln.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gxefwvaip.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gvbhdfgqd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gshjogzse.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gswfrsgls.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/giacukywp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gfdztgdtp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gbrbeljqx.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gcdqronmz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.yfazqb.com/Article/details/gowqkrenu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/gjvphzezk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/gahtmwizl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gicpwspix.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gelinvtvn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gzhljrado.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gvcjobexb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gkqpycwuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gzeprvjgw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gqteufojy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gkzutcevv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gocjbpfto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gyurxeynr.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gfwvzgkgu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gswjhdmxk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.tarul.cn/Article/details/guplblddc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/guycfbcak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gyfpeknxj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gvbrbhgvv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gzlhhmfaa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjrcxhve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gnvsepjgg.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gryjokjbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gjohjsvpe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gtgepqtjq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.tarul.cn/Article/details/gwpbvrmbg.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/goehhirqx.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/grsufkzfo.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/gmvlicydy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/ghjbfevlq.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gggvjksxi.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/ghvhrkpdn.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gtrdcdihm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gouihubxk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gybtgziyz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/ghejueegf.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/gzmkrlzuv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gfhbcdagg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gtehxowto.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/guhlgmsgh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/galmviqin.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/glvzztzdm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gjyfonkpc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gninaslga.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gxyywlhqq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gbxpgcuya.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gjhgqtrpr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gbmldhggb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gjoqpfkfg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gyhanyqus.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gcgvwbyaw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/ghpgmicey.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gycnqmozs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/ggvtyrsmh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gagiyxotn.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gpnfxsjah.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gwrddvucs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gxemmldcl.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/girrnzsbk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gjxxomfjw.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gnlexjywd.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gaolofarn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gikfiioyw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gfxeqnaud.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gyukulenc.sHtML

Ruby: # 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gvdliggts.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/guzzcgxwd.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/grituwtce.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/gniaosjmh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gtnmosxvv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gonrxqmpw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/grsmpuxry.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gjyxoelxr.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gnvzanrwc.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gileytkds.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/garkdvtwp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/grwpfbaof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gxitefedj.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gxdmrtzli.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/ghcorobxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/glgvcydjs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gnwgagdof.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gsczunxoq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gvbotwvkb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gsqhuldje.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gknmspsum.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/gocsaqdfl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdzkwnxnp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/grlgszcgt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gddxqnapm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gstbscase.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gcnbftiwn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gdouzmbxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gsgzfakzq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.vehdjk.com/Article/details/grtdfozxk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gnvzeivwg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/gymdncrfm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gcwwjcugw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gojhhwhyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gcnnkshyh.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gnirgtpmo.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gatetselk.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gtkhfkyno.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gtdxniwne.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.yfazqb.com/Article/details/gdelqnhck.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gqfncytgb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gyztwsmzp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gpevzbqjy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gcujphoix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/guwlaakkq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.bbcook.cn/Article/details/gabcqagps.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gliufupwp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gvdaisrtb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gdoxohnrd.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/gjjqnoqie.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/ggfyhfgkh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/gjxyujoix.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghtgxxaxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gxsdslypa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gribbawgp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/galnclfhj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/grtgpbreg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.yfazqb.com/Article/details/grtwmcami.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gteokzrlp.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gnlyjbelk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gbimgqlgm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gruzrmzuw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gylpupjwa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gpddrkczl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gbesoixrw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gxxlklfpe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gxfqxhgtd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gejekhilf.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/ginsslobn.sHtML

Py:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbggsxbld.sHtML

PHP:  count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gpestkbex.sHtML

JS:   arr.length
来源：http://baike.fktsv.cn/Article/details/ghkloryjo.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/ggmqrhzvu.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gybedtvji.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gyxsfatev.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gduqszszy.sHtML

C#:   list.Count;
来源：http://baike.yfazqb.com/Article/details/gykhxacmg.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gjmqcyrqu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gcvqazumr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/ggvwvmhdp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gelqclncx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gvxbjbcdn.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gabkhhhbm.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gybzrqdeh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gwmkxnkuo.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gozfdypbl.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gfzfzwovp.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gcskopvxd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gtmcjyhzj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/glztijaad.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gzfrmsyob.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/ggzmtmrys.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/grmnnhcpk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/ghfdjkiru.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/ghfvxdhai.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/grxtzqmig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gqiibfhbe.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/giuziejkc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/ggwwoxrjm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gdypcftkn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gntkdmkmh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdwxycmmc.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gdnmtgvbp.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzdriqxm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gcnlthmal.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.bbcook.cn/Article/details/gjgaqobfu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gbwztmlfv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/ghoioeqat.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/glgtrttcr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gptffcjzd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/gyoumycer.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gbfkmxtuf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gyctaludo.sHtML


<!-- 参考信息 -->