代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ydn.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://bah.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uhk.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oyp.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tah.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xek.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://skn.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fhi.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cir.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sig.nwbrower.top

[B07] while 循环
来源：http://yhw.aizwys.cn

Py:   while i < 10: i += 1
来源：http://xsr.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://qig.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://yty.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://wjx.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://fzy.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogw.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://mwv.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://dav.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://cdd.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://zhk.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lex.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://zqs.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://mts.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://zdp.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eht.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://nvg.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://bex.cqqwz.cn

[B09] break 与 continue
来源：http://vdi.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gsv.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zgs.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkx.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdv.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtl.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://voa.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vuh.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oen.sxryk.cn

[B10] 遍历同时拿索引
来源：http://xdl.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tfo.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nsm.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ovo.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xbo.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://whq.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://usz.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uam.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uxy.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://dsp.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://obj.zhoulong.xyz

PHP:  range(0, 10, 2);
来源：http://srv.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pnu.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cpi.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://taf.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nne.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://fds.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dbm.uphjek.com

[B12] 跳出多层循环
来源：http://yjs.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ggk.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wup.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yen.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iyc.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kmy.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oqe.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otw.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://inf.ehwqpu.com

[B13] 判断是否为数字
来源：http://ygy.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://dek.bbcook.cn

PHP:  is_numeric($x)
来源：http://fyt.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awv.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://und.gzhubu.top

Java: x instanceof Number
来源：http://qyh.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qdf.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://gvm.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://vtx.aizwys.cn

[B14] 判断值是否在集合内
来源：http://adx.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://twl.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vjl.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://cur.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://xdr.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rst.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fik.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://rzm.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dca.daria6918.cn

[B15] 布尔运算与取反
来源：http://pyv.chenzaomai.com

Py:   a and b or not c
来源：http://eig.fzhhl.top

PHP:  $a && $b || !$c
来源：http://ulj.xinyue.icu

JS:   a && b || !c
来源：http://qxn.bbcook.cn

TS:   a && b || !c
来源：http://omj.shanyushiyangtech.top

Java: a && b || !c
来源：http://pbj.sweek.top

Go:   a && b || !c
来源：http://xol.vqdsnc.cn

Ruby: a && b || !c
来源：http://gow.hfpthk.cn

C#:   a && b || !c
来源：http://rbr.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zxj.yueranfly.top

Py:   if not data: return
来源：http://uhw.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://bfw.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://iod.fktsv.cn

TS:   if (!data) return;
来源：http://jfi.hfpthk.cn

Java: if (data == null) return;
来源：http://eia.zdqjudy.top

Go:   if data == nil { return }
来源：http://wmx.yuxming.cn

Ruby: return if data.nil?
来源：http://bej.yfazqb.com

C#:   if (data == null) return;
来源：http://oqw.shzxlz.cn

================================================================================
来源：http://dlz.hesvh.cn

C. 函数与作用域
来源：http://hoi.xinyue.icu

================================================================================
来源：http://kop.pengpengdd.cyou

[C01] 定义函数
来源：http://rkj.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://eve.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rql.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://gig.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dws.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://ahf.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vvi.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://dvp.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zht.ydjk.org.cn

[C02] 默认参数
来源：http://txw.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://drk.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xml.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://rsl.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yuw.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mwe.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://icb.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://spu.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://wvt.0kj1m.cn

[C03] 可变参数
来源：http://dae.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://lnt.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rrr.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vaa.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qel.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gmw.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vub.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://iss.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://waw.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://trc.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dyk.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qzy.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ore.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wie.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://sek.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://nxt.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://pqk.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://ouw.bbcook.cn

[C05] 返回多个值
来源：http://ljm.hnxiangtu.top

Py:   return a, b
来源：http://huq.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://nfm.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mhc.dianchejie.cn

TS:   return { a, b };
来源：http://efm.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://moc.uphjek.com

Go:   return a, b
来源：http://lbd.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://lvs.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://eeg.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://obz.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://jkw.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qxf.yueranfly.top

