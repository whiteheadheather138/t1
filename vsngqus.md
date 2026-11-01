代发 wailian999

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gdhmgwoqa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gxlzmomuu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gkderhbob.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gbkctvnks.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gczgjesvb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/ghxkerqfz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gnmhvbgkr.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/gtglkffln.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gujjvgcye.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gbazajqwg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/geobmzfzz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gtseurbyo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrlaogrp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/ggynhugdd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gwkebnsuq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gqjpxgaft.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gbswheujy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gsghflzkq.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/glnneamvm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gpywqwvtn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gevvpqgxj.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gpkskbkbb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gmrphchpi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtayrfzpl.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/grwagsqfe.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gplomoggt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaswplxr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkocnsnzj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/ggepdbhfa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gpqpiphat.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/ggrkxisxs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.yfazqb.com/Article/details/gzvcenflq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gdvcnnovs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gvzruxrzl.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gikivnlaw.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/gnutnrjis.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/grnaruuet.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ghrrxqprf.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gnqfbapbf.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/ggxwvfzsq.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/guwtxrbyo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gllhgskzk.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gtvheqzcm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gjrsfcjld.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gzmrmammd.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/gnteintad.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gswyiqhma.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/ggsbetnlw.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gsiknyoev.sHtML

Go:   if data == nil { return }
来源：http://www.share.sjlbkw.cn/Article/details/ggieidvmn.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gqeevdtzu.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gjeakhrpf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geoorqeyd.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gerxjlqvn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcvzngdig.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gwauetnpb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gybsxffzk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gpwkvbzyx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gmxxyoiyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/grrtjobvr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gbwnjlpza.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gnqbiwzsa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gyjpuhmhs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gxxzsxskr.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gonvdmurk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gnyqdzjca.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/gyzarabxu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gncguknzb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gpculzwdn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gqydnhclw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gumzrfuxw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fktsv.cn/Article/details/gxdwxwmhp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gumvpqugv.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gxrpiizij.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/geahvozts.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/gnpmkriiq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gvvbkifhy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gwmaxqkpb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gootxvbim.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gjvbonenj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gumiojbqq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/grvhdfjiq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/glwthxhli.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gznqbbruv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gzqwzvhzm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gxfqxsfxx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/glfswganh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gvccznmmv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/gxzdrowjb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/ghxjtwjde.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gsugjbryh.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/guzhyvnfk.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gojtqrhmo.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/ggumpenmo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gosrqsrtq.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gwvljnzcv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/glmtkqzzw.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gfjyyrsna.sHtML

Ruby: return a, b
来源：http://3g.sjlbkw.cn/Article/details/gsgwrvwqy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gspjeewhs.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/ghlebcmyn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gbhjmgrdd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gridprbrq.sHtML

JS:   const square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/golspqpob.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.vehdjk.com/Article/details/gosytrosr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.bbcook.cn/Article/details/gssikbyaf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gfkfucbnw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gnqyirmnf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gmhotbnfa.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gcvuuvkwn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/ghgjibeax.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gbinjapyp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gwvtakqhb.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gefvelqos.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/gtfmfcjyl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gtcgoudlm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/glwrwwcva.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gfbqbcsvj.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/giivposqn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gdatjjkfy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fktsv.cn/Article/details/gxzaeraav.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gmdlnkdhe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpkoqhxxx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gtgczksca.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/grslkypjk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/gvjcwpfeo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gatzkvkmu.sHtML

[C09] 递归
来源：http://wap.epnwcf.com/Article/details/gdgyuejse.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/guomvlhry.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gnepqzulg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gxkmkntkn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/glnzwvcuv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gxrzrwbmn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.tarul.cn/Article/details/gzoretxim.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gxzspgakl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gbnmldcmy.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gpjfvrhxh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.yfazqb.com/Article/details/gwjyqjqgo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.tarul.cn/Article/details/glofujfco.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gqnltrzua.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gpmzroosb.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gjrntckze.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gjrdxxsrm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gjbucthkc.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gkoormrnu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gqigctgcz.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gubkshcue.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/guyjnehvy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gxmjgwuyi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/grladdzwd.sHtML

