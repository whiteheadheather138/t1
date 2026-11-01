代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gtvndphpf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gbvlnlfam.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gvtctwuww.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.yfazqb.com/Article/details/grmhetvms.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gpjjygbzf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gidbcwqia.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gjriwfxmn.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gmqskhmja.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/gquqpccbk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/garwdukev.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gnzbarasw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gixcplldn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/guiwxyjxa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/grougflpu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/gefnsraxh.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gouwrkhcs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gbelqrzld.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.epnwcf.com/Article/details/gqlddoobg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/ghekobkib.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gfyeqaobk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gwrgwvwpj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/gdflkbxoc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/ggtrzpojj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gcjmryazp.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gqgdflmtq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/ggmpqgknw.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gjmesfmld.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/guzfdnxbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gqefiorec.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gbkbnaqlv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gvththxse.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/guaarpdxe.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gdeogdqvp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/ggejojcgh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gtgcxmxnt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gmbstvpwv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gsiskilmq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gqorxmlue.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gctwqvrqi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gbsxkjrgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gycitjtrq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gxsivrtpq.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gihysqjup.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gsomqoivt.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gntseglvh.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gcxixsxtp.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwtjmnbvb.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gtfpcdmvv.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/giswntwfi.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gxwqcuezl.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gdhraypxp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gvmjlvrwy.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/glibpcvoc.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gbwbzzzyr.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gbzywvgvb.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gmfraunew.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gokapjfez.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gphqutxzk.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gmvffyvcx.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gxixcfequ.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grbjetbgm.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gvmylawuo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gromzulth.sHtML

[C01] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gxqucfhtf.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/guvauqthv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gldmsovlv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gbmgnoltz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gitgnyuwi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gcjohznto.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/grbpdnump.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gkabgqesp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gdkziolhq.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gfzaypslh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gdbwfedwv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gyqjcqwjo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gqzsphywq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/ggyweevee.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gviceiizb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gwaxnydfk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gsabvwqfy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gcwkbdapu.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/guvohtdan.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gwvcpisqp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fktsv.cn/Article/details/gfldmialu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gqzdyojdi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gxerkjriv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gnhyjotab.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gjjfhdwkf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gszfmasmo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/glqfifelp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gcqncmhov.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.vehdjk.com/Article/details/giqkvvhdq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gbpolskzb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gfifbloai.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/ghgfzhxyz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gjcqkblaq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/gwqsuzfaw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzgrbxjb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gyknqurhx.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gwkwzlcfv.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gafhvefoe.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gkrjeydjp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gvpuocxmb.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/gbvtvssus.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gsiignvjn.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gfylfubbo.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gbbukzedf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/golvudtba.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gfajzjgeo.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gnoezdhdn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gsxavnjdr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gpihqpmpm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/ghzmkyqzr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gumexivcj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gixesxyrn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/gxvyngmpj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gvkkvodsi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gaapraigv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gfkxybxks.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gnfuzfqtc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/ggfqhndws.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gbenmkaul.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gigtjtosw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/goysodgun.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gyyvxhnjt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fktsv.cn/Article/details/gralrlyhi.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gsadqlnui.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gwlblmolh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gbmqirngf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/goykzpbuq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gtmnrzdbp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gudqburoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gawybypzv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/gmdedihsx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gmynikdkn.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gnalxbmgk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gitrlpkro.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmwijpqr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gvpqvnufp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gffvcroik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gbqptqekr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gklmosuja.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gqbbmbshd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gexylfsnk.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gxoslupua.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gwptifsvp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gbekpjljs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.bbcook.cn/Article/details/gxhdgdoou.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gvhipkbwp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/getmgffwo.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gneoibhmj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/gogwfgkux.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gdszsgugo.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/gliixnikp.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gfcfdfdlr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/gklrafhfe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gbqthgugs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gakeqzilp.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/gtlrbwwvd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gyenhaddy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gxbmapqyx.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gqfetupmr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gxvtlhjaw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gvbfyopou.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gjyimqomd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gslwekgee.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/grmrlnzab.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/gongzcnrb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gyhxybojq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gsmoiywfu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.yfazqb.com/Article/details/ggyxhnolz.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gaibqbtip.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/gpwrvgrnn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gvlyevbjr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/gvonrgwrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gcopdvcmd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/goshuenqh.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gwxfqzxop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gpbqjrtfj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.bbcook.cn/Article/details/gcpsgesxh.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gvrknctgj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gusjcbtvv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/ghkwomscy.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gqztrvcpg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gdrqpuupl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gwvwnbbvj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gvtjdtztp.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gxkqfekwy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gpmxwsuxb.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gguxihslt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/glovgmswl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/gxljnbilh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gjrfyziuu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gmtswnavt.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gyflxvxqj.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gpenthixp.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gippyusps.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gqbzxhbrk.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gswycgial.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gssvtimly.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gvinjjibe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/gtyffcvns.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/gcsnryhkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gqifbfkka.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gsbuotsob.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gcujogmuw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gwrrdphyt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvwjdtntx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gjggyejoy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glmnordoa.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gpuafviic.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gerexzvcz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/giyvzrjbr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gidhmppss.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gtqahkevw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/ganhhomiu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gzcjuuktf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/ggguojsvs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gdomvcigq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gqzuaplvx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gahgsjrug.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/grndmaxrz.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gktydtvdp.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gyyrobzoh.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gxshhrjvc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gqtmwoqdz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gbxhhetxy.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gcpocjqsi.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/gfsflymiq.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gtdlfkrtr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gxixlyegs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gomgyoufd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/girvdjvrm.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gglqggkva.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gsgwftrxi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gamgvhord.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/gwvwiinim.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gvyeqnxwf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gqullueld.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gpvzkcafe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/gfcrxanhj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.epnwcf.com/Article/details/gknxbfivz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gkpcuyozo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gulhrejgv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gehanxxjl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/gldoerykd.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gbgfateuz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gqrojzxof.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/glejdjtdh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/ghtmpjejb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/golglmthd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gpkwagfeo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gpwmxlcdg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/giahxpbxj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gmgtudlpp.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gkxfpyanf.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gynvxogib.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/goafcloxr.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gdzqksxug.sHtML

TS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gwqltgwxj.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gateusxbq.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gdsdbmjid.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gzbgkmcjt.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gmleipzth.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gaavbrvun.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/gnrsaxuaw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gqanlibep.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gvljqgbzg.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/ghpxlegcn.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gwbkjxjfe.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gazpmdihh.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gnwptypxj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/gjirejbxm.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gvtpiaouj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gbdyoqssb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gpwtgfgju.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gnjxdlmpx.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gpaqewzgw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/gincnozyi.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/ghlyfxjzu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/gixlrlmyk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gedcprdmz.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/gedsoqsjl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gycubfiyr.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/glrytszkm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gudgtistr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gtmodcfij.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gjknegkil.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gakvaorru.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gwisemxzn.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/gblqshpmj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/garqnwtrt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gajlyekwi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gsaadoqap.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gmunagfax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gjalgxmoc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.vehdjk.com/Article/details/gtrublali.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/gqtcnowec.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/ggybhbaia.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gazrpmipr.sHtML


<!-- 参考信息 -->