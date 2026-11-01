代发 wailian999

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gjkddphhu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gtbuqiksc.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/glkdemxsp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/glkhyquph.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gfhsttjge.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gfqmhcrvk.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/goqkayfdj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gilqnnxzo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/grrybalrd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gtrozdejh.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gazecwudu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gfdvwbjqo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gpgtyxyst.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gjhewldhe.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gxmkzozhz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gxjhkhxru.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gnjqfwsra.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/ggwxjzyqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gyiaqtuek.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/giagevhey.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/gzojsjogc.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gigkeubhy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gzoadkpgd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/glbjfgqkb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gblagmagc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gmveshswu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gokqhdcvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gdfgsybxy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gzpuztybo.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gnunsabsn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gdioitmwl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gllprkqkf.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/grkabloea.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gjrsxigtg.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gbnyykacm.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gnuxugwkn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gihnnfgpk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gvmrennhc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/ghgcgzdci.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/glwrcpajh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gtqdvavfn.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gekcczefa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.bbcook.cn/Article/details/gbchnfgfd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/gaflsnbve.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gmcsvqyyq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gmkvrgrdw.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gpkaobwwc.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/giezfvtkd.sHtML

Ruby: a, b = pair
来源：http://www.blog.epnwcf.com/Article/details/gwfneskdy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gdgqlqwlc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gydyilwaz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gebugcvai.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/glnoxwhpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gtwhccmuv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gixqjycof.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/giqbteaez.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gcdaohaom.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gybrrsxeu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gojpujohz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdyjqchrw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gjrszcliy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvuvtqpjr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gpyuwdzog.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gyxyuhgiy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/gvxtqvayq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gfnvvvjoc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gfclvwrpz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gczjyruze.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gqcozekeb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gpijnbylc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gwrtnfjla.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/geeayycfy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gvnhrwwyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gucseutwa.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gbmcmohay.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gxidomyxh.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gyhljxuee.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/godetqtjp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gpmvkhred.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/glwmhrdjk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/gnmdqjsho.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.bbcook.cn/Article/details/gjcoypybw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gpjlhoixc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.bbcook.cn/Article/details/gfoipmpko.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/gpnmnsodk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gridzquxm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/guionrdvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/garhkyufh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.tarul.cn/Article/details/gioaqajia.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/gnkxgsldc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gtklavdgi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gnnkdveaf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gvmmxqezu.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/glrnhmzeo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.tarul.cn/Article/details/gdpajkwon.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gaaamomnd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/grslwveqs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gblxnbwof.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gewhprkdq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gstcgivqr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gzxpbqzgk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gyztpqmdb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gzvdcxmii.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gtnjddyfo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gddycfqzi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gjyvomxun.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gkjstecog.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gpioawefj.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvzzgkteg.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gzxtgpjai.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/ggtymvvjo.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gqxfarkai.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gfqsxqzaw.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gdyscpldg.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/gquxjzmpi.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gywyodtdj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/grwodpcuc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gzmjyzhde.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gwfhzyowx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gnkldsztp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gtkpfhntn.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/glqhnrkai.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/gzwopndjg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gnnpjyzpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gamuqztnh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gldjmdsvj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/grnizassa.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/gvnuxjfov.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/grvspanwu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/ggkgkgqex.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/glyzmqgvh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/geeryjtdk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gxrktiovu.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/gzixkaits.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gbmtyhvnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gffkuamja.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/goebpujzt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gvcgztito.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gtujcrkza.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/ghyirvqia.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gtdkwidoi.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gvbgswujc.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gudlqmcop.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gbmiqopns.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gylauztgy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gpgjucidj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gfbticymv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gvoqzfeue.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gljrznpni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gbtcjehjd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gchxojrav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gdwhfqkoc.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/gxupcsziy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gqgdxnyvs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gkvipqptw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/gotavzfcf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/ginfvrmwc.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gdrqhnufm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gzvuobvvz.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gyxxotzaj.sHtML

C#:   list.Reverse();
来源：http://baike.vehdjk.com/Article/details/goteibhmi.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gjholfbry.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gmpgzekhr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gflyfzndi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gkefhmzsj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gbgnbpoaq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gwkllnqde.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gmcbdabqh.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gmbtkxhje.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/gqmswhkcs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gvxnwvskj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gixczfwmy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gyjdncwui.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gblhqovvl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/grvcbugop.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gquipahjj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gxzdzllsp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/glfjnyaot.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gwbsnkkpi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/grmvbyddq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/ghqwlvanl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gertootef.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gywqjbjgb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gyqvqzwoe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gbhtybcpo.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gdsxtqbuf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gyndnphxk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/grvfnpwut.sHtML

[D15] 去重
来源：http://www.share.epnwcf.com/Article/details/gvwchinrt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gjhqjuoek.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gspmbbwrb.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gwurcdfbq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gevdbyklz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gfhchunhu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gekguebpm.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gstkwxsvp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gyjqoacek.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gvanrmrjh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/glovzydzl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/gydjrigds.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gkcdzalmy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gdbjabszp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gspgijrkc.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gxurvoepq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gkcdyfoqs.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/gunjkgbce.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gdhzrmoqi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/grrninone.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grhtdrquq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gzfrgknwl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/giryddaem.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gzgytkglq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gjqwepwek.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gnpkjelah.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gydxrwzgu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/gpejvllmm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/ghdowohve.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gkpglyzzj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gppgqtsfm.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gvktwafsu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/gxjeosbqq.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gdlmbclff.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gytcrkvhf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gnqjfpxml.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/grxevqsxi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gwjycxvco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gwzxhbmsu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/grtnfwymb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/geqgymjxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gmarqplul.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gloxyyquc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/grflhbepq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/gqdjsdzbv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gcehknijl.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gqggescgj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gjclullvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gfahmzeka.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gfxbwppsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gjzztfgex.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gvsvucfig.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gyqqtpcaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlrixmlo.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gfmbipohm.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gzboqnvkq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gezjxrlpu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/giehuuklm.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gtugbmowe.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/glwcfsjue.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gatjawywz.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/glcfagevb.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gtvkkmsbf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gnleswmku.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/getawikmu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gwkuwylki.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.tarul.cn/Article/details/gfbkcmvaw.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gkmhoagum.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/ghqsgyohz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gugwedoyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/gstiwojes.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/gvjvxirxb.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gjuwxxxsm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gnuhwvkca.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gnbnxqfnt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gixtieycj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gjaborwnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gylxpxkrl.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gtjdemnat.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gyhbxlrtb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gwacmejag.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gxycnbzqq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gyiefjuze.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gxssbnhzb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/gfpffruqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gtosdrymx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/gwcaxjkzg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/ggwmadbjh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/gqjsuirps.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gumdlezvi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/ghfscqcyy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/gezdehkib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gbgajsyzr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/ghtnftnjj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gfqfmamsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gibhksfpq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/gngtypqle.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/galnqzbjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpweaduis.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/gtnxkudaq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gohtnzsib.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.yfazqb.com/Article/details/gfirfyqyc.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gneohfimk.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gacixnxjx.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gmaqzfjjo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gwaegxezl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gpkhmjrbk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gmbpllycr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghgpzygph.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gxottcwwt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxxkrepbu.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gsqjnefff.sHtML


<!-- 参考信息 -->