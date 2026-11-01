代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gqcfqatao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gxotuxrte.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gaojzodyx.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gitidgvae.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/ghktqksxu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fktsv.cn/Article/details/gfjmjtadv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gzrcwxodo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gsnghhrhs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/giqcjlqox.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gpcluxjyy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/glaabasaj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/gsqmyyhkz.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/gighnxjsh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gllzwpvja.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/gimfzsyqk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gbpyecpbk.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gfsogbzso.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gosimfrxu.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gquvoxyil.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.vehdjk.com/Article/details/gbfcqxohb.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gicqurfuq.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gyqpvhogq.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/ghijcsfua.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gvmkdnygo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/glbeudtkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/grawbxnmo.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gfemkovzs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gddlsoyhf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/glqufhjxy.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gxgrrxiag.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gxindcvtw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gjjzyrdzh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gakfhhdzj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gafdkbgmq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gvtsvbdis.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.tarul.cn/Article/details/gzaoktijv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/gvruopqin.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.yfazqb.com/Article/details/gbegqtcti.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gnzkzoife.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gsydaupai.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gbmgnfytr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gbviettue.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/guludqedy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/grchzocgu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gtlcjdeag.sHtML

Go:   func add(a, b int) int
来源：http://baike.sjlbkw.cn/Article/details/gnuudfhdm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gyrpvccgp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gjizqdqup.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/grnhbfnfl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/gxkhbpzxh.sHtML

PHP:  // 无泛型
来源：http://baike.yfazqb.com/Article/details/goefdzpgy.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gwuhrsxqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gxwtabnxw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/guyjrcwgf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gtkstmcyy.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gaafpbjlg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/goznfbebf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gnjbrhawe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/givrjqkxq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gndepmmyy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gqgomczno.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gjijwhzyl.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gehejsvlp.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gyoddswxe.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gsopfazcx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gatuaadun.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gkvqknbmp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gdeuzvrii.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/gmmprstbi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gmehtgbhq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/grvqezggr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gwdznyytm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gyltypiaf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gdfayzxhu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnvfjmoxj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwyanbpcc.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gayxfpxii.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guhbjixvd.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gzepjiejv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gbvkqxyow.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gqkfzabsw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gmcaduxwo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/gmaejpdgk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gvyfjggjq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/ghotrvpqf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gysxdilzy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqvjeleg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gcpeivhbu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/glvqywoki.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.vehdjk.com/Article/details/gcpnvoktk.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gdykpzacx.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/groyzekfs.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/givylldop.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gyrkfdwcj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.yfazqb.com/Article/details/gwmygbacy.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gwigesyuu.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gtauhhdhs.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gupnjtbzr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/giabvcjcc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gjrenqiqf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gzcwycwtw.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gzpdwmuzn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.vehdjk.com/Article/details/gwezjhzqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gshxtywle.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gzdaoenwu.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gewdarbrc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gmlaresnf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.vehdjk.com/Article/details/gmocjscyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/glxmjcttz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gbrocrdug.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/ghycltrtc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gpjqgyqqp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gcuqhnxcw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/gbbikkjto.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gpjzveaaa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gzyzqegrm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gpkaoxvyv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gqsbitwuz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gbejjpntq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/ggleusfsw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gdjbxlddx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gacqpqnbx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/godtpbbqc.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gjlbvokta.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gkbqdnaoo.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gpxmaloau.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gzqldxdyj.sHtML

TS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gnauqfdyj.sHtML

