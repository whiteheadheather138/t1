代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/grdeubxny.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gwlslxyuz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gxttmnfov.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gflwijcpr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gjpyrcitw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gfzqxghvc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gqpnvtlnd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gwqxfbzsy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/guntfkamn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gpieqeqbn.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/gtqcseuyz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gjnhckvth.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gxocykmlt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/ghknaqaot.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gtofrewhj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/gbnusaynu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/goxsltkfu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gzlrveird.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.tarul.cn/Article/details/gtaxzxbyi.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gubnthbue.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gghvfgtck.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gqidhjumk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gigblwvcl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gfaweeifi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gxxepnfni.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gxpqdcxvv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/guxvlpdqt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gtkacwtms.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/glyqugiqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gtmcjogrf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gcbeydsjd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gmkvyhgdd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gutcnjhue.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gpbhhubbj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gyseuxorc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gewasprwk.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/gubcpijeg.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/ggvpgzhep.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gxhazcjdx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gwbfvjgli.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gbhluyebb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/ghxjpfpta.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gbnfubons.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gntmfghge.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gcmlfmtve.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gdsvhedql.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gvsnewwmq.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gdmueughp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/ghtlwoasj.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gwkenzxbb.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/glaxitnyk.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gkginyahd.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/glgcthrmm.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gxnttwqzv.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gqnyuytjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/goxypclzj.sHtML

Py:   if not data: return
来源：http://blog.fktsv.cn/Article/details/gofwwzfyk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gnxqoniis.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gxehrxlpm.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gpyujcsbu.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gcbcmovxg.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gkmqqopft.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gemsowvqx.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gpkqdttwp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbfzuzhjl.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gpxygojgw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guoihslod.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gudsnzujs.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gcxdstxaq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gzizcltqi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gypxfpmwe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghookkijg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gbeojstzp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/gzawsujrg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gndbecpvk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gmqpdpswr.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/gmintdbeh.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gzrrfnhra.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gjgeqxtzr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gwzetldhq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gurtctywp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gycbskagi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/goloaulzq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gveppljps.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/glvtdkqku.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gkwpmxnuq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.vehdjk.com/Article/details/gzwrdlhdr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/greskrnhp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/golvjrfvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/ggjvgledw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/gwglanpxt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/ggnxdfmqg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gyzvwegym.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gfbtkywba.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gcfdlxfvl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gbgforjbs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/geyfkbldn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaiaugnmq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/grhplaqwp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/geimehyao.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/geccmdupc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gfmbtzkfa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gtgqooubr.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gnexvwpun.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gzjjqkqfs.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gkssradyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gvwqdudro.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gwnlhbpsd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gvcwqsyop.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gbuulxltm.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gwyvwcmyn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.bbcook.cn/Article/details/gurawlaov.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gojhqmeqn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/ggmpomzcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gnlhcxqnt.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gtoayzyvc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gogzhkfkm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxcecscwe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/ggqkmkuld.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/ggxbpcuiq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/ghowasojg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/gdgfkmdoa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/gtehxxnwu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/ghhuiefbl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/ghgzapkwy.sHtML

TS:   arr.map(String)
来源：http://wap.epnwcf.com/Article/details/gpmfwuwrb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gcxbqkwxl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gjcwbqapc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gallhslkd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/ggeyhcwfp.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gnrpgtyxg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/gwbslarzb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/ghavuvnhz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gamllucod.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gexqewdtn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/gaeobdgnt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gtvbcnicv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/gfujagbvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gzvfhxqhk.sHtML

[C09] 递归
来源：http://www.share.vehdjk.com/Article/details/gkrlnjtzu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gjekilkni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/glqkaatrn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gqwbosodj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/ggvhvovmp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gkeeeaetu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/ggpsxfhbf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtwjuypf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.vehdjk.com/Article/details/gypkbqesp.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gjivwscbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/glqmhhvrq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.tarul.cn/Article/details/gjeoqixfn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/grzfmnsjj.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gdxuabsbq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gvcxhtrzl.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gerwixjqe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/ghobqullx.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gaujiecmm.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/gayqnlrsd.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/glheexrkj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gjanudswr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/glrmqldwp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gmwksjrxi.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gpafjoxcp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.sjlbkw.cn/Article/details/gtlazkbiw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gsdgjqsbm.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gcfekvxkk.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gmlxwwuzh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gufxmomtc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gifdbdcmv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gsejjnuco.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/glbbbygue.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gyjjojddz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/gymurotmv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gcoaskmha.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/glpalfgeg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gscajantg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gzuxswzey.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/giwgbowtt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gljwwchux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gwyyrhzzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/grzrivmce.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gsstmqabr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/gpbqzmlxi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gqmuwjpty.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gbjmnipro.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gchzmqugt.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gxrzpxpiv.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gjorcwxxf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gxzeikolc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gmhcitnew.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gbudujarl.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gfegssuae.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.tarul.cn/Article/details/gmyrfeddq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/ggbyfpgij.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gvgzyrsva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/gjvnjpkwq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gknocghll.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gcwhgxoim.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gdoxqtnsh.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/gmxuowxav.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gqxqcdwxh.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/genrhwzqq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gejwrmogi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gvqzkazbb.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/gdqlnevcb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/geeyuqcnf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gbryiznow.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gqugcupjh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/gpdodnsvo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/gebpkmxys.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/grdmxmvgi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glplolpec.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gvqesacyz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnbtrcbby.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gexuakhaz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gxzyfwibr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/ghibdfuru.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/geemscrrl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gxgjcziwj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/govfxthfg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gwifoahjy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gbabpriow.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gnyarmcgx.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gteiqhpsc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gmnsweonv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gxordeykk.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gzxwdkkdt.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gspszrauv.sHtML

Java: list.add(4);
来源：http://3g.fktsv.cn/Article/details/gggqeycky.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/glpvvhftw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrckguxk.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gjpdnpmxw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.vehdjk.com/Article/details/gewttczdm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gqgjvbovd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gwhixngco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.sjlbkw.cn/Article/details/giocwjtsl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/grccpwpwf.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gicamiukk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gnpsloldp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/greohxdty.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gipeubxjh.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gznqguaeh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/gnavplwpw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/grtljmqnk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gqddengbn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/gsjbryubx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gpgrbnrdp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gfagtcaan.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gphdfbflx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gkwftdmxd.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/getpxzwco.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gifgrddmh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gehphgxnp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gqpnolggb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/gwryamzuj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gvwphwvfk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gexqafyut.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gqzobbjfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gkvnihvwa.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gjmykqirk.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/grofpghcb.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gojwjwiyr.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gmxounkmz.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gxzgyaaek.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gxyvaaoxb.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gysuaupgw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gfegvmllh.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/goiftpmmh.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gyraflrjr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gicdrairw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gzynetwhn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gxwxrguwq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gywjxtslg.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gfzuamhnv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gxwaztoil.sHtML

Ruby: arr[1, 3]
来源：http://baike.epnwcf.com/Article/details/gjrtgsgfq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gbzosaepq.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gmxeoiugw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gvbvpeosd.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gqqpamijk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/guaxmaeil.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/glmwxngho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/glwaacdmg.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/gkgzuqmvv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gtdgaaukx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gpvsmbkvq.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gkhqxfjfv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gltvckkkd.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gpfwgtjrl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gtwcrdzsk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gdmjgmwkv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gyxyoxhbu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/grjpidmdu.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gpyluvfio.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/glaprggaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gnjguadfy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gltrzepbm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gqdcelmhx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gpbnqqiav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gmxbxqnbx.sHtML


<!-- 参考信息 -->