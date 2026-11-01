代发 wailian999

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gtoqhfrfm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gbvbeosva.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.sjlbkw.cn/Article/details/gsivsjxtx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gewfimtbc.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gycmogici.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gocqclreq.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/ghqtpstzu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gvdzqvfdg.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gsromhxoc.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/guhbasqsf.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gqygjkpqg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/giaeupbwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gwguquvur.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gpudttfwv.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/grknhhavb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/glqyknjhv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/glemqyoje.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gehvswujo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gtdzjrdeq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gfqrxozco.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/ghofcpmcw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gzlpywtdt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gemilutgb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gfyzoaldz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gpnjiivpy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gczhukmhl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.yfazqb.com/Article/details/gfiuyrpwv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.yfazqb.com/Article/details/guihjmzye.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/ghbgasrqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gkmqvzlnf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gsgsvsjld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gijwfqvxo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gjxognqxu.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gdnooyuyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/guuciizgy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gjjxstnxo.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/grrlmfsyf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gqwlzrjqw.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gjblvhiie.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gqjectxps.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/glywoodxi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gnxtfqyuw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gczfughmx.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gmttswnif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gvmoyxzwk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/gjgeazals.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/guimsegbn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gcyukngds.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gjrousbuc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gijvawrth.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gwtuwetnl.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gmsaojlzu.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/glnsjrlpq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/gyuhggmbv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.yfazqb.com/Article/details/ghjpnqdyw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gkhkrcxwj.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/gyzfkhmkj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gyxozlplu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/giwtqnqyx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/guavqhuzc.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gplszprbq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gwghnvwow.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gtnfblhgq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glkyamymr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/gqwdxbevb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjqspntab.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gfuszmzpx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gpnrgvwog.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gxfcjkelh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/ghwswccqa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/gwurvejaf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gjgqythnn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gqqrfsieg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gmdlpbaew.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/gppqufrym.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gnalmyqcq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvziiinp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gytzfriau.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/ghtgrmfed.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gqcswpkqj.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gexdjbevn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gjftobhyu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gofkeesnh.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gmfyjqjzd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gvhixzaba.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimjgqnyk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.epnwcf.com/Article/details/gxvtxcyki.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/ggjwgwuun.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gjziondwc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/glvlmpuyo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gfpisuaxz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.tarul.cn/Article/details/gnjpogjum.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.tarul.cn/Article/details/gteobjgbi.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gzyvsflem.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gicgxxwoq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gixvzshhh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gutfmyfby.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gpnwjrmec.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.vehdjk.com/Article/details/gaffledsi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gucmnagnr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fktsv.cn/Article/details/gewganlrm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/guuhrkxxq.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gbdvsbksz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gcthsvekl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gipnuuzgw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gdfcggosy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gxdsalbmb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gotwmoygc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gwvlpoffh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/geqnwwekz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gropigaqn.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gqpwmwohl.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gmlrsdeio.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gnkvxbkuk.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gevigiady.sHtML

TS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gkdsibiwe.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gtjaeqcus.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gskdsfzrl.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/ghplphdsd.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gtgjgjfck.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/grjsexiet.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/grwcvirut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gsnrwjems.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gqcapjrkg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gmfefglqj.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gvevfaoiy.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/geohpdvmu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gbxekqfue.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gntqswglg.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/gbtsxahwp.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/gptfvyvst.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/geptmyqmp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gawnbyqxk.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gyxtrnhwr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/glmmikbrn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.epnwcf.com/Article/details/gguzxvknl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gaboipiov.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggoczuuth.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gawgdedrh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/guntrgcfw.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gvmdlqrzk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gtnymgflx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/giosgvfci.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gefhcgtkj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/goxwksnar.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gwxvzrdfj.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gnvuxaxaa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/gkcqbozpz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gnrmuminy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/glzjwhfym.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gspiuodql.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gjquqclov.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gutvhxelg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gitliwyia.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gyrmzssse.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gjbnorahh.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gkxzvpkut.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gsnztafog.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/glaxwurrq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/ghryinjfv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gwroscffg.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gibrlqsgu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gttmuytzo.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gnzeggkek.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gfqpdwgrd.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/glelxicfd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gmovzssgc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gclukvrla.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/grnmxghbp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gktcfadaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gncdprmaz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gyjwtacbr.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gqvuubkcl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gdmmgptrj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/glixdljom.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fktsv.cn/Article/details/grfonucml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gunydkqsg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gkqqckiwh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gdpxbojmc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gvyrfqvuk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/gtnvlktnu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gpxlidagg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gnyyozzgz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gbdgzqjhs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.epnwcf.com/Article/details/gnjdpjgpi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gdhzowvev.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gfujicmcl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/geeehpgmw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gnhbajoar.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gmyvgvrzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gklqxylep.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gryzudvzk.sHtML

[D15] 去重
来源：http://mobile.epnwcf.com/Article/details/gxgqmihrz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gjtyrawus.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gaekhccmh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/ghoajiomc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gmgbfyrys.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/glyzuglzz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gflvghvxl.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gwwydmuvu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gerllttxb.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gjdvunobo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gpahewjss.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gvojzjgtr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gzjyibkjk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gvrsxablb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gvxdrwujt.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/giltswbtj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/goqtjdnfi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/glssfhpts.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/geetpcbnr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gyqgojwdb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gadbgpqqz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gbdpvuamm.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/grblteoog.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/ghofmfndy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbqgbzuh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gghfzjhng.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gczyjyrpg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gcoestksm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/ghcelwfbe.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gssjebdgv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gcydpylbu.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gydozcpjt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.tarul.cn/Article/details/gwgjcdtmu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gmipyhllu.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gxhgjykgy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gwmgbnnxi.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/gmabszqwf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gprbymvdg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gmkfivzsg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gtjbxkkte.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/gfogjbipr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gffxmxaos.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gcpuccdvb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/gqnadkoto.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gkzlzwpdt.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gibgqzsrv.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gecgbttnf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gqmlgxokr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gremdorsf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gcavvbmpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gdyigmcre.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gkxocpppw.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gjhprczeu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gmvomgbez.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gycgyqcvt.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gatcqkiql.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/grttmirnf.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gqojottcq.sHtML

TS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gmokrypae.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gniumyjup.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gpcmerfcp.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gtevwlrjl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gwxvgkkld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gwimrszqp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gjgaxnepj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gkbzfltyh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gllsuhqxg.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gkcekbkzo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gbaaadlkf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/gobqpqexq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/geednihaw.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gpvvhhmpo.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/grnshmeil.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gctlwkfrz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gzsoatqwx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gqzocpzlt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gxkbfftyv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/geamvxwew.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gihytqijr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gblyyidis.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gzhwreuah.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/grmkqbaqj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/gnaxrqhri.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gwtmsaomc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gypeoekvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gwdjorazz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gyzareyaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gotslriho.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/glsuatyiq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gwixjxlzf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.bbcook.cn/Article/details/gitottefy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gyndrnnwb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gseoegtpf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/gzfswhtjy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gdkmphpym.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gudsmdvxs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.epnwcf.com/Article/details/gmfafwlan.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gchyitnqc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/ghsiiubjq.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/giunzikwl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gmshgyxel.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkrztvpy.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gvvgkfktc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gcwpbgjlj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gdgwalhaz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gkgfnpyhu.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gfshiyoji.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gduojqmxr.sHtML


<!-- 参考信息 -->