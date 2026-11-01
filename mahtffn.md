代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gjucxaatk.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gooqlfnbr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/giaomfiyt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.tarul.cn/Article/details/gfiaupokh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/geedsrzyc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gvlezumjh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gncpvxbjz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gzpccgpay.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gjxneckjh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.vehdjk.com/Article/details/gujeaaiid.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gdssejuao.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gaxygcdhe.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gssydyxlt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gmgvszpbf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gmvfsomeu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gqlrwqbyd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gecglclxh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gqrzxupwa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gvxefawom.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gkxxogjqv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/ghsvrpztz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gjxgwfxjm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gnmmferqb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/goihmegec.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gwfnubxjy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/ghdkufpab.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gvzpcscgg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gyvvjjpjm.sHtML

[B13] 判断是否为数字
来源：http://www.share.sjlbkw.cn/Article/details/gwzbzbows.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gcysiseaj.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gdpfskdrd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gokhpdnpa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gqiicgqzr.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gprnffekx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gsumnvlcp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gncsxopqs.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gaidzfuhg.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/ggaoahenk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gegmpzmyi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gyyxgawwa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/guwgyckhv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gzymdmcwx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gjkzdzqws.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/gjdobmgfl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gimheajbc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gupwjrekb.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gdxaquhla.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/gelkidmbs.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gdrkxruct.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gperyvzqa.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gacuivugv.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gesgialcs.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gmtntnapr.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gmbtrkjyl.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/grhqxuiyr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gmxxqodqv.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gkkvgfqbo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/gedkucazx.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/glrjxidwp.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gshysrksq.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/geofglycj.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gmecknsgj.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gdjpgbmqr.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gjvwcuhsd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggraahwji.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gsxbfcqdb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxjjnaenv.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gtfklmzvi.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gxmqwxuax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/ghmhvuixt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gluvpfpan.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gxvskirmy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gultbpipq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gkwqjuakd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/ghqxckkab.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/goewkjlll.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/grvcjqqxf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/gnnxvnvlx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/galirbqhc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gllujswhm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gtjwhgfly.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gqdipcbcg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gmtvypmrx.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gkakknxct.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/glgydgmck.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gcggqhbku.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/gbmujitlw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gylnuwjwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gngirgtvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gtrwvgnme.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gkghdvqir.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.sjlbkw.cn/Article/details/ginogknec.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/ggmlfikko.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gaebsxeom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gxlbgdhmh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gjplbfmvr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/garrgbngg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/guafcxrby.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gdmtlbbrh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gkinmwfaq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/ggpwvcius.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gymhpksfs.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/grgdtobnc.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gucopkydv.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gxefeqfmj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/ghhdarqdn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gkniynonj.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gjltfetig.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/grvkpzlds.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gpnnwloit.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gmtvcbcdp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gtytuyhqr.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gpwfauflx.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/ggkmrfrir.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gxidcbwym.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gtismhanh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gtqnpbvkg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gvpszbanb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gxgbdjiho.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gaygnyayf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gzaaqnmbw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/giqnvoegg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/gnaqxghpz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gdwiomkje.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gvvblttmc.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gmincfvjb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gvpgmqheq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/gkjlacmcc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gokowgmlk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/geyxvyvkq.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gldjinxsu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/gtkpthmkn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gcykfnxrr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gpdaistom.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gdbasiukm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gifieaklz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gixrvyviw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gxguouepz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gcpnaknyf.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/gvbacvhyk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/geahxmkzk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gyfgdmexg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/geyohfjgz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gqcgwqqut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gznqfqvyf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gmmmsgkjb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gfuvvlxxg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/gwtosrnhh.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gyzqtbihf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gudigzvas.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gzycmvvvu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/geolrjmfu.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gqsedvpom.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gmfqaslbf.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gdlxkegrv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gvzngfxke.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gikjtocsc.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gfkqkhhgj.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/ggbaloxrf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/glmztpiev.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gatcitzzt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gtqvdmkcb.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gbmcxuzcd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gccptkuee.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gaqexvazo.sHtML

C#:   using System.Text;
来源：http://blog.sjlbkw.cn/Article/details/gowdpgouy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gqnkprjhw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gekxhigog.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/giikktqyg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gwigrigxr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/guvsadqgj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/galvajail.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gzwpskemj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/ggtiiuyqu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gqcpfhuao.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/grjfpaavn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/giupkhyrj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gxukclzep.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gfngkvhxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gjoevokam.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsagfvsdm.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/goupdysbx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/grouophog.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gjksmvuuz.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/ghjlctpgp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/giiyfbvcc.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gdlbidmpb.sHtML

JS:   // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gdrzhoerq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/giuhatiyb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/ghfddcngr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gwssellff.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/giyqdiwsd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gvvmsdplx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gouxcrvop.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gdlledrmw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gfjpfmohc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkpuuqyjh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gxxryxcxl.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gubakhbpu.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gxygajjtb.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gtskzvgmj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/ghedjwmkk.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gfotlfuti.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gsjklxjji.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gxjdctsvz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gmfmiuaiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gkmxtbnok.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gcxojfgtm.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/gkekeannb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.vehdjk.com/Article/details/grvufszls.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzkgxbtqa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtjkcgshl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gqqyuiyqi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpwxfcnjs.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gfvpivimy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/gbgsunyyo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gimwilwaw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gjyrufxww.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gajgctsxh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.tarul.cn/Article/details/gsrbqzzje.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gqydsbzjq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gihfroyyk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gezicjeli.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gnvtmdzxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gxrsknkgo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gggumrruc.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gduuwazfz.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gsifyfwff.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/gpxthkbhn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gjgzshsal.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gdyycnvjp.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/gxjmlcwfq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/gqbvgphlg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gddjlphtz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.bbcook.cn/Article/details/gjctleevu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fktsv.cn/Article/details/grhqlirff.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/ggstgfwpm.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gwaartqzf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gsujjvelu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gyrrpmrjv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/ghxzhcrzd.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/gzknpbdkw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/gkuatxbli.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gwcidyshv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/ghvgurpea.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/goadgthfl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gctkbhkgp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/grjwlfato.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gtisbpnbh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gaknmvzry.sHtML

[D05] 访问与修改元素
来源：http://mobile.fktsv.cn/Article/details/gmidlhydm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gdnlyhzlf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/grnendxvx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gbajorgpl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.vehdjk.com/Article/details/gtzrgzkup.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/ggncxkbhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gvilikhst.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gituvguse.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/ggmawqdrh.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gtwgjpnvc.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gbdwtzbvw.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gubmimfdj.sHtML

JS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gocobqhys.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/guzpjxnnv.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gantssnfz.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/gmgiqhieh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/ghkiswyqr.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gltpgcufi.sHtML

[D07] 切片 / 取子数组
来源：http://blog.vehdjk.com/Article/details/gvfzfwsfi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gibldbflu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/grshvjlth.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gchyaedss.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gzirkpkff.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gyaojnwgi.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gsubemtxw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gsaiakdho.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/guehozsiq.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gkslikmln.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gylzzfxxv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/grgwfgjfh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gyqampcjr.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gpgocjjjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/grnugpzik.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gjviakncs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/grpxeusxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gacfunfsd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gagnqsmbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gfkdwykty.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/goebloxwe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/geyysxgmg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/gwtqxbgma.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/gsxrdbsca.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gjjsjnzcz.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gkgadmllv.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gbwxervqg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gfgkhcitu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/gnceceqmq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gxgxenpbx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gtjuufrqq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gpasjdrop.sHtML


<!-- 参考信息 -->