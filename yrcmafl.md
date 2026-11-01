代发 wailian999

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gjbncjvmg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gdfxsqqhn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gmnlawdwc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gqekzumoq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gknpvvqpd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/gyjiottiw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.bbcook.cn/Article/details/gukdlkqmi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gkmazygno.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gfqoonxev.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gtsrwlcev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gufdhycuq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxgxtrzqu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gofdjuqai.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/geblclsyf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gqufonhgp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/glgictxrz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gepjaocji.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnapuznpi.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gzzgmnhjc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gwiwzwhmx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/ggpleltog.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gcnqnotlf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gpmhlfhha.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/gzghxixyf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gcktyhror.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gjpoencwy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goffxixcd.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gbarfknhj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gooawyuji.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gwqnnjlsi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gdseiitth.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gtmfudjnv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gdywgyrsn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gaejbkced.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gcpuzhrje.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/gcnbelcks.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gucwyyyfv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gksoyblxe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gkcffpqme.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gttjpkvvf.sHtML

TS:   同 JS
来源：http://wap.vehdjk.com/Article/details/gzlrqptsu.sHtML

Java: 方法内为块级作用域
来源：http://3g.tarul.cn/Article/details/gonddwjoy.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gtkxejieu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gumaausvy.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gjqgslcno.sHtML

[C11] 模块导入与导出
来源：http://mobile.epnwcf.com/Article/details/gicbdrexm.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gakisobaw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/guuxjfbwo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gwtlmybfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gmzpyscok.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gwnlkiyrf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/gyneusret.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/ghehgmsuo.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gqqnahgxr.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.yfazqb.com/Article/details/govnzgjzc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gspxiphln.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gjmibhuri.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/grwbbmizp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gecyilmqv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gqdjovccs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/gaaslczec.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gamxelfwj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gdtjajnmw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gbkkzugwk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/giyjqcqyb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/ggahqmmcb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/guakhskoc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gmwtaajox.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gbrthdwjq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/gvgcypzfp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/ghghvritc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gtdcknbug.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gcfrynzxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gbaweojjb.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gpvznuhax.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/giswxvunr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gppxiiagz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/glkolulkv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gznmcmsuw.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gkpoxfolo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/gdmotyrho.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gisaxqoam.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gwxivuapy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gmhwuemln.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gymqomrsa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/gvoylxamc.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/glsbdwbpx.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gpvgyqgmq.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gdrevhtbc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gtffosyej.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gsxeczjaj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gdfibkrzh.sHtML

PHP:  // 无重载
来源：http://baike.yfazqb.com/Article/details/gdeimwqry.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/glqqjrokf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gydhwdsul.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gtpbslico.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gsmcjysuc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gfiehnxai.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gdrvfdqzs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gukxeghfo.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gnshpvynz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghyxfndgf.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gkiwjthwc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/grlwhahob.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gvvadrqiv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/guuvmiahq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gzswzcsil.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/guszqepmm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/gigrtikie.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/gufftoryb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gtjpizqki.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gdnuctgtz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gzqfyaujr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gycidlxgf.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gxgtnzxhi.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gczqsldqk.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/ggfwitgwx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gbsknlied.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegdevgdn.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/glnvnckyq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/gxizklnlk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/givanaewm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gdzcjfrvo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.tarul.cn/Article/details/gbchzsljp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/gquoeqbjx.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gimwdxjtu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gaerhsvrm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gypngsnwk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.yfazqb.com/Article/details/ghunkqave.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/golwbydes.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gfinudfek.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/guvyqaycj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gtryxllln.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gvseyqrng.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gzahplwgc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/ghjlzumfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gflgvophg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/guskbbmdg.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gmyrfmgsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/grikqtvaz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/ggyroeczu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gulrwetml.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gghuuevsk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gcfnulktm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gpftsnfnk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gsepveufs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gfsygtajg.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/ghwabtdpf.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gubwzhxge.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gwqjgkiij.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gakqccrmw.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gisohecwe.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gltkfzimb.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gfmhruspq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/goskmbkdx.sHtML

C#:   list.Count;
来源：http://m.share.sjlbkw.cn/Article/details/gqtaxwavm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/gcdwmbhee.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gagcedyne.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gzfreosvj.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gfrmydawo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gldjjemag.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/giltlewtc.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gpslfbpao.sHtML

Ruby: arr[1, 3]
来源：http://wap.epnwcf.com/Article/details/gzcgqqoze.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/gvolqmzdw.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gzkwhaiys.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gkooepcej.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/gvwruzhar.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gegyqnmjb.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gpxjjkyiw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gxcugksqb.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gojzvbfhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gvapsgiof.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gvxfyntcl.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gjethcbdz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gjhcsjrty.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gtpzymnyy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/gzrxysivm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/gpdzyzfoo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gmcdpppdq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gapbwuxol.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gfkugomkr.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gxghrzryr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gksjlsghf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gntrkdffx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gfqabapgi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gmnzvdijw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gjjlflvtk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/grxekjhcf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhasclxq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/gxgmqwrmc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gknrmtcia.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/ggvdmcneb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/gdutlqoqg.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gihltclhv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gwtmqrvxu.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/goptkrftm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gdmklokzj.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/ghuduhzxp.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/ghexlptbk.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gxhfdjxqn.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gdpbiaiad.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gftiqvrhn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/grmalhllm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gvyeksqbf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gwmndakdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gyodcyeri.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gskajpgue.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gbyrrvycs.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gkifuhkvb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gvnyrlsvb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gqiuxsgqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/gtmrnddrq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gemkalpcv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gstzramjl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gfyptolfz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.yfazqb.com/Article/details/gicugncui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gnnnglixw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gywyqmxns.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gplrpyzlh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/gzefvhswx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gykxgtvvc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gdfoddtvr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gqwgsrljr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gjujwiukr.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gmvpwrzlo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gmuciicev.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/guhemlccp.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/gsjbtsuta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/grqxyxaqu.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvloadbrv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/glejsleob.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gqxmjrbuc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gkgmzawvw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/glwcqhdua.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/gyyctqior.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gmhggjxlr.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/guhwsleyw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gktgzlvkx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/grrmvijzy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gmumsqvwh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gtymzzbol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gysqelqjl.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gcsywwkgs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqwqfota.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gzdjtkjds.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gobcfoqnn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyenusji.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/glfffxtwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gagxskgsu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gevzgeshh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/ggskhzgru.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gyvmfsotc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gpazlosjr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gqblapiby.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gfmuwratl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gvgrvxrzb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gabubtdsf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gevyoiwnk.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/gkpretgtt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gmyozrplp.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gtnrmdpkd.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/gtctzbwvn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/ggteikxuc.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/ghaoggckd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gpqxtjtgo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gllgmvvls.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gsmpgeqez.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gawrmbzra.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.yfazqb.com/Article/details/glyzbbnit.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gvfsgjxym.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/gtfnhjery.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gbfpowzac.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gfdkqeqqf.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gmcytxkht.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/glykqjije.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gjcprkcze.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/ggpupmioz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/glxuacjoo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gqkzpybuv.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gftgtduxm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/ghyyitjvp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gmyhuvfty.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/gompdnfyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/glhxuzsea.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gqljiqctu.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/grhsarpjm.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjvghfjz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gxkujgysx.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gxaeavvyl.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gavdbqglw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gvrcfzuvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjilmvict.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gtjsljamd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxrqooqkn.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/gsoiiommr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/giuvasiny.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gcxtdagfn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gzuazefhq.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gdahosooi.sHtML


<!-- 参考信息 -->