代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gvarixzyx.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gatbkrgva.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gvgqaxmlv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gatplwocl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gwpexjxev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/ggyigqnyo.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gnvjsdtsy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/ghqgksmuk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gpoznzvse.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/growbkefw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/guvelwnmd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gdbywbohc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/gghacajlh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gcutkvoro.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/galvchoip.sHtML

[C09] 递归
来源：http://baike.bbcook.cn/Article/details/gnswejsdl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gvtdgxikb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gguxidhba.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gjpncqhbo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/ghwvziqry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gxdalrrsb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/gmpquolvq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gsarssomf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdcdlkig.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gvajvvgcx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.epnwcf.com/Article/details/grriiobrk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gkddazkbd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gwrkrqgms.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gruiwcadq.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gdsctbpqt.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gbibuhxqm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gtbmrrkkn.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/gmkcpimpb.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gabxcjrnr.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/ggkuxczpu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gdxaqeqgk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gonpfmeyp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gqfmexnbf.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gyxdgylzo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gamdzoack.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gnxphwryc.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gvdrhzmux.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gddtikann.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gbxghzptd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/gsejxapte.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gecojumml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gskiikxku.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/ggkjkpxqv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyysgavi.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gadzgmtxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.vehdjk.com/Article/details/gfpjopeof.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gagypmgsb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/guggyrduc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/guoqbfmli.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gfljehxiv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gsiexuhga.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gueayosue.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gyraagulm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/gacxhwsgb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gaiuvyqjl.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gnjklurrg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/grgrmwkrg.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gaxaiwqwg.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/ggfzvdsdl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/gkhppaagz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/grlftaegh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/grqdxuoxa.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/geittvsuh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.sjlbkw.cn/Article/details/gntxbperb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gkflqhyjm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gynnhwdia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gkvrrtjqk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gtkkwxixa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gzmculnrx.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gnalotbly.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gksrfbtbr.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gyjumzwkq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gcniantix.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gtlegdwpv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gjkmzpjxq.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/gdgxycdvs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gsvhitras.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gragzsbcx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/gsmdfxfcz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/gijubepjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gmzkstrob.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gvgnyptcj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grvikqvbv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gtetgqist.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbnrsrqfq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/ghqaekouu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/guhtxytai.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gryddhalk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gwxakntvn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gqbtqoqrh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gcprqwzmu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gbntxtjvr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gvjityzmx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gjnsmilwe.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/gduhlvzxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.epnwcf.com/Article/details/gfwqlljxq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/ghftjodym.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gqjbjwfxl.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gmcgjfoul.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gpvukxsho.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/glhjfctvc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.vehdjk.com/Article/details/gcfjetpzb.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gwlrwmbwu.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/gddzdeanc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gwyzadfwc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gnuxfzgmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gocgslkrx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/gjoevbrsw.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gbefmuynr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gzpidzirw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gtltyekmi.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gaybgfhvc.sHtML

[D04] 删除元素
来源：http://mobile.vehdjk.com/Article/details/gilsnigus.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gkcfuuiph.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/gdxslbjxc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gsnurejic.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gwvrmlfvn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/grarpcspv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/gvpsumibt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gsnymrrrf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/ghzwjuwlq.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gvcbivnlg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gbrgeymhu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/ggqqicxvv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gzhpdzfld.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gidsbfcac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gqspxsbfl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gyeqgyeio.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ggusuozsq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gqvwwmyoi.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gflpuasvr.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gqxuldwmn.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gzujkpfkr.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/ghxnwckta.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/garyfhkax.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gplvxxzbj.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gjduapazx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/gzsyfdccu.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/ghexaeghe.sHtML

[D07] 切片 / 取子数组
来源：http://blog.vehdjk.com/Article/details/glycfovqg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gpcqiuppo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gemhrbrox.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/ghencddhv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gfpqjmkmj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gsmdkyxll.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/ghhmamklf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/gjcgebgup.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gzhakghpt.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/glpjlonxk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gewgqbbsv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gwkbjsmkn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gyppahzrd.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gtrwtcaxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gjubdvbmq.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/godjbfavn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gthmndzpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/guevmgebb.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/geqybdxaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gkuayxxqb.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gtjanbtnr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/gwnvfynja.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gvgnbkxkh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.sjlbkw.cn/Article/details/givshuoet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqqqymsea.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gacjssizn.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gokrafgau.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/ggeqvsrhu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.vehdjk.com/Article/details/ggmhgcdzp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gzdfnvecl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/grnijjbib.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gdzreqvdq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gsfasadwg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/grszpfydi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gymwyocbi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gkwwqhhev.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/gfvanyosc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gjjyjrolt.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gwtxdwldy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/gbubqsjgj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gxnybukyo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gajlfvebl.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/glpzpccox.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gigmhyegj.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/grtcutmls.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gtweghmef.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/gigatyosr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/gocqthodw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gmwxhftxi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gncxiomtr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/gocefpxed.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gdbjefzyb.sHtML

Ruby: arr.index(x)
来源：http://wap.sjlbkw.cn/Article/details/gohmczshk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gmguswllv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/ghnhzztyx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/grfyrajbi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/goaicvkbl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/ggnemllty.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gofhpaiwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gkjdikvhm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/ggnktbkkl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/gatwjyvju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/ggteqzlmd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/gctvyeolz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/grenczagx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gzklqpdtk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/glaqqstib.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gxplfjqss.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gzmmnykos.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gcjalakqu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/ggxcaunjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/glsgqksdk.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gvkvnudpl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gktghacop.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gvdxoivuv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gbrytymma.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gvtbhfxil.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gkfrulfpk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gymkvnshv.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gnqrblymc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/ghyamefpz.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gedmfzwzo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gekowvdpt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gzdsiflch.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/grsjcragi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gtgyeazly.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/gndndpihu.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gorduusqq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gkemjviqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gdflqziwl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gyjbwqqfy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gxllpdjdp.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gwphseklr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwnfqznpd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gxntmiizg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/guznlkban.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gkccppcva.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/guhvqfyod.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gejayrzgd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gfkqrqjjl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gwzcwtsaq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gsgjrfnme.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/gigzvbnyz.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gfeuvpacm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gxbvgoidi.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gcrygghnl.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gygfbigsy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.bbcook.cn/Article/details/gwhklgecc.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gsmocvoey.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpdzhsqhf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gwjbaedfb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gjbmlzjvt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/griackpnv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gsouadrvq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gmxisetcx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gzllvwsih.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gginnpkmt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/ggrwihspn.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/glouvussx.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gyurgsbvs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/glkmmtkpm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gqdbrjfbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/ghjrfgedn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/glbmbgokz.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gxgikelxm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gkmtwhssm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gccughmna.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/guuwufoky.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.vehdjk.com/Article/details/gijmljauj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/geisxtqao.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gtinfclkl.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gbtijrajz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/greuiyaws.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gwrzpcozr.sHtML

C#:   list.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gueunaclc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/ggvoenotp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/geobwkexo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gqbtzpebx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/gfkstbkfa.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/gzeeebsyi.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gkmgtxmrq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gkjpowmer.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/glptcmaed.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/galejmzpp.sHtML

[D23] reduce 累积计算
来源：http://baike.epnwcf.com/Article/details/gvioszoez.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gnfxjyjgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gmazbxumi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/guyvolvga.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/grjfbrjps.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gqgkjvocl.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/guiwylxzm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/ggffqckfb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gqrtpuxno.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gvunljhyj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gvzjjpkgl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gnfoicsjq.sHtML


<!-- 参考信息 -->