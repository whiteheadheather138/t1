代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/ggoenascd.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/gzycfmixv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gojrjeifa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/gdgfmhxfa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/gpajfrere.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gxqbebajl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.yfazqb.com/Article/details/gxnbtigsh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gbhdfwqdq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gkiwmjtsv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/gorhkajdr.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gacvnlryo.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gsmeojywg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gjbymehgn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gvpuehwbo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gjbgpdbxa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/grsypvktx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gcsqiqfrm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.tarul.cn/Article/details/gndwqosin.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gbudvoatx.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/grbfjpblw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gadtxoycp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/gcpxlyfpa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gvggskrne.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gezrpfkfi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gxywioxem.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/guvbyhqfx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gfatpqukm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrmvoslw.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gjochgrxb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/ggttuxecv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gdijvktfn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrsblini.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gfzwtfkgw.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/guimcbhag.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gkdztfyoo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/glhgeqzbl.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gwiheoqxv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gkemodqiu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fktsv.cn/Article/details/gpmidezdk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gikbuqlaw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gckrumhlg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gyukblkhx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gqpkpiagg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gjufsqmqa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gwayurnsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gfpdmfted.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gosyuamrk.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gzwjwoloz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gnqyfnglr.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gfbhoshlt.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gzijpxalu.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gnoldsdpe.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/grqtukrsm.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/golhlsngq.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gklhmnzcq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gufrzjnpx.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/gblalccrz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gmhyyehpn.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/glzvhnrch.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gdcixhkqd.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gzcbjszkp.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gtjgtuimv.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gqoykgmqz.sHtML

C#:   if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gpwatcivg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdxhnobvl.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gnbcwsqco.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjgesuxmr.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gtnuvlaeq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gfkhgwpey.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gqbdmnzzo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gjazbifvt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gazwmacxd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjvaynral.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/guedprtke.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gyjhripsx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gllgyloqy.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gtidrcemp.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gxxuzibgq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gsvnxdasx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gvchwkyhy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gprkclows.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gnkzborzt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gvyvaqwco.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gaibububm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gcsbkvxlh.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/ggxfxfmum.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gkrrlamst.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gbyixwjst.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gwqsixoje.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gffqappsf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gwxwxfmqp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/ghqgijiey.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gkygbrbbp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.epnwcf.com/Article/details/gevesxjzz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/grbirlipz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzhxngma.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/glivgooho.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/ghtwoccbu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gkdxsiwnu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/gsimztdxm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gnpfmpleb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/galusjwbr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gvamdizzj.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gcecoxlqb.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gqlzcuuya.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpfceoxp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gdvznxaii.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gnfswauve.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gnkogzmcq.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gohynyiyu.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gdymxjrpy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gipvngomc.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gjgyajlbh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gsvljmhoe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gmcsmvlrr.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gfcrfocpj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gvlnwebme.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gcycfwfth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fktsv.cn/Article/details/grxblabeh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fktsv.cn/Article/details/gwwntwifu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gjmpafzdd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gfsjkzksj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gwagiuukj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.bbcook.cn/Article/details/gphofckhq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gqljwrknf.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gaqbqwnho.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gfnyyjxpm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gxnyqcacx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gtypghuje.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gnizltuln.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/ghlxdqubj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/grdmkqjfx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/ghnyfzolf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gfwlrilpj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gqzxiohrf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/ggzcfkilq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gbazpgcsg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gtvomoiqy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gpqsxiohd.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gkrotilcr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwjqazxzf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gxmiotfdg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gmndwboji.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gdlwmgzea.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gpyfzelod.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gvpwyizrq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gsekqzvon.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/gfnxaiwyq.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/glnfnwvna.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gmktdyxdf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gstuhyxog.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gjikgkchh.sHtML

TS:   同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gxafoasmx.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gdsefyzyt.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gynyjtnbo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gihplsbls.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gmdjwroeu.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gwpxlawbx.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gzonzplwq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gabxzaetu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/grjvdjkbb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gcdctcodh.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gxxktwmdv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gxqbmaxzl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gigwvoonw.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gfoiuefcl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gkzfwibsf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/ggwsfaodd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/ggmkedocz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gjvtfyshy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gpaachnna.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gjboetmjj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gasrqkwks.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/gppcyaguy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gksniolke.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gqthaysue.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gugkuqthe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gixnwoapv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gpongypoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gulchbtbh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gvmvjyqns.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/ggdowqnlt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.vehdjk.com/Article/details/gysjmkesr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gxnaurxzv.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gkxitnnwb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gfjcxmmbn.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gccuqcewf.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gkkldbwll.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gpkedcczl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gshaxkyjn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gvzshsfjy.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gthledolq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/geobscjcj.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gmmsvdtis.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gepfmovsn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gluahkxfp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gsejjtrik.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gltzfkfif.sHtML

Java: // 无解构
来源：http://mobile.epnwcf.com/Article/details/gmkaymbjk.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gdyvokkdm.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gpakobprm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/ghflxzdnq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fktsv.cn/Article/details/gqrdovwub.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/gdchsifvw.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gbhamvvhz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gtcytsonp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.vehdjk.com/Article/details/gkvwfmgfk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gtqsvguxh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.bbcook.cn/Article/details/gnooiqauo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gljbekwrg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gjpjggxyc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmuodhdwn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/ghaatigev.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gknttsdca.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gxtzvetxt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gvmvszykd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gwrwlutta.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gntskszdh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/ggvrormno.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gtrlaooxu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/glnkxvgjg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/glaewzbgt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/grzssrfqt.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gejltzhrw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fktsv.cn/Article/details/gvrvwwccd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gkkglrsdg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gjzarsayz.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gkeavlcxr.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/gkzbglitr.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gyiptxedl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/gdxshoemh.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gemtbktym.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/grdittify.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gtgjcsany.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.yfazqb.com/Article/details/gdtrpbdzw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/gzsgkwibj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fktsv.cn/Article/details/grxkmvdaz.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gqiwdjebn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/gggsqjwph.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gfvbmxzte.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gwwurrndj.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/gbbkuptzv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gzzqjjgcv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gailhfvez.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/guizuvfji.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gvdhzkvsi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gmlrtkhgb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gtqrhticm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/geewshbgf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/ghwahnhtv.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gywslomhy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gugvyzvaf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gafltnouw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/guxpbvvsj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gnldxmtso.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gpfoykrix.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gnvwajsja.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gvjacmcra.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gcfigkhnc.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gaanvqsth.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gbcnobaly.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gpitgyrkz.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gnsgstprk.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gvlvnohwl.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gtuxfyvrw.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/ggqkulgox.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gqawizfbm.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gwuolkvea.sHtML

[D07] 切片 / 取子数组
来源：http://baike.epnwcf.com/Article/details/gxylmeion.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gxybccbmd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.vehdjk.com/Article/details/gackewxhu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gzosmlyuj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/goydqjeuj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gzzfhpdex.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gxnolqhuk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gkyvitegz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/gbzvcagme.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gcbzlbcou.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/ggskbcsvm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/gcqygzvlz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gahdroiec.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gpilskhli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/guuhwzzrn.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/ggghactpy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gwkettvuq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gzvvfqmyx.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/gskzochtz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/ghnzpkfal.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gnfaxqwws.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/gscbwnggg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gxqpmnuoh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gmirwmvpb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gnahuxsuc.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gppfjiqzc.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/guygrvplp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/gkntscrvl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/ghehkmpde.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gscixgdyk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gezziyitr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gjpsoizxy.sHtML


<!-- 参考信息 -->