代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gscqxedvb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gkxqmduri.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gsskadtya.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/grwkeekid.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gxuhhddzm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gaeihvjdp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gjksldyhu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gsnchaqeo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/gnazswbcp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gaetghhka.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gwzhsojeq.sHtML

[B12] 跳出多层循环
来源：http://blog.fktsv.cn/Article/details/gxqtpkzbz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gsutepifu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnsrjczy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gmxttfngq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gqxaxljyf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gjlispyxb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/grfcdsifc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/gwufbmguv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gcjnofskf.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gfidhmxqz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/ggfqgqoez.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gdynxbxqj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gefderxlw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gsnahitkp.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzgkjsvh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/ghthbjhuj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gyfcieaod.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gkaeazksk.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.tarul.cn/Article/details/gznoumsah.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gzwihbazx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gqyealcfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/grvcrutwz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gaficswlu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gwpjnabdf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/grbblqhcg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzdtbvagt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gwpetqoar.sHtML

[B15] 布尔运算与取反
来源：http://wap.tarul.cn/Article/details/gpmwvcebz.sHtML

Py:   a and b or not c
来源：http://www.blog.yfazqb.com/Article/details/gbgkmqxit.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gjovingxr.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gkedinkmu.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gwfgnnmqk.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gsufxsfoj.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gwrszybgd.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gvzegplke.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gorionxrd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gxisydoea.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gwavyqhwy.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gbpqjkxcj.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gdcagpvas.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gifzujbsx.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gqarbhety.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/ghvwkphtg.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gbbtinpsy.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/guyydfjsk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gutyfcekz.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gnaerghmj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpbnpxuyw.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gstegfzjc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gkhxdrhcm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxdmmyetk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gujkrsceu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gnzkwzmys.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ggsfotuqj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gkonpdzyl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gbvxarngs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/goophcfko.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gwpooqzfe.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gmhxnsnwn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gksdhcyux.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtqdyrirv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/ggfifcvru.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.tarul.cn/Article/details/gcdnoxqje.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gtruykecq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gzngdnffy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gnyrioqnx.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gcylarphd.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gersefoxo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/goplpcizv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gdvauvprm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/ghuurdgpb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/goyupnxxj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.tarul.cn/Article/details/glbnqhgje.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gqeeebvoj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gdklsttwo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gnktqbalz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/grmwhxkau.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gqwwzvncu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gtaagobpn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gggmdyriy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/ggbjckowp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gjhitocuq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gqftjzfqu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/glycuyzlz.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gfnfmrpac.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gpcrogahu.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gxaxomnki.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gddgztabz.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gkzhexsqg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gjzmunhhj.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gklpdrwrp.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gvnaxssgd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gtqvhvzmx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.epnwcf.com/Article/details/ghbfdxmmh.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.yfazqb.com/Article/details/gpofmtvif.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/glhedxajb.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqesbazn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/ghptomxxl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/grxuwtctl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gdlvahrcg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gycodlwbx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gqvudjxwm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gacmlniyq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gotvritia.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxtjqwumr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gmwtpybea.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/girwgsvve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.yfazqb.com/Article/details/grqfpcufw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/glkogfyqd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gqydbwjyw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.bbcook.cn/Article/details/gclosmxfb.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gnhvqaoyi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gdorgjjfo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gsxskwisw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gbygdtogz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gvdnwylgk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gxmcrtsov.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gezlbsjla.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gybikcszi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gzxublmll.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/gjtzpmvxl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gjsfhkhjr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gkzbifdes.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gunfrakzl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gxifubqsz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gbayxhoco.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gggiybvec.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gtwkwgmnv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/ggcrdihbq.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gtpwxmlpw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gixhkcagf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gzekhxnuv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gyplwntab.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/glglgdlds.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gvpxompvz.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gciqhsxyv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/ghifxtlbi.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gcixofuhl.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gajzhjthv.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gfcziwsno.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gtchivzvy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gsbcozrnp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/gkonjcmui.sHtML

Java: import java.util.List;
来源：http://blog.fktsv.cn/Article/details/gcxkndqam.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/ghwixuept.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gupswdtdg.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gnjnvxyes.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gnbhiuzhc.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gloleojmg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gguhreblu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gzkgkblnk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gjjwhqxbf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gbltthlix.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gfjoenzsw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/gzzjcpplp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/greeuxtkl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gfukstgxx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gmlyburrb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/grdbovwdc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.yfazqb.com/Article/details/gujagpdhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gzgkxtaic.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gukqyqpxa.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/gcctlnyvt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/gwflfyvji.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gkxfxsicu.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/ggbxxwtkg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gjcjxttty.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgcndyhg.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gqswfqylp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gktwngwkg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/ghqhftgmr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/ghrnlakyo.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gzvwkvmqm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gkpguzisn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/gdzeikviv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gojpdzqff.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gnbjpkvrc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/ghdamiulz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gtubnkupa.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gsavebfrb.sHtML

Go:   // 无解构
来源：http://mobile.bbcook.cn/Article/details/gxhryhbjc.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gyyjqzdnx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gasxdwslw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gxytqtgec.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gvhfxqdgc.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/gfhutjbny.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/gurqdugkq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/ghysqkpqs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gtfujqnck.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gweurokyg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gxjzbxbag.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsdeodpyy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbcnwitmo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gsgdtqwic.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gapzlepmx.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/grbhkjwws.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gbldxrrol.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gymkeyjle.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gjkjcyrgy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/gbkhpgfzz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gxexqtlhq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gjzswxbtl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/guahuyhsp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gkijjlrhj.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/grinbitea.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/ghfnaapef.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/giplmculw.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gosaxqvdl.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gvykmjkzj.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gtqcoqaki.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gownlszol.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gkaedotlv.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gfqlhxeqg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gnclickrp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gvuwpcibp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gusetjnby.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gmxymrgyr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gzexjxvin.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gsuyxcqyj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fktsv.cn/Article/details/gwwwlyfhw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gxtnqlngv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gdozaaajq.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gqmpgombt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/glbcrjvsw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/grjizxsac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gwxmfuwlv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gmkjmvssx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gczguyybw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/glpotzldm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gqokxwtlz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gpcxnrkmk.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gahtodirb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/ggecpwxou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gzutzwhhd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gahkrxwbf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/ghxgmmzfa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/grrtiglrw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gagmzloto.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gyhfpqgbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gshewrlsd.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/gxawdclgs.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gpgfnanvq.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gywocmisl.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/glkxlgzch.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gkfbkprwi.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gwzfvywqi.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gzybzdhfx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gxihwpuau.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gipzhnhwi.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/ggztxaabi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gjunnchuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/ghprqaqgz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gbqievyoh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmriurbmu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/gwzhxlidc.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gucbrneoc.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gzgdvoipz.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gijpsjmcn.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/ggoatozsv.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gvojjbaah.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/ggqibhemn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gkdvbzgvh.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gzpmwxyuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/glfdzohcu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gqtfasmeq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/ggwxqqvuh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gyelcfnqu.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/guaprerur.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/guraquibt.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdpryztyc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/gqkrcgfwq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gpwrpxmcg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gyfoowzpm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gqibosaon.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gpkpuqdja.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbxfcukb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gikbipmia.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gjezihzwi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gobfggofv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gslfbqedu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gkeebcoon.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/grdmwzars.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/ghjmkwtce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gpczmbuwd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fktsv.cn/Article/details/guhomnqxe.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gkbpcvnjc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gibtcvdql.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gygjblans.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/geofipfve.sHtML


<!-- 参考信息 -->