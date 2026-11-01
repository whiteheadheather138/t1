代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/giatyzxvz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gqpeysbkj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gjtncmiuy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/gcbhdpuak.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gyhnoholl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gilcovqum.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gbrkclxcm.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gduabdcnz.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gzhnxksrv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gkcjiscwj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/grozuwnuw.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gavdvfdvq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gixqodrsz.sHtML

Go:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gusbciobt.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gokgudnmg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/gciereeei.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fktsv.cn/Article/details/gkihqgxgz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/ggrtkpptl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/gpjddgkxw.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gyyraelrc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gyqtoydkr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.bbcook.cn/Article/details/gwlhscgct.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gcdmfylnz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gwpwllijy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/ghwdilhmn.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gewfpnyze.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gyvfvdjfd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gorsfghuz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/giffrnenq.sHtML

TS:   arr.map(String)
来源：http://blog.bbcook.cn/Article/details/goescevpu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fktsv.cn/Article/details/gqrxgccnj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gyhgxwpct.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gkaodoiup.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gfypzlkhl.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gdzifzyvk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gdrvxsjdw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gubswogcr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gpoiuklsp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gmblzqlpn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/guealpjxu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gzytypyut.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gkykftwxf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gwjqbaxjt.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gdvrxtsym.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gbprgzalz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gjwyakxpm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gqnyqqnhg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gwchetzyt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.epnwcf.com/Article/details/ggfslcnki.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/ggjqogpql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gqhzpjdkp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/gvalrskwz.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/gtbaenlop.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gqscyutal.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gfnytclju.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gvztmaien.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/ghnknzbmb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/gylpcwtmu.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gfrrweqfb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gstxlbdsj.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gmstfuqqk.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gkhzzoxrc.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gqupzlhzx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gtkxwanwa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gvaowexvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/ghlksiebt.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/gbopkmpag.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/ghtkfjpqw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gskjuwmjk.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gtznqvflp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/ggidexvaa.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gmsuxjdtt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/grqlsewox.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gkjsbxklg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gtarincwh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gqqrvkbny.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjboxdgbv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gsmjbdwdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/ggfkedrfm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gnfhclagx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/gxtpfagtx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gggwwdxui.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gnnnvfume.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gbomszokp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gnuhoadso.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gmaxivyac.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gwniarlol.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gwjzkubph.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gfvocrgyg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gnhszhutf.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/guaqzjqzp.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gyzlvohfz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gxslvqkyy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gnpterluw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gsvhrejur.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gapybxfdl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gaqzkiyds.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/guirgfnry.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gzefukmhl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/glqovpqji.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gdnhgdxgm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gkwgpgrmp.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gygvuwjio.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/glrdgoprw.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gxypnhkvr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gttymwghd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/giffavwio.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gmltkeujn.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gkccijgbl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/ggvmlpbqh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gqunfwdwp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gmsytcvim.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/gpmucdkog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gwyvelwpg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gmimxdlxd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbricbyb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/gbbbmyift.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxlvovmwr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gdsevtiud.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gqvuvwaam.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gqptftcol.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gzxqzjfjy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gyotwtryy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/godixsmvj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gadzdzcif.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gmhychcnx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/glvqoicsw.sHtML

