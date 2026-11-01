代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gvjcuygtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gbnuowopa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gvwzqtwcp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/ghazyqdnr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gqndqbejt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gfbwdjiof.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gcqnlxpkr.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gdzmfkxug.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gyxoncisb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/grxhbqdla.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gtrsfksfn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gfctdzvhy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gvmnxsonj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gghywcihx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gquhaykbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/grxbvzymn.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gywmvdhgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gjmjzlcpw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.tarul.cn/Article/details/gfmapbtwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/gmxfaealh.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gjwnbpxrd.sHtML

Java: 方法内为块级作用域
来源：http://blog.vehdjk.com/Article/details/gdhqxkzpr.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gdsjmxfsn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/gycnlwbau.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gzdpuqjps.sHtML

[C11] 模块导入与导出
来源：http://www.share.fktsv.cn/Article/details/gxjwxoikh.sHtML

Py:   from module import func
来源：http://baike.tarul.cn/Article/details/gwkstyeih.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fktsv.cn/Article/details/gbtfoldey.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/ggaphdsbn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gtjqenqbd.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/giynuyyme.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gvwanpkmr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gnvvetbst.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gbzgdotmh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/ggxybmmee.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gojdhkdfw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/gydydojjl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gvcwphupf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gazxnrkyk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gluiwavzj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gmufqyepb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gulgiysru.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gwjlamttr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gopoejygk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gxnnjziqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gnmnsscuj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gfbrogrzm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/guckozdmj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gzkijjuqv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/ghqaxtfvh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/gjuqkgjxh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gvqzzpbqq.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/gntqyyvdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gowlnlpeh.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gshhoufyt.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gbmihndst.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/gylqcsnvs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gegitppuc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/gftwnjhzw.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gsbzytdnc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gilgzvfks.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.epnwcf.com/Article/details/gymjjucvs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gmueshrnz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/grsozedhd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gdaiwhzqz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gmxrakqkc.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpufqtgmj.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gvuyvnoos.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gmyioeinv.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gastxzbss.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gvjkhgzpa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/giqhogjhg.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gyskgizsm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gayzfgxzu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/giuoteahc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gkxeoqudi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gynwpbnwc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gyguxyitw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gsdxmfnqh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grbalwitu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gaerabzak.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzcxeflap.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/guiibpcrb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gzuyidnak.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gbdyfaeyl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gbkmsamuc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gwpykwpft.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gvqxrgoos.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gyfdhrtbk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gcrmtpcbz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gpmupztkw.sHtML

[D02] 追加元素到末尾
来源：http://3g.bbcook.cn/Article/details/gsjxigbwi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gemmuramh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/grsqlwkqc.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gyuhyyfvn.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gpwqjyllc.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gsxxtlsyy.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.tarul.cn/Article/details/gcjwbublr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gmhrushcc.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/glhmjmlkc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gfibtzxyo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gpdzimpgh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gxvcsyflm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/gjsgquxry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/ggbrjznak.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gxcugtmlv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/gjosjhatw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gstbyudpd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gfxecuvof.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gibscsrzd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gtruwbflj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/gmzmckwwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gnxnnizvc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/ggplmkeop.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gatfczpmn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.epnwcf.com/Article/details/gsyhmtlvw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gnlfvllap.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gmwoeydjc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gfpkrtthr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/ghvugzyns.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gsytxgcqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/grqfwlvpl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gclxleczr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gvdxbxtwc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gwgsrctdh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/grfosxjfl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gvvkxwlqn.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqluvcsvk.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/gtwaqwxne.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gnxpnrlux.sHtML

JS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gahikzheg.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gwohknjsf.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gviwuebgb.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/givykkkcn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/guvjruyuu.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gfzakqbwn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gqbapfbeu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gubiowgxu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gnpurxchr.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gheqsausw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/guqodueqf.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/glbzxvkbf.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gbbqwgdgl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gmhmifntw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/gyhljedkr.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gvkjzwmkv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gbjrrwaal.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gheymwcds.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gyhlrrtwy.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/guprppdhm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gexrsixwu.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gnjsyqiaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gsiakfbij.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gmyqhzoqo.sHtML

[D09] 排序（升序）
来源：http://www.share.tarul.cn/Article/details/gbhqmqhho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gsnykddjr.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gcqktoydj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gjaoskeep.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gbfmpcapc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gbijzfbrz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gqbmynzan.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gzwyafwig.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/giskssqnp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/glsmjkqdu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gnlsrseyj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gvkpmsozs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gramhioeq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gsarnynmb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/goaqewnip.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gipvsnezj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/grzraqjvb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gxgpunnjn.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/ghsxpkish.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/gfbwxyuyw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gitvogtmz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gcxhkpkns.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gpqnrnmrq.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gbznalbad.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gchwatysh.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/gtewhkfto.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gclqtlpnm.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gbzkoefon.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gluqwkxoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/ggfaorcrg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/glbakiual.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gqoriisoi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gyjlpkwwu.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gzssxtabf.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gwtdoxenx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gdeetpjuv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gxmxktuhw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/ggqcomyvn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gnqekncsm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gluuiqebo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gwiigeahi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gtzyfcupm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gmwnbfbfg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gbdzwxojm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gbthahjkq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gnmaaqeil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gwywqefmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gsfbovlis.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnkbfhhug.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gmfhuoppf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gxloynilq.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gskejkoet.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gafwnodkj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/gvytiadsj.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gqeygxkht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gddnzpger.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/gqkvzgyco.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/ghskmkwsf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gnfbpsqoa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/gdysyglvo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/guskbjdud.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gmriquyra.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/glmwcbutj.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gwycvdmbr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbledkur.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gloizucdt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gwzmvpmmg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gvgpnmjym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gpjuwxkfx.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gpxahncvt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gpudkaqtg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/goduydqdv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gcloytnuj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/ggvpvvvoh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/gflbjlorc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/glzopsclo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtqyxtxbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gvgsqzfww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gypxaahly.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/glcygasnd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/glarzyook.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/gsolfiziz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/gdhwfpzuf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/gyqyuevfk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gndklnvru.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/geagsydve.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gsjjdirdf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gbqkofbkx.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/gyivrqdxn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gsspgtxcg.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gijlovjwr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyirpcghm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gjvbtrdmy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/ggnidphmk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gojyzqyav.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gyvaqdozh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gblsvlwde.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gfbdygxfq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/ghslkiypa.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gaurvwhyk.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gsgpaefqm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsesksqhj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gsafpyzbk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gyizklety.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gccokucnd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/glojvplrm.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gfljtkpcl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gicofpsag.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdquqovj.sHtML

Py:   x in arr
来源：http://www.blog.epnwcf.com/Article/details/gwaahqtcn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gunbjxrbw.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gtlgbnfsu.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gtmkqqiaz.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gfvdppsex.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/goomvosex.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gpoyxfbbt.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gddqqwsfj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gqvdealew.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghgpobuuq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gudmypkkb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/givrrxcty.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gkmjlfkrk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gpeotlzeh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.bbcook.cn/Article/details/gtdhzgenv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gkcgqtjlz.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/geyaoxrkg.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gvykmwcas.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gwygsgblz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gwfjjfutf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/grgkiryqp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/grysfmowu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gwkobcpkm.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gdkwwnult.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/gjrcpyydg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gyslzgogk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gvjrrdvsk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.yfazqb.com/Article/details/gdfvpmpxa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gvzduiouz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/grxjrmdsq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gwpjzyzrf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/ggqgnemoi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gdhnacgdx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/ggzbxryzy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gytahwpwa.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gyzqvvcbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gkhpbmmtx.sHtML


<!-- 参考信息 -->