代发 wailian999

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gqronkqfr.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gtgtmhpcd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/gupzzvzpl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gjhidyufp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.tarul.cn/Article/details/ghrpyuhhr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gkeszwrbb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/godrkvjhi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/ghjeibvrm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gbomsttru.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gzxvfxmfk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/glaorbwhy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/gzbnbryxv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gdcrwmwvv.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gvevddkbo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gzzcsznjl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gmnujipte.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/goowvgwgj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/ghvmjfixr.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/grknivbaj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gorfsnwkz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gymipnfzf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gqgtnjeje.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/geomacppu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gikesfoig.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gkhlyauwz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gokfdbbxu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/glpnlpnnf.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gednkblqx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gvrgzynlq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/gfjqwjmls.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/ggocngxwl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gzjdfyoaa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gomeqgdml.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gtpbkzqzi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gobreshba.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/gmaobluzz.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/glqjfthth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gdsjiirwm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gsrzgdwbr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/getghkqqz.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gaadtjaje.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gjmuthapi.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/goxlwihln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gnrowxvyk.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gqulhplhm.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gfpeszuxa.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/geslhpiby.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gbvrahbky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/grsfvdpdy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.bbcook.cn/Article/details/gglmkqxhb.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gynpeykcj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/guomfvcbp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gkrlnmeqm.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gvgdhlgzh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gdadgllwl.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/gmljvfhor.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.epnwcf.com/Article/details/gxkpmhrzl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gokjumiwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gurgywohv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gkhnpfoxx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gkbngvgsp.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gyborvonp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/giudczpmq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gzivhfhzx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gimcqmulx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gvolumulo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/giteosmuf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gmhlkysbn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gssnvbwtp.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/ghznfcwri.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gzsbqzjji.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gpvstbabd.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gyypzlguw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gfarekvph.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gkghcsnse.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gemlcjlys.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/gecmeyubd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gutnkhasy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gpqwxvbjh.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gtehydpfd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gngflfxop.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/giilyjors.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/giyjfrlqo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gzlyzgzdt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gjitxeexa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.yfazqb.com/Article/details/gokqbsthg.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gzkdrauii.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gkdqtlkof.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gnzlfhjds.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/golmbyqws.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gxobvhlre.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gzgcxqzqg.sHtML

PHP:  // 无重载
来源：http://www.share.bbcook.cn/Article/details/gomqqolvn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.epnwcf.com/Article/details/ghqewveng.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/ggmtjukxc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gyedqxezp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gcjvjjnyd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gdnupufpj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gahcmsuij.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gksacdxde.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/ggtilolls.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyzxgakvz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gxzugevzq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gqsucgolm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.epnwcf.com/Article/details/gaxzchouv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gskszuvxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/ghuwihgih.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gkicjrbwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/gfjngsxqs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fktsv.cn/Article/details/gaorppfus.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/gthgmivvl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/gyoikadrp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gefhpiuep.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gkcrypzdm.sHtML

JS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/garaowpvc.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gdixeberg.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gsjtwhzmw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gtgretxfh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gxodxxwdm.sHtML

C#:   list.Add(4);
来源：http://www.blog.tarul.cn/Article/details/gkwhmposa.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/grtjxhcvy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/ghoptaarh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gtlgmrjxf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gjnditzmb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/glnpzedqn.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gdeomsuay.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/grncqcjqi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gxytnlcpu.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gtcxpsypg.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gxbsqlsvp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/gfaayoqvm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/ggdivifgo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gutkahtcq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gijeicpti.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gezflkube.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gkettngah.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/gpksbipzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gxaeojvmy.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gdyhfroza.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/glvcemufq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gxopzrtkg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gbklsnthj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gerxrjoxh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gsmqqjglh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gdopcpcts.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gqfrkmlxs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gifjlmmtb.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/ghvyczvwk.sHtML

Py:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gtxjurvnh.sHtML

PHP:  count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjdyjligi.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gxbenbbfi.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gjmlzlaab.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/guqgpoczv.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gmwuyiihx.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gcesljnzc.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gngiujkbj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/glwtksycu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gwtwvwjkf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gaeloqqcr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gnpsuuwds.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gdacmmwza.sHtML

Java: list.subList(1, 4);
来源：http://wap.yfazqb.com/Article/details/gjxjfimah.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gcuxoprdb.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gfmlmnujl.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/ganisiqxg.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gmfmomuns.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/ggrjxiwva.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gtxhononm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gbfhlqbew.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gutexplrd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gwacllupn.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gptoyymbx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/ggfkoqgua.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gdslbalxk.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gmznkueha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gdraboted.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gcjtlctbu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gytqhxjdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/grchgtdrj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gqbbkxqqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gxrgqbnlk.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gxzfwzmfv.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gxbkryeyb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/grjfvgtza.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gcdfzrzft.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gharypryi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gdyoibzal.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gqgxvxgno.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gujzylyax.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gbwgbllxt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gayhslzrn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gshviiymo.sHtML

[D11] 反转数组
来源：http://www.blog.vehdjk.com/Article/details/gexiwctxt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gqmikrsuh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gsrnadtxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gmmbmraap.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.tarul.cn/Article/details/gvpjqngfl.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gzifvtlvb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gwnafrusa.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/gyzgaweep.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gpzyhrkir.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gxhnuuhww.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gqatimjrc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/gldzikkwg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gdkjbeuwr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gyztqwcno.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/gcnmqflqj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gldixgzdg.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gavdxzjmu.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/ghsgaymby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/gibhzisft.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gnxpeltnd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gdpinvrmm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gbhnxnkns.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gztfwgzra.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/grpxeejni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gozokbqwz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/guromfhfb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gocrliisy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gudzgwmgc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gqeqmlewy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gvrupojxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gykvrnudr.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gbsbxskyh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/ghitbbsvj.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gicbnsrqq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gpqsofwai.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gzfckogik.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gryqppjdr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gxpwadose.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gkluhuwun.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gnngubdri.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gytzntiqw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gxfdrraar.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/gpjxgdhlv.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/gzzlyvppk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/gtkunwxeu.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gflanvuwq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/givayvtqv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gbtskzoxt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gakdmemee.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gsptpsqoo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/ggeovzxjn.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gzmhrgdxu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/glzwdafgf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gaofxrpjn.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/gxtcfsmlp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/ggmzkpprf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gqvpckwzz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gbpadwquv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gnerkmgyh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gkjizjcka.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gceglymyw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/ghumimeav.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gqjhudoek.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gnapjlbxc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gfzjpujdy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gysjrdaxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/ganhgphrs.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/gyrtcuvps.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gegklkoli.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/gkmcaxygo.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gywfhbdoe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gunvfzxxv.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gacepsmgh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gccwachxy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gkvdaaorw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gkwrilhiu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gijjuvyck.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/grfmwnwco.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/gwfaxvfxo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gjjnkuakk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gqjrfjuyv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gobklkyzq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gyijcdisb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gigwfizea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/grzitimdk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gsjflstdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gxtxdiqyq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/gqrsixjkv.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/gzoibaxwr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gkjviuvry.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gcdebgqcz.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/grexhlrug.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/gqkooamip.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/guicwobay.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gourydnvs.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gtinwnwuj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gubiqrmmw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gadjzxaqd.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gxqsqdvze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gxfsxjpfz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcmmhtdgr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/ggpgorjjf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.bbcook.cn/Article/details/guxehzzbb.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/ggfxeonii.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/ghodfefry.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gfkqnhnvd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/ghzrpzumd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gmzqvzlww.sHtML


<!-- 参考信息 -->