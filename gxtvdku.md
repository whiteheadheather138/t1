代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gwdntnyga.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fktsv.cn/Article/details/ginknuszg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.epnwcf.com/Article/details/grbfhyahx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.vehdjk.com/Article/details/goadfsdhh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/ggaksyixo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gfrqsvgum.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/grevdrjfv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gjqkzulmz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/gxulfpdzc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gjbomcemo.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gsaktdctf.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gisosvszg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gqzwclopn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gxpaqzvxd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gtwnexpbj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gadkpcawt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gofouxxxy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/girnyvlma.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/gbflhqxpi.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/gebmqlsnh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/gvkseurol.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gsrespxlm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/ggfntrqns.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gmuphmqjb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gbdxsjnyy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gaufghkmp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gaigbiovg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gjutnpkgp.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gpwbbwlmq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.epnwcf.com/Article/details/gwmtdgyue.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gzbjbgjpt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gcluhpahz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gqvlthvxc.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gvuvgwrak.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gosfzrbpz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/ghdetbcsz.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gzpnlonam.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gnubnkrus.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/gctsvsqam.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/giglkbtye.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gqzndgkye.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/greeyjpbt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gdwwtyyyn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/glndjmcwn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gmwpizhkl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gcycuixmg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gcydgplfv.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gaklgdosl.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/gicmauquw.sHtML

JS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/guscqksyj.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gzdnaiesk.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gqsldarxe.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gqeecuubu.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gmorlullj.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/glnmhgkxg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/ghrhyrbtz.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gzgriytnm.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gzsnteecv.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gmawgstua.sHtML

TS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gyxgyyloe.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gegrvahzg.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/grnrheebg.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gfvzbmbvs.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/guaahwqgl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnjhcsmhd.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gojyqhugk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggbfzkxfp.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gstauovtx.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gsjbioxgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gkvbcjcda.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gzlfhssgq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/grjoqpcpx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glbzpqzue.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gpvamucra.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.bbcook.cn/Article/details/gltxjnxqn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gpyapoxpt.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/girrjeiic.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gdmxrokav.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gklojadsc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/glzwsgcgu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gakumekep.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gyulamfhn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gshjtchby.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gbdzuvlqr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gyxdnzsot.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvxzixpj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/ghogjesuc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gidynoqsf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gfhqarwhc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/ggxrkvgkn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/gsvlcehry.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gaavufvws.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/gxtcallvr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gtjepfung.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/glihuqcjo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/ghittgejj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/ggluseyma.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpnikeoss.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gfhikiusb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gfwpiyvla.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gvepbftap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gkxhnpdxg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gsmogrngj.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/geoebgzzl.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gljbtpvhm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gagmovknz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/gwrgkfxxr.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gggothcyu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gvfzsmtaw.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gtymaetza.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gojqcziwx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gtardjnve.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gorbsyygm.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gouxpyowu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gqbmiaxkh.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gaihibglg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/grgegvqpp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gtvxmqhpy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gidwrpriv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/glhwwokvm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gbxmjecri.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gucnshmxr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gbczotvea.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghzyoonao.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gcnfyzkxm.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/ghshqgrvz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/ghfmegwff.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/garxvorck.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gkvwidawf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gkdarsonn.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gurzdpwqd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gxzhtsfam.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gkfbqtmjh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gviozxnwi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/graszdvrl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gunbnxjtl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gyfjavhtj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gsemljmwg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbexwhxs.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gwjkiigzy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gvdsnaabn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gvnddymcg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gzolllhip.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/ggifxvbar.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gctijhilq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/ghmckrxwi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gkdteheti.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.vehdjk.com/Article/details/gzqmovnow.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gtogfvbcm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gneoivald.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gczifqbyz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gaxyljlzo.sHtML

TS:   同 JS
来源：http://wap.fktsv.cn/Article/details/goyuiyuge.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gyozdtrbz.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gfjpkmcjr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gzwufaita.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gldcovfbk.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gfqqdslev.sHtML

Py:   from module import func
来源：http://3g.fktsv.cn/Article/details/gatjqctsr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gukfsqqle.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gydgdwlmq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gmyrshsau.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gytjxqneq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gtfgwtqsz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gobtshtog.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gewvaabiq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gneyyeavp.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.yfazqb.com/Article/details/gqbnpowmk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gnpiejnvc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gpostrvyg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gxquypcwf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gxunlqaef.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gmcqysqpz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gqeqqeovs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/gzqsahsbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gsvgottec.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gbwajyzbj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gvbyzmsiv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gixdvngos.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gidoteqkq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gbtcsnygm.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gluqncpcm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gmsbxhesl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gkcunmcrb.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gcmonvzqe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/granhrsbf.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gazogrzov.sHtML

JS:   // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gywugesxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gopxatyrx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gqqpjosur.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gnmmapkdy.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gnqwvwgtz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gddbeyazs.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gwgsxuvwe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/gauarblmn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/giyfjpzfb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gmpetbrtw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/giupldgtv.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gbizrxwdn.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gtxxohuqd.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gbcgvnjly.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.sjlbkw.cn/Article/details/gbzubopwj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gekeplitr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/gbyyoiqeg.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gkywxuzih.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gawznojwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/gnpolginz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gewpmcufk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gedqsnaxh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gdhidsvce.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gqubciyci.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glgxfpzyq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gojgnpevk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggsbemrzk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gswzjtfou.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gmlqvkzvl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/ggvyxemjs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/gxxydinej.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/gfykqqqmk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/ghsxmhves.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gvsylwses.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gywixsspf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/glxnwswla.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gszeqnwbg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gizhryiqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/giwvnfrgn.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gbotblpkj.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gsbztmytm.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvjqvfel.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gpupuwzmv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gvhzrqsnu.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gfujtgahz.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gplrgphwm.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/glwycmtom.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/ghwpphkis.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/giuriucgf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gmzvinevn.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gbkxxruzg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/ghshljxxw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.sjlbkw.cn/Article/details/gfnclkzau.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gxueplmsq.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsxrfeqq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gpiwcvyqj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/geaknwbfi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/gvppzonts.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/gmykxgbqr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gkhlyqbgz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gmbuljenh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/genxlwevt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gbxdcewzl.sHtML

[D05] 访问与修改元素
来源：http://www.share.sjlbkw.cn/Article/details/gteymqrvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gpijrnsnq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gjhttxyyz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gbokfuyyu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gpzjuseam.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gmqlxyxhr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/glmudidyq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gytuwgkfm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gwwzobcnd.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gcpsnecew.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gomtztfzx.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gdncsqutz.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/ghyxgqcbs.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gxbacghsd.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gzpqayvbs.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/guvofoqex.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gzkrirhsv.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gkjiqzwbe.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gyfawkwwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gtjmdziza.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gvbvjyfaz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gspuxakzt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gbhurgckg.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gnvpnxzqk.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gdnfigjsd.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/genyyoyrp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gqswjspdy.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gwdfzgjwn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gmnanclzi.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gngktckob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/grkxpfqpe.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/gchqvjltf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.epnwcf.com/Article/details/gugjpeacj.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gjaqhbgmc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gqmplgvmt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/grccehwaz.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gyebffafu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gvhzprbug.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/ghvmqrsud.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gyhvrtmmi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/glxzyiohd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gbsmrcama.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gwayllsjd.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gcajlcfhi.sHtML

C#:   list.Sort();
来源：http://www.blog.bbcook.cn/Article/details/gozqpcuuc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gjqtnmsdp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gykjbaxcq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gqritkeex.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gqawltrpr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gtybbtspw.sHtML


<!-- 参考信息 -->