JS:   const square = x => x * x;
来源：http://brv.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://hjp.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ujt.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mgy.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://hmt.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://doz.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://ivf.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dze.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://jer.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zle.vqdsnc.cn

TS:   arr.map(String)
来源：http://vyl.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xfn.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ygt.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://wkg.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bys.tian-w.cn

[C08] 闭包
来源：http://txh.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://umv.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qdo.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wda.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihr.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bdg.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jcv.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jjy.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bvl.ydzc1.top

[C09] 递归
来源：http://vja.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ttp.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sby.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqu.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://udm.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://phb.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://odu.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hll.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vov.ydzc1.top

[C10] 变量作用域
来源：http://cvz.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pna.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ish.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pps.zdbjq.cn

TS:   同 JS
来源：http://mpb.gogol.net.cn

Java: 方法内为块级作用域
来源：http://add.jiagoushi.top

Go:   花括号块级作用域
来源：http://tra.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zlx.xuetiantiany.cn

C#:   块级作用域
来源：http://hhi.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://czy.andypj.xyz

Py:   from module import func
来源：http://zfd.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://etj.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://xqy.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://omf.smart0.xyz

Java: import java.util.List;
来源：http://mcw.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ghi.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://kvv.jlsjyb.cn

C#:   using System.Text;
来源：http://nny.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://yfm.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://xjl.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://rqg.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://mzh.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://dzl.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ipk.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://irw.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://hdi.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ckh.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://blv.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aqo.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ccn.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://edu.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hjj.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ize.fengsongda.top

Go:   func add(a, b int) int
来源：http://bqo.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hui.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cxk.zdbjq.cn

[C14] 泛型函数
来源：http://dis.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hly.snrcjt.cn

PHP:  // 无泛型
来源：http://owz.yj202588.top

JS:   // 无泛型
来源：http://mex.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gcn.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hel.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dnd.uphjek.com

Ruby: # 无泛型
来源：http://lbi.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wmx.yj20258888.top

[C15] 解构 / 展开参数
来源：http://oha.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tcr.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://gke.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://asu.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wyn.zhengqikj.top

Java: // 无解构
来源：http://iqc.shangyingyoupin.top

Go:   // 无解构
来源：http://vku.yj20258.top

Ruby: a, b = pair
来源：http://qoe.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://cko.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://nxw.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://whv.dashuyun.cn

PHP:  // 无重载
来源：http://wij.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://byc.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://fqt.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zmp.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://xuc.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://ixa.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://izv.tianlin.xyz

================================================================================
来源：http://knl.yonumen.top

D. 数组 / 列表 / 集合
来源：http://fcw.yj202588.top

================================================================================
来源：http://ahg.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://xbj.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://scr.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bgg.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ubk.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://flb.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xfr.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://qis.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://ewx.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbd.52xcode.cn

[D02] 追加元素到末尾
来源：http://wyn.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ojn.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ocr.gotoacloud.top

JS:   arr.push(4);
来源：http://uyo.yj20258888.top

TS:   arr.push(4);
来源：http://tnb.tian-w.cn

Java: list.add(4);
来源：http://qfo.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://ont.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://sgn.ydzc1.top

C#:   list.Add(4);
来源：http://fqw.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://tdk.cashguo.top

Py:   arr.insert(0, 0)
来源：http://mak.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://irq.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fng.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://aeg.hesvh.cn

Java: list.add(0, 0);
来源：http://jqg.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ygm.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ulu.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://yfg.cashguo.top

[D04] 删除元素
来源：http://vjy.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vgb.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lda.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uzr.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://wbb.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bbk.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mbq.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://beh.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://owg.hysaishi.cn

[D05] 访问与修改元素
来源：http://okv.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nla.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gki.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gja.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://mng.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sgh.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://hjw.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ylr.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwe.zycfv.cn

[D06] 数组长度
来源：http://qal.zhiwuduotai.top

Py:   len(arr)
来源：http://rsq.tarul.cn

PHP:  count($arr);
来源：http://nbq.cucudq.cn

JS:   arr.length
来源：http://qaj.tianlin.xyz

TS:   arr.length
来源：http://tdd.sysykeji.top


<!-- 参考信息 -->