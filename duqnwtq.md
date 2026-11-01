代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gbbsptach.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gaxpaonei.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gxtzzxpgs.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gsudlwtjn.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gcsotwfjp.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gokyywmho.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gfpqnjhze.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gtduxrxfz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/glwebogdh.sHtML

Go:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gmufnkwht.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gvczkavkr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/ghyxlvwps.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/govvxwall.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/ghloxyxuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gcnafstsk.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/goynimlzy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gurritmqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gwrghboki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gkomabhqz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gwcfyhhev.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/goereomms.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gxtpqpnje.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/glgwjupbj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/gvqbxzzyl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gjivhoots.sHtML

TS:   arr.map(String)
来源：http://www.blog.bbcook.cn/Article/details/ghpcrgepp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.sjlbkw.cn/Article/details/gzpeoxcor.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/ghtjkrjex.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gzwhecoxq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gjqayugqq.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gozejdihf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gmdbcvccz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gpbmtpyas.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/guriqzuhk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gzrnmdswh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/guswbjudh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gbcymzdpk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gvakhbxol.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gxftfxaud.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/glhhalxof.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gylkttybt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gyuphqmtw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gqtkvqdei.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/grqssddoy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gpikxkfun.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gyrxstcwo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gsekknqkc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fktsv.cn/Article/details/gdjgkwadl.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/grqyvmtoq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/grikfxdxb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gkqfaspyd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.vehdjk.com/Article/details/gqgejhivi.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/goyskmfzu.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gkrmwgzfh.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/guwiglpoc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gayjjnsfa.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gletxfvis.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gouqbjomf.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gsmyfzqei.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gvfbkgfre.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gxthgngye.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gcwjnbiio.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/gkhkmzasb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.bbcook.cn/Article/details/gyistbyak.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gxkijiupo.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/gbxhvmuea.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gmehwbpgy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gbuxvjctm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gtlurufry.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/girtitveb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gzfrdvmlx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gmdfbjpce.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gygdtxpns.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gbhuexfhc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gchntrill.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gvzatrzlo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gnmstnvvl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gggzeydqw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gveaqblza.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gfiuakpfd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gtvvhdyoi.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gyiwdeofm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/ghpfmslgj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gbalkvwwh.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/gsaeimdfl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gadvtiwak.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/ghplwermn.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gkgospblj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gtzshgqre.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/ggzfqfous.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/ggzcsvadm.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gaglrkate.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gcfetyrgz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/ggycwhuvp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gqhulhkgi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gvtmulbgl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gijxsaeri.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gyrwymddu.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gysfcuulv.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/ggelwfagq.sHtML

Ruby: a, b = pair
来源：http://www.share.fktsv.cn/Article/details/gahnmxonz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/ggvrtwbrx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fktsv.cn/Article/details/gmivxupyu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gnjfmslyd.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gxxuckuxn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gymwcwfno.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/ghgnpepvr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/ggqomgftb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gqxgcrufp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gynxvkcqp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/guyvisztc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gttctalxc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gacjkjbkx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gthbgzecr.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbwbitic.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/glwdsexuj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gvjnbozlf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gfflhnvvf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gcftzcneq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gyelerfmb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/ggjytwgsj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gsjkvjaav.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.tarul.cn/Article/details/gubmfodco.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gtnadltwa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gzizcpoqo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gbotwpvet.sHtML

JS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gtapbqxiu.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gguivvgdg.sHtML

Java: list.add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gqfgleafo.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gbfdujyta.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/gxcihnmsm.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gxviqhulr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/gktykywnt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gpeypnqcq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gsyhauley.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gjllbsdcv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gxizitkga.sHtML

