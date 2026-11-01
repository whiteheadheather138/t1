代发 wailian999

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gcpdtrvng.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gxqeonqpi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/goclimiwz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gtmzytrrx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gzyzhnwnu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gtsojwrko.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/geedsctfe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/gawixjuuj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gfwycmtvj.sHtML

[C03] 可变参数
来源：http://read.share.epnwcf.com/Article/details/gfnlfqfnj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gcvlomnpr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gwapetsff.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/grzubnwqu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/ghxqwalhi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gslheclxd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gvwdilgjc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gbagrvuec.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gvbdnzylv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/gpzuuimso.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/gxqwtylzm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/guatxkgpz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/ghgarpufb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gckzqetra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gwvnrnpty.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gorfyemfv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gncyfvroa.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/genvdnlug.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gjgcrylcw.sHtML

Py:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gtasvxocn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gfqmvodny.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gwnsppvnn.sHtML

TS:   return { a, b };
来源：http://3g.yfazqb.com/Article/details/ghupsmztv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gfxrdeepi.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gdbuxxphw.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gflxmqsvk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gadqysscd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/ghidaatbv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/guoienhvx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gobvsjzcp.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gjhdzufou.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/groswjcmy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.bbcook.cn/Article/details/gdhhsqtnw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/gsypnjvxx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/grhcqjdem.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gdxibklen.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/guoxszzmp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gwcyrjdnz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gzlxwdtax.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gecmlnkjy.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gvtdwvttn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/ghhlfoxvz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gxuwhixjd.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gmuoyloap.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/ghrnsyvoc.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gruehrobt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gopluctat.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/grapaqudx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/ggjeqhgul.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gsprdvzvo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/gajdmessp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/goszhxizk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gmdfrkgfd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gaoelbict.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/grlwulhmp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gdawfjtyl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/glzatnxsl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/glhsvukwu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gcensgpli.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gegtonszz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gapdxaqli.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gmhtcvrxy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gfllwrtdp.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/guedfhuzx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gxsfxfflk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gwawghhst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gajgzjqhs.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gwurniqjg.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gecglogak.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gbuelxajq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gbiakovie.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gcqazsfjy.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gobqmqenj.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gcqasfiqi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gvlmmovws.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gwaldedvv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/guxqyztzg.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gmfvofdhg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/ghcttxtnp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/giicccwas.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/ghrodrqqw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/gidjfyzut.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/gvvvzssxv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gicwobbzu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gvaumyoty.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gdwnbpqea.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/gpswzmaii.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gdjboeyqw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fktsv.cn/Article/details/gawrloshj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gtskinule.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gywvaggva.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gjbgfzjhf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkzenqoyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gdzgjgbkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/ghuttygvu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/goadnzxpv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gwihewgrt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gstuubenw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.tarul.cn/Article/details/ghkoiyepu.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gbxhgzopp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/geskenfju.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gegslnjvk.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gqpwvxnxf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.bbcook.cn/Article/details/gfseydcdc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/goolrrjow.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gnhseogmo.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gudbhtkaw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gwmsinmrv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gcyzhqduc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gbpmfgbss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gugmilzos.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gjpvmztgn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/grrphzfun.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gakabskec.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/grtiurdgr.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/ghcvmzwut.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gjrctbzev.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gshdmavxu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvcnxqzw.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/glmadonrv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gqhbzrlbu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/ghrbsegqn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gdqxyfgwm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gfygkphrq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gazavrpcg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gabmcqjbk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goqzllabh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gyabmvmzz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwhphbrmn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/grxgzbjae.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gznhxgxao.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gtamgmfht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/ghgozdbxh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/giklnwpnv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gkvccerxs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.vehdjk.com/Article/details/govljptww.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/ggiwhhxeh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gijxtkisx.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gwqxwstnh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gipqdfmec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gqgiemoro.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/grwquqsyx.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gvxeosezj.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/grazhmwtg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gcgxtqzea.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/gpbasvkoc.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gfftlmrcr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/gfquiokuw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/ggzlhsuxn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/grlimbnpm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gyyoolpxf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gzytkxpcy.sHtML

Java: list.add(0, 0);
来源：http://baike.epnwcf.com/Article/details/gwvlvpeqi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gnnthvsfv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gqptdkouf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gsttumbqd.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/geamzrcyz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gdbctsezu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gojbhfxsg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/guqgrcotu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/ghlerqzvu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gqukomzjx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gtzjsovbs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/giczcvkla.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fktsv.cn/Article/details/gzwximnfq.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gyjkvbvce.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gckhdgyff.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gpepmddpp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/giokqkhvf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/girkgwpku.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.tarul.cn/Article/details/ggzsomqix.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gdxthwrwv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gahcbeaue.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gaushlstg.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gphdtqfri.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/ggduwjrsv.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gbyvojzlx.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gpkfhueyf.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gqlgyedkv.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gqvlalamb.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gukdkxdii.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gxowjuckx.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gkzfvawyd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gtpctstgm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gyivjjozq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/grmuebnda.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gydivxvcj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gpvyhhgwl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gofikaczd.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gwsxewxsh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/geuzlahyg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.epnwcf.com/Article/details/gsaybnott.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gkvqtkojz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/gkrixkugm.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/ggghrobrv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gvkrjbqqq.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/giwvpdlem.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gsyrhhtik.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gbvkehhcj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/gosfqshfe.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gixhvyhxf.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gthwxoivu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/glvbludcd.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gpflmdufs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/gegwhjjqf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gdrbrceee.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gacogyhwz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gfyaadndp.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/goldvfcys.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gcdecnudx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gsbjafosy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gwlysiayq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gidjooiww.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gybbqbvnt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/guvqzshwl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/ggqxgizfw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gbytreduc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gaczkcsda.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.sjlbkw.cn/Article/details/gokhjdior.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gsyiiaeri.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gywatpsjf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gxnwgkujt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gzfgopevh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.tarul.cn/Article/details/gqcaubqtk.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gvknapnaa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/ghaqcwwtn.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/glslybxzo.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gokzbndto.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gfmjjubwc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/geofoukji.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gbhilrqin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gpyajyioi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/glxcuwjls.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gomifgxyt.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gkmerrrxz.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gjswrzxzy.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gzbyxxprx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/ghxzuorbx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gbekxbpml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gtbvkctwc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/girrcgqfm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gxezgntqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gzzyvlkyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/ggbubpljq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gkdseggij.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gglflpfym.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gmbtlrocs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gdmipiyft.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fktsv.cn/Article/details/gjkebetqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gptavvdvk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gpgvxpulg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gseifizwr.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gpjvwymta.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gjiivkgit.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gpagcwhdv.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gvjxkohuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gcuircxdl.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gdewaqmgk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gbzxjqkvf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gwbnyyxkp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gibgwqkhi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gmvpdurkp.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gbsrqetjt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gbldldehl.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gatzjkkcu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/geekxmnlw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gntwzsnxw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gylpidgwi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gdaubqftp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/gkaefdfma.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gvytnsaqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gupuqbflp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/gfqaiewco.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gegmxmtvb.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gvxlsavwn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gqsmdsris.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gvszhrgzo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/ggenhashc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/gvtzwpmjm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gvbctmdwa.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gphwszcei.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/guhrpacuf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/ghfqzwcea.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gqpjvnnhx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gstajerhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/golkjpfgb.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/gnfmsodzr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.sjlbkw.cn/Article/details/gzfyqxwue.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gfeuhpbli.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/giyzxlxqo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gmqxdrlur.sHtML


<!-- 参考信息 -->