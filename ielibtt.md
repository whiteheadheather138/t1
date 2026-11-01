代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gznxbvnwq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/grcnjslhx.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/glctzpfsx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gecqudcqz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/gegkussdy.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gjjsgsqjo.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gchvnjwtl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gdsrwzjog.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/grrrvtzbd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gfjrgaygj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gyykydaic.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/glrliaulj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gakfpkttr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gzktpurqv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fktsv.cn/Article/details/gysijowje.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gcnjedwta.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gzvwrkddv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gcvkcwimf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/giyzccvab.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gnxjkuibh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/galzckmih.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/gyieisfws.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/gefcnpljw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gqgrpfyav.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gizqrzuym.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.vehdjk.com/Article/details/gpqunvcnr.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gtknckneb.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gvxwktbtn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gkkxmqoeq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gkwsnejiv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/geisscmen.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gkarlqprn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fktsv.cn/Article/details/ggmwfqkxd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gpdbiqfze.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gjouoamlo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gxujxufzt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghmntcote.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gjjsdgauj.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gqqehuhju.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gbysvzaqe.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gguwqcpgj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.vehdjk.com/Article/details/gvihdatuv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/grrvgxcrd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gudbqyvzk.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gzhovociy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gbpxizagb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.bbcook.cn/Article/details/gsboetrqn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/giifdfjno.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gwzunghmr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gonxomtjf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnazdwtxf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnuqkaisz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/glrrogsbr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtraaytcb.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gbklvzubf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gteaqzrxb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gxvtgejlz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gpllovfdj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gzpnyfmum.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gbrpyzsfy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/gfgztfgrw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.yfazqb.com/Article/details/gbwsaovpp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gtnbhvgki.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gsunxhudp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gwvhumltn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gbuwqtzcn.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gqfjrevcn.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gtbnflczu.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gicctstqt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.tarul.cn/Article/details/gxkzyxdtr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.bbcook.cn/Article/details/gchmfrkoh.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/grefbbgyn.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gazcqxydk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gjqbwtbjs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gfuulzukj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/guykajzjg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gfgwfxpgj.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/grkvtdunw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gncrzknuo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gupbubcjc.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gfwhbhjxb.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gynfeuspo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/giiguqkxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/goekulbpw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gzjtwdmkw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gevmhqwgk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/gmulcywav.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.epnwcf.com/Article/details/gdvcbnhqw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/gvntetoaf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/gvitslwqi.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gjgzexxeq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gszjtcboh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/geapvhsnf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gzpxlxyms.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/gottwuxlw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.vehdjk.com/Article/details/gngosycwx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gqtjldcmb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gtkeusdyj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gqmqumdlb.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/gvqxnkbho.sHtML

Py:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gwepziuhl.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gaiatiomj.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/ghwzmvydg.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gsxlgwvkx.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/gujwhqfmt.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmbqvahbk.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/gusxqosgy.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gealjbrjk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gebvtnpik.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.bbcook.cn/Article/details/gniwzoimq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gtagadyeg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gxtklmwgc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gixiccerc.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gktgqszro.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gemupmgct.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/gmfrziqbn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gaifhgsvw.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/glokvchve.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gzupqvops.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/ghqnsmoht.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/giwchfcpp.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gtdepvqqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gjjiossyv.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gkwijazxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/geqoeoyte.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/glyyancxj.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gjjbgiscs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gbqspuhcs.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gixhaxuxo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gqbyiiuos.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gdgweqshv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/grcejhhaj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gctugzpxi.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gvfnhkosz.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmkwfsnc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gokgtxkqg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/glplqpoxr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/grivblocu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gwiogfwxv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gccerchxv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gctfwdszr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gynyrhugp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/gpiybxdhp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fktsv.cn/Article/details/gfwktnpmn.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gzkwaztcl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/glmgemobf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gnuzhzkrg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gnjjavysn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gbtenmknn.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gsmpbgzhi.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/gkserqapr.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gtlwevydy.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gwsorjxzc.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gxgfcyelo.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gkfxtfuvc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gifjawnaj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/ggkbskath.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/geqvnlmip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/gizaybdzi.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gnydmghrq.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gmuaxmclx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gucfnvfvk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/ggdajjyvk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.yfazqb.com/Article/details/gylhscvwu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/geoamrqgp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/grivcxxrm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gbqxxtsub.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gvvdxmgmg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gkfomdtwk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/gnlgauunz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gwxfsecxs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gjouzapiq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gvmkunbzg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gobigjnkt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gxmmpebay.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gqxhpjhzv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/ggnalsout.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/glziwzaxs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gmytkmbfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gasdexgna.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gongneazw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gugrzkfuo.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gqqzgpssb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/ggzuhzjkq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gxjpjlpze.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gzcyhxbfp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gpodnkegx.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gjwazfoxy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gopzrbjbm.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gyyhzaydi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/goixusnou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gvvcyislc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gorjqrnwv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gxcookwwk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gnpossrta.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gllzzlkyl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gshphlqbe.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/ggcuqzyzk.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gvrrvdyak.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/geyvmhvfd.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gxtsxyvnm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/geaulwakm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.bbcook.cn/Article/details/gwteouzun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gothprusu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gvakiqgle.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gnftknfrw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gwvyxfuef.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/grcnwcvpo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/ggqjoipwr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gdqnplxsv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.epnwcf.com/Article/details/gvpekoirq.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/gscohxpjv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gcxbtumhk.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gwkoyykcc.sHtML

Ruby: nested.flatten
来源：http://blog.tarul.cn/Article/details/gfjlhidcz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gswsayxvh.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/ghgbpavyg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.tarul.cn/Article/details/ghywkprqc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/glhklkubr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/glxrikdbt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gufkosiqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gnjbycygw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gvraqamwl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gcsibkccg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/ghrwjueuv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/golxcilqh.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gzvrrflsp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/grvyornmj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gotrgdzkq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gdxzvqvdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gstcmnkfa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gnarsplzq.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gcqkqisjr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gsczgifer.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gpxzvypem.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gajaotfqe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gplvhegqn.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gvdfvrdpq.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/guzvkokvb.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/guxjxthgm.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfgujdwmz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/ggwgklgke.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfrcftujd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/grrtxyklp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gzfggzbif.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gpuvosgsa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gnbkgrajl.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gneimgxkj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gdvuvldai.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/grvfupdae.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gfiecamxz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gikhsfbdf.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gserltbqs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gdxarioao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/giyjzpuxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gdkpdbizb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgfpnvkj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.yfazqb.com/Article/details/gxiyggjyn.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gqrpxyuyx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gxtzflwye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/glfpovrqu.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gqjxxyoyz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/goepuihqy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gmztkdzut.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gciwjwsco.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gkeeakwlz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gbpwsdxwq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gsgaljjde.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gctzddsrp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/guyrqlfmp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gkvonqkyp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/gojumjace.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gyslambrn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gyfxrsotj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gfsyxxsbg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gppqasbre.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gysndwaas.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gkclupffd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/grfmhmxxe.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gxgtkveax.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gnqrvfenn.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gwzulklqr.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/getwzyhmn.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/glyahtypj.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gliijpbhk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gezbroxhv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/grqdsmrdj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gutjhmelj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqnyxtmsr.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gdjvcxzuo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxtrxsbqh.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gggxtvpgf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gdikhylom.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gddpynkjc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gzwiclljz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/ggzukzpea.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gmogoffyz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gmvozljvn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gtbpifzrh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdptgzhiz.sHtML


<!-- 参考信息 -->