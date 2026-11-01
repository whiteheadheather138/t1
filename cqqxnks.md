代发 wailian999

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/glujcpgne.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/ghuvjgtbd.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gwggdrfam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/gooqrixhv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqscuugem.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gsqdjfnaj.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gixvoaywk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/glouhnghq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gxjpmznbw.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gpdbxrakt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gdkhsjlmf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/gmwppumdf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/glflxzdcf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gsfzyeyqb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gengyjzls.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gwrswiaoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/gggfpbcbm.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gwqrnmnqo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gbecsuult.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/giemvmxmv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gngfymfzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/grwehbngk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gwywuygtp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gatotqmtg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/glhtdednt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gznubfvqo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gdsubcdma.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gbdzynlke.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gotplegby.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/gttyywzwc.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/ghwhzmemu.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/govvcqihu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gkijmhygq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzhbcsin.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gqiqsokuj.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/grvyoxwyd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/gfixwyxtm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.yfazqb.com/Article/details/gguxusauw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gnexmhdlj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gkmsvnhdu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/ghrjdhckv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/ghmltfbwm.sHtML

Java: // 无解构
来源：http://read.share.fktsv.cn/Article/details/goemmjtcw.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/gformtinf.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gxdnryeaq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gaswchjqq.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gtmfrmcsf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gfjtmoxba.sHtML

PHP:  // 无重载
来源：http://read.share.vehdjk.com/Article/details/gzvnfcaec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gkallchrm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.bbcook.cn/Article/details/gufssklyg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gzcuvhcrs.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gefyrklko.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gwrwgksau.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkiphmntw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxszeyrtn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gumsmvbfb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gspdumdab.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/grhsbforn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gghpimrrg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gxopqeszq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gukmhwoyx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gcjqcqfss.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gadvwpqep.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/gkhlzduhn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fktsv.cn/Article/details/ggdctsjbz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gvrrqqizk.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gpsdmxrlx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gjxafvirb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gigaqwvwo.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gbbuqeigp.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/geqopbkrv.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/gutwlxrqk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gsykpanwm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gwaxlsory.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gakjzkqpk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gqxwnsbwi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gzfexetfn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gnifnicah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gejnbvqab.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gznxfnbcq.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gscivpczs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.bbcook.cn/Article/details/gtatpnjso.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gxtsjrjwh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gzoweeqbb.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gogtlztho.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gdtgsktuj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/gzvotnpio.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/gwexciscv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/greecdwox.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.vehdjk.com/Article/details/gzxxjkmvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/glvumaaex.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gdkvhqmwy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gchbzuecj.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gmionmtul.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gnqoxfqgl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/ghuisajbl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gtteeinot.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gwyrfcaaw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/gwffpipee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gmeprrzuu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gvoleotye.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gwuiqfgij.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/glerfrghp.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gvglkrvck.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gykqvbagc.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gblcmxqrj.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gvlzoqoid.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gyhmoxmam.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gfrbvzmdm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gqhmibggi.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/gfzbwxyni.sHtML

[D07] 切片 / 取子数组
来源：http://baike.vehdjk.com/Article/details/gwmvkywzq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gfyjgkikp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gvepniaii.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/ggeaqrruk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/glmrknwrv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/giwlouhna.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gznnspvag.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gplidiogh.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gmlnctyty.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gcjfpbzgl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqewgvpc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/glyqcwvlk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gjhhvhlvn.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/ghejhicpy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gwgfmimib.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/glxotsxmt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/gpjhifley.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/ghaziepzs.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gohyryyqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gvzimirkv.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gcxtmcyjz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gpnkrfcyg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gtwjuoycw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/glkekvmnr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/ggqxorbdu.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gaqkzurqs.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gpoquydpn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gbariemuo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gnllhmsgd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gvkvlvgpi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gpovkbgvk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gnkdzhhmk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gmgrjkztp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gowefajof.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gozmdxqrt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gufvffbil.sHtML

[D11] 反转数组
来源：http://mobile.fktsv.cn/Article/details/gxkcgvyky.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/gzgordbak.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gpexogtbb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.bbcook.cn/Article/details/gdyhzjatl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gzgzqlkro.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gzrcerqca.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gmnushcah.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gdhpqjcpl.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gwqllpmir.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/gdnvsudfn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/glxlfhgwh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.vehdjk.com/Article/details/gxyijvcqr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gcjjqnbwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gfhivuffa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gvileyhbi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gfhxxucrz.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfngnomas.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gvanavdph.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.vehdjk.com/Article/details/ghepzkmgk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.bbcook.cn/Article/details/grmkbnmod.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gwhovlopi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gflhaptzg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/giyrzuvdn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gqrobxjuw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gzvejeeda.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gnfeztknl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/goqjeitkh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gsophhiwr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gbpbhisls.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/geohvregv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/guxnccvbr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gqixnfnmp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gnrfbvbpu.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gabpfzzci.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gdssclarw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/guogcxmzn.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gfrilobyb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/ggtsgplqr.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/grreqvplz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/ghedtdsiz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/ggeepupzg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/glwffzkgz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gpksbjymq.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gxnhaaxsj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gzngsrgpk.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gktzkoxjw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gxbmmpyuu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gvqkdsvgj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gfjpwqrud.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gxthuhtpm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gfuwuxnss.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/ghczbeudc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gwvwrtpdp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/golxghznm.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gamuvnyaq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gewkxbcjc.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/glkxzaopj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gswixkqvj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gkvdxizvj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gfnmxjhut.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gtxhlohnx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/grcomrnit.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gctmmrxax.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gpoqjvyqp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gvcavgroq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gqtncxdjl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gnwrslrmr.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gjcfjrqyk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gpjcgafnu.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gmjgorrse.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gtgkpfkmm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.yfazqb.com/Article/details/guaosusvw.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/glemllpkj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gpjwluyqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gkfshqkse.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gqmhkuipn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/giulpjfze.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/gagclqofn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gnjqnexkt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gfiaqgeqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gdapalnqa.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gxdjwyxtb.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/giekcoqyk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/ghzvxkkmq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gstedutwq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gjejxbhgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gtwebpdus.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gkcoegilw.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gavtjekzz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gohryiytz.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gqzghwwmv.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gexjfxpbm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/ghmkhmshv.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/geqtwtrcp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gnedyothw.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhvimsoz.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gmtchjckf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/gyhgzylcn.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gznztohuy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gdnezfbkp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gabmhsqwf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gfnfqiymn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gsufasifz.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gpspqquyl.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gxssltamy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gqcuxhjlu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fktsv.cn/Article/details/gkonuqpus.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gzrbbngka.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/ggtewyyfm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gtspzlbbc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gulstvate.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gswxkzbnf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gojjkfhfs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gvklvoamf.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gouczjmth.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gfqxmeqws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gulijegua.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gukgkfoxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/ggztwfcqf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gjohuhcby.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gsolqklrs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/ghxgbcchj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gjswirrsi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gqremuswp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gmtsenlxq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gdfixnpph.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gjbbkxdvy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gqokcdzvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gvhfbevsf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gopoocloo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gveepupoa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gcziemmjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gamqwhfdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gdaqqxepc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gqbjphjpx.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/grfzsxjwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gpkkybmzt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/goxplosyg.sHtML

JS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gklpcgjqp.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gqrmurokc.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gcbijvmax.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/grlpkvyvc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gkhvduvwt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gudhlavji.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gybsxcbct.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gaifqtdqg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfrkrwjcd.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gncgtogcn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gsbwyaswq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gifswntey.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/grrgybjdy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gpvhoeytz.sHtML


<!-- 参考信息 -->