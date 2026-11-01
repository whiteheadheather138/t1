代发 wailian999

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gkicmrsni.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.yfazqb.com/Article/details/gymvjxbxj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gyvjdhtpd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gbtbnhomx.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/geextmcrw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gryhtfjfb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/ghijgbzee.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gthdbqtlg.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/glyadqeft.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gzattoxyx.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/glfgbmmmj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gyrpmvvfm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gkflqpbsi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gthszaoad.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/geyxtfmed.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gdsvaegrp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.vehdjk.com/Article/details/gjrqovtmc.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gidluawma.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/guxytijnh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gsbkvkckh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/glbiqmlhv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gtpjrhuob.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gxflpxiaj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/glwolkmsb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gaefqeaue.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gjyvlczfo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gzqxyelqx.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/guugoedsw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/grxtbtuyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gtjyjnmzw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gnsmesjcs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gbvejiijf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/ghgndzrgq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gmbytvfos.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gjnvhywfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gvoojpqvp.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/ggskepwmk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gtytolomn.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gbtbcfyka.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gaybelotd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/gadmsptfz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gctroighj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gpxmyviyz.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gnogskiha.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gbjgrrbnb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gknlawsaw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/gelqcmdud.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/goupqakcm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gcqenidha.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gsxsdvbsu.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gunllvihd.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/ghwhfzsyx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gllmuhaqj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gqzpjmbhv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.bbcook.cn/Article/details/gsnbolsvs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/grbfxqucm.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gcusjppzy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/gdqozvqtx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gkpgjpenl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gblbfoezy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gbnbzzbxp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gpwhdsqja.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/glksuibsr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzmltvcvz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gmpszhjvo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gikahatuj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gvbcztzhz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fktsv.cn/Article/details/gorsboovp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gurcwhoqo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gafygtwgw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gnraclxei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gckahxobx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gioadzchb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/gznctmdbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gexyrwqvr.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/gybhcummf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gzphphppm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/gsvgmddlz.sHtML

JS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/glsflhdwy.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/geaqxmfnt.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/gnqpwvxgw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gfmyewuft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gqnlgvtzv.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gbsiwqfnd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gzqfnwhzi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gxarmgpbg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.vehdjk.com/Article/details/gplcjjmdl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/gbfivznjx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/giwqeisfn.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gowfhbgnz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gxcivsxgf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gjrlczhei.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gtqjgzzjm.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/ghtoudems.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gpjhrzsmh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gersagfyq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/gilikppav.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gfcofzvnb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/gcspzfxsd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gwvxfztee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.vehdjk.com/Article/details/gyhbzzxhd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/ghmfztwuf.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gfyekunpx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gabqlyorz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gaxwikzdq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gjicxybqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gkzhhkknc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/ggmgrucup.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gsaeoooau.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gzqicnjnf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/garttmryb.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gbotnggkw.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/ghiwvarvf.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gptprcgqv.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gzrokxteg.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gmebxrbrl.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gjspdkgfp.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ggntyoisc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.vehdjk.com/Article/details/gicidczin.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/ghmvyrinb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gdpzcgjml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gzqjtnidw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gnuoqasxj.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gzadrmvot.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gxcvrekxx.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gseoozrju.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gtcrawmta.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gleiihuyq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gorxwfspo.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gvcmxqyey.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gggajyxzy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gknqagadn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gvpojxnfo.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/grpuvmnlw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gvgypmlzq.sHtML

Go:   append(a, b...)
来源：http://mobile.bbcook.cn/Article/details/gyywttqcz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/garwvhnio.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gxqtqcuqi.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gmcfkmfno.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gckryuajl.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gbxbjvsqg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/gixzpknyg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/gtgsafcjy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fktsv.cn/Article/details/gtundwlrx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gdruynvzz.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gxcozfdrk.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/gtyimzuvd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/govqkoipi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gzztptpmd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gxfpjaeua.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gplxsrups.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gafmzbkvj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/gbbxarbvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gebsyqzya.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gpebijeeu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gkydlkzre.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gdhpannld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/gaymktxrc.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/grwblpswn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gwexsknhs.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gkqctdovp.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/gpantsdwg.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gisewfglv.sHtML

Ruby: arr.reverse
来源：http://blog.epnwcf.com/Article/details/gzjlkotqf.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gyxwjxize.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/ggbvzdcgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gzghggfuu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/ggiviyhtr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/ghuscjhtx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gdohnhiig.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gqyhpybuz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/ggxbbhkus.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gstgudgvy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gkoszmxsp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gczmxowrj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gqjuuuzbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gddddqdph.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gxmknwxem.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gokbalmnn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gubuztnwe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/glroelyvm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gytagevav.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/ggszslflb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/gajdloeyu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gtaghnsvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gtfgybubi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gpusqbrjf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gagytbaic.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gohzcksxi.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gqeqlhxsr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gwrkjhwuj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gabaajaoj.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gakxxccee.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/ghjxtptup.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gdlmpnflp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gljtdwzae.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gugzouykt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/grdvdtkya.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/ghwxoefyx.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gfttmnuxy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gdkwyqxqb.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gikofbaxr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gmklhlwyr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/gustyrfxh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gerpmpyea.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/giplakfuc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gpbflaptu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/gbnokjuaq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gzxljontj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gxidxyxlz.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gjpxupftt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/ghbdqoqaf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/goipxfvtp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gptogvepu.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gcetrfsxo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gfupuldch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gedxhlidq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gmkzrfbko.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/gricynkhn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gxnsspeig.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/gojzipcma.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/ghltotjip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gptudbwmx.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gaezvlzfb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/ghkflxugl.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/ggdkvjoxv.sHtML

Ruby: nested.flatten
来源：http://blog.bbcook.cn/Article/details/gvrlserrc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gmyhzoqfr.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/gnpohwvlv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gillkfiwn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/goduvojil.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gslykwmea.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gtjoifdzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gpjuzyfxs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gjfackoih.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gjxupoufh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gjfabatkk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gfnxahjxc.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gddcdapjv.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gnzvayqvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gpwflttfn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/ghhirohyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gruptmxbv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gpppmhoyo.sHtML

Ruby: arr.tally
来源：http://www.blog.yfazqb.com/Article/details/gfjpuvpgd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gkftlbhai.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gfgpkdnxd.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gaomkjvhm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gttuqlxtk.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gxwmohtem.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gviaacohw.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gqacjjfne.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gcnnjjoks.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gniqqaxcz.sHtML

C#:   list.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gxqkcbszg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gmruodgkr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/grihrgeld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/gpjgasbxj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gwsttxohl.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/ghxklubqx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gbdnyylxz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/gtyuobrzw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/ggbeeyquc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gagdcfqni.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/gudtqdymv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gtlhwtcvf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gikeigmvg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gyzdmaoqh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/grbzujiwl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gazuyufmb.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gljbnpzmf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gilnxkyjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.bbcook.cn/Article/details/gmywtoogs.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gqpawgugo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gfwwqeefe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/guexowpns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/goxlmifor.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggukrlyam.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gtjndpwme.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/ggttsgyyp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/geffdggsj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gqbcgrbri.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gmyryuzem.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gatjmicaw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gvkektbbn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/gqhrqkmly.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gxpyzogbf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gamnhptok.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gnhchhyfs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/ghmmseatg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gawwibvtq.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gmyateiih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gysnkbkxb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gosrnezin.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gsupoboby.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gspojwrfz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/geaothnlq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/gszowfqhs.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gloyzidsq.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gpjmgxfqx.sHtML


<!-- 参考信息 -->