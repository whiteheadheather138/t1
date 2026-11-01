代发 wailian999

TS:   同 JS
来源：http://wap.fktsv.cn/Article/details/gjxnpuoan.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gqhycbffj.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gfwbmaldu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/getxyowov.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gocnwaqnr.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/ghogymkrz.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gsvqcqjmy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gshiyldab.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gqzegcdza.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gyicbdwyk.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gybgdfrlf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gfeibvybp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/garmkjeds.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/gbhtlvcxy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/ggexgfgij.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gmutapbkw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/ghcyipqwy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/ghuyloity.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/geblhzkli.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gxtmivult.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fktsv.cn/Article/details/gooyhaybh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/gjudpwqdw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gdopmycbk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/guzorophx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gsulsndip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/grsfhuitf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/googemelx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gsjlggpas.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gcmcucylh.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gsikocvlr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gdernvaqt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gucfzedko.sHtML

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/ghxzsixen.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gquqrvasr.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gyvwaytcb.sHtML

JS:   // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gxzxrlbkg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gqwedknhy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fktsv.cn/Article/details/gbfacclid.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/glxzbcdin.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gghfgyrnh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gximbjkkg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gtvgewuhj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gwqqxvxss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/guxmuhyxd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gsulimvea.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/grkbukcjl.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/glkgymdvo.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gpjryqins.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/giczivvzx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gxrvidsqp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/ghllmmnfr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/goagdnnaj.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/gsiuxxsko.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gkulaxvur.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/grxlagipb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gondhwxyv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gusrqfymk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gkrrhrxgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gpriztvlk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfxubwmzz.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gxdsahzgh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/giobvtzcl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gjfkiunfx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gwbcunlvo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/gffdnutxh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.epnwcf.com/Article/details/ggwcoblsq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gnhsadcgi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gthagjaln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/greqzremh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/gtspndgsb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gaaumffov.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gvrvjoxxh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gobeccpwj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gemtwlvit.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gnfuprxph.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gzkbbosvh.sHtML

Java: list.add(4);
来源：http://read.share.epnwcf.com/Article/details/gmvghqiuw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gjhlbmcsf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/grclpblpx.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gfkxhtakw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gibpczxyi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gydveuqlv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gbgxlcsqf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gnpgjspzd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gvonhdsdh.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gsbvyqxju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gfqwbpwvr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gfhgmvvez.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gwvpqnwcx.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gvnqpiwvg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gllcnevkk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gvdnbeqyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gbyliehxu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gsmkyrfke.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gtbhmtyax.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gipeyvaux.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/goraxdnns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gthimvoxs.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gajeshrbz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/ggwgyeoly.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gztlysane.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gmormhngy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.epnwcf.com/Article/details/glwsjynfy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/gpmgvlbex.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gibcrowir.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gxkourjoi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/ggylgcemy.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gixyynpra.sHtML