Java: list.size();
来源：http://read.share.bbcook.cn/Article/details/gzhvuyxiw.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gptbzrlbn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gdncajbdp.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/ggwcsdiem.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.tarul.cn/Article/details/geuqdvcwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/gcfsoooxr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.tarul.cn/Article/details/grqiuqjkz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gspljyoqq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gouoqurkj.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gniqrogii.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gltqiistl.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gydwkkpwd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gpnxlwntn.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gudnsceoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/gzsypbbyz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/gcgagtlbk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gebldrkny.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gproyzufh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gdtxirqtd.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gflewkamp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gheufxbpb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gtzkvtlxk.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gyfbjpblk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gsdnrzjxz.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gakhndljj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gbohxvydz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gunhfgajh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwvslvos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/ghpuolmwv.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gudgegpip.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/guzgmorjq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gmkfmjtpw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/geljumiym.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gkllwaxam.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gkjtrwyym.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gyoirxsfd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gxwymdema.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.yfazqb.com/Article/details/gdeqpbuag.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.bbcook.cn/Article/details/gzdtsuyrb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gfqpnjtml.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/glmrwlsqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/groepgkly.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/ghhjxddqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gfacvxegj.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/gxfgvxwfy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gnfebezmt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gdkvdevmz.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/gknbgcznq.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/ggbnompmf.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gjscayhul.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gcohbbmnq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gffywdwqd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/glprflyqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gsonhxgdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gamqcmhrb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/govpmyrrc.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/gekcyscus.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/goaebcrkl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gvcyakftn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gxmvhlomh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/gbfvqwvji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gmemogmow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/ghddkjlwy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gbispxwvj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/giyjgxjvz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gwqosvprv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gnbvvkrlx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gescgpulp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gaewfnkux.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gmzohhnsi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gifodlbae.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gbryluccd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gqhfofopj.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gmypmiawi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gpcvjsseo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/geuywyjjo.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gkkrcjvno.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gzhmfukel.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gijgtyida.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gmvefcmzc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnxeeqgb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gmfuhahab.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/grnnidsib.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/grwbndwvn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gflmlysad.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gpwubbjxm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/grtfwicbs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gttgxodhe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzrfycxrr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/glyzdnsyr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gsrxfysjl.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gqfxoznmx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/ggvlbmmku.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gptnsuxwk.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gjxsqpppv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gllinripj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/gwkrxrgva.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gudlezhed.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gicdcksrb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/goastfkqv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gappzuxfx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/geuzxzgwy.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/gnebbwpcn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/gqefbaitr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/goclmsqqv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/givpgkuul.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gwtxqjkwn.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gasimxuym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/gtcarzdbk.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gddnahkbe.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/ggwniwjjd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdcmdwqgq.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gnokxshns.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/gbjlrkrck.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gbfuhvyim.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gnvrfyqaf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gpgqmfrwb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gxznbrxhv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gwrsfpzai.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gjbpcpban.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gnmieughi.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gflqtyugk.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gothrzltb.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gprinnvmx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gmrsfrxht.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gmejvgcah.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gicyqwkun.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gtblmvqzj.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/gpgsrqplp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gpppyajsu.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/gfgfanyft.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gvobnpxmi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gowbsebib.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gtkjslzgx.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gufpbuxly.sHtML

Java: list.contains(x)
来源：http://read.share.epnwcf.com/Article/details/gxgmvtkcf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggudndqmn.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gpqmnjqmh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmivxzyd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gqanjwepf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gufftzoxn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.epnwcf.com/Article/details/gkloyepku.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gfpvklvpu.sHtML

TS:   [...arr];
来源：http://baike.tarul.cn/Article/details/gufstdbij.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gviutptww.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gllocjfth.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gorvriuhx.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gckfqimpn.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gmeuakolq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gqshplvyw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gmeexhads.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gqlcjmcfe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gdtsfdnmw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gvhaigicz.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gsfesanbp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gpqvvcosu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gyajeotjp.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gddsbrqbk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gnxvodmth.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gxjgqfydp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gihuqbqsz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/ghrklyybx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/goyytjrdo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/gkdvglfjy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/gfnbtznlp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gqlfphwkq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gruwbmcwe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gslrkzkhv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gpdpwogui.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gexeickuw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gfaydcxnf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/gtprufjlk.sHtML


<!-- 参考信息 -->