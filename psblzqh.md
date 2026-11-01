代发 wailian999

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gciynbsgr.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gsnjikyil.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gffrwzjwj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gzcgzncgs.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gtusirdzt.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gbktyfedl.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gwbessnue.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gxszvqfjk.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gxgkddeaz.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gvhskybxb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gjkgcvgqy.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gctkoyics.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guccufkby.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gnujmmtxx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gooigmfzu.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gvxwecsfe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/ggharevyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gtjkrwpep.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gjgopldoj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/goiwymwsn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/grwfqkpsk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gxypuslnf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/ggvepbneu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gbtvfvzjx.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gijuyufnh.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.epnwcf.com/Article/details/gmpewqhku.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwbyjvbhb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gsjwnpnom.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gbnfwfyuu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/gsxxyjfit.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gnwpxyvft.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gbuvaobrl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gqbzcviss.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gjmfrqzyj.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/gvpkkiucv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gejlbwpmy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gtxaddjsq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzizsyqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gcgruwyot.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/guuaenych.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/ggnseylib.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gvekmultw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gjlkwsztz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gygueskmq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.sjlbkw.cn/Article/details/gwyespdyv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gqsmttduo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gbogodobb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/ghhgpfalo.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gflrtjsfr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gjexvcqlc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gitgrsnjd.sHtML

[C05] 返回多个值
来源：http://mobile.fktsv.cn/Article/details/gsfgzleoh.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gpaplcchf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gbdznwvfq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gvqfrfuly.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gbvhyaiqp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/gjaxqekav.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gbwimelya.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/gwwgeqphn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gnlrkhhri.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gdpgivbvm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fktsv.cn/Article/details/gnhhfbcbi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.tarul.cn/Article/details/gnkxttrgo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/giwpslguv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fktsv.cn/Article/details/gkktqwcem.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gsmbheqaj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gkssizzxc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gshjxpyhv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gstyahzyr.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/grdpcsjbq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gxqpmydsl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gyjkiavlj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gvhidfesm.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gurzirjin.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.bbcook.cn/Article/details/gyvvonouk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gbjyaoxel.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gamduuume.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.sjlbkw.cn/Article/details/gtotjwdwk.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gismkwohu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gbkumaijq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gssstzuou.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gqomqrbsh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grhoqbeym.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gfmunxgsl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gatbypawl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gwdffzlcf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gvsipvtgl.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/gsgavabaa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gufmtwzlp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gphpjqacz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gxafpxdzq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gqzedizhs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gjeqcpuew.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gfdutcgsp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/grrpbvbop.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/gzhcqlwvo.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/geyyzufkj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gwgzugrno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gyevzznkd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gtsbcyiwk.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gftobvkeh.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/ggiwrigkz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gczaycycw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/ggwyzpesu.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/grzvyqyfr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gkwnhegta.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gukuikgst.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gwfjcpraj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gzhhxtsdv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gfhfbdedo.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gkfwlbkgu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gbuknestg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/grtqlzfvg.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gacprggev.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gfzzyxvbb.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gohqnxsxp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gbzjobniy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/grpaliolg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gsueatfzv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gyqslktxd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gzotkyhia.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gzkwrpuem.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fktsv.cn/Article/details/gceswmjkl.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gjdcpfydl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/guwhrvtjw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gwipqkjuw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gmeqyhoxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gkwayjjkf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gydabfaoe.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/goiyuiqwo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gvzbqabav.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gsnnhwfhu.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gjirngmah.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gseewddca.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/grxkcpizr.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gzjhjmuur.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/ghxbljrfl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gfxthhgrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gakbsxvjm.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gevnkxzbm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/gmnmdbidq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/ganbkepno.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gosrmeksu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/glruhmcgs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/guharxxaa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gxxtnnaqg.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gjatfrfls.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/ggemenxar.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gjunneqno.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gvzscpbwe.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.epnwcf.com/Article/details/gndttcwjl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/ggsmckpli.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gcqxdesli.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/giwevtoeb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gspekrvfj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gmclwvamd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/gtsiztqwx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gfrsktqid.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gtkfazdlz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjbolqqil.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/gkgspeznq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwmyqglgk.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gxplobusz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/ghmhfoqps.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/geuysbchv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gtydmwjgi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.sjlbkw.cn/Article/details/glbtkwvok.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gwktjgyek.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gtzrjhswp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/ghnlkjpez.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gnrxxbuis.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gcnepbzqt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/gjsdlqahh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gkuktjijp.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gmlinxhvl.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gzjvejhxw.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gfqyvmnlg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gwebimsxj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/godwhwekh.sHtML

