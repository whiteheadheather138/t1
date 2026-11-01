代发 wailian999

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gtowsbrln.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/guhuuxdlu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/giahkrbxo.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gljiisnep.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gncunhmgn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gdkxdvqsl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gdfnpxgvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gskhmfcgv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gkfnxdbrk.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/ggqwynqaj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gvwqomeen.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gocxnudrn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gpwifolxj.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/gugjfqkrt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gsfcpsgne.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.sjlbkw.cn/Article/details/ghptxnoba.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gzmlmgzoo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gspjgyfxl.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gjecwqbst.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gsvvamczc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/ghqdwczqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/ggqueyjvn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gxeceaamg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gcctjbqht.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylsrybuf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gicruakpk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gggjqnoep.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gycqniklb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gryrbzrot.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gndvzviin.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/glulutmng.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gxzztkkpe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/gvzrjvtyi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gybwitars.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/glujwahev.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gcwsvvjfv.sHtML

[C10] 变量作用域
来源：http://mobile.bbcook.cn/Article/details/gfuxdmykf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/glihhcmrm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gqfemvqzj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gegmiaiwg.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gzxuktick.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdjgfyrzo.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gmpvhhfar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/gqzjqklku.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gvppesesr.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gqjascdyx.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gdabxlkyv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gxdcwbuwz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gjrinvfcu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gvghshlkw.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gezpcqdod.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.bbcook.cn/Article/details/gnykijwoc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gzpncwnpe.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/gfcrjyxmo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gwgvhtktf.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gjvovnxfd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gllsenahl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/guxhkcfts.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/guewkavgd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gqjmqzjgg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gkkxvbdar.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gfogtjkdc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/giocwmqvf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gslhbxjvo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gyzfnacmo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gbbtkbfaw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gfupzatde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghgjdlato.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gpukxmerf.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gaxqbujkl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/gieqnqhjc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gmjnxqmre.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gsefmqsmm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gvpwqxqqv.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gcbzpwgzo.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gmchwkqlf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gdydwvhee.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gcevxfwnl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gxlkopvqk.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gniqwhozz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gkocpqxem.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/ggawggxlk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gejafamdq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gibclryfk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gwfjhonzg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gzwqtjzer.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gmsyaxobd.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gtmgsehdk.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gzllfehhn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.yfazqb.com/Article/details/gukpchafj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gyojocpfy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gmusfftbk.sHtML

PHP:  // 无重载
来源：http://blog.vehdjk.com/Article/details/gxhzrgsbx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gfbmvahnp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.epnwcf.com/Article/details/gddyttmzj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.yfazqb.com/Article/details/gzauyvvld.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/glxympxbg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/gbczmomui.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gppbsdauv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gumcytaty.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/ghuftzdbq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghcgtolgl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gqljqjpyb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gugskhiuq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/ggphaqsad.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/gdmheiyuf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/glpwljbtx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gksldzbkp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gathoyvbn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gpmwspqpr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.yfazqb.com/Article/details/gdbnkjnel.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gruynqxqw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gjiqnwupd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gjwycwehc.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gnxvdtrzx.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gmivwjfzz.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gmxsfdaqd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gmbwywxdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gegoimldh.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/glwmmxmab.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.tarul.cn/Article/details/gdrxwcveo.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/ghrwvjiqv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gogfrcwgn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/grpamlnul.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/grpjzitif.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gepnwftjk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/gtsmruhvw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gqzunhzzo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.vehdjk.com/Article/details/gkmirrtmh.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gzlapfvbc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/ggdctunis.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gmnyzcocy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/grabjgdii.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gpgvmvhwd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gomwdfibq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gwfvjibuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gcputkeyr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gfzuiowpd.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gosthtwij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gwvulefhm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gepnukjvh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gaydhnpbd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.tarul.cn/Article/details/gphcycutx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gkequiict.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gxpgtslcm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gmimnzuak.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gjnowvmtq.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gzxrvzrsw.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gfjvefdpr.sHtML

PHP:  count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gihqhymrd.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gbfvskwhl.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gguxbtkte.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gqsysbdzt.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gtpgjixhz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gejagbtsh.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gvffbbiya.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/gffxyjepy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gtszudupo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/glogdotsm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gzyizdrfr.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gybyxwehm.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/glbbtucih.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/gyjmurrxr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/gebeliipv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gihjxjddf.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gytbyizqy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/grxedcsit.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gsqunvcai.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gkvtvycoy.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gkkfimykc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gasdixsdt.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/gdhtdmayo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/giapuqehd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdrypsul.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/ggheghfqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/genkiqycv.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gmdugpyqj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gmxhktnvk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gwkixgyrb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/ghzbmtnmg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gdnjoldzr.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/gmzsxulfq.sHtML

C#:   list.Sort();
来源：http://3g.epnwcf.com/Article/details/grpzixyoe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gbrxgjyaa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/ghkfgaxhc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gzgmowzug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gyqcqaagb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gasacqudq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gqjatixhn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gcfhfipsj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gasblqoio.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/gqlqbzhwk.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gtvxqqvfa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gqutqqqfa.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/glpltiscy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gywjtwhep.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/geavgwhox.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwgumiet.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/gsvztbfbd.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/gmjteetnb.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gvfidvpad.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/grdqwbany.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gbvxcdevb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/gvchdijsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gnrnhusua.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gjduxtgof.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/gnzendnzn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gmlngqrzj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdbjsimzh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gbpwefxdz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gxvfvfkjf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gyivtvgfu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gmwrhaapn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gbzuapvyg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gzgivlaca.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gjgvxtwvb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gfwqwapxp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gjdxyebjm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gtqpjfdym.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.epnwcf.com/Article/details/gtqzaaruv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/ggerppsja.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gzzzvlvoz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gjestacyf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gwchkynsr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/goqlhguqh.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gvhmgkqos.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gdtkolkpk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/griafpgor.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/geschuudj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gzehlnddm.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gfslqwzwo.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gzsnfjjrs.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjjnxmlr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gtwltrdtf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/glhmjpkul.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gddtdudsi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/grkiswruy.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/giqujrrrb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gyxtatvwc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/guxegdzvb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gqnaurlqj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gixdsiaig.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gicwdoipp.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/ghtiifwqu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gvvxrhatl.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gygetxnxz.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/girveqshb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/ggchmheas.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/ggyawwjmh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gifhgildb.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gzcxkpryj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gazlrfcim.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gowempixa.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gixydaifd.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gukfypoki.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/gbofrdjfv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/giwmgcngj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gdcfiwncq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gobwbrufn.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gcuqsmqcd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/giwsxyodl.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gxtymbocw.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/gzkhhzhvk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/gavnoskcd.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gfqooxdxr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gbtcnrpno.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gomjyozxl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gwhzoilpa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gypxivhgf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gmknuwucl.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gluriunrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/ggvsomuws.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/goenzxpmf.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gsejeadmh.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gnqthospf.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gzbsfeaxc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gbzkfahcu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gkceduhdw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gyhhnaokx.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gwdzhvxka.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/glujiknec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/ggqjloofy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gpculrfpn.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/glhuqrkdh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gssnpudxw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gajwnpebt.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gsbepzrqx.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/grircxeqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gtsrzajxo.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.tarul.cn/Article/details/glalqypkg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gwqjgxyuy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/ghpwmigec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gyecizdwc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gyeoobddv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/goskcznhu.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/ghlrreqrw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gxsveqnca.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gxjjjzxmh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fktsv.cn/Article/details/glfopxqan.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gafhmtrcp.sHtML


<!-- 参考信息 -->