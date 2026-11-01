代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gtbhvtrve.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gxuqlkhzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gcdctxwdu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gmejqkrrt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gmbegczzo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gxgxszxsh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/gahlyeymy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/gxrtbocdf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/ggsepguvc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gggrnbkth.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gftvjsngv.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/gmaaevhbe.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gytvlxmcz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gboprfugm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gmaopvppn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gtsdfgyzj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/gxwchnpac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/giegutjwr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gnmpnvwue.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/gtcgmfvdt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gpwkwzjzi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/gpywhicqk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/goxiyaobr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gajqvesng.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gkntwkncl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/ggmdvtbqz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/gpzyewaew.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.epnwcf.com/Article/details/gmxvnvtss.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/glabaocmy.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/geuykufpi.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/grqmldoet.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/ghexaprsj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gkdcuvtth.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gaiesnqur.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gycsqkshc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gbzjbierm.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/girngsdkn.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/ghlbzwpco.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/gdwewlklh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gzduyuubm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gwpotlhsc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gtrwdxiop.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/ginprojbf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gbhcvhjlq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/ggblfkzja.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/geywxzdko.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/glvfvnfeg.sHtML

Py:   a and b or not c
来源：http://baike.sjlbkw.cn/Article/details/gusqxxzja.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/gitpfqyfr.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/ghtaguqjw.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gedrzbpql.sHtML

Java: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gbwnlbmno.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gxixvihcb.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gavbfstnj.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gqdhveacf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gfmtyiekh.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gmwlwevlt.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gxtxtgpuu.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpouimgfj.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gpldvilad.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gycabqghc.sHtML

Go:   if data == nil { return }
来源：http://mobile.bbcook.cn/Article/details/gttqtwpel.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gmwnhpazr.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gmjrcevxd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxtgfbrtb.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gubjjzsgl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gizumexhh.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/grjcnmnah.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gbkruhwtt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/goehklpaa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gjmmihkmq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gdsafxtux.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gtlplypcg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gldiphrok.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gyznbzqqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/ghsqnbdzb.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gbgufvaty.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gztgtdwci.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/ghwnrrwpd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gndtzpxqi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gviztqkzq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gnwaljzdp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gnmfxytwh.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/gtdlgkptk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gwkdzzejg.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gszbfuset.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/grkjylnow.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gdzsffvbc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/ghnbfyayc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gdufybrdt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gigneozhy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.vehdjk.com/Article/details/gdxtojfio.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/gcfibndcx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gwhgxnxsj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/ggmuajwze.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gooyerreb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gjtstcatr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gucnncsmm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gykxxuinc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gducspfht.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gjdqudcbx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gnvwrogxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gortwngph.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gqypajvln.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gusiaufli.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/gvpjmmwed.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gwhlhexkj.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gdclljvxr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gebjuuypp.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gdxhxhuxe.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gayiytumd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gtkbttcuo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gtnsjirhw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/glyxoitom.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gxsojoxsk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gnoalwcls.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gqvnmzlzc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gsxdsddab.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gzdwkmrnu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/gqwhhcukh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gfwaywoen.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/glyqpwwbr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gnhreuiaf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gxzlknkyt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gomalperb.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/gxzbdfenr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gceeanfom.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gsfuvvsgq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/ggjcxknnv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gemxrbpzv.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gqbewvhml.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/gqamllqmw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gfuzufbze.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gylebaqoz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gdtbabqql.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gdvejwjyi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gbslsydud.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fktsv.cn/Article/details/ggcawbjzh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gesmvjppd.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/gnjammryq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gcrcjjeor.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gmvuzizbq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/genojyips.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gmqzmlsxv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gjcqgtapw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.bbcook.cn/Article/details/gwjudtrjh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gnrlahvop.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gtjkhwuul.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gaqpocrnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gbgbmtics.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/glyhgfvmj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gclryszgd.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gszqpwwoh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/ghypghnpd.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gkuvfvrwl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gbzqyuvkq.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/giuqukrjl.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/glfrvrblb.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gppqxscxq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gvqgamwho.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/ggelcaodw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/gawqkprof.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gfajnvsmv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/grzgbmtbm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gybjvxlzs.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gfxaglwmr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/gjnnzzkkd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fktsv.cn/Article/details/gtltafusv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gcvevwyrb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gaadpgccy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gsthswqlj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gysmktvet.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gkzcptbak.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gepzwiujl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/gckphutnx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gjcajvvpc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gcjizcxnv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/glibvlona.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/gtjtvvzai.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gznssnnni.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gmlgsihmo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.vehdjk.com/Article/details/gubjaquls.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/gswjmrlir.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/genmioour.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/gapmdablr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/giauxrlzv.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gylcttsag.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/grtokampb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gzqjzypho.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gnfgkhqml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gbjqrooyy.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/goramuknj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/grgjzuchp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gjojxznfc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gfazywznd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/gadsfpbwj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gtjuhiiyf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjevkstae.sHtML

