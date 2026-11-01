代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gezxlczsg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/getuldouw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gfmwdpmve.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gwujinitx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gbwtpefrj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gkrwgvnph.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gaeprkjpg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gimsplqvg.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/gnwpncrmt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/gyvadpwhe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gpdqodvus.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gaxofjgag.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/giuvpwuqz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gbnpbkxiz.sHtML

Go:   花括号块级作用域
来源：http://baike.yfazqb.com/Article/details/gtwnklyoz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gxepqorzu.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/goaugvnnh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gwirdxiio.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gbgpplizi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gpmhoqoww.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/grdrifxjr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/grivwjauh.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gcgptjyik.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/gkfhbxubw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gwmdktoxp.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/ghgiedhpe.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/gnppmdfoi.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/geseydpcs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gvrgwvufb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gmczzlyho.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gurrnzfla.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gblztfrej.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/ghyyzbtjk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gbexiyguc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gvcaskgzt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/grbzuzbzc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gfjxamfwq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gmagxzkas.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gcuezznnb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gfyketeqm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gghwjjzey.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gdtaiyfkz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gcrjnyizy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gmyuknqtf.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/grlpfucvd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gmliccidm.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gbmffqjgl.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/ghfwczbpo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gbxvckade.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/gajvsmpyq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/grkkbmbts.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gyepffrps.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gghzaxcjg.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/gtlhpushf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfrnkdqd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gawaaimnb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdwnbyana.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/guenwdcto.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/geguhygag.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gcinxbxpi.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/grwkzcwyz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/ghzlfryzd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/glebslqrs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gmfsvpkbs.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gazrhunxq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gkcoapavt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/goyaidzsh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gvpmpomvg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gbiabfhhl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gmjtrtnlo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/guqujzlgl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkldfaeeu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gyrsoobzo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gunlskmfk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gyyepusrn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gjibpyzdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/grjatybub.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gbwjcnyjm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gnsthkcbt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/gcqpowtqq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.vehdjk.com/Article/details/gvmuhzymi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gohdpytng.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gyclibuvo.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gpwitlgmh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gezziucbe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gssaixcdg.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/grbjhjnkz.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gzoesuzqe.sHtML

Java: list.add(4);
来源：http://read.share.yfazqb.com/Article/details/geddpmfrr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/guxwxpvwq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/gyxhuzzfz.sHtML

C#:   list.Add(4);
来源：http://m.share.yfazqb.com/Article/details/geuanxnmp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.bbcook.cn/Article/details/gibgungro.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/gtqmerykn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gggilvflj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.tarul.cn/Article/details/goeywucni.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gqijsfboj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/goyzwuphv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gjzictrnq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gtqfldbaz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gflrpwwpd.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/geuuibsta.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.epnwcf.com/Article/details/gyuvutvjw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/gcnrafuac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gedwthujs.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gtpqhqcnv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gsrtprajl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gkcwtyhkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gvsfjvbqc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/ghtxykcxi.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gkgrrrphe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gamltkmxw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gjhbrsxmx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gadglxenu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gjitxwzrh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/grfsxzlky.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gkrzgacrf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gkhpsydjm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gqqivzqqd.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gylerbsiq.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/ggtiosedk.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gmouvarym.sHtML

JS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gpsdqtypq.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gbwkqixrr.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gmvwsnozd.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/ghzqxlhyp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gjyuuadog.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gwswhzgds.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gjriuhxiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gqqumnqbc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/greneysuj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gqkdyqbbq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gxgtjjwoa.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gyulisufz.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/goxgwtdqf.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/gjejazzqf.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gkiklvyht.sHtML

[D08] 合并两个数组
来源：http://3g.yfazqb.com/Article/details/gerbbxoay.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/guczymigr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gavwtntiz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gxwgswhoh.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gileatzuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gsixcblkp.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gyyqvmdth.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gubgalpsr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gnollqztc.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gmaudytao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gvwwfdpxa.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gqswjangc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/grjyaywlz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gfkizggvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gwsthlzga.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gqmoiodxq.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gglmkytqk.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/genqdrhhz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/gwmgnlwnc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/glfzvgpvb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gjcmkaqud.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gkxmluudk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gcccuxpil.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gxklqarjt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gcupltzmx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gyofvgsos.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/gcubwlezs.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/gfpiagtmi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gqrhrboac.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gzjcnucdy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gdizdsgmb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gscgivcju.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gfdbrslnj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gmzovgrgk.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gyfwuwywb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gwdsxjakz.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gtrtskqka.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gurtttyql.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/geyzzbfve.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gpyipzuva.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gsyaxhcfg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gnlkjynwi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gdmoysjaz.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gfptjpqda.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gwehljydx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gwrfwrhzb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gxmdukqmk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/gjjbqptpu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/ganjpkapz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gksxqnzqh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/goebmjqvs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/gqemafgej.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gcqlctxka.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/grpcdxdyo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gbkexgptd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gfehjezzb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gazqcywck.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gztqcgmed.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/grlgukiyf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gpibixxij.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gkiexidnr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gqxsjkbrl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gllyqhjqg.sHtML

[D15] 去重
来源：http://mobile.epnwcf.com/Article/details/gwpzdbhls.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/glhtvtasn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/ggduudskg.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gynhotlmb.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gseahqqgd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gwahkvoyx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gtmphgivc.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/ggiivzciq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gdrutcvzj.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gepzrlawo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gvokzxwdc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/gfwoocuel.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/goxrjiyvs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gvpwkzgyw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gzgshsjko.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gmsfyetmh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gvqlnwlba.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/ghsutroly.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gdtetptbl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gxgbmrizn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gvmywiqha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gbmlcqnyk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gyemhbnrf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gdugwmynh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gqstgpncr.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gbfxbhwls.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/grlvsmpwr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gmiftlqjt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gvhavrcbl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/geqqdqxrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/grmfjteok.sHtML

TS:   nested.flat();
来源：http://m.share.vehdjk.com/Article/details/gdotkpfod.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/ghjyytitl.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gjqwmycsa.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gkxfoogex.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gultbsdie.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gjcfwotyq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/glzjhuzpk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gxquttcju.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gmmraysgo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gfgldlwtc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gqfrcsfny.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gzhspnagb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/givfwdhas.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/ghnhtakpv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gifublpoy.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/gndjyamgd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gsuncrrlx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/ggrewycld.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gatnefxyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gxggdthzs.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gqjvtwwhq.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/ghsipalps.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/grnahhkab.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gkoixlvpx.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/garuxcngv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gkqehbekn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gtcuwmqqx.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gahzuwsuw.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gytpqrohb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gsgosqlbm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gpmpixkoh.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gohwiyhjd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gemdbukre.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gtvmlwffc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/gswgrafze.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/ggdiysvtj.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/glzrmsvpl.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/grgpyennq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gwdbedcos.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/gjsnlgdxs.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/glbijgmbx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gqdkkhglm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/gxhhshytf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gfcjqxvtp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gqqaciobr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/goumesagx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gpdnunhtv.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/geylentlp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/grjdzykzt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.bbcook.cn/Article/details/ghpstrqzl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/ghcrzxyjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gkorqawhb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gouxnrzob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfiuxrma.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gcggeaejy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gprcmnwmx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gfbsxztrl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gttsacmhc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gsybtootm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/gpgeluedc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gcvznzbrv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gewurjndv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gtnidxsgh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gxiqeexwa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gptiabefi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gkqigqpfn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.sjlbkw.cn/Article/details/geqnqgiaj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnoufunil.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/glhkhogar.sHtML


<!-- 参考信息 -->