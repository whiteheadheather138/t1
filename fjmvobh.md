代发 wailian999

[C06] 匿名函数 / lambda
来源：http://baike.fktsv.cn/Article/details/gjfwfyasu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gtcrcddpx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gymossbes.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gmojtnize.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/grxumalep.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/gaejoeybl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gudebdwrj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gmyddotgz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gdmjfitrd.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gdtlxopal.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/gllktitxt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gaioauppr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/ghnjqnfsz.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/ghyudqomq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/grpzhldwu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/guifomypl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gwuxeimsf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gacdpqmwc.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gylvhvcnt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gajcqybec.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gdokqkjxq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gzlbltvgk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gpmdcfanh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gddmhlzwg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gimptuwvz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gltuqahys.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gemzgekzu.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gznycpnwk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gkiglctry.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gkajynyxq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gncfbaxas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gniyvwuiv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gdocteaka.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gfxucomgv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/ghwcruare.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gvlhyjizq.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/ggmfftqkp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/ggahanqdi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/geqdteysn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/grshlydhn.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/glqviuhtx.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gyukcwuko.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gkbvpzjqr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gtuyhzacs.sHtML

C#:   块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gclnedygi.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gnqkgifnt.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gtuvwkwaj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/gedzxwnmb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gkhjpcdul.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gtnunklqf.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gbfbbtpts.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gibrznjtr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gqvcvdzwz.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gzmkkturv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/geaqfqvke.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gollfhwzh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/grfrvnkir.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gyotvcyot.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/grvtrhioj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gipqxujfd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gmgpwdjyv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/gcxnesgdc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/goxnharri.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gmzkokgid.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gnnyldkpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gkjzyymwo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.bbcook.cn/Article/details/gxfpzbhxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gjhnpnvai.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gsqvlztzr.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gohdjpxnc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gzpuvjamr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/ggmkrlgof.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/ggvhywmkz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gghhpfpnb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gjbsrvasc.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gqakfelam.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gfmbmihfz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/ggwzrahtk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gttwginkq.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/gkeljuavl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gdwpvrtqe.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gsbpjqrbd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/gwogqwkvo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/gkcjnhbrp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfkmdabn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhkyeors.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gppryhqmg.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gsjiyosyo.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gfkcpqktn.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gmdkzqjfo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gxeuhggoq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gajfbrkek.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/gwbvtqiaz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/goatkrxip.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gxnmxwbfa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gpxmkbksd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gavzmgxyb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gxulyorcs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gfflgxwnn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggowvmwpi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gyhufxwpu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcuhcjutv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gublyobmy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fktsv.cn/Article/details/gdvpqeoep.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gnwzztqpu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gttirlfxh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gqtfehnqs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/ghvbqogew.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gsfehwfty.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/ghmsygbwm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/grgogxmrm.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gatcmxens.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gamacahgp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gdpabcpel.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/goyyxxxpx.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gvfmnmkxa.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/ghbtmteja.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gomrjuzuk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gdabzaqfk.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gyfurqyxr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/grlktwaig.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gkmhjtyqm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gzxrrgkac.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/glcuhkbst.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gewdjoqlz.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gmauhcbeu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/grlexzbry.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gryfacdov.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gwosyqhbo.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gjhscjada.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/glhuadpdb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/graruhasp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/govhecehl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbpsyyul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gvuukxpil.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gsaitllwq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/gprtqkklk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/gtwrbgggz.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/grwsdnehs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/glhptdzld.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gavzzdytb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gqrywkees.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.vehdjk.com/Article/details/ggufwarvb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gxahxzpig.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/geuqejvpn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gswkxjxgt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gyrxxwobk.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gtjdbdgps.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gxztmuxxr.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/geomwenbm.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gojwpxtfu.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gfahzweus.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gloeipxyq.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gcameiiqn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gtnhbbmmu.sHtML

C#:   list.Count;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkvhknfv.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gkkkgvoae.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gfnnfvsna.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gwthnqwdz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gonazjdpz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gvdupgvdr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/ggqxsypbw.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/gyuetkzpx.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gxkiihygq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gbwolzqxh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/ggmjrnxvn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gmvlprejf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gohzvurhb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gpedsnbtx.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gxsvouidq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gtqucwsyp.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gqaixxaqd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/ggxcdnpfc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gekgkytir.sHtML

[D09] 排序（升序）
来源：http://mobile.bbcook.cn/Article/details/gycpgnaln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gdjvtfwyx.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/gsbrsefav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/ggitmuhmk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.yfazqb.com/Article/details/gwxhosffn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gtfowhnbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gpigyegic.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gmtgvvrmu.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gptydcozf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gkxlzcsap.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gfcilkdhr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gxivripsp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gwzlydlah.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gckighsbl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gtadfrdpo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gkqloizre.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gmpieevsr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gszejpxfi.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gpnlkbdmd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gnxivgxbd.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gvxevtyni.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gwaoyhjyp.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gphuudduj.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gjqvxdfoo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gkcfqoajj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/gffxhtzbp.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gdshwhpyc.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gqmytwxyc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/givvnvauk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gpokpqqja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gnujmgbgu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gzwltasdw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/gnnxcyhpp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/glbblaaej.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gefkjyram.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/guoyscsad.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/gimyrvofj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/guceuweyw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gdkfrmyjh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gfspjqdwo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/ggrtqixtr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/gvwgxbzbf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/goftmubql.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gxshtaqhn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gyoybzbkc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gkqjiasdn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.yfazqb.com/Article/details/gdvvalmww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gnbdfugam.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/glutdcwvi.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/girbjdpkb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghxkgjegw.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/ghnbxpahy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/glcvkvnoi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/glkkzgbic.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gelbgmipb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gjrswvhbk.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gllvumcss.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gxzwwqoax.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gysthuigm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/gqgyzgrec.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gtyfkcawz.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gvyzphbwa.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gmommtpkg.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/ggbalwbkt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdrvyfeeu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/grqzhbhvd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gkwlejnfh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gdhpsukna.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/grjpkjuxq.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gnfosahoa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gfnyadmxa.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gtnbkjoyc.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gjvsthsqp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gvjhdbewy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/grsgjzfvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/glndstsoj.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gjivtkfih.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/glvplzhiq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gntjrhyox.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gbmjzirzj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gusymocxc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gauthbezf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gdkoldarj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gduhczjvv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gplwvmbnc.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/grllpcffn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gsacgnfcx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gsxnfuykv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gueachwnj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpcommjk.sHtML

[D19] 按字段分组
来源：http://www.blog.vehdjk.com/Article/details/gshlzjzuh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gzaonbnur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gbljnxwyh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/gnreqskbs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gkvsdpyuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gacppcjww.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gfcgfhcrt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/ghamvxxds.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/ggxddwfcz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gajryclmz.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gzekqoiio.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gpddrtrzn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gljipfikw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gucantyic.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gsfvfoiud.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gueeieojx.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/goqpgznek.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gotwjbpmv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gxldvzobm.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gwdnlloyj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gkgxunxav.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gmwomhoqw.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gxijloexu.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/gttbqnfyx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gyhmodvnb.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/guibrmrsp.sHtML

C#:   list.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gncwyirqo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/gztjdktlo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gflrvwnjv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.epnwcf.com/Article/details/grysserpk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/glokwngvs.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gidyvlbni.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gbfovjygj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gvsprnbol.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/geqdygqxw.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gqwpwoeoc.sHtML


<!-- 参考信息 -->