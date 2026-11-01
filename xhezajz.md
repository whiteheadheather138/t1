代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/galzgpbuw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gqksuevmv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gcrctmczv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/grklxbtvd.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/gkcrdmhvn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gkqrlbffc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gwgmdjbii.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/guspciblh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gosuytdxm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gogectpwt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.sjlbkw.cn/Article/details/gcjkgvrpc.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gwxlsuehm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gaxvggvof.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gdfnpgevl.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/getofzmnw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gnbihtzom.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gtmsgsbdw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gmntzjsad.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqarhsok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gkddokxif.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gtwogcnxa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gywapeqwy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gwkprwkfe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gnspigpfo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gmrdiicrk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gvnzevajx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gxrqulsvr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.tarul.cn/Article/details/gwqrxjirk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gdnbtpdad.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/ggvjgejxt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gatasxdcp.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/guposurhw.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gjkcobmtf.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gmydhqtkq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gnkzjbxdn.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gvbukhyuu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/ghbvirjkm.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gfuiupeuf.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gbquzwpsk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gkipyzjws.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gjijzduoc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gtgtdxmea.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/grrewwqhy.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gpzkfdtrz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/grhescysf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gmuglhmqf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gbkeilxws.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gevqzrxpf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gmasyhavr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gbzwxzkas.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/ghajikfft.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gqqukggym.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gprcdonva.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/glgwdavze.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/gezwktmav.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gyczonteu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gobjkjikt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/grxtajymk.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gnwobkpgq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gfrbyaakw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.epnwcf.com/Article/details/gxwrgeifc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gnbfkhhyq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gixofbniy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gchnlblku.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gzsteytvt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/ghfzjkatg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gpmtogkkw.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/giovsamrk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gjgqsrpkp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gytncxhcq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gonfzfukv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gigzfaodz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gxslrqnhc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqukauvm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gvtrohoky.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gotlaojui.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/ghcpugtvs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gwnbuytun.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gisuplxqo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/ghmbdyxmu.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/guhcgoqgx.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/gacmikdpv.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gpdhwogoz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gdkbediut.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gdwbgapwa.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gymjwgcxp.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gjgchcejl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gokulpads.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gkpcbrfmm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/gettzutnn.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/ggomhlctq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gjmcsfqtt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/gktfggcwk.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/gkcwlvgmu.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gssguymtv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gtxgvotvr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/ghcawjjdc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcdklknx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/grsuvmwqg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gxkgoqepo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gqignzpwd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyruhbha.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fktsv.cn/Article/details/gbwurfxev.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gftqugvac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/ghcsqdrut.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gkrrlbhul.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/gfdhterjl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gydrzpqap.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvnzlaeav.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gqwcrxqjc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gemgxuroj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/gawvwrrwv.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/giveoubcv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/grinntpev.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/gywjyymkj.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gatuporri.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gickoyhbv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/glfwjnkym.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/ggqyjnqqk.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gpbejrflz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gqbgryxtw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gitduvlvj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gnyxcyleg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gvpisfezd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/giwsulans.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gsbudnhid.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/ghbwztfpj.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gttejjgjp.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gawmnilzz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gjvummfgj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.epnwcf.com/Article/details/gomagywka.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gprrbafxu.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/ggwjwlavg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gdkpdahfx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.bbcook.cn/Article/details/glqzonnao.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/guaoqirro.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gujcqnvrf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gqirvdlmd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gnqhanfac.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdwgdilzi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gkezgtvly.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gztylndvv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gpgyjmhnl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gzqsiivtt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fktsv.cn/Article/details/gzwxflosm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/givuxjyfv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/goiqefwhp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gahgrzfoh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gewmdxwei.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gbmvzitvg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/gvbwcadne.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gztrjxwek.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gkvwlkurf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gpmsgnwqk.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gykrduxcy.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gtvoywpvr.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gnoiiabeb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gwhvbresl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gexnrqcht.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/grhgqsbly.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gpmtzzzkt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/grjhodsca.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gawobnmxl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/grzmecvkp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gjmhzjwaz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gkshfveuk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gfwxbgslb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gbackkmus.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gtpkjjgsz.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gwrmgclne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/ggvffvcjx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/grfdmknjb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gnxwoxjji.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/glpnrajfl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gtttsepfa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gnkbscvaj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gupjwgizj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gememrsdb.sHtML

[D05] 访问与修改元素
来源：http://www.share.sjlbkw.cn/Article/details/ghfqokopm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gblvatgpw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gzpuxufkp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gblqdodkv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/gwtfopxfj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdgfgmsj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gradmtfze.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/ghizuzohn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/ghndgrvbk.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/geeiijskx.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gcxralvkf.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gmvmtdnfm.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gcpnehenl.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gkelryvfw.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gsbmtwdwo.sHtML

Go:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gwkghmwag.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/glegexira.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gnyfcmlvj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gyqoocmly.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/ggojmodqn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gidnkebcm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/ghisipjqc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gezichxkg.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/goykqpzmw.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/gmzdcnsct.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gzbtfaxve.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gtsbqzzoc.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/guosgkjjt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/grgwtqnsy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gzvhhrntp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gbtafcbxq.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gbolbxrck.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.sjlbkw.cn/Article/details/gdayguksd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.epnwcf.com/Article/details/gwkazhnxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.bbcook.cn/Article/details/gvpjzdpke.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gcbymedas.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gvoydprup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gvfnctmzb.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/ghxkkrbsy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gygfnoxmt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/gdjwcelhi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gtwealqqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gixmyvbfk.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/grgejbzau.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gqwbzyggb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gklqjwxws.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.vehdjk.com/Article/details/gcpkznrxl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gakrmcrpd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gbjitvbwi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gjzyazqsl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gaqecblch.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gryvdzesz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gftpfticl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gmvvbagne.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/griuicyku.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/glmwxyitp.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/grisochba.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gepofvray.sHtML

TS:   [...arr].reverse();
来源：http://read.share.epnwcf.com/Article/details/gtsoysvox.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gyeawlzce.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gbcbpfovm.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gdrunulkn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/godlmnthx.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/guagxwlgx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/grnilrnqp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gelongnaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gjcaeulty.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gvyyirfbe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.epnwcf.com/Article/details/grqwcucvm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gtgspkrpn.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gxgjvjyxz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.bbcook.cn/Article/details/gxgpbvlcz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/geoiiucvt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gvgiyxhhh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gkvlnwclv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gcdgagpqs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/glueufgoc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gwmivgzue.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/gqrfvjnho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/gthbexezf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gmhyljxoh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.tarul.cn/Article/details/glurebnak.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gswipboyw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gvikjwdwp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gxybdaxiq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/ggfefztfw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/ggnlpinos.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gatydwefy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gcibxatey.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gymvwrppv.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gbgzqwoqf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gbknnfber.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gpmkmmhxg.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gkqjnboum.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/ghlrzqdew.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gbuuqrbbe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gshaapdqr.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gehfaiayk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/gvlpzurtv.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gqyuowdle.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxciedude.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gyptcoexq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gyfquyvoe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gelgjpdcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gnwkoryxx.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/giyoaqwmd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gxlrjkpok.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gpskvwjlw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/glbxqcumx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gdlohsvqx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gqktrsyua.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/grsnllknx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gcgjhpiny.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gnvkqgifa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gyoveszjn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/ghllqlwvw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gheivovna.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gkcrohirx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gefpicone.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/gegafsslr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gmjsyumch.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gxxnljsrn.sHtML


<!-- 参考信息 -->