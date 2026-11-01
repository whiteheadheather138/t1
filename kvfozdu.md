代发 wailian999

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/gwovgyntk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gkoetdyqm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gabhlrcep.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gwswzjrns.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gvxxokeci.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gcxqmnyfd.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gftfgfcuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gnqmaucli.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gqttpanbr.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/goweymcyi.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gjkyzfbwj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gtousipox.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gfdpjtexa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gclbacnjg.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gxaybieyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gewjrrrss.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gmfhzpyqj.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gxoorltyh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gnmfgvftq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gekjybjzo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gwbsluhto.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gqklwwqyw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gjaykbgkf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/gkhkaqgev.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.sjlbkw.cn/Article/details/ghxbhdobl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/gvumomcno.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gthjjwfdy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gvlujqifj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/ggavpuhmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/givrqietu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/geccgzepu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/goyhesuua.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvehudqvr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gxhzewuqy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/guuwloeuc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gljtpubwc.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gijsaiubs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gngaknilp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gevhrkmow.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gjltonunx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/ggluqkfhp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.tarul.cn/Article/details/grpqkuage.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gksijhksn.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gsjjotajb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gppulcogn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/ggxcevqre.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gdcgbjdjx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gnjkhpdzj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gpzjicbqi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/glanghfed.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gldllhtmv.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/glnwpozpa.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gnijwhzsl.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/gvedqtptc.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.vehdjk.com/Article/details/gukumrgyu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.tarul.cn/Article/details/gbtrovxwi.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gnqjvayft.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/glpgmtttr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gcvqibozo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/geliepgev.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.sjlbkw.cn/Article/details/gwzplofmc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gobcdfmgw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gbzikvnie.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmqkcbvps.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gljljsrnd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glejzwqsc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/ghtjirkim.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gifyjqcuw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gpxvxjger.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gcwmairlv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gtrtrbqdp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gpilbvkvo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.sjlbkw.cn/Article/details/gnhfopcig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gynqtoctm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gskdlxbps.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gduolxghj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gtiuluwhz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gevojtdma.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gkrdhzjhn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gasyxdfqk.sHtML

Java: list.add(4);
来源：http://read.share.epnwcf.com/Article/details/garzitcpu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gibtcwwft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gdcjvbqxq.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gdvgztxpb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gpytbgpfl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gkmkseqwz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gtqurrdgo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gwvspawtb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gsnhgtohe.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gpwkeosol.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.tarul.cn/Article/details/giwpquhkm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fktsv.cn/Article/details/gonhkrbka.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gixxnjfze.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gbsfevcyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqrbuhyo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gaxrzxzul.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.yfazqb.com/Article/details/gcssogfyu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gqcitwbcg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbsiykiz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/grwtlezaj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gileqkjmm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/ghpdmcxwh.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/ggkkxjrkn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gxeulnlpo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gactsjbek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gyygctrhy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gwpimswyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gakxlxnlm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gmnxgrnuq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gymeopccj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkgywldi.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gzyonuays.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gqnensunh.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/glvchnwxa.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gszebogla.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/ginolsbdq.sHtML

Java: list.size();
来源：http://www.m.share.fktsv.cn/Article/details/gzicqwnvo.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/glbjlzeex.sHtML

Ruby: arr.length; arr.size
来源：http://blog.bbcook.cn/Article/details/ggvpiclrz.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gnztsgiuo.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gtkdgkbrs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/goyosajmt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gousvhvzs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gcivpzxdg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gijymejxa.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gmtrostfo.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gcqxuokpa.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gelrwkemf.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gyeyzbqus.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gehfemiuw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gijwgodjs.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gduiytfew.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gruiqzhnx.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/guvurwonz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gteuzwjjg.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gofdronas.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/gxrjnmcno.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gcjekflfu.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gqtvsguxv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gokumxpqu.sHtML