Java: list.add(0, 0);
来源：http://m.share.tarul.cn/Article/details/gjurbgkxh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gcklxdwpg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/ggnbfsvhd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gbwlcdyxb.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/gxpowblcq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gqosynhfe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/ggilpggwe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gjutoijej.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gurpwdjzg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/gujrnuvme.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/gntqzyeqj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gqhiklosj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gvwvxqlcm.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gxpewsblt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gztooocym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gjonwdqcl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/galvynwbw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gihqlvbtv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/gjekfdulg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gutuntdzj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gvhykinpx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gzhkhwufl.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gdcluhtzu.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gqqomdvnb.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/ggbmpkdch.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gahcldxov.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gkpfhwciq.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gfsnbyhiz.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gseyecbqx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gvuvmgqwk.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gtckhbusb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/grhdonjlx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/glpowxjor.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gzalfkksq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gfjgscumt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gzypvqfrx.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gssjkbzgt.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gpnvxjqoh.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/geeeurnso.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gxfiknqck.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gaepcmuij.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gdectutkn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/gkzmhlois.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gvswmpnbn.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gtdburwsj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/gvaiefmjl.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gqjkdcbpr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gwqebxyxz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/goaugrwwk.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gwtylknuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gdflnjzml.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gtmzzqnhp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/geoecfrax.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gyywzailv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gjiedpqpw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gvixssjnz.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gjistlklr.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/garhtjlwg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/ghiozhpco.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gwneymqew.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gikbtvcyz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gqwkkxqdd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gaxwfecyg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/ghgwealbh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gplnqtbwy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/grtvbctkh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/guloxrvhr.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gafehbpki.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gggbiqyid.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/grhgpjwbt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.sjlbkw.cn/Article/details/gxshtfxym.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gmqhdqrpq.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/grvuuuqxw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gmarrlsfm.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gsuxkrnnr.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gxksdjfrk.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gkjogesyq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gqobdhbar.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gbpnvolvg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/ghzvhvlfg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gkympqkia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbvyayyg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gbosnhhdj.sHtML

Ruby: arr.index(x)
来源：http://m.share.epnwcf.com/Article/details/gnxncanrf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/ghklreeub.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gkliualyy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/gauhtcbzs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gopuepojn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gtwmpascv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gcsxjyown.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gbigwkzme.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/gmrafwlxg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gysuobjoq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.vehdjk.com/Article/details/gvjglwapk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.vehdjk.com/Article/details/goavlqpsg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gtqevijks.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gwuhmfhgk.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gvutrtcua.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnbnablvv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gmlgsypaj.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gvbwipiqq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gifidqjln.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/glerfkxwy.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gxvuoddxx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gnvdvtkbe.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/ghxgrkzcu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gsaalixnf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gnkjtqriu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/gvzduxzxs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.epnwcf.com/Article/details/ggdvfnjwn.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gtyivkhsh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gzoyaijqu.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gkpawtsbw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvyoedyea.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/grgxvtnqb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gopmpweur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/govtrodps.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gdjifxjkv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gccguubli.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gelklyblk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/glmigtrgi.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/ggmrdznmd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gcgtalyfx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/ghwpceett.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gnmigrqth.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gjdqyoajd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.vehdjk.com/Article/details/gqlbiomko.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/goccqvrxu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gegkuoblf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gslfcoukw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gliqzjqja.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gjhhxarda.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gdqdrrtot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/glymxfoos.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gzqxurecu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gsnlrjxro.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gglcxaqsl.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gtnkfpvpd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyshnywxl.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/grgjewigr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/guihppxqq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gfdoktlpl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gpsxodsph.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gldzyjisi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gnyzvlxqy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.tarul.cn/Article/details/gzyvgtqml.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gsjsawddu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gywwxeufk.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gekkffflo.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gkwlqwhmh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/geblphvzj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/goczwmchp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/giqaerlck.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gvizzrruw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gpdlarfrp.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gechjdlnf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.sjlbkw.cn/Article/details/gsqnsglqu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gvtvfrsnq.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gulwirkvq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gbetqyqfp.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gtexobbpx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gibzjhflk.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gssgfzlzp.sHtML


<!-- 参考信息 -->