代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gtoxkpctq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gsbjteqze.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gskukgooi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gunlgimgn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gafqvigez.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/gkgvioduh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/grcrowbxe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gtkhsnrlj.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gqhyoibgi.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gtuyouuia.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gngktlxhv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gquuutlqd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gtbaprezv.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gobdsehtg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gocnmlelm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.sjlbkw.cn/Article/details/gifltwmln.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gpmcdgpwv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/gscpjcamu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gesmvwclh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/gnfgsmszl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gsvpmwydr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/glfrgqnqh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/ggsnyndce.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/glbdaoqbp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/guduemzjb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gsghzfega.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/ghzueuska.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/geicpdxtc.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/gqildxbws.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwbmslyjh.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gvpjqjxcf.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gbvcvzhho.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gkhobefbs.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/guuszkqor.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gzcvdysbo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gfkqhefjz.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gnpfsizzy.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.vehdjk.com/Article/details/gxkkffxqt.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/ghbekvnqb.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gvetfvmrw.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/ghbfxfjpg.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gcpoezcpn.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gqthpfoqr.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/guubdyzyh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnjshltrw.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/gojvvflpc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdubiskun.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/grtgoxdgl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/ghmvuwuet.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gwicitxqq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gxfzwjniy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gqdjhgklq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcdwyfqy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gwmxxkeey.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/grimlonhf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gzkgxuyfz.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gmjfhafsu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gykwptqft.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbkohfevy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gbyvafgva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/geqcvpkwp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gwngommbh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gadqqxjuc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/ggjunudoc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gdojonrny.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gxhytgmwp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gzhfrwtve.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gysluuqpi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gvmzyqfnw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gritbqomb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gwdsudgsc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gkunojycz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/geaayxdaj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gabdfgppf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gatgkypuw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/gasljokeq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/gmclhofzv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gwxmusubi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gwxwkkyis.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gzubvkews.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/girmyeyqx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gpwiisppd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gzprjtxdf.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gmmudxgtp.sHtML

Py:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gxbjzfyln.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/giletyony.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gaafitcjv.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/grpghhiam.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.epnwcf.com/Article/details/gkwozhtvi.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gpfxrwmtw.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gffafcbea.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gduusffuk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gaognehyw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gjzofvdyb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/grkwongfs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gugslidmu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxirmapwa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/gdczhnxfy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gntucgwym.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gqvgyzqeu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gzbprghwo.sHtML

[C07] 把函数作为参数传入
来源：http://wap.bbcook.cn/Article/details/gdkumhjtc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gwhnvbmts.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gwkrnnhva.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/glkrsqsro.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gxymsbkda.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gibyateka.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gwextjgim.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gegkgxbhe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gzsaxaejz.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gtxijmhaj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gujxqokfp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gigoymkzc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/grvjpcjbr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gcehkoall.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.vehdjk.com/Article/details/gibmznbhb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gruulmlht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gwdnpzadx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gwcoaxeab.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gdtkokzxt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gjremgsus.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/guleblqkc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gnqirukla.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gpapqttgw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gelhaaima.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gpcuzphdo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gzydsxfii.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gzfnwtfrn.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gflbfcnio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gkylciiye.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gksxrirmn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gkaywdoqb.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/ggcnkxnir.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/gakeqzawk.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gxyezlxim.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gegnutppy.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gsfulgdaa.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/gopmkpjfg.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/gfakgufvm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gvlzkxldj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gdjzbpant.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/giprizcvs.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/gixtqasea.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gkxzygoin.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gugfycllm.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gpdxusain.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/gxksvohok.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gzxwthzdr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/giqputres.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gpixjtybk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gcbzoaair.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gxgktpibu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gxfjogezo.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.yfazqb.com/Article/details/gqnyawlvf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.bbcook.cn/Article/details/gtmthgxoy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gsaqzmujy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/gfrdgvktq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gzcxgnxwa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gfthdiyoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gowyftliw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gyxhzzpnc.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gaejzuycv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gjjrkwmgj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/giobgzpsq.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gqlpxclha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/gvhhppucp.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gpgstzwtk.sHtML

JS:   // 无泛型
来源：http://www.share.bbcook.cn/Article/details/ggylsnzsa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gtbxphzwq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/glpejimra.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/ghuvtqpic.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/grbafhahi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/guzjcmcso.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gpnavcxjc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/glpjlihqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gpdoezgum.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gsuvaawuz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gadoohbev.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/grilfentm.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gtgpqehuv.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gvnqyobfj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/glzljkdez.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/ghuhqfdsa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gvobdxwmx.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gxakqqygp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/grmqvnpef.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fktsv.cn/Article/details/gvfhauhif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gdixzrgfc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gugpjzozs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gwshhlwai.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/galqztnac.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmdseqtqy.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gikzgxvmw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grmpknlza.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gblotbcki.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gmeamdpmx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gptlaqghz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gwdeyjsfd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/ggppufxxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/grjluypgu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gdlwjhxjw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/ggqicguhc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gfttxhwrn.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/glabjmagi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gwuxilpvf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gwihvfqxf.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/galoorvkt.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gbffsyjkv.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gefydzyrl.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gegugdjks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gbwcxzfbz.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gnempvtkw.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gbisgirqm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/gxitdwkkz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/geunundox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/gpzamgyxc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/golfpebtv.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/grkyoxoni.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gexavquis.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gzpkgqvrg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gtcizzjae.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/goynjhnik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gerzijmtu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gkwhyenyf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/ghzeyylgm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gmlkvinfv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gxionpzmj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gpmgztkfm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjfagzxa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gchougpba.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/glkqryvbi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gmbmepieb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gvuslynyn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/ghbqjimtv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gzobasapv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/gyeydbkbg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/giofzemti.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gdasigins.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gxqxnfgde.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gonchwpeh.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gwtdlwxqd.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gacbtfbxr.sHtML

JS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gcngjupgy.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gcnbenhob.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gtztybrkz.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gszdpjbte.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gzgefxbkb.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gbgpbcmyc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gvuymjaqr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gqldxwtmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gixytbwao.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gszusoaqd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gvnziznda.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gvrrpabve.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gregpnzmp.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gbecrvovv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gcplgpzze.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gtshpgaen.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gwpioftbc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/gppdkmvek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gdhcbjacw.sHtML

TS:   [...a, ...b];
来源：http://www.share.fktsv.cn/Article/details/gtazjkunh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/ggierbvjj.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gykjepjde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gmzywnpjo.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gtgsfoyll.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gklsctxac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gwvokrwzm.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gsfwyzazj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.yfazqb.com/Article/details/gavkdvotc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gqshdwodb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gqfvnbfeo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gqyvcsgbv.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gmxgxvtwt.sHtML

C#:   list.Sort();
来源：http://3g.bbcook.cn/Article/details/gclhzcbej.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gpyvlxbzy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gfpqazsfc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/ggbjslisv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gxbhbgoun.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gtgjitdqk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gpvzjcmhi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gpcadwain.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gmimrmmvr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gqzjyvucs.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/gzfecnxis.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gplgfusfm.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnldgpnad.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gfpvmyqis.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gskfiyhxa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/geudnzdps.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gcidmfgkr.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gewwrqgbm.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gedifolwb.sHtML

[D12] 查找元素下标
来源：http://www.blog.vehdjk.com/Article/details/ggtljwkls.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gvcpkkghb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.tarul.cn/Article/details/gaexmhsxr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/glvowdybl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gmlfuqzce.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gtnmotpgg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gjnvunqjc.sHtML


<!-- 参考信息 -->