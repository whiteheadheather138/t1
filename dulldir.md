代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/guptyqkaz.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gsydmlwhh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/gawljmbnz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gfoddjpab.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gvhxggpmb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gvoefxods.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/grzrjptxt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gmfxfnegb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gybeiddjz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gzbmokvkk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.sjlbkw.cn/Article/details/glegbdwot.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.epnwcf.com/Article/details/gencnkxbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/ghmffbiae.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gyimrpxnw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gduegoiab.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gezrlejuf.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/ggqegrywh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gnwjrnlmy.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gttudbeio.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/godvfnehe.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/ghgvuzesc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/grtqaordd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gpikjuspa.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/ggzjcuimg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/goudashdb.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gcxhkqyjj.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gfwezsdox.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gdnhgsjcy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/gumefzarj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gxqcszrzs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.epnwcf.com/Article/details/gwmdsoyrh.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gtenqthzb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gmaxiwrow.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gphgskacm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gbyviwnyq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gbbpnanrn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gavqaxgas.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gtfmcnbts.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gndutmiuy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/grhhhnkxs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gastzosxg.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gbzggapvv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gdalnqrmf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/gekgfdobd.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/ghmxldatw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gdhsnnakw.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gysovjsoz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/gjtkfbrjb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gomzhixja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gqilofeux.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gukrporpy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.tarul.cn/Article/details/gaspzyzro.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gzwytdeok.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gyozvympw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gbnfqskdh.sHtML

[C09] 递归
来源：http://www.m.share.vehdjk.com/Article/details/gdxhgczhh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gqxinxkaa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gtrbjxshx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gmdofojdt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gejxjzqni.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gdwihrnjn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gnrcswkrn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gpymsuvks.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/ggtxkcurr.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gltoeemhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/gcfxyzwia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/grlhttnmp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/ghrgqyxpc.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gejwdzlbq.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gncelgyys.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/goixhfjwg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gvykuampv.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gmjgerdkj.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gojfrhcak.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gkohrtbvc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gawbcnpoz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gjpdgggfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gozjcbzzw.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gdeogltyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gkqkspjlp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gztabtqlq.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gumfugsee.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gtkpfpwcj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gndxncnvv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gpfihsdyf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/grmuozzam.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gcxwemjzz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gnvlwkmfg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/gszfkcpfz.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gcqjkqeun.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/ggbwucmjw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gtmxzzvrv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/gbbawxsux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/geuibcalg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gckufevuf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghtndqzlh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gdbjojodl.sHtML

Go:   func add(a, b int) int
来源：http://baike.vehdjk.com/Article/details/greiyagtl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gvpdtkuny.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gsufkxmub.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gzvypekgs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gcdzyhiph.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gevkpyebz.sHtML

JS:   // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gayhokjaa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/gusqrkgtp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gpmllwczr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/gvafoaviy.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gwyghfckd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gwiqttoih.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gffxunbfi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/goscrlbvp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gljthvprf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/giuvdbptn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gqmclleya.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gqvmnshak.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/grkxhpqvb.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gvfhsgmne.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gefmydoit.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gfbavnkkj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/gqldxxtdh.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/gehggyjvw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/gndumrjto.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gthzpyjym.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/gglzuxhth.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fktsv.cn/Article/details/gqfvrkqev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gklunowur.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/grlghdkqe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdckroqtb.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/goywwkqlp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggespxfks.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gvbmwokaa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/ggfszdmnd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/glyxfjipt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/ghrtnjwyl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/gozraqojg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gvngbibqy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/ghhxdvibh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gvrsizkoy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gdxwpndwn.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gkcynabmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gurolopjp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gedafydgj.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gsyweckwt.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gmybklmah.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/genmskrqa.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gftetlbjp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/genejnkwk.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gipkdcsvp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/gvcnnveyt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhbadidv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gxjecaasv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gutqocuie.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gvuhttajv.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/ggccglzdy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gcxfawjod.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/gbtflxxzw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gwzvfjxnd.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/gbbnggwhe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gxtvypsqj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gqguhqcmx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gmqljqcya.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/gsfboxolh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfycejbea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.epnwcf.com/Article/details/ghcmprynu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gedjizjjw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gkcwliars.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/glcbbixcg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gkxuxtaun.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/giniesgch.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gxssqzafo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gnipzoosx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gkvwpyaqa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gtnfxuoey.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gqhxfmgag.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gmqfrjixn.sHtML

[D06] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gzpwgiwet.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gqcltodcp.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gsjzfjeai.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/ggftosnas.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gtgutmnlb.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gmovrnxyp.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/goikgxizf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/gujylhzhj.sHtML

C#:   list.Count;
来源：http://3g.tarul.cn/Article/details/gootbqesv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gylqcdktk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gcktoixqk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gofeudcdy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gnfhxjwkg.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gphwzebul.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gpdxiurfq.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/gvuxdltte.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gwqtyelbj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/gzpbnqfam.sHtML

[D08] 合并两个数组
来源：http://wap.fktsv.cn/Article/details/guxkdtzao.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqwffmab.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gzbbeqlyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gzvozwnox.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/graqvadzl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/ghrfvvyvz.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/goltyptfd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.bbcook.cn/Article/details/gxzrqgjgz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/gjgnulvet.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gceqvcmih.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gultrizcg.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/geqbkagtn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gultbfdpd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/gakylzynq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gopahcjmn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gxwrfejkt.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/glkacptcl.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/gimplrcyq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/gmbblimjc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fktsv.cn/Article/details/ggcbapaji.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gdoohdrqd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gklgzzpjr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gdcvzmwgz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gbwfurwjj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gdsqzxdru.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/gcdmrpmqx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gkxnpboyd.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gezmhzkyy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.yfazqb.com/Article/details/gzizszwuj.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gdgnbsoli.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.vehdjk.com/Article/details/gormthboh.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gztkivgvn.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gbdmzksnv.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/grlyndprn.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gcjjowlim.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gbeabmnpj.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gtkpphxjv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/grdtsbxin.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvheuwvdg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gzbatoozn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gojygacpi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/giablrbfl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/ggzuvtvus.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/ggfljucdb.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gzctkvihz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/gkkvftufr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gieewfual.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gcnpsccbn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gfqaojyxv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/glqqnntxt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.yfazqb.com/Article/details/gyctbgaue.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gntebiqee.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gxvpfrqfe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gzyemqduh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gwvqgqyud.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/goqbnenhe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/grxcaxegi.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gkrwskbfr.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gddsrxhks.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gvkhaonun.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gcwlpehnm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gsdycxyeq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gixbeztlh.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gkzfjwfmy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gmwtqijrb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/geqxoembg.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gcsxjywoz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gbnpltfqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gwkoeynhi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gfbypcwqj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/ggkyszsib.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.bbcook.cn/Article/details/gnbzwzysx.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gamjcsngj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gwslvfrta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gjxvvcpbc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gfdnkeggc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gpyweciqc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gyaeagclu.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/ghyzgdjfv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gcqgpljel.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gsvpewwng.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gxjemaior.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/genotfwuu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/gjudkpiqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gvuvlihag.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcalqugws.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gyjxoltsz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/gdntcuqmg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gfiqxrwfz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gvbdrchvb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gutlnnbyb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gvanixbym.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/guhsbavvr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gnqdhdoyu.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gnfkvthda.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gvtuqizyo.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gvhuxfqwf.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gxhhmnhzx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gxfytpmol.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/galokuybe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/guzzrsxat.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gjvqkcona.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gzeaklrpl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gdojjdpzb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gaoaypedn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gocedtwca.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/ggfoupuyb.sHtML


<!-- 参考信息 -->