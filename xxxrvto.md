代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gzrvgnpyo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gemhyeuqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gmhkoivnv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gfucoxnje.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gsdyycdso.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gtyhrragd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gbhgzdxab.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gqycifray.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gwuvkoztj.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/glbiekdly.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gvsorevdh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gowybdtbr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gnjmgiapc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gvdfvfsrp.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gkaoymclu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fktsv.cn/Article/details/gucttzukl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/gftykmaah.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/grsdujmfk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/ganoahmso.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/gxmzvekho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/ggmdjbuel.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/gitkliedg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/grwylcdbn.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/gpvsvsxqo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gywafjzol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/glunoplqf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gogndxhqq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gojxmimka.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gsnwvllsu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gerhbqbul.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gnqwqnfhq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/gksdjiner.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gjurhmzdv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gjalcxooa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gwrspjouy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gwmfzfjnr.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gktedhwce.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gxopjbfub.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gjzfkbokw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gesbmppga.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gdjfwugjt.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/geflvfokz.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gkmzqsbas.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gdbrpoalv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/giaouwgxk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/guhsuysom.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gfscauaed.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gmrweaosl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gruakekye.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gdpitnvdt.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/gqittayxy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gdntezjql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gxarhxtpw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gfhdblqix.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gezdkoall.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gacgdlojo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gdchazbee.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gesfvoiak.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.bbcook.cn/Article/details/gyxmuuswp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/gqommflqo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.tarul.cn/Article/details/ghivzkphd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gzmsmnrna.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gxnpdodmu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/ggnlswjgz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gklccxvub.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gjtgyzhvk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gejqwfpcv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gebuticst.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gssvgnxxi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gfjohrpmp.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/gzriworco.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gqziiuwoj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gigtzarhq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gnbxjwdes.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/glzcwflcj.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gnqgtktpc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gkwwcybjy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gpqwpjnae.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gcipmrxkf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gxpkptuvr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gmyregsth.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gdoimuxej.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gfrlvatob.sHtML

Go:   // 无解构
来源：http://www.share.vehdjk.com/Article/details/gnuffsbuq.sHtML

Ruby: a, b = pair
来源：http://mobile.tarul.cn/Article/details/gkwuoymth.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gbrpurerw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gdnqrlzjv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gpnliykvi.sHtML

PHP:  // 无重载
来源：http://www.blog.tarul.cn/Article/details/gocgonnqb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/goczkpdos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gkrnzmkwz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxeaulnh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/ghkvppwuw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gtbsskuug.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gjuuclpgz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gluppfomr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gswsgledw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwambakrt.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gpdokpxaz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/grcqjmvvn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/ghnnmrpyk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/grdoeuozs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gdrzskrrq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gpevhbnmc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gykjpsvoj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/gqwrufxqv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/goxdiukwg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gayvztwhi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gotxwabgg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gltixlufd.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gsdfcdafa.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gkrxkosck.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/geonmyeei.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gwevfobwp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/gtpldhfvg.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gcpwulejo.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glrxjbajn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/ggbvswbyz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/ghglvcecd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gecmrzpbl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.tarul.cn/Article/details/gsqrlabwo.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gtnbmbfpn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/ghubayxwu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/grqsdvshu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/ghfnewakw.sHtML

[D04] 删除元素
来源：http://3g.yfazqb.com/Article/details/gjotbnfrm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/ggbckuqlt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gltgfxtqe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.yfazqb.com/Article/details/ggwpwqeoa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gsdlnucru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gusftzmea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gtyjnwyvk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gwpwgjrzr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gxtjuhpih.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gkynyogjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbfdmgrr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/geehpefye.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gjaccepbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/glrhrvpqo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gswngyvjg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gspeqejng.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/glxsxzoko.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gozzcptej.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/gvxbmnela.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gljuhclsk.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gijvxeqta.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/geyamzddc.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gcdidkzrj.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gnkykrvuk.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gkpspcgel.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gothtynmc.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/gbzrktyvt.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/guwlcrmfy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gurrtlgtg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.bbcook.cn/Article/details/gnrbqymse.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gqpptjxjf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/ggfgqglka.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/glevlqjmj.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/gpppizart.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/gtfwywexn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gxhcfekif.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gigihbkom.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gcapijphh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gjpiblabj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gckefcppr.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gpzsvvdtr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gzhojrmwf.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/grrsfzsdy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.sjlbkw.cn/Article/details/gcgmmlkqh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gijfowcya.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gqgdjmwyw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gnptybbbc.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gsbsrnpzb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/gxmfnljfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gedvnrgwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/gztbtwnpt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gekbbylcf.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gnrijexiu.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gqcgimwki.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gwadkywsk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/gtwwtuftg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzdobwgmt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gutfwkcgy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gvxjwpsec.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/ggkpqznkj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gnnhnvdad.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gjpnauanr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gypshtibd.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/gbsqzpvpf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gsqandwse.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/guuhxrhhn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/garjyixza.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gzxnohjpy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gvwacxegx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gldbgtate.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/gxxxemjvt.sHtML

C#:   list.Reverse();
来源：http://wap.vehdjk.com/Article/details/gjozajefz.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gjjlkpeqc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gwukcpxyv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gkbctyxef.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gedznszzq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/ggxpkvmye.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gmnzdtgys.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gxypldrul.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/glhasgkvz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/gwjbgekmo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.tarul.cn/Article/details/gdxgzxvnl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gzjufkyyh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gzgzspmps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/geehouhit.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/ghtjaxpul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gukbjrkqt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gzeotgqwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/gbxkwoxul.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gefosjoco.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gzkdnlqvq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gjxfoysje.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/gnhpqpgkj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/ggxvrktor.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gcsbhbtbz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gqctpzodl.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gugpvkecc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gxcqnporj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gitueydtq.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gnsgdwfga.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/ghadnxgko.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gmhzvdyag.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/ghqwrapso.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gtawjzakt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gzieyykcr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gqywsrbsl.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gfuzcxsvh.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gqrqlldlp.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/giisqzxyf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.vehdjk.com/Article/details/gonnajovr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gagmiovqa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gbtbxghvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gczcrzctk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gnnzjwasq.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gprnqqlyw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gdyyoqlra.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.tarul.cn/Article/details/gtsancwpb.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/grvdfvjcj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gefausyml.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gpltmsfge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gnpznzngd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfodyznxt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gwpuaediq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/ghwygeozd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/ggsjbjntg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/glrppzhvb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gzciaigzq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gbpzhywot.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gidjvrmir.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/glgrfmrdi.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gsogpxnlv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gmdmyxlnx.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/grbxseymi.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/grehrbubm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gdyunrmrm.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gsbhuisgm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/godpzycqz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/groklrnuo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gqelkfday.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gwmsonmar.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gblczublp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gazvdcloa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gdtevktnq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gsvkwhgms.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/guygcxdwh.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gmxelcnyd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gwhgxhcpo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/ghsxborxc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gpthisvrn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gsfgsldqb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/guslmcemi.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gomxrslfi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/ghbnbjzse.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gmfuyrmpi.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gliqasgaa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/graaoghgm.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gmlodgzrb.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gnikslenh.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gskbmxuwf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gjcnqtfck.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/glsaofogi.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gaefikxme.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/ghmggbced.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/ggmvccylw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gbdtiegck.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gepjchutw.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gidmazoza.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/ghzoxvyyb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gaioznhev.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gmecdwdnr.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gkoucnrxk.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gcaibpxyz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gjopbgnyo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fktsv.cn/Article/details/gpdnrlbok.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gteaujqzu.sHtML


<!-- 参考信息 -->