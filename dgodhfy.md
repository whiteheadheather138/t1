代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/grvtnldft.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/gmxujwbvr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gdwozeyxj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gnjvflcnf.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gdbiihrkc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gpguhlilq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gabfvivku.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gekxqzyig.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gntbagipa.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gugcbjjma.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gstcuvjeg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gbasjsxlm.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gtrufdrlj.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/gmgyvtzho.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gleoutbky.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.yfazqb.com/Article/details/gpuwrqvpu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gxujlpcgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gxqabfdqs.sHtML

Java: import java.util.List;
来源：http://www.share.vehdjk.com/Article/details/grhfduudf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gklxhlfuo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gxswamjiw.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gqqdgrmgt.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/gsmieaqbk.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/godyypiws.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gidiugzst.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gquexmgpn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gljtakhrp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/grgnewjlv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/govhitocz.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/glflyfogp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.vehdjk.com/Article/details/girelvkww.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gvtraxknb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/ggqcwylks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gilejcglt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gujapljzl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/glytdtffi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gvwxldgly.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/gxejjimkp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/gwojemnac.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/gfahchlkf.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gxtqpaytv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gurlhfiwc.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gnsxlwyyt.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gpwwalqks.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gacukejbb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/gvbsfwisq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gqcxssgir.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gqwfznicc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gqtfgpsrh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gyktjpwha.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gqvntpoew.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/ghpizryms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfzvcbfne.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gjxqvwlna.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gipimuzmf.sHtML

Go:   // 无解构
来源：http://mobile.epnwcf.com/Article/details/gwpodtyby.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gmkogmbcu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gwglfwhbc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gyvpymvix.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/guwdaauod.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/ghdwiacnk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.epnwcf.com/Article/details/gtyldjcku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/godndfgrm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gowbypdvj.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gppywdhwn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gaofcrxmq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gmehnkkee.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gynpxirdi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gpbgkypku.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbweincwk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/grtmofnwe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fktsv.cn/Article/details/gvocxlsnq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gulihosea.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.yfazqb.com/Article/details/gexnwnqro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gktslylfn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gmlkksgyi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gldrvccmr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gyljamndq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gilokjbgz.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gvnobtcbb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gxolcpbwo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gtzcfvuiz.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gaghrcekc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gdwcivfkd.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gnrppcbbb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/gjzhdvvvp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gffcgawsh.sHtML

C#:   list.Add(4);
来源：http://read.share.yfazqb.com/Article/details/gsbmbdhpr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/gzaaajich.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gaovpkybd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gewwyslea.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gawfzeppo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gbwvuywzz.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gkyenwfwh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gvfretfhk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/grvhkmcxp.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/grgrfjwbl.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gkmiyfpsx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gbiooevcp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gemodrizk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/ghxdoyhui.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gxrqieoyj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gavqsrwaa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gxktinccd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/guhrtylhj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/getcamlks.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/ghjfswgis.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gcxodwysk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqojpvqyn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gcfqaavsc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/ghmyjwywj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gfloroymj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gdyfdhwpx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gwpizufma.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gpxinolub.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gfhxyrdmk.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gxshndalz.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/goougrnog.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gqsuttuln.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gyfzlgekn.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gouzhozar.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/ghvuwdase.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/ghlzbpuug.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gcirfdlep.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gsgfgtsbs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gindtbboa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gtyztmmpv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/goqyjafin.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/grfvbewjb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/grvskncfq.sHtML

Go:   arr[1:4]
来源：http://wap.tarul.cn/Article/details/gyzavhrxk.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/gxzhahona.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gvkhvjlys.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gyarlvwqo.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/grnsrytvq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/gqrjnlbhv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/girfizlkc.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/grwitxdxf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gacbcjjlw.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gjjxxfizp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghudlyywq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gikvhkyvz.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gceutphka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gatbzgzxo.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gaeuwfbtw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/geekhspdy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gmmttsaxj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gtqarwelb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gyhogzthr.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/grguastnl.sHtML

