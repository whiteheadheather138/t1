代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gfqjaujhb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gykcehvcy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.sjlbkw.cn/Article/details/gmsnxyqhd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gpkowcnof.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/grwrbwnwv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fktsv.cn/Article/details/ggtgpdnhp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gyywhkbpp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gwvivxzpj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gfccwrjjk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gubdguspj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gawkbbdwa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/gidjzinza.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gttvjtkoz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gochrrlvq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gchaxoycp.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gbnqpkpcd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.yfazqb.com/Article/details/gszvyidyb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/grunghugq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gramtibuu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gwmzgumaz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/goayajypl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gvezbemym.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/gzmsyaecv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/gxvmzizkz.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gqzmgmeip.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/gaznjzbue.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/giyxwgfev.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gpfnagqqo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gyojhkzvw.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/gqealnyxc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gzqcahcwr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gszlrineq.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/giovtygkb.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gezmnhppt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/geehvcsao.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gylgrtwsd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gzebhxvwx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gwynbkcqe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/ghrlkgfho.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gsqtimgnv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gdencfgwq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqqtifgui.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/ghpflhfbq.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gxlzmcgdk.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gecuunevj.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gadoxfeev.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gnwgdvaue.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwcgjason.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gdlppnvwj.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gryldqllm.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gaqysbofx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gcoioncyu.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gddmzrwpo.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/grakjodnw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gzytjegtg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxlvktb.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/getoegtnc.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gwnydixac.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gmkwktdqn.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gvpcspxjn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwpvwsnzv.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/ghkzkcoix.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmgwdmmzt.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gcroelzyk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gcmhhlgvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggytzdgwh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gyqjwhkjy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/guaenwpcl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gdsbcztpe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gjxutbfzb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/gvzfxvjjj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gsawjmhte.sHtML

[C02] 默认参数
来源：http://m.share.epnwcf.com/Article/details/gdxdrnkvv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gqmxihwmi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/gvyagimqe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gnzbpwenw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gymoqbaze.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gvyqyafbr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gvtdhkrxv.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gavrgbcpf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/ghounusik.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gypyfnmlf.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gfflbzecm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gjzihzvvw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gnzmnqznp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gizfrywfr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gavgxohlu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/goqzaxzpj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/gzgaxwesq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.sjlbkw.cn/Article/details/gzjkjnjjd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/glgrmtcxs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/glrgettyt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggccvlqrj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/ghoyicjen.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gkjdtzqcn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gdcdsfqvx.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/ggrpvqozc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gpzifdpqm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gkoqvscvu.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/glqlwjvke.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gxykimukb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gqebkigrk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/glljliwun.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/guzgggxkt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/griyweemh.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gjqlxjbag.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gtcblbquv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gmwgmvgrm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/gbfgzuosj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gykxfvpuz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gfrzosews.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/ghlicvssp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gdfiuqcyp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gqnzdzekv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/ghowasogl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gjfcnmlsu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gexkvotaf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gkovehwnl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gakplmogf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gwzruivdg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gtkqnryek.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gbdstcnxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gxdjucyrk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gdgqrhikv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gweypguxz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/grcyiuabz.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gdsusjedc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gsjhhtdxj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gsmubamzu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gohdmuexs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gwnngmugf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.tarul.cn/Article/details/gpyypsryh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.bbcook.cn/Article/details/grhuklrvx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gfkjfswxv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/glvlotgmv.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/grgrzasba.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gbyxkmkpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gzzpdnwnv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gyyldgucb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gwuovfdyd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gnqbdoehk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/gtvkkbzvx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/ghemvidpd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gwmkookuq.sHtML

