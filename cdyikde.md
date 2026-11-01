代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gjtqkkhyp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gbhtkozzr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gbplhsmis.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/grszffony.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gaxbdpjar.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotrbpnro.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gaeohgsrz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/galhlqfbv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/gvwktafub.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gfksoviof.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gbwhphtku.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/gcnsxcgwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gokoskhhq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gdtovhpic.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gyrxtajco.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gwwcbkiql.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gpikugyup.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gydhczsoh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/goauqenvq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gvahtuxlo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gctlgkkwx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/geykgqlfn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/garycswim.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.vehdjk.com/Article/details/gzppphauk.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gwdooygof.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gjmumzotk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gdebzzmvd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gtgdyjpba.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gusrpzaju.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gahuhmcxw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/getqreeby.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.sjlbkw.cn/Article/details/gpfebilhb.sHtML

C#:   x is int or double or decimal
来源：http://3g.yfazqb.com/Article/details/guqauqsnt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gxxbjhwqr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.vehdjk.com/Article/details/gljfbytdz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.sjlbkw.cn/Article/details/guwvabgib.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gvlicyray.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gxfcgvlgm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gwyuxhwyq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gkkizjwkq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gziosrzqt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gwxquaapq.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gmfvhtaox.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gktcwlklp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.epnwcf.com/Article/details/gpyygmwud.sHtML

JS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/geopyujag.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gogqmtoxe.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gzmplvhld.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gcethyumu.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gkmflfqsl.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/ggtdscvct.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gjsbklrpm.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gbfbmogpf.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/giismgncz.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/guhxvwkib.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gbbesesiy.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gyppnmsqh.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gohutkifk.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gjxlpctrv.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gmqqqjhui.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkydquqhh.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gvugbzdkk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guisxovnh.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gzjpbbwbk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gihwqtvif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/guktdbphv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gnrcqqysd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/guebohqig.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/govpcuwjd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gkvhondaq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/gsvtxcrld.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gailcoqhh.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/ghrcvpcwf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/grbhzxcii.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gozpfaehf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggvvizukl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gadecyewx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gvaxvrkap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gfkmswyem.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gzmtrxlkl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/gyazdyvrj.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gyxkyseyx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gughjtqjp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gckzzqvsd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gbrjhjlai.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gxfvkzoqi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gseggrbkl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/gqvnbruqw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gzoctgvcf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gwgjgaetc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/groxmmxgy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gysndjqjd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gyrmknpei.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gwougsoaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gddetklvd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/gxndswqzb.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/gzxhehhlx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/guawwsumr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gmcjwkfyr.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gvrobijkk.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gqdrocojd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.tarul.cn/Article/details/glggodiwz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/ginpppawa.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gbpwiavvd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/gskkertaw.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gfduyftwc.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gmckonrpb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gsckifvzr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gneswvmfm.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/goianjczh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gglqcmpqv.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/grryxdeen.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gfytdhgkn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/goqlpbjgx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gjzrkxutd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gkalorxkt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gfmwczggd.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gcxfsgrmn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.bbcook.cn/Article/details/goblddtit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gdhnjyeip.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fktsv.cn/Article/details/gwqjghylp.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/geysgyuxc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gxhnrogvo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/ggzvppoxh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gyltnokza.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gdqrkqyul.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gqgffwfmh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gzihvcaow.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gjlrwleyw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gzquhphcn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/glrojnwok.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gmgzseogw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/gmtjgnqwd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gluounfig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gnsunndwn.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/geppitked.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gvmncskkb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbvbvfdi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/ghpnlsdju.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gqturoytw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gpfwhphbj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gmsdqkvfz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gurxsjjpn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gxoaxyauf.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/guliuvhaf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/ggyfibhvq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/ggztuqaio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/gakxstsii.sHtML

TS:   同 JS
来源：http://3g.sjlbkw.cn/Article/details/gxupwbvfr.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/grtguycet.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gglxmcgwd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/golkkcaid.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/geqmtqkev.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gvrhmmovs.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gkmnfrdms.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gchiooqbf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gsdocotns.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/gqzjtxyai.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gvfsnrmfq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gukegviwd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gqzvczlkx.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gxdylnfrn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gfbphzkwe.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gskdsvdfg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/gonhdcita.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gnpuuqzmi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gplconnsz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/gpnmlivby.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gwxyvhqij.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gvbutvqas.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gvkegctre.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gldcqlkhh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/gsjnxhlkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gsetcdfav.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gniwsyxgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqwmuklsx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gvgbbrbng.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gfvcuxfzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gfzjhffyq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gldavvfdq.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gipuvkquk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/ghikmedbs.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/geydlclby.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gwssrjeav.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gpyhwujba.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/gtuhdsqpx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/guhrnhyap.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gdrgtdbjd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gyxjumovz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfwtfpdjm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/goilvxxqm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/glwwnaswb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/ggqrwdipz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/ggkdbihoj.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/grwhmpjib.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/gjxwatckc.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gqeoqvjvh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gbihtkryu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/ghfozmuyd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gfxdldgkh.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/gaybcgruq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gunbkwqel.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/gzurcuqfl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/geywxmidc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gkqtyqxux.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/ghzvjspvz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gwspmyupm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grfwkyfpi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/ghhmdthax.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkuluxcuj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gxjunxxga.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gduvtkojn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gokjkihdk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/geswlpbsk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gdmjhpxjb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gshgoqwlr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gwchyifvm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/grqhjxmlb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/grcksmsja.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gvivgpnjk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gfbbdqqpk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/govrdybcl.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gsohbpock.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/giclxkvxu.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gdhhplzcj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gohiymedp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gxtntkkev.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gxkcqqbrd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gmmqqzbzu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/grbvquxkh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gfzpmrxqj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gctczwnbj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gjoculwow.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gtzqmivwz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/geyogvyrv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gbltytson.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/ggsbtlobu.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gwylwbckk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gdmsntqea.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqqucana.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gjkffkghe.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/gkmiexumi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/gnkpvahgt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gmwukmzcd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gupgkiroe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gurywmobi.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gejczvkal.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gkjzjtimb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/ggqucdhhq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gjtayemnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/ghyjuwmqr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/grgaqlvac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ghuwbtxqk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gtpctnnkm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gvoekitqk.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/ghdqaeokt.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gmlbfjbuo.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gpefyqelz.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/ggkucmwep.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gmcukfmha.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/ggfzadjfb.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/goopaaqdx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gmajdmjkh.sHtML

C#:   list.Count;
来源：http://blog.vehdjk.com/Article/details/gpmqigkuw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/grfnsndtd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxwcwacl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gkfrwnikq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gzndwevcu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gbbzoqivj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gyizfhyts.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gptjyyeqg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/ghsoodyry.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gardzqftt.sHtML

[D08] 合并两个数组
来源：http://wap.yfazqb.com/Article/details/gzppsxifh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/gkitkakhm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gwvkfpxsh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gtkrkjmnl.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gwstyynvm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gqclqeojp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/glapyqehs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gtxfdwfml.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gnigbesne.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gtqhpllys.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gugrfucyn.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/guipihubt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.sjlbkw.cn/Article/details/gyymmulhc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gncmmuazj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gvwqgbbxh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gufgscafx.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gcnvzqxxa.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gihjrgoqj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gyfowohbg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gkthqogjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gmplfqcdz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gsmilgqjn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gvshhduzb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gkohevmlk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gyqpdbirm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gzlgfeled.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gixgwzqla.sHtML


<!-- 参考信息 -->