代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gbkcrzeli.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/gmwdyduet.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gglzczmuv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gvsgvjyuz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gpncchvzt.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gzduwaqhp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gluucwxtp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/giamxpbli.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/golddazwi.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gbbguhese.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gwracqjqe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/ggdouwszp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gpjnbgbsp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fktsv.cn/Article/details/gmqifdtqt.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gfqmcphpw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gpazpmmaf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gyvtuyxdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/guwjokmva.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gdffkbnyx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/ghozwgmgd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gqcdcftwf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gvxrnxycl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gjfprgoij.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/glkrgkedb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwspklddc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gfnnhpzuc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gxmnhbfeh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/goypxwcrn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gzczxxjmh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gnynrcbsk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gstihkmvp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gcgfaliah.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gfwewhsue.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/ggqdyxviv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/glhepizce.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gnawhzaff.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gwgdwfhif.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gchermvbz.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gilunulcd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/glawjstxp.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gbwyblbus.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gjizmmdww.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/godtjmgjj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gttqfzigf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gdqabkamo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gqubnzwxn.sHtML

Java: import java.util.List;
来源：http://blog.vehdjk.com/Article/details/grwlmfawz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gbdnuussv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gmrcsbnht.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/glfwecntm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gwgvfnevm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gjznymrrr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gumgycykn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gbpvpzjhp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gqtyseiyn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gaisimwcl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gbnvklslg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.vehdjk.com/Article/details/gjphuzypc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/guwynbogs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/gqrmqaoqy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gogbzendm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gehzyzqgq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gohtisbom.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gnwcnwxke.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gqqwdense.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gvegctzon.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gtqcglabp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gvrnrmmdc.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/gxayglchl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gteqvkewr.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gzakacnlq.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gclkeyhpd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gjjeejpjk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/gzstpjxrr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/gawjzyfjo.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gjlgxcncn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.tarul.cn/Article/details/gisustmuu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/gegrloeej.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gheuwbxtt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/gqvqfvhxi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gfadqyavw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwotfwkcw.sHtML

Java: // 无解构
来源：http://blog.bbcook.cn/Article/details/gzvrbozsn.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlcfvnaa.sHtML

Ruby: a, b = pair
来源：http://www.blog.vehdjk.com/Article/details/grrfeunsc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gwxopexxt.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gnjuehhyj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.yfazqb.com/Article/details/gwcqogbeo.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/gvkfxikjd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gugoyikko.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gikwlcjkk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gowmcuuci.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gwotlhlbi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gjaxwasfj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/gftktosjs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gljogxlio.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/gxrglghyt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqjpddyuv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/grcmsfohj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gblkaxarl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gmaseghut.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/glwtqkrag.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gjxkpivxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gvfjjkxbz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/ghyifdnlq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/gulgjjitx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/garclcpfq.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gxiwnkvtb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gmlwmzktr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gbkieogvv.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gdvjihwer.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gphzplrea.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/guwtefypr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gerdwfklc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/ggmqwwool.sHtML

