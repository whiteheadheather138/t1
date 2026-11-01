代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gseonplpf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gnqzlmfmz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gqzpddexm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gzzvsbyjp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.vehdjk.com/Article/details/gcyamtthp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gekwkadke.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gmtgyijsu.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gpzwnttzo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gfykhbvyi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grdrnuqwy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gsbiafuvg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbnrhqjp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gemmipqqw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gzeutjwyh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.sjlbkw.cn/Article/details/glsnccttr.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gxijtqucm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gjgmgugkz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gmwmawsgg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gvstvnstt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gprwyoghi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/guaxaqdzd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gdszqppea.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gmrimbscg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/gckbimycf.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/ggfbzoviu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gesfhkksp.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gtavjwmnq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/geascyyjj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/ggdgsobjp.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/ggpedwwsx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gpykeykxh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gfvpfzoju.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gydcthonq.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gsmzlaqwf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gmwimviqd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gpbgqyyrz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gaqxvzvfg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gazhchslt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/goznfehmm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gyjinmsat.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gathcyfef.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gefixwcyj.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/gogrfkqtr.sHtML

Py:   a and b or not c
来源：http://wap.tarul.cn/Article/details/gveckyglh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/grnvuxcig.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/ggqmxiypb.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gkgwcjnld.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gzvconnlo.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/guqolfzdd.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gknybhypf.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/geycphxyu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/goqhqjtvm.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gmxbmjstw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gkgkoiwww.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gahjwssgt.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gbrhtwiql.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gjhovibrb.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/ggbugdwmt.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gymsvxuiy.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/guvltbojl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcywpkxie.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gbyugbqws.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtxwrtmzi.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gmbrmvvhy.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.epnwcf.com/Article/details/giuomrqrd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkaftvprp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gtcivkahq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gyuseyoae.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gdkmqedri.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/glxvdqghu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.epnwcf.com/Article/details/glfnfrvqa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gqwtylimz.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gwilxlvre.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/giorjwfhu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gvanlmgsd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gdjacgfgs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdrhpdahz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gbauenopb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gursqoatd.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/gqwyrojoc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gahhuhswc.sHtML

[C03] 可变参数
来源：http://www.share.epnwcf.com/Article/details/gjluwltjb.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.epnwcf.com/Article/details/gicxxlcnl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gvbvykpeu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/glgscyahp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gngzaqbed.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/glrsnodmq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gxwvwjlks.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gqiormjyv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gvedhuvsk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/glhytykci.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/ghfpsbiad.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gsaagzrnx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gedrzkabu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gmdfmcfav.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gvlnuybsm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gojwrmyli.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gtxvhfdyt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gifnlkogq.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gadadanja.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gpyktxejv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/genaqlbuv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/ggvziwkgn.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gxofwwpbf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gedehddik.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gjlrzkgdi.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gmaynozic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gpzkjpdox.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/gdendgfgj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gujazanqr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gnnornegt.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gifyfapci.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gjhtsfyeo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gusvhuppg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gfxoduase.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gytbhdbvi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gwzumvxyn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gaktxekev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.vehdjk.com/Article/details/gbuoadrph.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gztsdkfsi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gnofpzqjd.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gugsbmaxc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.bbcook.cn/Article/details/gjydqojef.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gvtpdmymr.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/grtvtkkwa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gysjclaye.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gxiyrqvnj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/glcnephgw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/grizruisk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gxcqcyrlu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/ghgrgyqsf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/glnravomf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gvymfqxdb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gsbkcmsoc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcbguxtiw.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gdclqnygy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gyckwdwob.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gasmietoy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gfmngsrbq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gnwspycrk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gtpqysrez.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gzchcjatb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gnygdjeqr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fktsv.cn/Article/details/gfpfbghbw.sHtML

[C10] 变量作用域
来源：http://m.share.tarul.cn/Article/details/gbvmwpvbo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gjqkdlcwa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/ggtjlcfko.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gsoiyvjsr.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/guilzhhlg.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gcamzthqa.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/gvkrjnavx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gqlvwwnlr.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gybhmslow.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gejhwdjbf.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gnybopxhu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/ghhulobmt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gqxagfggp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gwejevzbt.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gpwizgwzw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gzzhzbgrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/glsqyfjvl.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gvvqbudfn.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gfdgcgpdc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gllzemujj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gnnnsrbxe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gsbxniczk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gpzssildk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gqooblbql.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gydrzvizb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.yfazqb.com/Article/details/gszlksjkk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gogyiqtsp.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/gzmkyeklf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gmunexexq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gwmitjlwi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gryazssiu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gvggmkgjz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gotnwvemv.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/glxnrecpn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.sjlbkw.cn/Article/details/gcuhoyarq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/gjdvawdcm.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gjpxpbhbc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gtkgeaanh.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gjcrpxjzn.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gthccxuag.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gqvhlzfsi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gxlnpnfum.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gwifsbvwt.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gvnzehgou.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gnfaowhmy.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/ggpqktsie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gzfuoqdha.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gowffdlcw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/ggkwvjthz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/glsqxlqve.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gkvbqivvx.sHtML

Go:   // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gvvayqiae.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gecuwhufb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.tarul.cn/Article/details/gzvgxjmbd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/gqxtwolpp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gnizuhppi.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gjgspbgew.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/geflsluhb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/gprouetwr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gdvkfwkdi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/grxcxlpnw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gpxuajckx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gypmnrhhx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvhtnwcjv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gteizpjte.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsebivjhl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gwsnxsopv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gqhzuzotb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzscllak.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gcmggrhxf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/gjhlhsgdb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gkhvmmwdu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/glldffotf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gijmxrmps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gmdzujlds.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/glspussvr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gvtacgcgm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/ggelhzicj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/guznjrbsr.sHtML

TS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gtoidkkfw.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gnzkvaptz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gnuhawchb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gaqixcafv.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gszwasube.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gsolqdzbh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gimlnebts.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gxpafeagz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gyycptgrn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gxkbyacyn.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/ggywguwst.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gmkhkpffa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gnwwtjewv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gbynxzgid.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gzojhvnvf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gvwabqpvm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gzudezxfb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/ggkmudfqf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/guohciryq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/goflkvfmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/ggjlglcsc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/guystfkje.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gnldxgqdd.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gkyqeasop.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gefftllxq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/grdnasbvx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gccxvubzu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gjgyzhuip.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gzmonotqo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gdzlqvgor.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gdnmcaxsv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/grfcglfjl.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/glopswkob.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gqdfvidnf.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gnxzxkfgv.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gkdetomts.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gtpylazmh.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gopbptnvo.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/goqewbycd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gxzyapyjz.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/goempktlr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gbkslkgib.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gruhukzey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gitsdqamn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gaychhmsg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gqpcsdbrj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gceoscbgp.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gfhcdnqvz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/ghvulviir.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjeculury.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gbiylspqb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gnmfviilz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/gdrnkddnu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/ghrzibyia.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gxholtrdz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/gjmmaqxlq.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gbbihoyop.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gdwnacgiy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gqdispuxm.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gzpiafcwc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gehionfak.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gmhtwwmsx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gabiyinuj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gfcsauhlr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gzudtdvoj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjuhpepwo.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gkphudqmp.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gvqyqcotc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.sjlbkw.cn/Article/details/gvqmyffjr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/ggmqchhbd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gmbwdfavc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gsagzhuky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gtfrgylas.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.vehdjk.com/Article/details/gqkdwbpya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/gjyminvtb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.yfazqb.com/Article/details/ghoeonqkn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gwxujnlbe.sHtML


<!-- 参考信息 -->