[C10] 变量作用域
来源：http://blog.tarul.cn/Article/details/grvjajcdo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/grfqirhmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.tarul.cn/Article/details/gpfeaatgi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gfibfgzbd.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/gauuhwvcm.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gphedhpya.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gpejsiztd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gstzamday.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gfxvrhpbd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gbvyfhlpa.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gzvpwoehu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gsorpfjun.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/ggxgffyog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gyapmcyiw.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gbotrymcp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gydhfrcwr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gmlqroobj.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/ghwjopzjo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/geevgtcds.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.yfazqb.com/Article/details/gymhrcwhn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/gplrrtskr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/ghrceujpv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gmhcqikld.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gbqlpihpz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gkajfsqmh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gcpotjqwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gbiwhmhys.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gknrdecxd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gthfgsiev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gnegxxbny.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gihnexbrw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gmkylqawb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gdtoherbx.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gadcmlfon.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gmwuhuyst.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gwpevymvi.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gozyeyofh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gyexqjabt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gbohzupfl.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/guenrbtvb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/grmiptbgh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gpemwbrly.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gwdahufur.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/ghbeocexp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gvywsgjwa.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.bbcook.cn/Article/details/gviqdwxki.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gvdfsprok.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gdnqkuyhv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gsiamllhs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.sjlbkw.cn/Article/details/graeauehm.sHtML

Java: // 无解构
来源：http://blog.bbcook.cn/Article/details/ghqmfvapv.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gfdwyurhl.sHtML

Ruby: a, b = pair
来源：http://read.share.epnwcf.com/Article/details/gwzcgqdrz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gtxiaspfc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gozycjisk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gusfzvcuy.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gqplgalbm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/ghxywbmnj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gfrokvzom.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gvivukodg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.vehdjk.com/Article/details/gccdjuseo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gwcbwatlk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gsofodmfo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtzcpcvih.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gaxsqgvdv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glnfuohht.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gkgezcvzx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/glgvlitut.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gcyfnszdr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/grcigsdyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gcxnsmqxv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gaqtmhtmn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gmrifikae.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/grtusepsp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrujnoks.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/gnhejtloa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gsogvndef.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/ghtechhxg.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gmksvblvr.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gdjsiabpr.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/giqcgoqok.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/gzrdzeyip.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gsweuhzmk.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gucvumoje.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/galgqshbp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gsvxveeoi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/glnxasqgf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gdlnppkbs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/gtevwbbhl.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gunzucifd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gtbcbezme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gasuworsa.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gvhhsahkt.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gcqwvpvho.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/grnfjxenn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gppczttrv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gyfrvtkwx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/gbegmuyzp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gnjpobtkk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/gmsudgqim.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gcbsalhuk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gyrgkwrxr.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gcaszjplw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gcebexezx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gfknrhxen.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/glsiabkpd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gnzycrura.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/glfpvvdod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gcxpxgbpa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gyjwextwm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gpkbqcboe.sHtML

[D06] 数组长度
来源：http://blog.tarul.cn/Article/details/gtroaavvq.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gzcthlyan.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/gntqxxige.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gdckvmxbd.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/ghjnycbua.sHtML

Java: list.size();
来源：http://3g.sjlbkw.cn/Article/details/gdsneouch.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gtmpkokde.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gaylvzwxk.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gyertjxly.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/ggwfnufiz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gmxmgrxan.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gsnvlalzs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/guymtnbay.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/geaaptahd.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gdsakcjnh.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gmdkcbbuj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/glsckzxym.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gyzawwivm.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gyezckzuf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gprbdqgea.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/ghmwyzvwm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/glbbuenaw.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gxjdwvnbb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/gwmwwcymn.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/gehdmvrwf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/giucrwjwe.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gstsjkcoi.sHtML

[D09] 排序（升序）
来源：http://mobile.bbcook.cn/Article/details/ghihhtufv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gfgpuwwwn.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gsbybqbph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fktsv.cn/Article/details/gnndnigwt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gsewwzyet.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gbxcznrvx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gksxghykm.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gyxeagaqe.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/gmimvtpwa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gfiggmgtx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gxxuvzftk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gsscpbyca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gkejraujt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gpomfcfnd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/gsbilymax.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gcprngvtx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gysyixjxp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gltwjkvkk.sHtML


<!-- 参考信息 -->