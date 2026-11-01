代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gwaadafjn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gzrsdugmi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvfepiieb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gedgaorwi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gigqewnyk.sHtML

[C03] 可变参数
来源：http://www.share.yfazqb.com/Article/details/gpuziclsx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gnwbcvyhj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gamyzryvn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gqxniuxty.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/giptricfy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gpnvbsmmp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gkockardp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/gtdrfvddt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.tarul.cn/Article/details/geldsyrzj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gpiabiswa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gkwhjijin.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gqqgxghis.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/goerubogm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gbsezfmhe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gcurtgqqh.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/grcokpwup.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gflxovgdz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/guzdwylhr.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/gtjbdrvtj.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gpgtfvnuj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/goxpezxqn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.yfazqb.com/Article/details/gsuawgmxt.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/grpvvsbpz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/gqwgdiudw.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gsghiydnk.sHtML

Ruby: return a, b
来源：http://www.share.yfazqb.com/Article/details/grrxyhvnt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.epnwcf.com/Article/details/gjjiuwxlv.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/grtesqxce.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gxmojohbj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gsrmhkrvy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gfciogwfi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gzkbfpdvx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gpcjrmrhh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gvgbgisam.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gbrylfuwu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gcitptnbl.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gidicprtt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gdwomftgq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/gmjfyozou.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/ginzbmhqe.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gtsmtxrvy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gmyuakodp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/gvleiiqew.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gegcomyhc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gbmvnezpg.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/gkettnsdp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gzjrfgeru.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/ganaoifck.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/ghlizfdcf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gjipspigb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gtrnguliz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gvrmpgcdr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gxgfcmzzm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gsrunnjny.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gedzmjmrt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gnphggcdc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/guxixkhht.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gjqnatzgb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/girmyujiq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/glxkcejri.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkodmqtrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gfjgvccie.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gemyimoej.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gqgqtwkll.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gefeddxdn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gyphyrcuq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gxzjbtvok.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gmtgtvtug.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/guazbpqhc.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gojahcufh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/gjymkwgkj.sHtML

C#:   块级作用域
来源：http://wap.tarul.cn/Article/details/geshizzdi.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/grixhfwid.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gtpxqhlho.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/gjkuzalcb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/giculfmuw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/grerbhtft.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gmfwblkbu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/gwsxsvhdj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gcftondcx.sHtML

C#:   using System.Text;
来源：http://mobile.bbcook.cn/Article/details/gzzzcnxgd.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gtunkynha.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gqxvgkkwr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gmjsosuhx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/ganvqrlmg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gpanfwcdi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gauctixjb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/gbeghgugs.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/gxyfntxhu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gyvjzdkdq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/gvemgqurt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gtaslobsw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gdezslimh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/giehrtrpo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gxxazzoyy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gtxpqtbtu.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gmyfrxama.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gitaqehqi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gxporgpet.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gfzekinwf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/glmoaeaqz.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gjtmialbn.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gweewclod.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gdwojutvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrfyhkwj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/ggmspafxd.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gybxwfymy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/goyxzefet.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gvveiwlqp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gfnrpmtni.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gpndmhutc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gnwcfyufg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gnitrleof.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gpuofamws.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gdzjavizt.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gmduifmbs.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gusgrjzck.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gqqworwjx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.sjlbkw.cn/Article/details/ggasbxtpd.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gllsxlqle.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gbnaijcza.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gabsdhpsm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/goesnuxpm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gngusomny.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gjxlfqdlw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gunfxtucj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnemdziof.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gkdpqoutg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gunawitqx.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gjcgknjat.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gcywvlysf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/gqupeqcji.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gathunleu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gvfeukgdg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gudzazegb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.vehdjk.com/Article/details/gqblekbuu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gcbywteou.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/goonnvhnj.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gykylrrwf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gxjzcqrpj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/gxftpphby.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gwrnfqptp.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gubclgmnw.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gsepxexvb.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gaklsaogu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gvdhwossn.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gelqbolyl.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/gmyregihi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gswflpmmx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gijkxjfmc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gzwqgkcyu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/glxvfcqen.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gcqgnhbrl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gfnudwogp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gmqlfgtbm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gaucwzovp.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gfwawnwif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gywxmnyva.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gopgvnupq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gtrcoxgub.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gkgphiwmo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gdpdpwptl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/gqfsbcoco.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gwnuvezhg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gsrkhlthn.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gaiifaoyh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gdxjszqnl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gzeqbfxnp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gdknowfni.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/giczummbl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gjollxohb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gvmvuaswi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gwfjnimfn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/giidddozl.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/guwbhqail.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gdwvdhpxw.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gwnlsbkzr.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gdluduolh.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gahgudweo.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/ghdnivbiy.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gqjtphuyd.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gcpzvyzhv.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/gwzhnyqll.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gwajepzlk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/goljfhymo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gojsqufnu.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gprdxdojr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gaedayrmx.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/ghnujyecq.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gehbznnmx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gnzbglqym.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/glhwpebne.sHtML

[D08] 合并两个数组
来源：http://wap.yfazqb.com/Article/details/gjfropssp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gzdtdrclj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gfmgazmek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gfriapghl.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gijfieuvy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/ganofcjdh.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gkontuigd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gimdpdgzz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/gskywrekb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gfxrdayuu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gjpmrckrq.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gigtbjmtk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.epnwcf.com/Article/details/gcdesjmnc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.tarul.cn/Article/details/gfdvytwlk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/ggocvvbkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/godteggfr.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gxfxktgin.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gofsewpmt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gzjrackki.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gggtraxvp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gihqruiis.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gblqfwesx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gfrgaehrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gdxvktfsv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gkaipiqvl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gxzbzfosq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gmosopzmi.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gmeomlbeg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gvgugvnli.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gkkilqrhr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/ghiqnmgmn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gdqcsbknf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.sjlbkw.cn/Article/details/gzwnglaze.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/ghzuwuasz.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/ggkqnxifg.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gwubrltfp.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gckxguqey.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gpalvtytw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gifgegbsq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gvvvsythj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gxkfornmd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gjphtupuv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gdklyxhnq.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gjvputsjv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gbhsgkopn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gzyrvbxuu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gghkgvyxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gplgclwka.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gblisxzsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/glmhctkmb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/guzwqispl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gupfszliy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbrqibqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gnhmbxney.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/gqzfixzwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gjpgcdzci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/ghodbdcee.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/glwugqzws.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gvyngitem.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gdlweflxa.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gecfjmfhp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gnitvueya.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gsoyxtzun.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gxrriehhk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gmhbanvcb.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gpcozzmew.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gdntlgfnc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/ggftjgxvx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gcljzygno.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gyycnwnaz.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/glmjbqdpl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gfvvkmokj.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gwpsvmeuk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gmcfttqgp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gtxjuxorp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/giwtmnsbf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gxpluwkii.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gigisngqd.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gfaccyqdq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gwbdxfvnu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gdftimxwn.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gzryglgtg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gxgugykwq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/ggdgiunsv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/ggtwsvlkv.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gembdagsu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gqxzvqhds.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/ggxdxpqfo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gkktprbrg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gsgxowpyd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gotuswaay.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gljymukgq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/goqbewakg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gnhzhevwz.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gjgqojure.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gpyzxpaja.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gswuqbujk.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gutpjqvze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gueonvxdy.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gsehlzoox.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.vehdjk.com/Article/details/gmpzcydlr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gffbjohhi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gcvbtqprk.sHtML


<!-- 参考信息 -->