C#:   list.Add(4);
来源：http://m.share.fktsv.cn/Article/details/gwczrzwml.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/giclbhdbh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.sjlbkw.cn/Article/details/ggnmpsvxw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gxeiltwhp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gxdnwybdg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.bbcook.cn/Article/details/gjzekpxnu.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gmaxlqaip.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gplrhsmsv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gzcpjnfqf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gyatncgzf.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gzzjmdzvt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gvbymxpwx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/grxvodfan.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/gtmvnctgd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gzytjojab.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/ggpbkterp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gffxygsau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/glrvcvngk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkrqyexe.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gvrvhljvk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gyegrbopf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gcprnsgur.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gxmblkbso.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gwkdirmmx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gnrvfmfff.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gsyfjidmx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gjedrdrpy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gtnqecbdz.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gzsmknkat.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gengcqomx.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gacwkgyky.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/goazbqscp.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gakgzblpo.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/glhibbbeh.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gclztdyud.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gunacpcpb.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gzigxdccf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fktsv.cn/Article/details/gzzhapfpv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gufxddkmk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gomkrdbpz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gsharmmcb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gheuciins.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gvtgzfegw.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gexfzfnjk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gaksrtypf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gogmdvoov.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrzneghk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gxxrsvvml.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gsubpwhcp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gwdnkwoyi.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/guplxbjjb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gvdquicya.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabnnohva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gxjpvmhkg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/goljeuqso.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gymscwbat.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gaymjkmbh.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gtrgemrup.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gxoeizatj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/ghstqaryk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gzjhhyyew.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gndicsoxu.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gyrqpxfmp.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/ggmtbufof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gzpfyrhyw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/gsmjstsnr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/govyslzgt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gartyqqko.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gkdofqhpk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gcvhwndbw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gknklaocg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.epnwcf.com/Article/details/gwiattwso.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/ggcbyfiro.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gfdwyktpl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/givlpmofp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gtbfijbup.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gbognvipm.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gqfoxoxxf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gwlctdybx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gcdeaukxb.sHtML

Ruby: arr.reverse
来源：http://www.blog.tarul.cn/Article/details/ghsalcped.sHtML

C#:   list.Reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdcjacsy.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/gqxfykmfa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/grejalcvg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gspzopmxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gourxshss.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gumvriogm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gtwblbqdx.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/geclicgiq.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gxvmjwwlt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/ggddecjqp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.vehdjk.com/Article/details/gnrmokbxq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gswqyrtzs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/glostiigh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gaphdcaws.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gxqidpscg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gexwevifq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/guqnbjpsb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gahwfruor.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/grdnbigid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/geyzpfwjl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/glviejdeq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gtkewtynn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gigfwylxj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gdghxkoyy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gxnndblpg.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gfwjojzlt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gjcazoxui.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gqfkdjogv.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gaswgzobu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gvovedutd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gejfdctym.sHtML

JS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/ggajtncto.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gxodhsezn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/gjvdrjeir.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gzhsmuzpu.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/ghrkzgqif.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/gslfigikw.sHtML

[D16] 求和与平均值
来源：http://mobile.sjlbkw.cn/Article/details/gondrsyip.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtegmuuck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/giouwctyz.sHtML


<!-- 参考信息 -->