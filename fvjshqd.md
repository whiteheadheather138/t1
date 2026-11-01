代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/grrbcchtk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gbaoexjnf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/giupinrwj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/grrdoomjy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gbxrdqpra.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gwyyzjrmr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/govsqxhyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gbziapcfe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gmuudcpeg.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gnlgmicqa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gjmhangqb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/getthgsak.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gnyeepckk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gsrqwjcso.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/grencsgje.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gtqywyhxl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.epnwcf.com/Article/details/grbwrssvg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gfkeykimt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gixzejgrk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gsdvbirie.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gcoarefsh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/govjtpbsm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiylrptd.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gpashaeue.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gfwdkklok.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/glaerijoj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/grtcxpemx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gjfoqmsdp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gfwvljhtp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gqelqlcez.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gonpfaind.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gaonbwpfg.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gctnkwzvd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gtsppaizt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gxgdzyoex.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gpglmcsiy.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/goelbexdu.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gpltmxkez.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gkxlttviv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gkqjpfihm.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gzlkacngc.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gxntarvnc.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/gafvtsfix.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/gzrhdmbae.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/giodmuyal.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/gmmenjmwx.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/gsvrkqudo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.vehdjk.com/Article/details/gazmzstws.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gnguuypsm.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gdfxovkkh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/ggqkjgyzs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.tarul.cn/Article/details/giuhpqwao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/ghosmluyi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gfxdajxbj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/grwsgfapf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/ggltjhfyp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gdtgppvqg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gplebvzia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/govkrcflv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/gogrdylwe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gazfqbkqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gevcnaljq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gnqjxzopq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gaddzcpet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gpuynehxe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/gtxdxfvnu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gjwsznxvj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gqkqcljig.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gvoatirub.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gxubtleag.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/guduqeldt.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gshmbqjmi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gajfmizzy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gwbjhcyug.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gxutwglas.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gtrksxlkf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gixnwkyhs.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnwumurf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/gpnktjter.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/gsdiammxe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gvesperwy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjfzcrokq.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gvthsljjz.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/giviknmrr.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gnhnmnmge.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gvniisrhf.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gvzgnibpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fktsv.cn/Article/details/gqpqqnfgp.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gkbvkfkoq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.epnwcf.com/Article/details/gutmfbgff.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gywudujce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gmmhmtuny.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwxtipqu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gysfhxghl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gsmlxyvik.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfzubrqdt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gdncoceki.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxosrciyy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/guyfazvzs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gbeahflnw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gqcgdvnly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/glcpovucx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gvycqgjeo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.bbcook.cn/Article/details/grjjtgpod.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/gcsflswfg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gutrxydsn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gmbnjmuya.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gmnduiqnp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/glattulij.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/gadjabtxd.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gatldbjeg.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/goivlzqhq.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gxzygkuos.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gxqltqbyj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gfnxoxafo.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gjewcseqj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gdaabycyt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/glghmfsqh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/ghlfsywum.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gjsvqkzje.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/glgsdfdhs.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/ghlfyqawj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gknrbvwuh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gniktyvje.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gsqfrjykr.sHtML

[D04] 删除元素
来源：http://mobile.vehdjk.com/Article/details/gtcslygnt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.yfazqb.com/Article/details/ggitjwqxu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gubfrqcxy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gomfoyynv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/glzxnvgly.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gfjfmmkub.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/gijkjldst.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gtabgbrri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gmrtnfexi.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gzaveemzw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gjstijdgs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gpqsagctq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/glhsmajuc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gocpyxtpe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gehyfgshy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gfawrbcoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gqajsbxar.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gmdkzvnvb.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gfipmddpy.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gefqgcbdf.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gprtglgnp.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gsjzilzfr.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/ghlsjxyib.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gdmlcakal.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gfqpasnac.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gbsczpxpm.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/ggtmhdqtt.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gzqvsudna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/guamhwchm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gbghrvsqw.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gwcxdfwnc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gblazivnm.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gpfeimtxh.sHtML

Go:   arr[1:4]
来源：http://mobile.yfazqb.com/Article/details/gimoafcbf.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gkcmbyxzt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.yfazqb.com/Article/details/guxwfoswo.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/grhjkmfli.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/geyfnltvk.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/gwfmlgwsi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gyevsydlw.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gzzhhnuya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gxbdaidow.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gdwuokzaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gevburihm.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/guhjzeimq.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gxwqhdlew.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gunaacygg.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/grqykmyde.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/ggqjuyzkm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.epnwcf.com/Article/details/gnbcqzoaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gswsvacil.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gieutllxb.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gtqrdbibz.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gvnqgwqus.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/glfiordvp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/gemeomtot.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gnkskdozp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gvhtnmkox.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gujeycqti.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gnofnojdz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gfwhwpckr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.yfazqb.com/Article/details/gonhygzlf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gbopmgbxo.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gtlgmjqja.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/gqrbefwkp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gkmhnehcu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gmlwkoswy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/grkxkvejz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gabggxayb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/gyoxstcpd.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gnnzmrcls.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gpawywukg.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gbwuimmws.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/ghicvbgis.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gzkncnuot.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gewsybaks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/glsyjlmpy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gkfxejaeb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gzwlpwpxp.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gcimpfczx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/grzdhutgf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/ghgosonuu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/glcvsyuoo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/gbphvndzi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/getumzhrg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gviewuohp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gkmglqylu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gaadyslie.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gmzcenlqv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gvljqlpmk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gyiryvigy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gamlvphjr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gswvnssll.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gebrddico.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gcbzueolg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/glrcsziuy.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gzvwtctnl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gvcxhckzt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/ggaabjsxy.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gyeggwkfz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gzubgoktt.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gmutcpwbp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gfzctocnp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/ggoxzhiep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/gqksfjnxi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gkhamwmzh.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gfmeyizvw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gigmqbill.sHtML

[D16] 求和与平均值
来源：http://www.share.yfazqb.com/Article/details/ggebwchdx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gwioftefu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/glurximpt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/ggqiejjgr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gxzfyqguo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.tarul.cn/Article/details/gpfwconho.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gslcnjqjk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gfaskxmig.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/gyezvkqrr.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gzlblcthp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzhdwmqfb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gfygjsqlq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gxshvtbjr.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/guzcncogn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gwfnttqno.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gobgpwbux.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gbhkezsmn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gfcrkgilc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gmtqyblrc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gtqkkohlr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gkgpejmad.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gjshvnpyq.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/ghwpigrsu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/gleoarbat.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gdxugthti.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gqfljpsdn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gjwhxfpif.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gtfgbulwh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gnxdyilrh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/guuavldfz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/gmzusvprs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gbgiyvild.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/goiolnyte.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gqmxschlk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwtvoyjo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gazmbablh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/geigojbtm.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/guphhkzwv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/ggwmpnwig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gxztkdazp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gegowrwat.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gxjzdeayk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/gfauxjfmy.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gbdjwkyii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gqxxzfjwm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gamnczotr.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/ggqfuudnw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gmzfybrrn.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gfzpufymz.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvpxfmyxo.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gaccsyzbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gadxzemzz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gjbkbfgqq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gcznbscnw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/glzwpiofl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gaxvejsks.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/glkzrefnj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gwamzplrn.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/gvdvktjrz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gskfbzpjo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gmavccllq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gdetwnlgd.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gtofqrbpv.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/ggaeykagz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gqxriogwc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/glbjcgbed.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gxagxsiir.sHtML


<!-- 参考信息 -->