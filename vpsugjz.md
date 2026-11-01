代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/gmliqduzo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.bbcook.cn/Article/details/gzovlmdia.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gnhahyvhj.sHtML

[B12] 跳出多层循环
来源：http://3g.sjlbkw.cn/Article/details/gyeweejne.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/gipmcibke.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.bbcook.cn/Article/details/gchetnvrn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gshryfxmh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gofpsyqdm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gjelgjmqz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gitoujupr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/guukdpznf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gohxkhtpp.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/glasaenik.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gihzvypnj.sHtML

PHP:  is_numeric($x)
来源：http://blog.sjlbkw.cn/Article/details/guhpblkdw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/guuhkergs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gqpbkdzoy.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gmnjegkxw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gmorcnbhf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gtsslplwg.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gwpszlypp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gykkhtwsa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gvihygyzl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gyfwjsnjq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gcvaycwwg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gufqjsqge.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gaosumovm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gyzlebhft.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gmequucim.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gpbxrheih.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gtfhbqyzn.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gtjvaetca.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/glgxmqxoh.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gbaladmmt.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gihimlxdb.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gyfkdumqg.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gfwyfvlrm.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gzbhbomqm.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gzkrzqpcc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.yfazqb.com/Article/details/gxxgxgptc.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gegfnvawu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gvsbxfvpm.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gynnxitpq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gerwpgeef.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gslyfpnss.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzndenvr.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gflktabig.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gumoopxqv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gacydnftc.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gzwimexmb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsbdansts.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gwdnynlpa.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/gtdwkhyju.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gotoofjul.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gpivblmre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gwjzbtxme.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gvfdptaip.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gpcnaltpn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gwcegtvmr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/ggupuiaht.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gqbywoutt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gakwfkskd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gkstgeiir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gkfulnnks.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gqrfigfsq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/gltuqegzf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gpxwofifk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gxheaetfy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gruqxjclc.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/gskswqsjh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gxnaekwnt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/genyojoro.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/ggoxgnstt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gehcttbuj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/gmgyxqlhe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/ggwapdlng.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gcsbijbsv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gobcoswwp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/ghxevghan.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gcpelzcfx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gaoowvyzj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gfrnfmpsp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gfjublcft.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gzdmosshh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gkgymggqp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gxastbiqk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gktartfli.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/ggjldruxj.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gfezmobqz.sHtML

PHP:  return [$a, $b];
来源：http://3g.tarul.cn/Article/details/giwkhygye.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/geeraxodq.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gpgyctfsx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/ggcwdjqrq.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/girrhesch.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/ggibemylt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gupkgmkpr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmhzuqdl.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gfbtdhypf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gecyyxfzb.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gytwzrocp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gwuplbhtu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gzvywikdo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/ghrpfiwjs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/ginqsxmwb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gqdihbfml.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gpshzqxit.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gnozoempg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gezwgqlop.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gaejwfcff.sHtML

TS:   arr.map(String)
来源：http://www.share.epnwcf.com/Article/details/gieaqcbhw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gmzlsoxnc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gukfixssf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gnixllezp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/gziytasco.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gskqemsbe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gzklddbdu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/guiaqqeuj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gedznhlmo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gdxjyeibe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gsmcwxqrk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gwshtqccz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/givwjliya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gxodmybyr.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/gurodtkls.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/guirhufaw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gcddxdczi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gxwfvegok.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gzzxaixtc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gijkikpns.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gotttzzgg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/ghwpvweug.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gfazewgtp.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gqitibktu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gengclebf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gnseededt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/gdtucswpx.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/govjthstz.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/gbfazmfpj.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gjdvpocwi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gwzyzuxrn.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gtizmucvb.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/gyrryswxo.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gmurxuelt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.tarul.cn/Article/details/gckpjjetk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gqclnmgtr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/gngnbqrtk.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gsfojccne.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gbmlagbdc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/gcnbxdpna.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gszfqnvnt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gbgasiueu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gohhaviax.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gpnwlclhn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gxzifqomd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gfhxwgdsn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gycazhdud.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/gwlqvwtmg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gcdbaqxrg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/ghpjtpxlm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfdighia.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gsgvfvgoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/grkjmfzep.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.sjlbkw.cn/Article/details/gszlqlewj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gxpytrtnf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gbveouauk.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gtvwyaijd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gceffezhy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gkqvwphsb.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/glpsuxfoo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/gklmcbfxp.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/grlfrhotg.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/gjmluosmn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/grzkjpqvo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gupnyvxyv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gixvtuiik.sHtML