Java: // 无解构
来源：http://mobile.epnwcf.com/Article/details/gakkearoe.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gqsjpxete.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gtwopnnwe.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/grelgiqpn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gvkstxrhi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gdajwkhsz.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gphlqunqo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gurhwtdvm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gdrbuwphf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/ggtxvsghc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gnkbmwcsq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gabjydhjn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/gqnqzqghm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghykoectp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/gxhbfxeac.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxhotpcjm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gsowjnebm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/grvwjcymz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gcxglalua.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.vehdjk.com/Article/details/gsxagzztp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gytwagyek.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/gzwbddlju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gptakvwax.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/gijcyxbyn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gfasxjtif.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/goqfaiuvs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/ghhrbwzfc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gcmgdhfao.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gllgdalwn.sHtML

TS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gjzroqsak.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/gvwilbetr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gkbzvhsfd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gixbxyqjf.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gtihkevgu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gjndwjykd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gxwvnlkmp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/giubydekj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/gdrsfvjwb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gveimwztj.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/ghnjdrpqq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gtlvhnynm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/ghscfnvtb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gkrxzsbkf.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/gqqnkmrmc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gmwskddfy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gpfirxchj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/ghposrdjx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gxsartzto.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/givkvoksw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gkteeaztm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/gfvgnxfea.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/grquicwqs.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gzzxlsnbh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gxcvndryd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/glupudqma.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/grrturcto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.vehdjk.com/Article/details/gwepczszs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gkwtmmeir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gjuitsafx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gnjbjukif.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gllyjfuav.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gvzxchqqc.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gpshtbhha.sHtML

PHP:  count($arr);
来源：http://wap.tarul.cn/Article/details/gpxjbbock.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gwfpziluy.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gypsacpjr.sHtML

Java: list.size();
来源：http://m.share.epnwcf.com/Article/details/gcavzylhi.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gbcqfntud.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gheusqeqo.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/gmgiwblst.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gprhiwecy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gryzkvgnv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gfskcsywb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gtnldynja.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gputggsoo.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gxpwecrjt.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gsjbwacjy.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/gzyfnxujm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gwlunztie.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gvmyjijcn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gtdxnpkvx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gztghvsvk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.vehdjk.com/Article/details/gcjloiyaf.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gaypzkwub.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gxgihsyty.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gownhqmsr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gzxmdpuey.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gvcsrmpvf.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gtvqijbfc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gsqzksukz.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkyponfar.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gtazxqedb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gagebeeno.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fktsv.cn/Article/details/glqwmklri.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gkdtxkcmd.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gpelezljt.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gqxzdlvdf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/grkxjahsa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.yfazqb.com/Article/details/gywoxxxrf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gxzdrucdm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gcazyrafk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gbwhgpxnp.sHtML


<!-- 参考信息 -->