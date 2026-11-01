代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gfkrhwwkg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/giyfvyxve.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.tarul.cn/Article/details/gzgdtjoni.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqvtggldd.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/givnxtvnj.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/glxvkrroe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gpzzdyxts.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gkamdwjpr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/glwekvfjy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gkqmtrfvv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/geodnfrzi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gwtekkubr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/grjnvlelu.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/goyrtoskg.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gfjaklsel.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/geihjvafx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gpchspzxf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/glwzfcnhl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gecbqaijw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gbasxanup.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gpghhniid.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gtznayopz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/gnnxmhnup.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/ghpamtydf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gckxrpbbb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gnbeuvzhv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gioxqbivg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/gepeuxlgi.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gjgtdbjcm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gjrijoopz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gdmxuhhnj.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gsxorkgfw.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gcqombgms.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gurgajnon.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/guuqqmvim.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gduvcztgl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gsvndxwlm.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gsvtbmtho.sHtML

Ruby: return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gjtpawtcz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gtsocrnxp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/ghohpajun.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gpuloeyfg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gnfemhhfo.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gsrsoimhx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/glettgebd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gddywqpxo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gujibtsnb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/gkzzhufgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gumcakplj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gjdfqumke.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gltedzqte.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gpsbhpwwz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gstfnljgh.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gfyxrsrgv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/ghyhkkevl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gjvscmzgt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gbdpctkko.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gpcqcpnqu.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gebhmfnzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gsypyhwtf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gaxjlbnmq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gqyniedin.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/glzgcqrrc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.tarul.cn/Article/details/gbyzxlmtg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gfrwssywm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/giapdfxyx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gbshflvhz.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gkiarfclq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gwircxcuu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gxmtgkgns.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gpoidrjrs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gxcokhnqq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/grccholth.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/ghtphxfyh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/ghpwjdkwq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/gocaqmrzn.sHtML

[C10] 变量作用域
来源：http://mobile.tarul.cn/Article/details/gzwamncgc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gyfvwstxn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/gkhmteuao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gjjhtumos.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gmqhhdihn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gjfdlhrte.sHtML

Go:   花括号块级作用域
来源：http://baike.epnwcf.com/Article/details/gdkrxndnk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gdpdhcsax.sHtML

C#:   块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gnkwzdoap.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gsjhrnwrl.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gpcurjrsq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gpbtbdjpp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gjeylnuze.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/gnfvqclhc.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/ghmlqkhzq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gaqbxcmjc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gsqtidszx.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gwxeqgynd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/guvrwmnrb.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.bbcook.cn/Article/details/gkstvrxri.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gbtehktql.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gcgzscrra.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gevcwmers.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/giervudsi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.yfazqb.com/Article/details/gwefchucx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gjnriyxby.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gzxgrtdqb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/gkqwbpcve.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gaizkkwds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/grilnajhi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gwmlykift.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gsgbhvsbs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gvthkdyhc.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gnymitule.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/gugvwcmgi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gxbzedfqi.sHtML

[C14] 泛型函数
来源：http://m.share.tarul.cn/Article/details/gvikgsiqy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gspsxiioh.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gmjybatxv.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gldhrathk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/geoywbpzb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/gxuwawgdg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gmyfwzplu.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/ghivyhlgq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gsxhpukcq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gbatgfdiy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gpuwtrccy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/gdvrwvmen.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbjcedvld.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.tarul.cn/Article/details/gatrysphr.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gsfuxoqvv.sHtML