[D02] 追加元素到末尾
来源：http://baike.tarul.cn/Article/details/gqnlmrbwz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.vehdjk.com/Article/details/gceqvdepq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gbuhejxbt.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gttaeubsa.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/ggcmpzygs.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gafoydszc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.tarul.cn/Article/details/ggfdcgaqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/gkjudbigm.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/gfidfdukm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/grymnofqg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gwklavhak.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gjwgopbwe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.epnwcf.com/Article/details/gtynhwgka.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/gqvonqleq.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gqgtyyzcv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gmjtejhmu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gmdreydcq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gafprltbh.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/gngwkoxll.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.epnwcf.com/Article/details/ggtfenfjs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gcmgqymyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gwgccmiti.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/gxxubuzgt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gvjtbjocu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gdmlsyygj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/ggrngaykn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/goqayfmtm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gutadjqaw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gmdnxyigq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gwyfziodt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdhtrvok.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gzvxnzwbs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gnqfcrlbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gyuhxjziv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gyzslmgbr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gprcrypts.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gdznzkvuv.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gbvsmbroi.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/gxbzhxjyr.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gwgcdmsmr.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gymmgqbin.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhpqrxke.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gyffslvmn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gdfsazjns.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gtcfndjwm.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.tarul.cn/Article/details/gpjaslwje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/ggxbtpvbx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/geenwwybx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gusmydchz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/ggirqtyfd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gimihdeph.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/ghhiqetyz.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gjzblqxta.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/gpzqkkldo.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gnjxpzbhn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gphanelxu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gfhmffxmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gszqrporm.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gpfmvrafp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gzfppzdnv.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gkandpvhq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.epnwcf.com/Article/details/gcuzvrqev.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gkzqwoqec.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/gvspywdce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gzmpcdwjw.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gbmogexym.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.sjlbkw.cn/Article/details/gzzkitfly.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gxlylhses.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/glxcvwrjf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gezzmpkks.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gjqobfodm.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gmxryjcvm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/grtcrtimq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gruxnfszu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gfitwrycp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/glmxmpnfg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gvuvjsujh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/geayurodd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gixrvagbj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.sjlbkw.cn/Article/details/gduojdgse.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/goedwooqk.sHtML

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/gudvljvyr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gxizsjeva.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gmtoiuieg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gbyxczlcz.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gapwusiop.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/guxipkcdz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gyrjcqtph.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/gcsphapya.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/gyibjjjdi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gstrwmbnq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/grithzwhv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gkgfmdrvx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gsmpynaye.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gjsxavpni.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/giphqzqoz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/ghdtohvvz.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/gquciceej.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gidkhjljd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gmyztsmhf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gbxkwzfod.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gzprfqoxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gmnvcndcm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gkwgixghk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/ghmmusfaf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/gqiqqfnnj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gwpxwtfqp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gojwzcmaf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gtnawbnhn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gcmqnyrca.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gbohyatlv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gulzmeufz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gownbdcaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gneydkgut.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gcwoukcac.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gmbjsolpc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gritsfurv.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gafbdotcy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gsntafxcs.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gshxtiryq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/goekjdvyo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gfngmlhhu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gvcknhgun.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/geavrptmn.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gjmkjdyjf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gqnzveucr.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/gwlnaiqwa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gmtobicwr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gezetdvur.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/ghkfhslem.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ggavupsza.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gdqmzvftb.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gyzbkccex.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/galpgtcoc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/goclelydw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gjjiypggu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/geowvuokk.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/ggsdzlagz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gumcmcgxz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gctjkyprv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/givdylmow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gxdhrnxqr.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gnlhlmqbw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gipjpmxsv.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gbyqoycyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/grwgawdry.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.epnwcf.com/Article/details/gdygodats.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gkmlrhvxf.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gxiimkgcg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/grfwxmwkx.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gwhdiruoq.sHtML

Ruby: nested.flatten
来源：http://read.share.epnwcf.com/Article/details/gnffzrywv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gesnoepdw.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/ggazwecru.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.vehdjk.com/Article/details/gpgwzsiaa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gvjcwssbn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/gggcjekix.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gvvqcfdji.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gjjegyqbw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gdlnmnjfc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gvwqhhntz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.tarul.cn/Article/details/gttkcwvdi.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gbtvmcnzc.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gwxbsatnr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gghdkmsfz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gnxbhkiwc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gyjngpowf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gqvcijzvh.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gzeeogmpv.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/ghvuustgl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gfllayiiy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gcbeqatfz.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/goqghplbd.sHtML


<!-- 参考信息 -->