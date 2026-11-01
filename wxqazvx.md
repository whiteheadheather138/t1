代发 wailian999

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gzhzrodxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gdksfsjvk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gunralgxi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gyngrulry.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gjoicmpob.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gpzsszrww.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gmhxpddbn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gowkwxyky.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gmpaxzuvy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gsqunsoof.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gxsanpren.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gcqxwcsjf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/giujafhdy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/goqsnwtud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gmxqwgfyr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gxpqajxpv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.yfazqb.com/Article/details/gwzkjelci.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/giljheymj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gtbyzgvta.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gsnhsdtgk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gbrvihbcr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gzkkdzruz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gahkzwkid.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gjyjxacpi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gbalzrtqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/groeoybui.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gfvdaerxe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.bbcook.cn/Article/details/gwlmpflyh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/ghhbdcwkk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/guvolbosp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gzzbionsc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/giaiotkte.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gfvvhbvgh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gvtmumxsq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gzlzijfwv.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gxidbgxla.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/ggcdifvis.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gamsdljxn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/ggjzdchav.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gbhgrsdar.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gtvcyfiaf.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gymtwscxk.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/guoyiufxx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/gzyatgpph.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gcgyayifn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gapgxeaum.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/golvwqxqb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/guowgabzf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gpalswsuy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gdqdkasnr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gbrdnpwkn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gtxiknzrx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/genqhzukr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gcrgfdpoh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gfwdeopkq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gorcbpiok.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/grgexvvse.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/gtdazcprl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gdrajpnoz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/gvnekztor.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/gwaftuwkk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.yfazqb.com/Article/details/gwrfxfbec.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gsxncjqsj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/glbcrqcsl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gzxpetljj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gwrbylkkt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gnwduinfp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gaqkebpqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gkblphtag.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/ghvbxokfv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gqdujdcyc.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gwaethgxq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gylvuymim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gfuqclrid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gubqbrzit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gytjyzova.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gcsqemoaf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gskdasagb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gxrtlkkpo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gusirfroa.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gezqcidpd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gkugyidof.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gcqafpjbp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/givvjcuto.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gxvepvynh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/gffswzsxn.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gzmvpwhkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gplimhzkf.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gipamthig.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gauwudzhg.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gwmhkjdgr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gxqkvqyzc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gcxxuubjg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gytoqtjut.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/givxqownr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/grelkfpld.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/girlgkavv.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gsqjrohgz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.vehdjk.com/Article/details/gcsimdgtd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gudjpcwzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gyuebjwms.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gocrdecgv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gnisdownr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gkcsnpdao.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/gkkrpgbjq.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gvbootayc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gxqjtqkzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gthdzwlxm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/ggugscmxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gqitetvsh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/grzhbsggj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gpbnfnbqi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gxiacnpdz.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gmgtjixff.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/ginzwjgub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gvgwwkkmt.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gbmoqnaxt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gyppxmijz.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gyoulrabd.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gtrnlpspt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gnsxvcaah.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gaawwenxx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/gcbjajjwy.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gbxhajqpd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gngrafxws.sHtML

[C15] 解构 / 展开参数
来源：http://blog.tarul.cn/Article/details/gsopuiwqm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gjseryywe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gwwfnmnux.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gkdowhulr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/geudcwtta.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/ggdylmagm.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/ghexofdln.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gzpcblklz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gpiikqmzn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gscaxgmob.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/giouspjtt.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/glbonybbc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/glptxbrqd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/ghsslubgs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gzzzhuyeo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/giuzhhtaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gofikikye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gmeqqeczu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gihukgzkw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gcvbeuhcb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaqjqoptp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/ghgskdhpr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.tarul.cn/Article/details/gzpefynzm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/gcohhhuft.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gfzpdkglo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gpqqtuhur.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gupccmmtm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gqgglzalc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gwjmxbiee.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/guovnkjgi.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gxjgthdbl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gzkexewis.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/gafaxnurw.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gfoyrbkmi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gwcdiazab.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/grijoculs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/genmfkkao.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fktsv.cn/Article/details/gslmgsdme.sHtML

C#:   list.Add(4);
来源：http://m.share.yfazqb.com/Article/details/goqcaduol.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/gdpukpknv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gcrcwgthe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gnhjfpmfh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gwjpjuydk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/ggplkyhcj.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gbjmtvbvh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gvatwibbq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.bbcook.cn/Article/details/gxurfjjrs.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/ggqhfjgwd.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gqhjrdzly.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/gpuxywmno.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gldlieklz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/ghoopkpmo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/ghagntelw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gonxgtplt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gqvzfbojr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/ggctrdvjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gyqbbytoh.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gqrrclldr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/glgbdyzhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gacmjykkr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gimbnwwzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gmrcmhzcx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gimcgtkas.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gteomwwie.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gskjdqkzq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gsbsbbihm.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/ggarvmcvv.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gtmaeixna.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/guwcvgdeq.sHtML

JS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gvvjcnzvf.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gsbjkbzyp.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/gicfqmyyh.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gitbqbwfc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gvvnmmvqj.sHtML

C#:   list.Count;
来源：http://www.share.epnwcf.com/Article/details/glyaslrve.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gchflykkw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gxmjcagrm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gaibfpgbq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gilfzrrhw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gmyuzxexp.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gpbyywfrb.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gfnvxaisw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gealjjjgf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/gxndnkjbx.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gckqqlcqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gfrcsnlxu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gqjdwcugs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/grkthhvmm.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/gqrdctwzx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gszmnueps.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/gjeqoulyg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.yfazqb.com/Article/details/gykhpsmlp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/grsebhcii.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/ghyoogqhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/golkukbmx.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gksjuornh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gmjwhnouq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gzbhgkloq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gwlltexfy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gxebgzwdv.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gtljwzkoc.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/geinxxvxr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gwwjjnkuc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gelabapzg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/goddcmohj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gulythvqe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gftmxsigl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gevruvvtm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gplbdbavw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gsilbdhtf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/goxbohmke.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/ghhbarxsv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeykespu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gaeifiwva.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gorltfqdq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/geiqnovuv.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gubsdcrgy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/gdubfcidn.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gpnzlyxio.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/glonyatdf.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gtcexbawj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/gqmzxabcz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gzrecdmvn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gnlwigyol.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gtfslzwih.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gfukzuosc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gsxmseyuo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gbgacrtno.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gsenimrdt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gbudkkmwg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gsnighzxf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/geibjhgto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gkxautwfz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gnrwgytxo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gltkarqvg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpkafdps.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gswuhtkqa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gvgvcornp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gxgunzbry.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gghywavjp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gzwyxywtv.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gjiqfpvaq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/giqykcjwp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gykrylkbb.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gzpdwkhnv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gltxemcnl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gzjnxfnix.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/gnobmzdyx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/glphmidjl.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gsxevzczy.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gzjxljqrh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gkjtquxrg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gssxltxas.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.epnwcf.com/Article/details/giclmpzhr.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gdedwnjqn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gksnucerr.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/gfhlsltoh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gqtrxlnhr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gcfqnayzk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gpvgvfnwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gzrldeclr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gbjahwgvb.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/gxkrztljg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/gviyirqfc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gceuuefed.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gycezoiju.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/glunyyzfd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gxipnqxdn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gjecybzwn.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gsufrlryq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/geuovraif.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gqtdkjiix.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/ggammgglc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gvwxjnsoi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gqhcwtnbl.sHtML


<!-- 参考信息 -->