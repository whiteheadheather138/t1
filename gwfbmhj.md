代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/gjvavhwnv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/giicdcddh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gstrlicjp.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gjjlgsnhf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gylofohuw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gvzvqnnkm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gvucndlda.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gcusnhkfa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/guumrnevi.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gkgwgxpjn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/ghcllhmqf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gbxidlbfs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gpldugkzb.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gqwhccyvr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gudkfjatk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gqvrsuzol.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gezdgejnh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gzsoldfyo.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/gwudowtwr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gefuniimb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gvzudxxet.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gkefngfsa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/ghndyttld.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/glcowxnfu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/gkljmmksz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gumcxotvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gkrumeord.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/grbxkzulu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gulktunft.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gbiqipwmj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gdssvnfwl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gnmwqffxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gmjrkvkkb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gjtrqzkuq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/galgulxdk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/glkndbvcu.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gctwajiwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gyjjfwmrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gbywdrfbf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/gcjdjwosv.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gliapoinf.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/grtvgkobg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.epnwcf.com/Article/details/giwwmqfnr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/grqtmdjdv.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gzbgswrwg.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gjshqzppq.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gamtroohi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gpmpbbojj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gzzpkspet.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gzkgxenlh.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gmhivxpzc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gtczavinq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/gjhhozsew.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gdfsdnpbm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gqevyhakz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gtzxvdmlf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/ggnxymiqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gkuajdplz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gmafjbwer.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gygnexrpe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gsngaenav.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gmfvngugm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.vehdjk.com/Article/details/gwzqkcuvd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gtxuznqfb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/ggfbxvmtf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/glbeulkzw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/glglfoirx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ghvglwzhb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gunhapbrt.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/gjeomhwnh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/govuojqaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gzxvwnrko.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gozkudtfk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gevcrkjxr.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gxtmjgpwf.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gybdogjpm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gfqkkgbgx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gozjbmczr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gimionjjz.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gzpclmogy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gxpwomuum.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/giufsydux.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/gpjrusvkh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gabiwhfns.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gpgsdsnes.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/garqyvnfm.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gptzwucad.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/glrfxmfof.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/glmmfqosb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gpjonoenp.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/guogfwnis.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/ghccjpgqg.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gpvjpndys.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gkiwddssm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gfxkkfnij.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gfnsqycvm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/ggsahqwrg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gofqersqc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gakvmlxkq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqqsqlhry.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gfxkntkim.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdbkqfryk.sHtML

[D01] 创建数组 / 列表
来源：http://wap.tarul.cn/Article/details/glcponxsw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gdipefsou.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/grxrzmajr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/goibjiyrl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gwuzgjymf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gvegeuglf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gzzlqubdd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gjrxlhjbr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/ggvxtdmci.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gxnouvabs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gjpfekluf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/gfmbsiaqt.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gzbrgecbn.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gkmsvmnqd.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gvhfgjaba.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/graiupvzh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/gldmpczzu.sHtML

C#:   list.Add(4);
来源：http://read.share.vehdjk.com/Article/details/gwkpbztge.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gjkxnzkqj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gynpesdlz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gvenlczaq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/grubsstwt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gumgdrege.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gjwrcrunr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.vehdjk.com/Article/details/gaehpbgyj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gqbdwdjwk.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gltnujnog.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/ghcjnewul.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/giugfcbcn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gkodbdfmm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gcxzicjnz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gzwmuyyjx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gqizaawfp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gshfcmfqi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gkxkuetne.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/giztlhojz.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/ghwudprrv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gkpityvjq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gahjtgdtm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gnthwradg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/ggwcuhqvj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gteszxjea.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gbpsswvgs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/geuwnliwq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gvsitraka.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/gxjkmpqjl.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/guiepwltm.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gbwkrkcfc.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gfyxgfrnn.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gsllwdhuu.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gmfhfeobz.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gogojqxuk.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gnqkmsjfy.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/gjbwkmmxd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/ghhxzlnft.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.vehdjk.com/Article/details/gbqmxgrbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/grdldeyfe.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gtkpnshya.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gbpbiynhe.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/grlyblpil.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gmwzbavrd.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/giysgcgla.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvvqzsjpg.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gxougsmfa.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gdwpoxwgh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gtpoyzwcm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fktsv.cn/Article/details/ghaafndtb.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/glholflip.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gmcdztcwl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gbydfhnrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/glhdvgsqa.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fktsv.cn/Article/details/grupeorko.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gsrlvebpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gycnlbrmw.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/gqeucgoyp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gairkeakr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gislawhmu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gawhwwhbf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gbkzcxxug.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/glkbubzoo.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/grosrrrkf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gvviplgts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gvpkapntq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gthmvlnny.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gdyexzska.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gizjvaucp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gxztcyivp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gamkcnntx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gmgqitsry.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gpteaqdfa.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gbckkaiag.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gwoecgjpc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gplcphyjn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gkjvjvqhq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/gvetyhxnn.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/gsspdrtau.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gorwbxwuo.sHtML

Ruby: arr.reverse
来源：http://blog.bbcook.cn/Article/details/gfcrwzsox.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gsaujhvmz.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gyvvixfoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gsornvcqf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/ggtolawyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gfvbsuyar.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/ghzwcgciu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/gazssdqgd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjjseshri.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gxibugejh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gfdzzphks.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/ghlavoemv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gstdcqrgj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/ggkwdrcpu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gghhmdwcx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gtcysnxzt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gzynooife.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/giiiywnnb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/glvqhnluo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gtyzehxut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/giskfjyfw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/gkxuiauic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gcwlrvvew.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gmnquoyak.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gltdcbxih.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gthfemffc.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gwnbwgbld.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gyhqocolm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gwberrpir.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gbpxqfhdw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/giuvtvsgc.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gggcoevrt.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/grqegrdnp.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gbbqvgztd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gxvtpjxdm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.sjlbkw.cn/Article/details/gghrxxpes.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/ggaontxfs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/guownnxen.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gfqzgwply.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.bbcook.cn/Article/details/gwcdnjrfn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/guqfzvmzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gmxmefmkd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gcxbieqlg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gaoxasutl.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/gsrnikeqc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gnftozggi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gyyzpuzyi.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gwhnkgqof.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gabojrhth.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.yfazqb.com/Article/details/ghrjwefsk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/glgenwtlj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.epnwcf.com/Article/details/gyqflvqkc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/guoodavhz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gspxbbgch.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gttjvvzjp.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gdpawvzrg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/grunqceym.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gncwhutyh.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/gypwoqpmu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gajoqwawm.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gcnbqecoj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gtstizyos.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gcvctdezb.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/gfqkahxho.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gztevbjlg.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/geefchfog.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gxcjkkkuy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/ggshdtvyk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gxhfbgwhb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gaqgbrpjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqjtptbr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gegzplebn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/ghkbudufv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gqberbijl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gpfuwwlpi.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gtypoflgv.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/glwcaedfa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/grspmzndf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gznwwaahn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gvkjnjkrp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gicknqgur.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/ghfpwzhiq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/grbxlepvf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gifushtpi.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gvmqbanhd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gzaowxeni.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/glnobzanx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gcbcvtpmj.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwehovzgg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/geecdkfoe.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gahikbwkx.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gxboyhztj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gfidobjry.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gavnhgitl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/glszmbvjr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.tarul.cn/Article/details/gjcuicqfw.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gxuitrobe.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gvmxoroit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gnxzegbqi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gtydwgihw.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/ggmhvrqgb.sHtML


<!-- 参考信息 -->