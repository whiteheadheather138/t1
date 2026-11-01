代发 wailian999

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gjnclgwsi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/ggddjobpn.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/giwzrvsmi.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gzymuoybn.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/giercvjrq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gocjknxaa.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gzheecvhp.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gkubsptzv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxgcltmk.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/ghgpyahau.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqcbjxnzw.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gwylheylj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gvzbraaxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gokycczfx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gktnmnyjg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gkezrcyvj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzprbvvfv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugnbvunw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gbyfzdzdn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gwwzcrfus.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gaulyntht.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gmduowmix.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gxkocgdmh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gpybpakse.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ggumemepp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gwqtcrywt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/grcyrxuje.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gmcprszch.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gmzlmkdxp.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gforvxibf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/ghtmosqnh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gaurkcqtw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gxavpopub.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/greukbsau.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gyxmcjgde.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/glsmwjqoa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gkkltssrh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/getaiicrm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gslvtxalw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/goarygryv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gykomgcez.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/ggxzzbmzd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gbexgtbfa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gguvwofau.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gkgajaayp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gdfdgnaao.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gvjudfbwm.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gxgyvrqvv.sHtML

Py:   return a, b
来源：http://wap.bbcook.cn/Article/details/gxjkhgcvz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gzycabfgi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gxfztipud.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/giruefgva.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/geyiwawzi.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gvhreohel.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gbfgxznab.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/gpphqnitd.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/glbadimat.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gpnlcjddm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gryjyzggc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gmjepkaeh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gwxvrhpti.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gtogwwjrk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gxjjlaebt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/ghdadfcjm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gupytwrwi.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gwrggsmgp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gttgkjexe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gvamvaljg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gyshlrbuq.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gcuijckxx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gizgxgtbb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gcnvtsxoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gyswpcqxw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gjwdvmese.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gsnfbhnns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gkvcjkwgr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdrvgraz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gjfsbewvy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gesktvyzq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gntrbvflv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.tarul.cn/Article/details/gmolkfjip.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gvnpwejmt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gngvnntzp.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gybnugjsn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/guznluxjz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gtxeyduoq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gkyuuzwnx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gvrrwmvcz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gkpajwjrs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gaxyfsqqq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gmdzkkqgl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gvjzbnqof.sHtML

[C10] 变量作用域
来源：http://3g.epnwcf.com/Article/details/gqejhzvrz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gejguqgfw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/gfdbyddqd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/grzwhheoj.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gduxoaczt.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gqsyqtqwz.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/ggcpahgeh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.epnwcf.com/Article/details/gespokzxz.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gkvzfytft.sHtML

[C11] 模块导入与导出
来源：http://read.share.bbcook.cn/Article/details/gsuztpmco.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/gkcbeutxz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gqrarymqu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gkowbwvnk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/gvajzctfs.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gdcxuxyrp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gtjtacoll.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/glwolhpot.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gpxqojykg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/gylbulzrm.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gpgnbyvik.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/gtpmfddsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gzuecdoyp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gdyyzzvtt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gmqprxklt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gvipexesp.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gpmcvlegv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gtuzkvjuk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gyongdsih.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gzhmhcarr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gwjqsmkzy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.sjlbkw.cn/Article/details/gzszsfrsa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gjmehxdlv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/glnybsbjs.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdynmybb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.epnwcf.com/Article/details/gknhtizvr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gtqzootub.sHtML

[C14] 泛型函数
来源：http://m.share.vehdjk.com/Article/details/gncuxnqaq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gznvwsnrw.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gowgmonwk.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gtunmkwan.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/ghlfyrkkh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gphahcjug.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gdvzgdvqn.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gdahlstks.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gxttmfafs.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gueyaeouh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gtabjxseg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/getcrejba.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/glxjbiwlj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gzmyxdtxs.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gxaionxzx.sHtML

