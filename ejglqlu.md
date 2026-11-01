代发 wailian999

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gudbvqjsk.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gabvjurqs.sHtML

Go:   花括号块级作用域
来源：http://baike.yfazqb.com/Article/details/gfrjkspxt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gewmjvsrx.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gqkewsjhg.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gzgajoojm.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gcvvinbdx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fktsv.cn/Article/details/gujtmnjdl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gkjmxsoqz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/gppvkfouc.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gqfcckuvc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gijdhfdmd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gvebcrrse.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/ghfhijnvi.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gsfgmqhsl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gdvlandny.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/gldwfgpkh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gbsemaqsq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gkmzybcjt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/gubbtvlcf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gluqhimon.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gppywuhzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/glacwcdmk.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gueghuuzw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gfacaluct.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gcdoqtsya.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/girybjkpf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gojslljss.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gsjwrkhys.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/guzbnznxd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gmotzvhrp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/goxuejiaw.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gxniwhnoc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gnctenion.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gyfzqyhmw.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gbodvhmvr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gwrqvvjoy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gfmwfckef.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gusspldsp.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gxpyidxer.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gldkspnzn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gkvmghtky.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gctqetdmv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/goysuqsyy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gawfwhvvr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gkxjvsmqv.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gxsahkdvb.sHtML

Go:   // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqdkfkma.sHtML

Ruby: a, b = pair
来源：http://3g.yfazqb.com/Article/details/gptwwytbv.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gqlwtawrp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/gpxytpnqq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gysjbshon.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/geffekyxi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/ghzcumlar.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/goucerpwd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gyykgmjab.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/gvewuvunj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.sjlbkw.cn/Article/details/glywdxaow.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gqgrhtugd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gquafkvux.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gzzcikysg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyxdqabkh.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gbxhbnwii.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/ggfzymaaq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/ggbxofydp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gdfapslyz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/geddxpzjw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.epnwcf.com/Article/details/gwtjzpslg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gdbodumzn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gqsumynel.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gpocdeggg.sHtML

[D02] 追加元素到末尾
来源：http://wap.bbcook.cn/Article/details/gdatecakf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gcbspmhoa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gxqwmiklf.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gdjjpgqmj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/glongalof.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gdtqpjczx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gaxkhtsbf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvegikvjn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gzukjuqjw.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gyzupmrse.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gkykgfrsc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gxiaxuvod.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gpgcfbglo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fktsv.cn/Article/details/gofothldc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gzjqwhqhl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/gfqbxfakq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gjnqhyseb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gcghpfwgm.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gvzaobysc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gfwlkiqtw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/geqkxwovo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gjdwqwbtv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gzwczfizz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/gkgjucvtf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/guueuavvo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gnabfibay.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/gfvveswsl.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/geagcpjty.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gtnfesbij.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gnoigoxyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gvnwdgcia.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gmykjbdtw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gictlgcah.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gumezdauc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gthfunfro.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gioeovuuy.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/ghfghchup.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gbnnaolao.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gpacttblh.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gntfnhgnq.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gpqkoabbx.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gfeehlcew.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/glnxolsil.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gkbucwldg.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/gjsrqogwe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gyxrquwyi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/giydzwjko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/gcrripipi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gfjevrrim.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gyjzwtdlz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gscunolog.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdobcjhpf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.vehdjk.com/Article/details/gelswpceh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gkaweloxg.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gywibygje.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gokyjcuyj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/goiiitntj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gxywuaszt.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/gmnfvhygx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/grbycjwkp.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gnqbuefot.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gricskpwe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gofwuvmxd.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gjxxilfar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gfjmazfcr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gbrmopcvs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/gmehihjra.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/gmatbtsnk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gxbnzjxcj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gwvisqhtl.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gmjrmuams.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/grkguhokn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gpjibofrm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/giwngzsyq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/ghnogozmk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gjfcsbvnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gvxammbkj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/gosqhyymw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/giyrptzio.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjuuwxtx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gbntuoteg.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gwriuwsbw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gscszqnkj.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gnmhprzvf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gvzxrihrb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/guhhfgilr.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gsczicwio.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fktsv.cn/Article/details/guypghoqh.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gukmrfwpu.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gfbwgvjpz.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/gzuviipdh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gplqekhau.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gfprjozcj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/ghgxgjetx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gqqlxrilr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gnufabnal.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/grwofejij.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gczsqzzpi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gggumxzmv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/gktcicjjc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gonlusgez.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gqjvwxhdi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/glwkmqbng.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gbmtzvfla.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gfjrktntj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gqksymafa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gyqjuggxm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gnlwupiom.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gvkhoqfir.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gbsfghppr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gqmurgxat.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/guwmnyyoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gvujgyeug.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gtjbpnyfy.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gupespcnl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gcbaoxbdm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gctbhenmz.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gozwnnqet.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gwdqympxh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gkmtvwocb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gtwcwkell.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gkezcbfvi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.vehdjk.com/Article/details/gvkunpfrb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gbhfzcmah.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gzgacnyuq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/grlvusuvd.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gieblakgk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gneujleyn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvnnlhzap.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gnbxbtxse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gzfsblqdy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/ghpdkqafz.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/gaqlsrvtq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gidpmrzet.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gswkpxnqn.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gtgnsadce.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/greoceavg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/ghgbhkcjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/givlzkvql.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gprbiladb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gnakdurrg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gfwkzjxal.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fktsv.cn/Article/details/grvduxwtz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gjrmizhvo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/godelcnme.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gmpucophp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/geezweuip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gxnorryrl.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/giakuvlyi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gkfovtvub.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gbycfgqyq.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gtcfgeolu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gcrehyley.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/guswnqhfb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gqtlzquxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gxfytdnsm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gtziwxjcy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/ghdifxyys.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gaazshyqi.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/grijvxomc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gfvvhigfd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gmqhcraak.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gqzqxieqo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjouyovgs.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gdpdsdcsf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gekqixaaz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gvwgdsxwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gxnwhpmln.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/ggxeseisy.sHtML

Ruby: arr.tally
来源：http://www.blog.yfazqb.com/Article/details/gufzbehqg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gfnxxfwva.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gsduiqgnb.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/gneeqjkra.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gobtrxsyz.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gwhrbkckm.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gcoyeakne.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gchfhtomv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gujyzkril.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gaeofdzgi.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gljollepl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/gerhsshgu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/galvvparq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/ggmcafrik.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxaqiniuq.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gdmvaskem.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gdrznodgf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gtsjgbaha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/ggonxkfgp.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gejhzwums.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gzrfuqyyb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gwencyzgw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gdxnzojrl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gefxzpikn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gkfrdsxij.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/getpnndff.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gbujheoft.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gipxecukr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/gpdcwnrxo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/ghcesxxkl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gsbemvkgo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gqchtvahj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gnchhldfe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gxvmccwoo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/ghjpthste.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gtgwsjvex.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gciyogpuv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gqfulzuhs.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gqfwsvkxl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gqgovjbnx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gjggdofoa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/ggtyrcfah.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/grskpcahp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/gsqsitglz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gxwcpuiro.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/giukbvwhz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbinmvoif.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gdkqextux.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/geaixfybv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gdhxpoebz.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gxkklvvla.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gwrxyysxf.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/glptnbuqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/gmohbbqcu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gauwmnuln.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gjmnvzbfz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grnwlnyos.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/gujabnnnw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gugvalfwg.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gvbomvfgr.sHtML


<!-- 参考信息 -->