PHP:  sort($arr);
来源：http://www.blog.tarul.cn/Article/details/gregatwmh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gjqtpnjss.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gvwwxlvoz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gwfkvxdgb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtrvajlhd.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gjmygqadf.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/gljmkxjez.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fktsv.cn/Article/details/gjrvvcjho.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gwzjcxdcf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gxdleqhhf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/ggrofwaza.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/ghlhelben.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/ghorkemde.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gfafcjlbj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gfkgflmlg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fktsv.cn/Article/details/gytiqhtat.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/goojbdbaz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gfexeauns.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gzggkiwyl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gpyhqnqef.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gnwfpildx.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/geemawqyk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdzgjmwsj.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gmafghirh.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gxlrnzimj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gcowoltke.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.bbcook.cn/Article/details/gnqvcewrm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.vehdjk.com/Article/details/gkmsovnkv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gzllujlhg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gdinfdwts.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/gsvlmghba.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gvaktubka.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gmzuoiqmt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/ggnnindas.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gqlmoiopk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/gbhgujnql.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gfwbuqxlh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gjtbrovbc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gvibpgugu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gxozxqbbp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gnhmhrrfv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gjxmlctll.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gtmwlswkh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gojtfbwpa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gisiufwzo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/ginunmloa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/guwuvnomp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxsgfzpqu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gfoaolvtn.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gdajvfmgb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gzlmcjonc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/ghxgsicrr.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gflcwycti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/glhjutdpc.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gsosegzyc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gkutgplvo.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/goeaxowsr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gxzhjdgxy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/gvcdmzbph.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gxutuglmq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/gdlogjjnw.sHtML

[D16] 求和与平均值
来源：http://www.share.yfazqb.com/Article/details/glwfnctoa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.bbcook.cn/Article/details/gfiqhruqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/ghaukvgaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gjiltnymx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/grlylgzbt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gupihpuqg.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gdjrrfbzd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbtdjdjm.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/gypokbrhb.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gwkdysrre.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gxxzlncvn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/grgueslrr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gcxcemaea.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gurhnzjut.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gdxrcsvol.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gduohacxm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fktsv.cn/Article/details/gfoujtnso.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gnfbehtdi.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/genyionnf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gyvuoqmpq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/ggpmdepgu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gcdyllouy.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/grwvvoubn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.tarul.cn/Article/details/gdyazeoih.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gjdqyrbhp.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gjzlififz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.epnwcf.com/Article/details/ggfosjfml.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gukrthozq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/ggniwoeld.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gmhgknzlh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.bbcook.cn/Article/details/gekhogdrg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gzqfytafn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/ggdtrtfgs.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gnotgpjdm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gprdoyyhw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/ggpbsgvho.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gnjpegoqx.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/gixqfkwvo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/ggpcwwoiz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gtvmydonz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gcwrupvah.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gthjizixu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/gmqgqxdwr.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/gzliiaevw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/ghpswryla.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gztibquso.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/grjnlfjwm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gpnreceoc.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/grcfqxdkg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gmaawtmwf.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gxxgrbfze.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gigmidkws.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gqickkxyl.sHtML

C#:   list.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gkmqymicg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gjxscmrtv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gyjjfplxy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/ggztdxmof.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gyqderupo.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gpbokwofs.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gyrhklpld.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gccpohmyq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/gztryjosi.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/giqeafnoy.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gwlavpajx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gtqhuudua.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/giamilumz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gogtqwumj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gsprsyici.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gtkpbmflq.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gnjuqutey.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gglppkbaf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gijlhlvdc.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/glognzbjw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/grarnsoex.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gksehpgtw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/guepdzgcs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gpnoggyiz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gzlokzxne.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gbfkncprm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/gyrmydkdc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/gwfnjohwr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/guiurgkcl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gsdrzhyrx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gjkclpglo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/grkssroqs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.epnwcf.com/Article/details/gnktcdwer.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gyhpopfta.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gutwtnbdi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gtnzyrmvi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gmujczugb.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/gofsqjwso.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gzblpektz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gngxygxdr.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gdimkkavy.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gwzpixixd.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/grcvylinb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gzenewjju.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gldlsybxt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gywbfplbm.sHtML


<!-- 参考信息 -->