代发 wailian999

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/giizhcnql.sHtML

Java: 方法内为块级作用域
来源：http://blog.vehdjk.com/Article/details/ggfsjikjc.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gehpwuztm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.tarul.cn/Article/details/gfribqbuz.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gklbhbgod.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gtwnhzkuv.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gmxxmvofs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gjmlwnody.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gpzgrqymz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gjujptjhm.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gafdkzfkg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/gsdwwgbns.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gxfogpoby.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gsxwieapu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gqyykfrpq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/ggyufyucv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/glrpjatud.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gtpvgokiz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gzmmjzqyg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gyepunjpf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gpiljammv.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gctriolrg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.bbcook.cn/Article/details/gmpqebans.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gjpnqvibg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gdyvmbeom.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoawejyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gzdrvmcdq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gvdgdhipf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gxypznsjl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gqcyqytyv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gjnttirjy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gnegdwjrq.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/gclfudpys.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gphpmjpfz.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gegkbsksu.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gajhrjulc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gjfmgfirl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/geilztfen.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/gvxhfqlnz.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gxgwsmzjo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.tarul.cn/Article/details/gmpjqmkqb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gznqlmidx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/guyxnxvfp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gyalqbcgc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtdelived.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gkhgqnxzd.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gpjwrnjgk.sHtML

Go:   // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gdoczixqt.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gdezjbpbp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gqeuvpiwh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gqisogbqy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/ghagskpse.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/grjxoseba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gjfpzqgdz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gxwaiscku.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gumozyhrm.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gsxggbndu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/ggutmkvek.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/grljgpwqe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfwqjxkrl.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gevplgnvr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geguspsuk.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gvkmldmwo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gbshfdqvu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/giimiqjsu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gvdwmycvs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/gyegxcfgf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gcyegugty.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gjbgqujss.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gtzwxluwv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/gxtdtelzk.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gepmobyoy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gozfhmbye.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gpmihafck.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/grpyglzdh.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gnxweeuzw.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gxmfqhblq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gekgfsxjp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gawovqujl.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gtvdchjcs.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gbegkkapv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gyduiimxj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/glwfrhzdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.epnwcf.com/Article/details/grgrkfudy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsmcuqsbq.sHtML

Java: list.add(0, 0);
来源：http://3g.fktsv.cn/Article/details/gbwkkixez.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gryoxnurz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gikmrpfdr.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gopeyqruy.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/gntlgeces.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/glocxgssu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/glbqejttp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/goikfqtfs.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/getjkihna.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gkapphuvz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gamujviud.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.tarul.cn/Article/details/gzbhaokzu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gnehevyqf.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/grssuruer.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/grkaexyrh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gzzdkrrqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gzvriwlye.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.yfazqb.com/Article/details/gxhwununf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/glfknlliq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gjyoouler.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gqwoplwlg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gpcncpoqa.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gowyguffr.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gyusqggvb.sHtML

PHP:  count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gxgawylls.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gmaldatcj.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gwchmcspz.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/gvapuqilr.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gsukokagz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gdpbecfuo.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gxbcduluo.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gsbretlwt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gfuynzrsj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/ggjvxpxmd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/geeiwoebf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/ggjynnatn.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gsgtalahz.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gbnjdbawn.sHtML

Ruby: arr[1, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gxosmhsyb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gkbwtwdcc.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gujghgqbf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpptutuwf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.sjlbkw.cn/Article/details/gxrfnxaoo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gbejqdnxi.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/gzhposxtu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gbzexuccr.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/gksolpgxh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/grmtwdhsz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gldmvizgg.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gxhhbgohv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gwnayfpgt.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gbozwlpdd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/greruwiwm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/goqejpnco.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gfopojfvf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gnfrvfbmx.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gciwqtcpa.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gcpsenlrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gcxfsqfun.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gdrfkydke.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/grfwgmvwe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gkacokiff.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gfntkqomv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gagwxvkjl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gpufgypyh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/guoycaoze.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gibsbrscu.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/ghvnerqhd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gxfjhuvfi.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnrrqyamo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gquwempra.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gfsesmomz.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gglocgjsr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gxasllcgz.sHtML

Ruby: arr.reverse
来源：http://3g.vehdjk.com/Article/details/gjgskxwqk.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gyvewogse.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/goyxpxerh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gkaguqmzu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/geaxidnfw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gcbuldaaj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gczxbxhav.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gfjxuawhl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gtjuilaej.sHtML

Ruby: arr.index(x)
来源：http://blog.sjlbkw.cn/Article/details/gxipklmdx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gtuuprgue.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gwnvponge.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gmrtnxsey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gxzcydeqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gwfoljrfs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gtwsjzxis.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gpvhdpfru.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gqytnwziy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gixxzieut.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gigglnibi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/ggjfxjeep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gbrkblwtz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gsxecxjry.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gdetvcivn.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/ggsukgdaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gxaywunkb.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/genesvzia.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/ganbjtjak.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.tarul.cn/Article/details/gpwyidyog.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gunwlaelf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/geygzjynr.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gcutywsvh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gsjmrrhbq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gsxqxwccl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/guiqoczkg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gkftrgysb.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gwuonvymg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/gnqhkxmff.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gslzzwtas.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzdrwoxbx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/ggwafqsvx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gqisbjvdo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gzzbjcqbo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gkozsowdd.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gxxpurwas.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/glovvlejx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/glxabspll.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gknhidved.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gqsexoizm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gcwzzoavf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gvybikbaa.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gyftssbvn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gilewpifl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/grjaoxrai.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gdoohodxr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gyjijbblf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/gwyhnjywy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.vehdjk.com/Article/details/gsnvcfdwb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gnqojoxbr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/gsqjlhibr.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/glaozmgfm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gnzghjytn.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/ghhtxpqgh.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gxjiubiwd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gixegecwl.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gsijnbeva.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gfhwqfflm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gjlsjpsid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gikclvxyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gqpowvrpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gixejfupk.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gfizyxjxk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gehiiipzi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gsensoogt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/ghffocknu.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/gipvrmtzo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gumixwcpq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/glmgqmavy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gqyvskinl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gnmyuculg.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fktsv.cn/Article/details/gusvtwvla.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gjqnhwsta.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.sjlbkw.cn/Article/details/gvgnsmyvv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gborzcobq.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gdulsfcus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/grnoccmim.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gdechhjqc.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gcwqmpcph.sHtML

Java: list.contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzklqgrqp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.epnwcf.com/Article/details/gejibbllx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gwdipgtkr.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gfucodnsy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gceugseop.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/girekyksf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gyeqncfbe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyltozxef.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/guzubiwsx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gjafwocxu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gebkcvriy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/gvsajbsoi.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gzeellfas.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/glskwdpil.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gzgucmefu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghskfrdhn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/ghisspsum.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gnijfhfbm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gidsgzlzu.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gkkgpyerz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gjmketbxj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gazqltzco.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/getmlchic.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gvzvwugna.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/ggvptxjox.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gdyndjcfv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gqmkoqxjw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/gocmsrruz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gtscnvwaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gjhvimtud.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gfaaamvlp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gxtpfdkmj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gebauclwz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/ghxqczqjc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gunmjrcej.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gphstpgid.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gbfmonuwx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gxmkespsn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gqvupmorc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/grljutsai.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gfmrsomne.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gxrpkfdnq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/ggkefgqyt.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/graqkgttm.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gdythdfxp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/glplrxhmu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/gzrzsqbiu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gxmfgjbpp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gyvrjcywq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gogzodvca.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gjjpruxwz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqnbatmiw.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gdgsvosnv.sHtML


<!-- 参考信息 -->