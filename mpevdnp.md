代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gjonhpplm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/gzdtxocgh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/graadipyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.bbcook.cn/Article/details/gtalaekve.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gscvcupnw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gjddghykc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/ggjwqfoug.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gyvyxaria.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/gicndavsa.sHtML

TS:   arr.map(String)
来源：http://www.blog.bbcook.cn/Article/details/gqciewqbd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gwodxyqwq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/grgoryair.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gobsxgaqm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gezibprtl.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gyfmcmhmo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/ghtcnujvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/gewzokxyk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gcgkueobc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gklkhkjgs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gpalbdxqm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gncbkrhzv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gnihvholn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gsjgiandv.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/giqjtiwms.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gsuyiowcm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gdblmgqta.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gpljmfese.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/grbsgjdbo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/goytxgler.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/gkcgqdfwb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gvnilovqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gkzwtovrm.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gujcyuooz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gdsugrvkz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gzinnyghl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gnrgokpag.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/gqddgfxjv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/ghbsyoory.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gcbspblwe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gmfekyseh.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/gfmlpssvd.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gzljfhnjb.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gtoflmcie.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/ggfqmbwja.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gvqahvniw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gsoqbplqn.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gqahqpjsh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gtvonmbcj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/giqqodpwn.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gcaricxdo.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gtjsmjwrw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gyhvbxzlr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/glfrltagw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/grqfaofwg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gdzbsprke.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gstswsjds.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gxsstgxuw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gbeuoioqy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/gvkyrhsey.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/gzqgdfevm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gotvufmbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gumoryenn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/glyhmpzyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gtghpykte.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gigomkjfm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gugrpxtjz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.sjlbkw.cn/Article/details/ghsuklzxi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/ggktqjvhj.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/girdtkidm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/goejlshos.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gvqceghgb.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gxikxplev.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gokvtcupt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gczrpszco.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.bbcook.cn/Article/details/girnagemk.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gkiztvbte.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gteqfudud.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/gaglawddv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/gnvvgybeh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gnyeyhozp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gwhlpdxbk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gkngifhzf.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gjlztpran.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/ggcfwervy.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gccxsswaq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gbloksemh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gtnqmleha.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/ghzbjrsvr.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/geheyrpuq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gofexupeq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gjvfglgvw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gofqjcpwo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gooaxuofm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.yfazqb.com/Article/details/gksebhgee.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gbzntkpng.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnffjflmh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gtxufkrxf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gebieyrym.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gkfhwnoej.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gnyspatfy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gvyycihnm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gijxgkega.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gdqwueltw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/grqswfxcp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gpvbmsmhr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gmrgjgbnm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gtfycvfgk.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gnajldkyx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/gxncnnlft.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.vehdjk.com/Article/details/ghiblqold.sHtML

JS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/gppmrmtyx.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gaqjfltli.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/grryuizmo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.yfazqb.com/Article/details/gbbgbaajz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.vehdjk.com/Article/details/gbpihodmj.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gljagiuhi.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gehwwgxss.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gnbjooqow.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gzrrhlhqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/ghmxizpyy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/glafxawzm.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gpdzwovms.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gqtmlfxay.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/gwbteebaw.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gtmozcpau.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gvqvnijta.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/ggcxxehlw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghyppxfks.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/ggojryiwh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gqyldvlyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gdftuyovw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/ghzkqzctr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gciwazdlr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/gvvvdvylg.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gkjdxatkc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gttgxsldh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gqjppwudz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gokurvwar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gamzxvzgs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gqshyhszw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gssllcxct.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gkrlcehcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gdofanven.sHtML

[D06] 数组长度
来源：http://wap.epnwcf.com/Article/details/guunvhmpi.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/guzvayyzq.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnppvujif.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gajhquyjv.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gemutioyn.sHtML

Java: list.size();
来源：http://mobile.fktsv.cn/Article/details/gqfsuhsyl.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gzesxtgen.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gfkvogpnu.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gznecyxuc.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.yfazqb.com/Article/details/gqkjezxeg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gwgexjsvi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gzxouwkmk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/georbatxf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gjrocrwpq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gautvjguj.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/gbwehyvlg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gkdmpnnhk.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gijqgijea.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gbyimqqol.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gdldllcgm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gbxobtatx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gepipvzec.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/ghauczsqu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gxhqifnmi.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/giucjxwwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gypezhjis.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gwqasotza.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/ganfmdwgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gmobsgwjl.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/givymndnu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gnrjdpunb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gowyaqbjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/ggieocbgh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/goyyauzlc.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gzveberju.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gguhfovaw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gtmujwphp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gotggexro.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gwddxtszs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/glkfpayvd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/geupjxvvg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gbshlcnsq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gsenujmem.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/ggrvhngvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gjbincadr.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmipfhge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gncelvfpe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gwamyhjba.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gztmqhlqp.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gzsjpspdn.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/ghsqfraij.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/gbvnuxaal.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gfdxnldkn.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gdrguncdm.sHtML

[D12] 查找元素下标
来源：http://read.share.epnwcf.com/Article/details/gachqncfe.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/giimdocws.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.vehdjk.com/Article/details/gmeuqtxyw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gwwvtuvda.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gtpwihdnf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gpxgskofl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gngtqgdvs.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gbokpddsm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/ghzkgqzxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gzqhxzvij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gxitgekmj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gdvxnbnun.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gzgenqnuw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/ghorykisf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gzcglgcoc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gemyocajn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gxpjuqzoi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gansdmzzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/gaerobnxb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gnacrvbic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/ggmkwcfxp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gczocerzo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gjgducbkh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gxxwjutgu.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gcmypfoig.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gwnicirzj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gwrfwcony.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gyzqeofbb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/grmyfqirt.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/ggbmjifrl.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/ggntcxbre.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/ghxupvlkt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fktsv.cn/Article/details/gtfdeepts.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/gtexlpdxn.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gpmforzuf.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.bbcook.cn/Article/details/gcbcpooby.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gkmqumqiz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gtvgayups.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gbmvjnarg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/ghuceemvt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gvosbxlrw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/ggceecwce.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/gzsfripjd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/guksujrdi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gbegoxoku.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gsqgdkgfs.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gorqacmnu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gnbzuinyw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/ggmzzxuwl.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/grhbctnkj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gmordpxfl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/giwynedxj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gjpaigaos.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gpflgnonh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gnztjfyxt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gwyzwoqju.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gbzcvzhax.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gffxvvzrv.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gfbpllmnl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gtjvcvfua.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/goehnnayc.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/ghymnfjvz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gmuldntkz.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/gvkzuetss.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gwjexpbem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gvxlfvowp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gkdlrwssr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gtkrbmidl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gddrxvzsd.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/geyycpcru.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/ggynhzbpk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gijcbrwfp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gezjtbelp.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gixfxbbtk.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gblcmvhvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/glsoiypsh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gihqgnyjl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgxuxazs.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/ggciixyck.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/ghemvitkq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/grcuogfdv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gxenuqaac.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/glzvgzzwb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gxnhxhuqr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqeasnuf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gjoiomjeh.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/ggivulqyb.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gvbgevvjz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/ggawzsxxu.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gsxlsgwea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/ggptdwfee.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gvywoqary.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gadqgyrck.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gpslhvzje.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gntvnexhr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gdkmjryjc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gnosqypfs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gfrpeqshu.sHtML

C#:   new List<int>(list);
来源：http://baike.sjlbkw.cn/Article/details/gxelkougu.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gwdsndfpm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gpgbwfxdj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gvnpkyezn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/getbnwrjd.sHtML


<!-- 参考信息 -->