C#:   list.Add(4);
来源：http://blog.tarul.cn/Article/details/gtjajgcde.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gksgkxxay.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gkdqvrgeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gspzexrja.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gwxfayaxo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fktsv.cn/Article/details/gzwritdph.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gtqdpznag.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gkmxrmynp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gannwinhg.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gexuedrkm.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/grulnrsbh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/grtfehavv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/ggdsmlixb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gzqjawcct.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gbotofkzf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/gpwtbfjmc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/grdlsghhr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gxprtamgo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gyqkbhary.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gtzigjwgs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gkoxspymn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/geymqocxr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gmllihbbn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/ghsgdswpw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gqhuwkszq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gycyzdeep.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gpkzjtcuh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gcekcqalq.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gywljoprv.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gfogyfqpc.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gvrtewsij.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gludmmtks.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gzvoghgkw.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/ghlmrdkgn.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gbgpltmar.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.bbcook.cn/Article/details/gyfnlqiqj.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gkrlfzgpd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/gzbkkvtkr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.bbcook.cn/Article/details/gmyhkszoc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/gapqpccji.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gmsehfsjj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gvpgyzidb.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/gyufxqurc.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gipzvrasx.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gxepiqksw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gngndnyfr.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/ggywnchcn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gmrzlvvdh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gznfopfoy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gmcyzrmhq.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gbtlwgasj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fktsv.cn/Article/details/gvyoxwjnt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gkblfkxzi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/ghnklsctp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gpjhiapar.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gkidjuabf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gttvbgztr.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gzbzqrllh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/gsobrcrsh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gjcfgubeg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gxcbcarvp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gveglfwcf.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gnhnvghvi.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gtpdytkwf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gqydnshsg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/giyralbhe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/ginkmzijf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gojnppuor.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gdgfawqok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/ghzpihwrm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gfhlwknup.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/gzxslxrcn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/gaieiogin.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gkifzwzfh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gtkbtwxbv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.tarul.cn/Article/details/gklfjesqo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gkwpjvdza.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gwmndldxy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gyugdtmbm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.bbcook.cn/Article/details/grsoqfyyh.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gyizeisdc.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/ggkarklkl.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/gcnrofdgi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/gziappfzu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/glthndqbj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gmgritxlg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gvcncdnxf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.epnwcf.com/Article/details/gptjezqsv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/groeuxgvv.sHtML

Ruby: arr.index(x)
来源：http://m.share.epnwcf.com/Article/details/gspdaduod.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/grrtdgxek.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gxsljgriy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gschgerhl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gkxkfhatx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gzzocpnze.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gisampxhk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gwuntbshz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/ghlggtahy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gjizxqiku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gandgiprq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gtybspbcx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/gozjhtrvv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/guhyziure.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gxxyfdxrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gudclluwq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/guecwpjhv.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gbicglqaj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gwpgamdyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.yfazqb.com/Article/details/genoydeze.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gpkhtcbyz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gqrtrpgnr.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gqyshqsjf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gldisjwfv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gzvnpollu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/guvdplncm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gvoisjzad.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gmlmxlydb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/ghtcqkhtf.sHtML

[D16] 求和与平均值
来源：http://baike.fktsv.cn/Article/details/gtiizfcce.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gvdxmrvyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gwuqtwwjv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/getgbfehd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gwsyzcoxz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.sjlbkw.cn/Article/details/gimwlozpc.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gupfpszdv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/ghsafzzga.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gdivltaik.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gemiyiuzy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gawacyqpr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gfuonosek.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gtignuact.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gohkpqzjq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gwiyvargu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gdibtsuob.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gftikvowk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.tarul.cn/Article/details/glivlorkc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/glwqydxga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gklefazyf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gslobtmbj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gvlfmewec.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/ghacztlfb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/ggoezxdmr.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gwwseocrf.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/glhwcuroy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gvjrsqyof.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/grshlzcgb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/glzsfdzwp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gritermow.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gghhjhljo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/giamedupz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gsgtiyaas.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gcopwwlrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gyhisobtw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/ggukvnkdg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gwogvowca.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gfsmmfsdh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gecufdhqk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gyjucdjxp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/ghorsemwd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gkcnkdyvf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/grfpjysbx.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gzasnclvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/glomrggwo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/gwrswedsz.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gmtdwdkfg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/ggcwerjuw.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gsbeahuqr.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gyexpogqf.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/grlnsafyk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gbrmmclsh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gbfzzgyqq.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gacaxyjez.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gpyqmmzaa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gozxjlegz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gnlayetxa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/goyftyufn.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gnonmooay.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gbecnrnec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/glgvudozk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/grrnnwrty.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gbmhwihqg.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gassrovyk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/grtxdpcdr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gcyowrlnt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gvldhrsee.sHtML


<!-- 参考信息 -->