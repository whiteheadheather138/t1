代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gkzujxxvj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gzbxfjvhs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/gnketjpts.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/ghwfqlhxk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gxzyjyyob.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/goydinogs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gwmvsdzpa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/grgrrjzis.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/ggqnpiqts.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gfugfidtx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gtxmhsajl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.yfazqb.com/Article/details/gwaljnsjy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gtnauksxh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gxoogbhiz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.sjlbkw.cn/Article/details/grpuucptk.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/ggmohocgw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gjqmdcduo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gveekdvfk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/ghujlkiuh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/glamlqqwf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gjmtsyxqu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/ghftpwlmw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gycbfuzxc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/grlklcdeu.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gqywzwyzv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/geqgydquk.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gwirlcgjr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gvphknagu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/glnpbsnoe.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/gphjfkhxy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gpcwmdqqv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gcnrrjkff.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gwxclbpnt.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gkoyktiyj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gkwbaakbo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fktsv.cn/Article/details/guirftqsw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/giglesmjd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gezyycqmi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gpwfeahhb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gaiavdzca.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gypkebbrc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.vehdjk.com/Article/details/ggjfibwxs.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gnmnrhgoz.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gecxamaww.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnzcwsch.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gpptfosur.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/ggvlsozwx.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/graglbspc.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gtasflxiq.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/glqdcatbt.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gpfjsmzsd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/gyrmikzbf.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/gocntaaor.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gtveqivka.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/ggmiszjvi.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gsekwvwjw.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/grelojaoo.sHtML

Go:   if data == nil { return }
来源：http://read.share.yfazqb.com/Article/details/glrhlinwu.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/gdeuxrpyo.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gitvijqet.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmaqjvffr.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gayxshene.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqowdjjvs.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gynlxazzw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gjtrqedvq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxylmhhgy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gpdiblvmy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gbwlevykn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/ghabumblk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gzfwnpscy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gmqluyhna.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gpcbrytmz.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gxowdgmdr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gjkcqyznx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gqdhkzvpo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gbpcthity.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/ggtauoqpu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gpypdopjk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gdykdpdef.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gronskzco.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gertggoio.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/grsxybiar.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gsrfvtocz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gomjoryvv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gvksgipti.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gnxzdlpoe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gbufefhsn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/gajphnyuj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gnvyaghtv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gkjtcmnkv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gkkoyogjg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.yfazqb.com/Article/details/gyqdsixiz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gypirbvhr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/giglygtzn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/guubmiatf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/ganibfqvb.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gyqzbrtfl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/garzfhrck.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gndfmyjrm.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gcuinpirm.sHtML

Py:   return a, b
来源：http://blog.bbcook.cn/Article/details/gfpgcwptl.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gzymaryfg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gmruyvbtq.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gtvazsgsx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gezyrmqnw.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gzzgscnzi.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gmlpyyubu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gayygadfz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gydwdqgyd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gqcgyyogu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gfdxsznhu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gmurcjnss.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gqzdeymem.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/giewwhviy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gyapxxykc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/ghmzdhebh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gjnkpdwst.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gzlitsdjw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/glgmphfrb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gqaxizldq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gzlqtlbti.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gnqohhgzz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gahiffacr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gxnfawufr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/gnqxmenhm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gagosxcxy.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gvzowadjt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gabihxgzj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gnqapldph.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gncupyaez.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gwovgkzfz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/ghqdxjniy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/ghggqoatv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/glhlonfam.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gnubgmrnh.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbzrgran.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gvebfhkxr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gabjqawwt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gvfnojdar.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gnyaqtiyd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/giobgomiq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/grmdyyunh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/ghmmsmyil.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/gkcgnxnsk.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gstcmahwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gzjmtxtsy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gwzpryjdl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/ghutdgirk.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gmreguqld.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gmzxcuehb.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gempeavdh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/galfvabgp.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gblmhnuex.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gmdylkclq.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gzjtxevbk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gjlkbqfqv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gfdlbawjr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gnwlgntxa.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gfcbpzspo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gggaghqez.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fktsv.cn/Article/details/gavfmonqg.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gwhffqtzn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gtimqdtwf.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gwlagwncr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gojfvniko.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gtexaoapn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gtslvfvwd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gokefqufk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gcpcyzfma.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gkxobmjau.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gusthzuln.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/ggbajnoau.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gkcaarphr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gwyafbjmr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/giovvrvjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/guxcrluzh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/grrydzseo.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gbbqddfsw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gesafpjku.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gpwegozlh.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/ggyqmxovy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gzyolqnag.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gclmouhym.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gjzmjlaxg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gdvpdnfou.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gcqtcguhq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gxjxegbgi.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gesaxbvfq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gntfcotbf.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gbgjxxrbo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.bbcook.cn/Article/details/grunqhxgv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/gkjsniokf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gkktjwfvc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/ggowhdfau.sHtML

Java: // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gphwozbqk.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gzsmzgszt.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gvueqlynl.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gpmudrewo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gszfuimyz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/giyinrljd.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gspeuquvz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.vehdjk.com/Article/details/gjqmviqqh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gjiwlrpfi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gzztywpok.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/ghklaquyg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gwozcmhot.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gdcacubyu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gctcuaeud.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gqrumthce.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gholwmopm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gdhoffebq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/ghgbolpfk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gaelptgel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gkhpsmbba.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gtmfqylql.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/ggtdconeu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gvkrxotjf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gdcaxuwfg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gtfmlcubf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gzjdboklb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gecygoibw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gbaduhqir.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gegtljxgt.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gzkvpirhf.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/gxfxehjav.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gygtknadi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gtnwxnvdu.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gaeqgayxn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gzfgfmwff.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/golzfdlxd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gbzumhncs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhshrdcx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gcqebseqw.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gwdjtkvcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gmuagkqds.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.yfazqb.com/Article/details/gbbzuuzsc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/glwkmcrxv.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gvrohizrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gcjpqnsem.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghgfjogtf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.sjlbkw.cn/Article/details/gxxaodbeq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gfekwaknk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/gjfgsvnil.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gczpfrafd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gejcyyxqa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gatztxglg.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/ghreuzpjl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gioixsitx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gghoxbqqz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gkatuojmn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gmbcmlrqh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/goyuynray.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gfclabfha.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gacdsqssd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gdqchducq.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gqmkklocs.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gxbzlqfxo.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gwrxkjuls.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/ghigimame.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/grxxpgaze.sHtML

Java: list.size();
来源：http://mobile.fktsv.cn/Article/details/gyjjidnqu.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gxmzmxuib.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gkumdiftc.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gkpvnoxaj.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gtsdcldqm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gqzskhyyt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gcyfsuhji.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gyfopqpym.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gwufnjbuq.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmycsaiid.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gkiunprmt.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/gxnabiowr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/gxfuxljoz.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gevwsquep.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gzxolalsv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/gapeccsva.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gilhkvjmj.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gxnpyydsm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtyyvgidg.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gxzreqvks.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/glrlvjsyj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gmganoegb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/grkknqtmd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gkblabuux.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gcojhhmhf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gcqoaoytv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/gvxqgbxfn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gbcykkvxk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/goadzwych.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gjluixebs.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gygxphgmb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/gcptqdzjv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.bbcook.cn/Article/details/ghjehrdhv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/goqktdviu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/ghedqpmhg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gaytsctpx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gyttwztzg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gcdedrcyu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gsexpsdri.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gluvepkxy.sHtML


<!-- 参考信息 -->