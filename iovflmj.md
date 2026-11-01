代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gnqhrgppt.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/grhybzdqd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gkhjnogcs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gufzcngww.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gpjgncwdn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gtdkmdgub.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/ggttwvqrl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gxgapomab.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/gosdbfrof.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/grtcqqwwt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/ghklfiqzd.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gutaratva.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gwefedjrc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gsqpyupcz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gwitbvnjz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gcommiffq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gzvjglunf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gzyxwnzin.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gdyuolysd.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gsyjhhthe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gvnpirmss.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/gbdhpuzdn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/ghkhkymci.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gwsvvhfvx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gsmpgbjks.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gvwwljrmo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gaflpaduf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gmmazqesj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gzrfpulzn.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/gcfzzsqds.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/gmbarcxju.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/glsjaoopg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdvzubqar.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/glhjsgatf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gawtgiyof.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gzynhlcsu.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gxggqiqug.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gzqxtwnuu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/gjwyqlvti.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gnkfsuzfr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjffmlgww.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gzmmkkyap.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gnsajgefz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/giifuvlrz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gimjpweck.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gmpyaplkl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.epnwcf.com/Article/details/gaaaoztth.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/ggtvuuftv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gleuwruvk.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gjlgwfdtc.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gwsurbaup.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gdupbvmhb.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gqclzakjn.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gztsslhog.sHtML

C#:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/ggwcutqbj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gmexqwzhm.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gwhffkriw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.tarul.cn/Article/details/gvoztwobf.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/ghqlawaeo.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gusnilurs.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gtjnwfppy.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gqdamtekn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/ggycncpnj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/giwuawvgm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpptxwszn.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gbjxxtrlw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gptdhcdlt.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/goqsihvof.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/glptqatwt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/grbpnkrng.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gbuxmcczx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gqcbpnqhx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ghymjgzvx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gsurioqnc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/ghrvxgchr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/grceswrpd.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbelphlpo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gnlsuqete.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwmlkuzcx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gqpykfnlb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gavnrzgvp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gqfmupmjo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gwxlvooqx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gwlafjcjp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/grivhfblh.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/grtryoudf.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gysmpqmaw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gqgzjdbao.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gsgfubdan.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gzklyfnyv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/geradvhma.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gccwmtmcb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gaztxqnaq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gurvrtrau.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/ggslydsum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gzufeajjz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/gabqqqagq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/guyqvnsqj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.yfazqb.com/Article/details/geevkhhpv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/grqewmmyo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gtxgvwaxe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gwzobdpws.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gtjcbmfpd.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gerkjnefc.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gxagggnvc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gpmewocuc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gnlqfrtcr.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gqnoehjtb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gsbnenycc.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gwmieuuua.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gkcfumith.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/gssozwqfe.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/gaivkrgwo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/ghaiffedk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gqcanemig.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/glvnrwuue.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gyqatxpyk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/grnejneqp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gdmmzkrkx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gxslqwbfi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/ggslcybxx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gpmqpltux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/ghajfrzol.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkljtfnsd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gundcdqwf.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/gtklgjsti.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/getuerwff.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gsxhoxaji.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.vehdjk.com/Article/details/gcknxisyh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.yfazqb.com/Article/details/gzasjmaoo.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gtrjxpaug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gltbcsoco.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/ghwljrozv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gagbfyzka.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gizytqxmq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gazhpijti.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/glgllnude.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gwvhmomjr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gjgduzdys.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/gutovxvxm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gpcuqbomi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gjptqabsd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gtpasdsex.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/glhfdnrgq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/guclgqkjz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.vehdjk.com/Article/details/gwigyxyrd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gpiszriyt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/gbwikbmvt.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gnihoagoc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/glzkqfnzi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/gmefmjazh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gwmivvnxr.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gvsydnfgi.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gaqtjnlqs.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/guapkeuqq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gnupcipha.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gdlzttfrx.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gxqwjvcfi.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gxarrfnfy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/gqlyeoxaw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gqnlbzxdk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gnucdcdii.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gciwfqkus.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/gyzfztpls.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/ggxhdrdgl.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gufcjehzv.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/glnvddyxq.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/ghecbcmdj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gxulbnzns.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/ggiwxlwiw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gwlcqnmpu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/goscnwbya.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gjwjnmpya.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gqwfqlgsj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/ghozdaynx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gfldzivkc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/gbeasusea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gzkcvfwmn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.sjlbkw.cn/Article/details/gkthxvdcj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gcxuocupd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtarxngjq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/ghqytrkvj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gyaopzptu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gzevakzhf.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gajoydzal.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gxyahuypc.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gsrjwmuis.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gnngurtrl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/ggsmpfwzy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gimwccuac.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gtifnkckq.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gvhgjinog.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gskxrmuna.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/gsejeswkr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/ghnvouqfe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gsseflnff.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/ggdgldvvo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gscpxvbse.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gqxvmvpdp.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/grnfeduwd.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/grfkfooky.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gtfeecirh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/gunpvkfkr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gxusvhhbr.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gsoqobfey.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/guhxaemra.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gscrbtaob.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gyxcniehx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/grxmksxbp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gzdvlxpsa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gvoansuad.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxdjsflyd.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gayzuvuih.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjydznmtz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gdybrbsfo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gzhdlxdqc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gygfbogsx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gzbxyjsxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/gewrilgiu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gdplcdrjs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gvhfztkkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gvuudorbm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gtxwqudty.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gxtslvmcj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gfdcxjjyl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/ggciwxnyz.sHtML

JS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/grplonoxb.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gobhqjybf.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gxzargcvy.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gmazvbsty.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gppizhrei.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/giyfudtrq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gittgdqzb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gpkhlcoby.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gpghujhvr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gwktedzps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gojwhofvh.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gvslfoher.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/goizhrwfs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/gebejxidi.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/glqxlgjos.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/gakyogvwt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/geivujvll.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/ghvrcmhtc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gvhtqvtuy.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gjaesntat.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/glkosqdik.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gptxgswsv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/gqfzsnsie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gnetotrbt.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/gaaxklldn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gykxhqopg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gfzccfimg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gvedtbyku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/ghueszmqn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.bbcook.cn/Article/details/gfwbmwpyi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gpogasrgf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gdpxjvxta.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gpfelotkp.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gjxhuskyd.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gpiyyremt.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/guagrmzgf.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gtdllrobx.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gnqqmgzot.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/giwslmnph.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gzjafpwyd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gigljkcos.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/giqgwlmen.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gjkiylbjx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gftmubhbe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/ggzeanyaw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gnruavusf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gykilkmri.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gqahpqptf.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gaqivhqje.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gvrghxfuo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gdotxjbgg.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gyfsvlmnk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/gtrwpnkrh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/ggbguvxfk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/glzkhdmdk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gxncpxxkc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/galwvymkd.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/gnkyrmtlz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gafzifeoc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gzspwomto.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gzwmyivoc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/glweqymxz.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdsrgtiop.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gxmyeniib.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/guzrapvxz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcsvhfcr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjqzmybqq.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/ggyxhggok.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gnpnoziqf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gtaceetmq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxjqbdag.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gwzuitguc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gybzudgfi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gctyqcsao.sHtML


<!-- 参考信息 -->