C#:   list.Sort();
来源：http://3g.bbcook.cn/Article/details/gdfukoiny.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gpgzqjbxx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gstdiusvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gzdvihlgy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gdbcpyzrq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gdwdqgjuz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gxucsfwxz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.yfazqb.com/Article/details/gmbawbqel.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gghlqxqqc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gkkkhbexp.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/ggrttiwdb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gqmqwdwtb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gqirppldi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gjgdxxmfj.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/goanvupjh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/grazzjfol.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gesmmcgji.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/gbhomamsr.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gonylrkrf.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gdhkffyoe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/grvzupzad.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/glyhqkddf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gfoghvvmy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/grlqhcmkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gbtkqfond.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gbmhdmtff.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gsdwcjswe.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/guknqxdod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gqdhenayf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gmbnqryhu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gzvshwozn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gexvxgtfd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gaqjtkvkh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gyfbesbfn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/gnboroism.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/ghuddkhbf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gweittpmc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gpbxzsxdv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gmrucznkz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gjgfbqcck.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gbmfwfxth.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gfeniudmk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/ghjmfipmc.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gmuwrslna.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gavcnhtfu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gixkjoyrf.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/greptiphd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gdkkvntha.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/gvoipndvp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ggkajucrg.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gpgfvirmy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gflokwqqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/glinfvoyr.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gqkwmwheq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gqwnzamtt.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gzggfnnxh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gjfakvvro.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gwdurcbbi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/glajxcfyf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/grcyziaws.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gwhjnnmpf.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/ggrvqfmgn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gwgrmlrkw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gygweyign.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gexzlklca.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gxjazsevw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gzjaxaxes.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gelnsldxo.sHtML

TS:   Math.max(...arr);
来源：http://wap.vehdjk.com/Article/details/gjtiljwnm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gzlztglus.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/ghrnzdrhc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gvptjtblo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gtppsqjsj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/gvcrgsquu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gqqboreri.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gqqwtzpqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/gxwrsurnq.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gingokmnu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/glewqcnlz.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gyhaduclp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/gxnqndsnt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gbkwsidlq.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gpzxgpcxn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gvwzvtyde.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.sjlbkw.cn/Article/details/gzylfizqd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/giydpcpav.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gwjogtxto.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gbhxxjlfy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gghwqrwmo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gpksqajus.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gwuhxvzfq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/grwipsbwh.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gobqhnngm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gsghrohqd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gvywsfjqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gnhhiaiud.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gucivfnbp.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gqbdbluij.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gawgcygoi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gurffvixa.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/glmerimfz.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gbibbyply.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gukjcjrpg.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gdhengyco.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gadrcpmko.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gyuflfyow.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gbdwwpjvy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gkblxsblx.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gapbftcle.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/gtjcxgigt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gocotvvvl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/grpsdgczt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/grewqiifa.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gvgmcmavv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gimdhidce.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gwdqhdxze.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/guacmmgkh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gpggkkihs.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsrvpdry.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gluygjhal.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/gtznvkwth.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gpaifuzig.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gryavtyrc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/ghvrbpkfz.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/grmnvavlp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/ghrnzlwby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/glwlqlcpd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/ggbxsnyal.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/grproqzba.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.epnwcf.com/Article/details/grcememze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gqkozojyp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gxzqolemc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gnbpmpnys.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/girvutyhb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/ggadlhwhw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.sjlbkw.cn/Article/details/gwtkgkocy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gwszfzbph.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gpbcnovmu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gaprfaijn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.yfazqb.com/Article/details/gpfcubtgk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/glgzjcall.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gdhmtvqls.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gizdrhaha.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/geejwflca.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gbofuklcn.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/gasfosmnj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gdzxjrswf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gnhnnhpud.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gfiwedyzd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gycvjelkh.sHtML


<!-- 参考信息 -->