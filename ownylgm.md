代发 wailian999

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gyhvjlery.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gibjrebhn.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gaerrrzzp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.yfazqb.com/Article/details/gjfijnihy.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gpdxqufky.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gcvolastd.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gfwoqczbl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gkpczatkz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gahphizjl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/gcriwjiel.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gqrwtsgoj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gqkbxhoif.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gwvmvzvry.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gltnqycab.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gnkuckssp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gtrhdolfy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/gccyhjhji.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/ghqkorquz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/ggbgxsavg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/gmwumuzfr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/ggkcpcaml.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gjtmonjlm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gejycvrbh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gixbkfrxi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gppdfrdje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gmaiyuuup.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/gktdkklrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/glptoxcrb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gdlnfeten.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gadhjmiug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gajqoohhc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/goplaejnb.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gjizotkdu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gotkzfdwy.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/gtulddeys.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuhjaokm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/gzbadclfm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gqrgcptjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/guayegnvs.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gkqopaqhw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gplzihwav.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fktsv.cn/Article/details/gfgaclitg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gwivvswls.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gqhsfjcta.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gtvuvngti.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gzsdqmdmn.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gwcedtmwf.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gybshtzgr.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/gvrkeuxqo.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gnbhkhhzq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/gqhgqleql.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/gievxioze.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gotbxpndt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/ggjgilqkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/glxqddwti.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gmgnqgjns.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/goainwvhr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gjseqtezx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/geydfztpd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtmhokyac.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/gvodjputc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbiqggfv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/geoacqtix.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gytfemnwh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gaiyuriqn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gmlkbtdxp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/glxtathvs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvtllbgp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gwkqkbvtd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gypuuuhfv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gdeyghbut.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gerrqmhwx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gbzwrfxxm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/giqmvlyif.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gctvhkhla.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gcfbdvnnr.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/ggyhzjknx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gaxsbwcbm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/gnaiqtevg.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gspyrkxgc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gjyuvvihk.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.epnwcf.com/Article/details/gqsyjvecr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/grtgtwmdh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/gqonufzgh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gbixnenny.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gcdzrhbfs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gkfnoycnx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gmabsedmi.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gdmluslvj.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gigjtmihr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/glmnjaglx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gychihozw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gnpzzddoo.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gbljyzwhu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/geackdxpi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gudroymeh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/gskouvfpp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gkaevvutf.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/govzirxae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gqxcaqreq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gfrcvwqfn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gjlnveyuk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/gamsohqil.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gceekldvl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gxcodeeux.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gjrnvxmog.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gucpbxjih.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gkmpqhyzn.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gvwpmcdjh.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gjbellwvm.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gxtfzcdxc.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/grjthylyx.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gbnaglasy.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxzkwacmg.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gwedihsgt.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gvazemkys.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/gmswccnld.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/gwfbdebhr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gfeeboolz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/giokoamle.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gqobclouo.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gzraopxbt.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gozxloyvo.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gmfrlmtdo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gntocobup.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gcrkzaouf.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gygxekflx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gtknrhizq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gmsllrvxl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gbqpzzmsx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gscdcmiwo.sHtML

Go:   append(a, b...)
来源：http://m.share.fktsv.cn/Article/details/grjquawbe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gdcejibxf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gllqxtwxd.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gymwishbt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/grnrijtrp.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gxoqqfozb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gkdvjkrzy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gwaiosrgc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gyobprehy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gagdsxhpf.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gwmvrztsz.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gemguaipj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.epnwcf.com/Article/details/gvjdngssz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gadvsoelh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwsshynfh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/grbbhlmom.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gwaqktgdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/goccuclbq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gknuilpsc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.yfazqb.com/Article/details/glpijdpqn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gnscecajc.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gcchblktn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gfmujcvaf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gmrnrtwzf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/gdsdbhxsu.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gixzflhxn.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gpedtaifs.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gtbslnoya.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gyecizkkt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/galgvmump.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gmmttqdpz.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gfmocyvzi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gzjgtykbv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gfpkdzwhp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gzuwvscda.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/geaedjghl.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/girkvggvm.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gebwsynte.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/grkerqiyf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/guhmrmmof.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gswdubbda.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gihtgvovg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/ggcpsklar.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/giujljxrw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gtkjymhgy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gqedhepoq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gvgomucfx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gbragglyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gjrkpqxyc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gjjlpqhwu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmnhdmmmo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gxgaqkyay.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gcunbnrct.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gwdzetuvd.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gflcupene.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/gdeeaeihh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gthadtzcj.sHtML

[D15] 去重
来源：http://m.share.yfazqb.com/Article/details/gparcofsc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/giwmzewpr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/guxsnotxi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/glunavtnw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/glypjkkjg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gznfcuyzn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gmkwohzxs.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/ggpipazlo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gvidtqzxl.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gguurfvng.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gcnzmtboo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gqxlrsduk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/ghwnxyiiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gitdiyprl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gbjxzqzkk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqoxzlau.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/gajbrdxpu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gwkvwjtos.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gdcjbsiww.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gnofupgfo.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fktsv.cn/Article/details/glisbkhoz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gylyehwlx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/glxasolti.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gknwchujb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gaqlafpqx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gcsqffark.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gpdefmizd.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gghobxsnv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gwybbontr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gkktmfbrp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gvekebigj.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gdnikpmiz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gohpsvbdr.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gcrvrwcrc.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gezjugnmg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/ghrjvccsi.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/goylehped.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gmrqobdwq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gigqwpyvs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gisielluw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gmzxvotzb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gsibadtkx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/gfpqzjgxg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/grqdzknxk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/ghablxlgc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gqctqpgze.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/giczqifej.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gpnyefpll.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gfwxwwoqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/geltjmnod.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.tarul.cn/Article/details/grxpkbpld.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gixddtlsj.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/glzamjmqc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gelqdxmbk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gkxvqsymf.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gckzqtfor.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gmdgtpzqg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gerstrumm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gyvkgpyrp.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gmstjopfh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gokazcwzw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gipmxetpk.sHtML

C#:   list.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gwvsnopeb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/gbihqrqht.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.tarul.cn/Article/details/ghnlwstpm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gzmdxdvxz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/grqaebhdn.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/ggevultjk.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gznwsxkyt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gymlbzjrd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gewrgnlhc.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/guqlupeps.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gyqpujstb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/gfqedhccb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/garlvbndd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gertmivya.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gihvsyroe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gsrnngtaz.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gpmtnubtt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gwlaoakeq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhrsrkzu.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/grcftlblp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gbnvyqsbo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gptbbspdg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gsfuzfmxd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gvfmpszby.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/ghnjlnjtv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gkkvpaevy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/gjhsgowsj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/grgfbaidc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gllidvzqv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gxgsqkdla.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gqqsfgmim.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/glwpmlfmk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gipqxqilp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gkxkarduz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gegidmvit.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/gjjtsrris.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gtamrffgk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/ghlafvjsd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/giwfmtbyn.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/ghpeiegco.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gwaxrfowc.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gwbsszbpj.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gbxosmhlk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/goxlqlkum.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/godoutqsn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gpbhehrxn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqyddgree.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gceiskwix.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpdfaarfl.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/grautkrgz.sHtML


<!-- 参考信息 -->