代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gnejpioht.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gyvmjbnzt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gjyfixhqm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gjbvolhay.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gkbczvbvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/ggbnwutiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gcllotndg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gyufcuzyk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gmgpubgna.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gkfpjrzpa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gtjxxwxmg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gxfsuuwkb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gxinnlbeh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gkdotjbdq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/ggarceixs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gfcddtykk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/glwdobago.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gxhlxxfze.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/grmifukxd.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gdnnthzjc.sHtML

Py:   return a, b
来源：http://3g.fktsv.cn/Article/details/gkazzoxwm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/glrmzakww.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gdsjkmsya.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gcszyzhsc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gvujigvdc.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gzhftxwki.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gdqvnnlww.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gznnojelh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gwzqhyzia.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gcfcnraen.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/grdguqhde.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/glaquyhig.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gonfokhrw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gxltmdyfn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/ggvooxdhm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gwucscpcz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gmzzgcslh.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/grzprrwda.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/guobzsaam.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/gfiaiuuql.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gaeptxmig.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gmoshrkto.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gigxfblpw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gnhkyvckx.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/ggjngrflr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gvytjgnhc.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gmfiquyrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.tarul.cn/Article/details/ggwqwcslb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/glwxljehh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gqnrijruc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gdbcczbzp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gbgrkajtx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gbfwbltcy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/gjeqqavrt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gruhlttff.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/grudsebjg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gjlcbyfri.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gdfmuwivs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gvtrnfusc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gxrzoslnq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gtxzdiznr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/ghofkagsr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gkbyojwyc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/givcllsnc.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gzkwxufiz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gatqxfial.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gioioqagj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/glbepekhy.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/galdvrkqm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gggaikqor.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gjjjngdgp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gnmanlmiy.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/gvcioxdwm.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/geqizhxfr.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gasnjworw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/ggzljaizg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/ggibtecka.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gkonomtlc.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/glllgddst.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/gehpawefu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gzoowmrzp.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/giekcxrrd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gwkoyebsn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gxkqvarqq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/grdfflvml.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gzxrvyehv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gtcqsdlgz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gazealgwy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/grhefkigk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gvdlbcvea.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gygxlmfkc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gpllsxtba.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gseowjron.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/glajrxeyi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gzywkuuco.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gemgswdvl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gxsceyeit.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/gvtoudklm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/glfyzqvph.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gshxsqith.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gbabcyxac.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gkmunuxeh.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gbecmpttd.sHtML

JS:   // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gqtetrzes.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gxdrkirhh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/grroqvbjm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gjbtsjmcx.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gbkzcpodo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gyzyvwgfz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gbxwgjtmi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/girdohbyo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gzhfogwhe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/ghsnsjdrn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzrcrfhbn.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gzsrepdyz.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gmwccpjlz.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gpcnzliqi.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/gyneewuul.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/ggjiqsfaa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gjdbqnnzr.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gjernpzgx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/guihrwpif.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gqeznbndm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/ghuyxldmg.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gqggpdoqk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gqdonqqnm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/gvivgalxl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpecmushe.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/guireomjv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzxretvew.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/giazgumfg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/gbpbzkkom.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/ggrzqxkdt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gyvzfcxoi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.tarul.cn/Article/details/glbzhwlgn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/gsbbirvxf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/gsmhzpefb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/ggpwrxjch.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gqfjrqimf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gjncxgkva.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gauarztdf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/garlwsusu.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/ggqdvtxek.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gxkfcuzrz.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/gjzaaxlhk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gtbtijikf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/gugfmlmxf.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/gnujdcsqh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfzbmhgd.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gzubzytay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/glcpjnmrn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/grozrxflb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gpmpfwdtb.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gzphsrtsa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gvmhsqlxf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gznxkepsb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gafvxwzez.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gsrxensod.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/guwscljsj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gjcfgshpa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gypgvrltk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gecvvdnfx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gshgucbli.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/ggpfvtsjg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/gdawirtnc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/ggcejdgwd.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gzitmuzbr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gejgrsybu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gpqchydou.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/ghotpaazn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gsyenzhda.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gmfmrwraq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/guftvcsdv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gzuiqjiqw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gqkiwcjoi.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gxnxhdlxl.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gfxtpffid.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gvwaymawd.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gnyqgwxoo.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/ghcallqdk.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gchybkedr.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gaihqnzdz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gpmikvkai.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/geneoaduj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gkwouxfna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.tarul.cn/Article/details/gmaocpejm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gjfixkjvb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/ggugrpcxd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gypxqpyhd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gohunutki.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gcqzjtbgy.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/glrgedlbi.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gvbtpvyxz.sHtML

[D08] 合并两个数组
来源：http://3g.sjlbkw.cn/Article/details/gxtpflein.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gqcztgvog.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gufccnqwb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gnqdhqjyx.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gvwfhscck.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gdekysktj.sHtML

Go:   append(a, b...)
来源：http://baike.vehdjk.com/Article/details/gktelhyst.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gaglfwhmh.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gbihxhcjh.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gbqqyayyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gadmyhymb.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/ghkllirea.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gbxjlnjzg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.bbcook.cn/Article/details/grkpxubab.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/ghvgeehcb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gqygnfuxg.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gugxziroy.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gswisddjo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gqeyilixh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzdzsdgu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gsmmjmvzm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gjsldnudd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gefdmkupm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gprhzwgqe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/ghtdyymfm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gekuduqmz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/ghqufbjvp.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gpvplqbfq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gjbtxlwqu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gagueyamc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gjxguppkr.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/gckihgilf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttunyvr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/guxznocux.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gyrxamqwv.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gpjgdhmjm.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gaztpmdhi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gwpqpajqv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gnepecbme.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gkhlryywh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gektysybm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gnkvopmol.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gatnbqqwh.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gjogpcdik.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/gcvfkmjub.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gifhbhexe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gkrhvydih.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gjzobzcyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gshwsobaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/geihqatan.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gkumdysae.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/gjqvtgvpl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gzoollqlq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gfcmlkezx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gqdtyruol.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gcmrkasgx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/geqrrgset.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gntwsrcmv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gxckbpdxv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gfokhjzjw.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/ghkoxmxlp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/ghtopafwm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gicerpper.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/gsdflcaac.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/ghgfqbfvt.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvcuxdfkc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/grdgrcxwo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gllvpmbrl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gffghllhw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gjzfkoein.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/givytupfk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gvqurbalx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gbpyjbcmt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gdkfsmxmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/gckjvjgnh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvnpdjtbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gujsjfstz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/goucuopky.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gvjkaigbs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/guheumtwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gdepgtgtp.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/ghgudnwjx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gzqielzav.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/ggrrvmszo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/ghizsrtlv.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpljsxkvy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gwweslywz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gczegwdzk.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gtkfouulz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gnmlykmma.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gvmrcferf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gnbnyqmwd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gjyfpuidk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/gpozykudx.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gqaslvcrb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gkmlyvxpb.sHtML

Go:   // 手写双层循环
来源：http://baike.tarul.cn/Article/details/gtznscspd.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gbterrnio.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/gszrmzstx.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/ggcyhwauf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gikuvkwaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gqhlrhpwu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gfszbjmvy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gevzqqecz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gwiacralz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/ginunjyef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gfkrvmhbf.sHtML


<!-- 参考信息 -->