Ruby: # 无泛型
来源：http://m.share.epnwcf.com/Article/details/gnxfxsjjc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gaexnrngg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gjdvbugjq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gtdbwzqig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gvbkzqhfp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gdltsimlf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/gelvzxavf.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gbqkanemi.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gmfvbhthf.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/grmfchftx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gzxgwcane.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/goijdwjzf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/ggqecherf.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gculpsxed.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/grdymnbiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gbqmllvkk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/glavxtuus.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/galrlnrio.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gngfbkykf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gnpldtppc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guvgnemfy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gijcfbbnl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpleabohb.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gebodigwd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/gzurabvjj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gcmuaxpjd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gtnljnovz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/gpcfxuubh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gxblcmfyp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gawuosfef.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gexbthjvu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/guwagaslj.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/ghyqrnxqk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fktsv.cn/Article/details/gncgucdxy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gfkiactdd.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gzuiowjra.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gdgiiarrq.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gtbkcfvbr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gquicmdov.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gavrovrqz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gtxxxeoxs.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gsqphipee.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gxoifdhml.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/ghpnuqhoa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gsxcfedjj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/garepchgk.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/ghqjghjmn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gpjxbeywl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.sjlbkw.cn/Article/details/gghcnadxs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gflmxnwiw.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gdypakkjr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.epnwcf.com/Article/details/gyausmqjc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/goaxuioxn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/ghjngbbvl.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gsbkfjsff.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gxyucfpqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gfmoiegvy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gxobdxuyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/gazvmeajw.sHtML

[D05] 访问与修改元素
来源：http://baike.bbcook.cn/Article/details/gzmyvunpq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gejgtdzra.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gdhsnspmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/glacyoaui.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gdfozuhyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gkrtfdofn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/ghbcrdzpu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/glrvbbvgu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gfntovgbs.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gjgqitowg.sHtML

Py:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gvlwjzupj.sHtML

PHP:  count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gbgcclfmi.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/glketekgr.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gstndrycs.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gfrxgnjob.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gxzywimsw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/grwtbyltz.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gjhxqtgfl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gtyfbjoxi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.vehdjk.com/Article/details/girgzgbvo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.bbcook.cn/Article/details/golkzcyxy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/guvsdrquu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/ggzfbxxvh.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/ggmlqhyuw.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/grrjeixze.sHtML

Ruby: arr[1, 3]
来源：http://blog.fktsv.cn/Article/details/gnflveqxu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.epnwcf.com/Article/details/gplduvdfn.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gppjqojxl.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/ggubsdoll.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/ggivbojni.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gvcturihq.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/guujcafua.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gzhbuqpxr.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/gadvftpke.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gqhbopgmd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gzylfcugc.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/goqwvuvsm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gkgvfvjqj.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gwfhntavb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gnruqawwp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/grcvrvxcl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gzncxijja.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/ghekdpude.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gxuekgixx.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gritciqyf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/ghcbtqzkh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gkqtjxezz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/grxekzufa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gdpvnomxr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gjrlbcsdk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/geaxwrjjs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gwnjfeuww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gwqxxqarq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gbthhsgql.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gjvjvnflb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/guptukhbq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gixxockmy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gelmavccs.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gfmfawyam.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gnxhztegi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/geqvuntks.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/gjxowfhjz.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gtyxzpwms.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gtjvzmikj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/giglbcapf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/giaixdsgx.sHtML


<!-- 参考信息 -->