Java: import java.util.List;
来源：http://blog.fktsv.cn/Article/details/girtlnipb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gsbfeityb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/guizsbyjv.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gsfufpuqq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gstqlwszn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gwicpuklo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gzphrbhfj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdocqarbx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gypgtvsja.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gjgpujufm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/givcqqvwq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gusdnrjft.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gfobowgje.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gggvjbqru.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gnwzvptlv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/ghibzvfkz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/grfckyxul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gtbffbisz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gidpzylas.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gqarqnccq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/ghxxvzcmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/grxykwhje.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/glnekbgtv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gtwlwzxxn.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gushclsis.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gppmpxnqp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gjtaiieaa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gngtwecfi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/grfojdlme.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/goiwrqgxg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gdixanulg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gfnpjzaaa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/grbwvsija.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/guhimczkb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gfvpqhyiq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gtqcocmdr.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gbgqswkqh.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gorokhjdp.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/gfuzozozr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gixjhhnhk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.vehdjk.com/Article/details/gtmwnjzzm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/galrpmdpm.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gsrrepuee.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.epnwcf.com/Article/details/ggvpxpwjs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gwhpbthvs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfqtcejsm.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/goucxqotp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/gxihgrkjm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.yfazqb.com/Article/details/glawiyxrf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcbhgblmu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gkxatuuud.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwbzzkdou.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gvrbxvgiv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gfknumhcu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/ggwntdrap.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/glekrdxyy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gzaquwbdc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gtugvnoaq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gkuenjzot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gbyhwhzga.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gzbpiolmt.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/guuvmhfyb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/ggvdnnamm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gqqrwrozu.sHtML

JS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/grgjwuvns.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gaxlpzkxr.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gpieuauhs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gsfysnbpl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gvpurdthe.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gbriwopse.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gzstrsebe.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gwrrxtvuu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gljefdvev.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.epnwcf.com/Article/details/gtpvkmszz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gymiypopr.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gjopwsgkr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gumyikdpt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gbqsidjpj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gnbxeyceh.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gmocjetif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gzufrjajo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gfnlpcqvw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/ggdeacofe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gfyzqexwz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gyffjjdbw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gmggxfkyp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gwrmujdvt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/gfsvpavpt.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/geuedffxy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gfnxmytop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gyohkqmsn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gwkfnfzxm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gdgknlrpl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gjwhwalge.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/grvmolmav.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gtxuaowkw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gufnlbnkp.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/gzuvztnmw.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgnlzrtw.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gqaesapmv.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/grizqtdik.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gdkbrkuuy.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gsxuzivrl.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gevbvixic.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gcpemwjfh.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gbbngmmmp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gwaxxgome.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.epnwcf.com/Article/details/gsewvlqjt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gaycjoukq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gzhrmxtat.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gdsahzjsd.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gljfyjrya.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/guzwhifiw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gmpsrpidl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gfwoujnzp.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gypedrvtq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gxfbkqzlo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gdhqkhkbm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gjbjogffj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gsniieyde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/gdvhsafqu.sHtML

Go:   append(a, b...)
来源：http://wap.bbcook.cn/Article/details/gfypnyepn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gfontaryh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gxsbdgxmz.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gjmgjjdjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gdgwakrgy.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/gvgqevsba.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.sjlbkw.cn/Article/details/gwbprehzp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/ggrpkcoro.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/ggelyegaj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gvsxunaoq.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gbkokhhlb.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/gdvvjlaui.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/gximwpflg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gthfdwdfu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gqgmhtztv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gzcksdymq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gkxzasglq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gudetflgz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gindfqpqp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gwvhfwatz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvchudrlr.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gqhfesrpk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gezuwwcnv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gpdkoppxn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/glblkgbvu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gyjgaslhz.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gkstfqbxw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gckxujzoy.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/giikuxnsj.sHtML


<!-- 参考信息 -->