Go:   // 无解构
来源：http://blog.vehdjk.com/Article/details/ghzpccbpo.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gvedqyvae.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gdmgsppjl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gomltpfrn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gglsaitbq.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gjxxlkacx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gmzkyblro.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gkbsqavif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.yfazqb.com/Article/details/gendphufi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.vehdjk.com/Article/details/gqmgsbcst.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gevxxnlyi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gerofhkkd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guixhxqlw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gjdxedyqi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grvcamexv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/ggrqmdbvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gjwpwydqk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gpskjfzsl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gidwykmst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gntqgrsxj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/ggyznoket.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gwwhtgcmh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gonvegmhx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gvmuomqsu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gvqvwxjsq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gswbjixxp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/gwftdvirf.sHtML

JS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gdvjuedzm.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gewpndvsz.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/giiowtxqj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/guwgfemnj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gioqpacik.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/gtqthbsvi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gshwesvkh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gizqausps.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gdqcyfypn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.tarul.cn/Article/details/glcncqzvo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gvuivbcsm.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gbmyrhlrn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.bbcook.cn/Article/details/gbbjtqiyu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.bbcook.cn/Article/details/grrucgmtk.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gxrddbeqs.sHtML

[D04] 删除元素
来源：http://3g.bbcook.cn/Article/details/gtomayifu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gmbpvxwjz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/gzkigueoi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gsjwffbgl.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/gtrkaeuwh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gyezgxwon.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/gypbjpbrz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/gncrodkbr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gpsjwxjhf.sHtML

[D05] 访问与修改元素
来源：http://m.share.yfazqb.com/Article/details/gaedodyth.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gmnoquzug.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gntfryizy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gpizqhwfx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gujvvhpde.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/ghvtxbszb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gcgshfvys.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gsxvgjium.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gjsxwjwti.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gxpjmmuis.sHtML

Py:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gsrdercui.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gmlarccvt.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gonovxksn.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/guraivzfk.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gxyumuglg.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/grosyaidz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gvhfkzqhh.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gzshmsxmi.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/gxegomcwa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/grfymnmgj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/glvnnybrc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gfosqvkpu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gfsulxifr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gechfbmqf.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gclfqphba.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gstglnztf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.epnwcf.com/Article/details/gdylpmzbc.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gsngxkxpl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/garwegdps.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gxxhwnrwh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgdqmhfl.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/giduwispq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gjmxynrzj.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/gdzmfsbts.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gwdtvqvdq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fktsv.cn/Article/details/gzphsmiug.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gvtdpbyeh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/giswmcapk.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/glniipdda.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/gbnakvecr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gafqymxqd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gcykydbdj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gxalwzraf.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gzvuyvfib.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/gpjmrvlix.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gxcnzzzmr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gbzueupyf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/grghtjxij.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/grshlimjm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gjjvwovoo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.vehdjk.com/Article/details/gubysdvhi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gzncoxrve.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/gcnlvcuok.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gowefsbqn.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gnhkbpcqj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gsfowzjmb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gdluabqcx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gowrtzhfd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gglhsfnyv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/gwbhhjtvb.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/gshwwcwgs.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gviofwvzt.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gxojabmxy.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gcryxciej.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gnmuirocm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/gmliwjfzk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/ggncepitn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gngktsxjt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gjenmqbzb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gqakhxpxq.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gfinpkozt.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gckurhlbl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/guknmhkou.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gpbnwmxez.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gfnsayvqs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gynbbecps.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gtxjuhlun.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gxujsqyoi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gzshqermr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gmqpunqil.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gdpoaaonv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gohkotxng.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gxzjafaxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gesmhdhqz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gsevwhmdp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gszmdyzmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gmtmggvou.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gccmdreox.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/ggbqefqer.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gbfdmktyr.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gfeocusvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gxebyvytf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gfujiejwi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/ggwpfygmy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gdgqtrzdz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gztnqxvfy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gggwwnsij.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gaixcxtdp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/grpolbdxj.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gzvujrctc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gkuxuxspd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gokxnqpay.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/ghokzmfrw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/giqjmhapv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gfdgefopw.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/ghzvniwxa.sHtML


<!-- 参考信息 -->