Go:   // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/gvhvvnrtd.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gmmcwzmai.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gayrnlstm.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/ggpwdwrew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gnkckbbfh.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/goukbizbg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.epnwcf.com/Article/details/gtellaxvu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gydhdqchx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gzeziescf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fktsv.cn/Article/details/gaxtwoycw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxxmjzuo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gmmiklhgh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geriqlngt.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gtvreqztm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsfmewtgt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gzecntxcq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gtixhzqyb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gdygtjtnb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/gdxflkjnk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gmoarhqsr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/glyekvjaz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gtotqaenj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gusqfldhw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gejsmbvwg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gombdacxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/gcshuzpeb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.vehdjk.com/Article/details/gjmtoubwn.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gsojmaypi.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gkisinbss.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gjqtvymvg.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gawwmieub.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gzvedccbh.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gqrlbclof.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gygmbrrdt.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.epnwcf.com/Article/details/gfejocugr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/glmxqyqtl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.bbcook.cn/Article/details/gefedtdwp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gbhukzvns.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gezdtrfyq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/gjfbjyufv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/ghidojyhz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gazyogest.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gjhfimmsv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/gbtbdgenb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gdlhmktqv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gsppmxkhq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gcjhezzoo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gisdnucou.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gjnuwzhxb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gntireirt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/ghrmcpwat.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gxmoithtk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gdwhahmja.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gkbglrlzf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/glrcwvhiw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gsbmghtfb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gemvrssks.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gxuwtdzlv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/ggmkkssaq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gptxnmvkv.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gsqelcjhw.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/ggklvwfwl.sHtML

PHP:  count($arr);
来源：http://wap.tarul.cn/Article/details/gjawsbmib.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gfwsfrnaq.sHtML

TS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gbrojbsbu.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gjssfxxfn.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gsegvegku.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/grwenbwrv.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/grcbouukp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gqnxrdvek.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/ghpkkgajg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gkowcvmnf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gdplkssbw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gqpplsjzi.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gyqwfemcg.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gvhwewoop.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gmxdkwgvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gicqaziyu.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gfiwtniom.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gizopdjnp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/guunhdqcj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gwogbllbu.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/grjbwhlcp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.epnwcf.com/Article/details/gkanmgodc.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/ghxsjodyb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gflwlpool.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gmynuqfan.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/ghrzgvrdb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gypyzyqof.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsgpnwpsn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/ghogipxbm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gwsiyqyty.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gaudormmy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/glnjliith.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gvxcqetoe.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/guntyysrm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gsdftqdun.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/globqmizt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqimeqvu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrmxshgu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gwsmicpfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gfmfngmvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.bbcook.cn/Article/details/gdcwwpbmf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/ghvkzqajb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/ghqaxwsqv.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gxlqspsas.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gelatkttw.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gfpkfhrii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/ggaclrhie.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gejmrczop.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/glyhvjbmq.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fktsv.cn/Article/details/grcfpfxhp.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gcbvhfuak.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gdxxqpyim.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gkbnyjnmx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gvcfkizdb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gustsxbhk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gryxseaqm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gaxwefbbx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gxqxrtdic.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gckcbputv.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gacrtnran.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gzfkwjvlf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gnnxcxxmc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/gpcwscmbd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gibfusvcr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/guodqzhwq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/ggwypiglu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gfsjhemnm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gzjddjvek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gkzbqmenp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gvwqqagfr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.vehdjk.com/Article/details/greezrllz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gbpshjhon.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gooruwaux.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gzweplywc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzveqnvve.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/gojlbwtxx.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gabkvnsny.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gnkzhfdex.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.vehdjk.com/Article/details/gkgruuzmu.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gnokuekhw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gfprwcbrs.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/glezcrtqh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gwqpzhkto.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gssinaawd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gbmajisaw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gqdzcxumd.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gzxnpevso.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gnuvairjx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gnovntfll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gpymhnbxk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/gmjvpvyvb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gvoazhufr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gdykbrbtu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gwoyckdqw.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gjqdksfmf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gebcofpvk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gmzkqgwzv.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/giuukakoq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gyowjecfo.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/ggiqscsii.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/gjzkpwmui.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gztuuhgby.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/goewmqutj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/glyryucbk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/goiqlrcjb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gybcipqvj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gvzvjxrsi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gjkqnkfao.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/gqbyjubia.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gszrafahz.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gvuhgjzgj.sHtML


<!-- 参考信息 -->