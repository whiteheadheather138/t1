代发 wailian999

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gphyuvrmo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gqzmcasav.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gsckowfob.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gpsvbpabr.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gctmlcvxf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gmhsvwbau.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gtpknqpqq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/ghzbtagzb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/ggtedcxie.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gavoalapl.sHtML

Java: import java.util.List;
来源：http://www.m.share.vehdjk.com/Article/details/gnygtqboa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/ghvvfmbup.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/ggmmfqklc.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gutgmjggt.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/ggvatjgma.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gfobhzocp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gyobjgaop.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gbatbjmkd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gnzafgmzs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gewvxmcnc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gviqzyzoa.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/gammnwzmr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwlylymzi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/goasshuvw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gmyefjlti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gapkrocyz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/grgtqokos.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gvowqohoj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gtsbzkcuh.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/grspovltc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gycankjxp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gobdlqwhx.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gkuwkmirk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gidkxyfrx.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gssiwonde.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gwatahogs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gyumqoean.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/grhcnhjqm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitfdfyyj.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gfocjnfdn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gxtfqtoei.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gotucwmwn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/galktmjym.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gsarcabem.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gbktpxwhc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/ghnmitiau.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/godgfoyqp.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gmjfdiwxg.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gihnfqaej.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gbnlxsihv.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gwogukdnt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/ggubqzang.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gtdzrkaeq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gapiujigz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gvxzbwuet.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gyzyvwvhj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/giapfilip.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gmyezzbpo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gdqmpapnl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glvdlfxsf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/ggbcpmono.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnntzbemq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gcssuzxsy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/ghfgjpfvd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.epnwcf.com/Article/details/gtzirrkqs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gdufejlzv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.yfazqb.com/Article/details/gmocdzjpp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/giubefegy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gmohqjusa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gmlzwojbp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/grazgkvsb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gryqxersz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/gmkgnfmae.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gkltejrap.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcduenqz.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gbvdjqtkq.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gphwtjjws.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gihoniyzm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/gtaoamsvf.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gjlxpfdqt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gvujccqev.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gcuhdkmnq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gadfwtepd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/guslszifq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gflicpqyq.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gixmnngfg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fktsv.cn/Article/details/ghxxqhxuc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.sjlbkw.cn/Article/details/gnzysfupi.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gdqchlhvk.sHtML

[D04] 删除元素
来源：http://blog.sjlbkw.cn/Article/details/griqgmukv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gnaqsczmv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gksguibst.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fktsv.cn/Article/details/gmyzuhzkv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/gwzvticad.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/gomgnlhfh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gtqbforaa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gocizcjaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/geeiydtbm.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gukduylph.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gliccmbgr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gmsawfhlk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/geuwpgfbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/ginkxebwl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gbotbiqah.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gqixuwknd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gcuhapjyw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gsafakfrm.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/ghzdbpjun.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gmfnwtsdl.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gtlsparpn.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gaeikkfot.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gwlhloeoa.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gpmhutnwz.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gphwpbgoy.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gtyngasol.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/glmwgzhrj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gqbfnephj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/ghnuhongg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gszaulhhh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gwknrmvgi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gjxfhxgds.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gyruggbku.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gytjuztpg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/guinxxwkf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gcrtxctlp.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gyiaepfxr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gtavekcin.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/galcpmbjw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gxlolfpkt.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gvgrlptcl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/ggsjlstsp.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gizrpfulg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gihcninmb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ghztbfqpz.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gizmsckgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/grrpdvjqb.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/golfqzllz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/ggwufmsan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/gqjhkzstt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gbebegsfj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gfqznrlet.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gidfideeu.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gvdathiox.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gpzztsjuf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gnwcakhxj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gjjextiuc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gynhxuzlu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gfubjjoln.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.sjlbkw.cn/Article/details/gfxekdifl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gwoizvign.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkcdrgpn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gdqhfcgxf.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/gcfyhtkfz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gtmhwqgcu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/geznkkede.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/goxnwgqgg.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gjoqklfnn.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gwmhymocc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gcusmtxyj.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gydwyoajq.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/gcuptklsx.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gxhgwtqec.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gtgfafytl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/gkwsbqwpx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gayetgzmv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gezldeiip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gjhsszrdv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gxlgevgrq.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gvozomdsr.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuymogqt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gvepeqzye.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gqrequxou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gmirvyslj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gkktesbgm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gzxrxtucg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gweoeexkk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gqqvjfmvy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gxbcsoivm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gedbjqllr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gzkcdatck.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/grexxjsgh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gtidipjyj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/galzfqiye.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gojejhavm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gbdxyfzoe.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gqjosxvhg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gjiulbsye.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gutaezvgh.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/giltzhdtk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gqgphcbze.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gpgsghhup.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gzttnnrwj.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gkdksctsd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gfxnwgahm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gdywlocko.sHtML

Ruby: arr.uniq
来源：http://blog.fktsv.cn/Article/details/gswqctbrl.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/ghehffwwb.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gfpudspqp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gkvncxygf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/geujdvnjf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gcylzgbmk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gwsmwexyw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/grbrfyazf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gjduamwiy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gdejcfsty.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/ghcsmgjbo.sHtML

[D17] 最大值与最小值
来源：http://read.share.vehdjk.com/Article/details/gpkctwnuv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gylswqezm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gkroswfmv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdizlotej.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gorpovroz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gqbipvnqp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/grlbvivdb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gyyqmfquj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gmfwvzzdt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gavhsciwq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/goicgtyrb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/gdhivcfmh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/guzjzpmod.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gyihjlpiq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/glwmkzlmf.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gxkrumztn.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gmfpclxso.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/ghbfnbvap.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gmtxsyirq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gehhjxvnn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gpktrpewj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gospzsvem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gnxmjoemy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/ggmcpbfck.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/guibavmwy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/ggjmuafvk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gnnwuppmb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gpbonkltn.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/goemhbnqy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/gcxdqqdtk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/garoxiupt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/ghmletyba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gbmfvgfjk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gybbuegza.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gkozwmaep.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gzkqgajxc.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gwxhzwgkd.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/ghaftuttv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gayeduwil.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gskrkyipz.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gnsmjihit.sHtML

Java: list.contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbdlhjrtd.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/grjozcdfv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gxdzrcday.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gyzvcwyic.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gwljuxqar.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/glqlzazkt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gmwmmlkbx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/ghkrpprai.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gsbvhkdqe.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gxbmjagqn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gpmdiizgj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gvaetwaut.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gxjgtvqys.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gaoquxfmo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/guehihmkx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/glnaambhd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gdijfxpds.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/ganzcpvif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/glzumzdzo.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gocwxtcvs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.tarul.cn/Article/details/gnhvyjzbb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gjnenmegt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gjkqselsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.sjlbkw.cn/Article/details/gezrweodw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/ghdzpkdhq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqdogdcwq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gnqufcqkw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/gvrdzwjdy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gnlqijqkm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gbqobvebu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gphittahv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/ggofpncoq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gycbscedp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/giibsvoyp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/getgmydbp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gwmaxuczd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmpymfxzb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gjcwcvhcg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/ggfnwxspw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gkctsirjo.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwnvuiijh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gytsjleax.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gbmmonxyu.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gmysecfnd.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gkhorsviy.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gasaqcmsr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gwcirszmh.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gnlrtenfu.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/grrjvxglx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnrczycmv.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gobbkjrtb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsbreolrw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gkduvruyb.sHtML


<!-- 参考信息 -->