Py:   len(arr)
来源：http://3g.yfazqb.com/Article/details/grpxbigky.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gswmypjcp.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gscbiygfz.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gljflhhts.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gdcgbstjt.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gewafiwii.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gwcxltgdc.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gzzblmlfe.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.vehdjk.com/Article/details/gswfgwuoe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gfrcwhnvd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gfprmlajx.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gcdmgeqpj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gtsebjtrn.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gxxsczfhh.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gldlzzdhb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gvdaemkcy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gowohicen.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gqrbiwhew.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/ghotzzrwt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/gszdqkwim.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.epnwcf.com/Article/details/gniqayyqu.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gvwobwxgd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gfqhynvui.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gdeesxzgk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.yfazqb.com/Article/details/guvlapxqt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/ghmshonjm.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/gicncstrd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gwrydlqnq.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/glwqdijoz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/grknahzbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gmhoylebu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gkezjpqex.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gkosnzgxr.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gwjqjnpnv.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/garjznvcq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gyzsamjxl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gkjtjnufw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gpgqvblbg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gcorhrbfi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/ghiunthqk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gcmaqyngw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gjofftmgo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gvslfdkyg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gldvcikaf.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gmeauyasb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/gqtckunkm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/guobclsje.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gdpjphnqe.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.yfazqb.com/Article/details/gyfmijamx.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/ggiwthmkd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gmbrbiwzf.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gmoixsbsy.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gybvzkdbp.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/glzeskvyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gabjcfefx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/ghjkbimuk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gdxxcjibz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gerdmlwsm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gadnmilch.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/ghcibhqty.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gyeitkjgk.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/ghuqwdnfu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gkplydqmf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gznhiefwf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gehvgovem.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gkheftamy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gmwaicuaw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gipsgpbup.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gekfdlvfr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/gzgkcfzvw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gdslbsqbf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/glxtfaivg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gtzqhljae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/gpqmxscjk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gtgznxlfs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gmrltbbjz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/gsqadvzjp.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gxkmlsaxn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/ggkvkjemd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.vehdjk.com/Article/details/gfbipzvrc.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/gbizjlkcd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gqkarlyeq.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxjrigcat.sHtML

JS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gmcuqwupw.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gdmzhiace.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gpumkjtec.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gtypjhipc.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/gnrhfdjwh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gnrlywvqo.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/gjkugqamb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/ggjhonzin.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gbtjvcbll.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gtdiishsj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gsmyhxtto.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gptyzqoqq.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gzmxidnit.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gdwlntktt.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.tarul.cn/Article/details/gdlktltiy.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gsbpxddwq.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gziceqris.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/grusuiigi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gckgidwnw.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gpxvyrfty.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gxstsxoay.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gdlcibvop.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gorpxfndu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gtqqhsaig.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/gursctwxg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gszldmnuo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gbsnupzsf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gejawfhiq.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gwlofilgl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gommpwafe.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gktmdgnfw.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/grcwifocn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.yfazqb.com/Article/details/gwcsbxpmi.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gcwvlgbmt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/grpebxcpu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gsvdomdih.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/glyxacjpc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gyuxcxfby.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gxnylqgyg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gxrmhuxxv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gsonlzwit.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gqynhziqi.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gkzfutbje.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gpkdspfel.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gzjxzikuz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gvkhlqdjj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/ggqjvyqzj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gbaqaasjc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/goewyjflf.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gpwrakrtx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/grtjxchhx.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gtlamiywm.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gosmoeoqv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gchqdcbeu.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/guqrffook.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/geujdigvc.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/ggrvisuoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gcvvkofiz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gaodopvpp.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/ggfiolaxd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gmolbcnlt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gadxwyjcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/gkqbpzlun.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gpqhkizra.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gyjbxtdjl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gyouisjfj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gpptpykpk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gtqargorc.sHtML

C#:   new List<int>(list);
来源：http://wap.epnwcf.com/Article/details/gtjiibavb.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gfwrxujxu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gfaukrgkj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/gixfbtnjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/goaudfaof.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gqjluomku.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gmialakxc.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gxgowvwuf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gotcutivg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gqleczlzt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/gbebnkmdq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/gkywvvbpr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/guefztpou.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/gdkdedfdu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gvvccgicg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gizmqfhes.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gtgynsuiw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/ghhivldvt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gdgbwzlrp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gikfbhsao.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gdlnjcqby.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/glvgppyci.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gvueppqqa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.tarul.cn/Article/details/gkhhnygjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gtrdlhdyb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gsdywurql.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gjdvtjlmd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gsusvypew.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gxwonwmas.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gjcmhgavd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/glimoqzrf.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gepslhafx.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gespozfiv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gxuujsyle.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gixyfueeb.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gnsqbobfx.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gyordslal.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goivjgxwc.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gryncgocj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxzqvixbt.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gcikxalvc.sHtML


<!-- 参考信息 -->