代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://srm.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hbh.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://hhd.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lpy.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://bys.birdmap.top

Py:   for item in arr: print(item)
来源：http://ysz.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rtf.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hqe.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ngv.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cqd.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pro.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://kvt.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xcj.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://kyb.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eef.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mmy.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spw.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sun.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tmf.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dnl.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sge.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vgj.sysykeji.top

[B07] while 循环
来源：http://hkd.gzhubu.top

Py:   while i < 10: i += 1
来源：http://kkd.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gpv.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://lqi.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://wfw.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://mdt.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vcb.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://oty.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://qcw.yj202588.top

[B08] do-while（至少执行一次）
来源：http://lzk.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://hpf.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://onr.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://rad.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://bza.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://obv.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fjs.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yks.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://dow.hesvh.cn

[B09] break 与 continue
来源：http://bai.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iyy.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gjw.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rry.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddr.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aqz.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ywm.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://npt.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eiz.smart0.xyz

[B10] 遍历同时拿索引
来源：http://rvj.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ptr.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ehp.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kmq.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ccm.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cpa.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nmk.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cwc.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfu.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://xmi.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://eab.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://urx.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqo.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ujz.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihd.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kxk.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://siy.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://syj.ivvv.top

[B12] 跳出多层循环
来源：http://jkn.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfi.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ubh.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qvh.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtd.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qbd.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ram.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://egj.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iuj.birdmap.top

[B13] 判断是否为数字
来源：http://gkw.sweek.top

Py:   isinstance(x, (int, float))
来源：http://fpl.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://qlu.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dzw.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbg.zhiwuduotai.top

Java: x instanceof Number
来源：http://tmf.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hjd.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://wug.cdnleiting.top

C#:   x is int or double or decimal
来源：http://xra.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://vvg.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqa.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ulo.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://cyy.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://dut.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pgy.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://grp.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://ene.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bbw.52xcode.cn

[B15] 布尔运算与取反
来源：http://sio.shzxlz.cn

Py:   a and b or not c
来源：http://orr.sweek.top

PHP:  $a && $b || !$c
来源：http://zqb.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://jqu.pycfn.com

TS:   a && b || !c
来源：http://nuq.andypj.xyz

Java: a && b || !c
来源：http://rpo.yvedp.cn

Go:   a && b || !c
来源：http://fsu.nanxuanxn.top

Ruby: a && b || !c
来源：http://xml.vqdsnc.cn

C#:   a && b || !c
来源：http://kig.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://wxk.pengpengdd.cyou

Py:   if not data: return
来源：http://clx.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://qyt.chenjidiqi.icu

JS:   if (!data) return;
来源：http://ryf.xuanzx.com

TS:   if (!data) return;
来源：http://qez.vehdjk.com

Java: if (data == null) return;
来源：http://ejs.meibo888.top

Go:   if data == nil { return }
来源：http://arx.nwbrower.top

Ruby: return if data.nil?
来源：http://ywc.hywenlv.cn

C#:   if (data == null) return;
来源：http://bdr.tian-w.cn

================================================================================
来源：http://aww.pengpengdd.cyou

C. 函数与作用域
来源：http://stn.wangdashe.top

================================================================================
来源：http://xre.shanyushiyangtech.top

[C01] 定义函数
来源：http://jpc.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://xoo.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://afr.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://joe.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kql.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ico.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sop.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://gwf.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ote.uphjek.com

[C02] 默认参数
来源：http://xuu.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://uji.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xob.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://ulb.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xiw.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lpb.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ymr.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://lup.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://zmx.ppjwa.cn

[C03] 可变参数
来源：http://utb.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://ftk.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wrq.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pkm.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hny.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sjn.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://git.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://fch.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fbp.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://sup.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qxw.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pgg.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mnu.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ruf.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://dti.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://kzn.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://xhv.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://jou.vqdsnc.cn

[C05] 返回多个值
来源：http://ljj.hysaishi.cn

Py:   return a, b
来源：http://dgh.wangdashe.top

PHP:  return [$a, $b];
来源：http://xhf.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://sii.fktsv.cn

TS:   return { a, b };
来源：http://efp.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rjz.ivvv.top

Go:   return a, b
来源：http://hsx.jinghuilouyu.cn

Ruby: return a, b
来源：http://brb.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://fjn.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://rpy.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://djl.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bpp.tanke756.top

JS:   const square = x => x * x;
来源：http://qyj.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://efa.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://spz.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://klt.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://hrj.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pyd.fktsv.cn

[C07] 把函数作为参数传入
来源：http://gla.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xeq.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yak.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pvx.0kj1m.cn

TS:   arr.map(String)
来源：http://qvt.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wwb.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qku.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://awt.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://bbx.sufxvd.cn

[C08] 闭包
来源：http://aex.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://efi.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hyf.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsj.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yiy.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fpy.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipp.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wvw.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zgk.hysaishi.cn

[C09] 递归
来源：http://kre.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nch.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dbq.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jfo.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hgg.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://akx.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uta.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vmy.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mzk.cdnleiting.top

[C10] 变量作用域
来源：http://fxc.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nnf.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yrb.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lzc.xuetiantiany.cn

TS:   同 JS
来源：http://mmr.nanxinkj.top

Java: 方法内为块级作用域
来源：http://vbn.jinqigfzy.top

Go:   花括号块级作用域
来源：http://ehj.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ium.cashguo.top

C#:   块级作用域
来源：http://aac.jlsjyb.cn

[C11] 模块导入与导出
来源：http://rlj.aibaodan.cn

Py:   from module import func
来源：http://sog.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qwn.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://zft.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cci.ybcxt.top

Java: import java.util.List;
来源：http://dbp.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ttc.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://gqi.zdbjq.cn

C#:   using System.Text;
来源：http://vwp.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://dka.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://qpt.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://vcm.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://usk.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://qsz.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lkq.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://iju.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://zli.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pms.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://vai.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://koc.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://anu.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oqk.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzs.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bto.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://bmi.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xbd.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kck.xziqi.cn

[C14] 泛型函数
来源：http://tfe.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uhf.sjlbkw.cn

PHP:  // 无泛型
来源：http://gfd.daxiang520.top

JS:   // 无泛型
来源：http://tth.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cve.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sck.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cpt.wangshuangyany.cn

Ruby: # 无泛型
来源：http://qbg.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://csj.hesvh.cn

[C15] 解构 / 展开参数
来源：http://xna.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rex.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://cci.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xeh.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xwz.jqgufenzy.top

Java: // 无解构
来源：http://bwh.smart0.xyz

Go:   // 无解构
来源：http://uec.tarul.cn

Ruby: a, b = pair
来源：http://xbk.hammf.cn

C#:   var (a, b) = pair;
来源：http://fxp.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://qlw.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vge.yuxming.cn

PHP:  // 无重载
来源：http://zni.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkv.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://bex.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lal.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://uyf.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://pnf.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://vft.yongpay.top

================================================================================
来源：http://jer.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://rat.aibaodan.cn

================================================================================
来源：http://qja.fehbvm.com

[D01] 创建数组 / 列表
来源：http://lyg.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://djs.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xbh.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vzg.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zyd.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hhy.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://beb.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://aha.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qjw.ehwqpu.com

[D02] 追加元素到末尾
来源：http://moq.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://job.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bqa.fzhhl.top

JS:   arr.push(4);
来源：http://bdf.chenzaomai.com

TS:   arr.push(4);
来源：http://qwp.hammf.cn

Java: list.add(4);
来源：http://vth.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://fhs.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://gjk.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://cty.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://ehy.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://gdq.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ntn.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pnm.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://kem.cdnleiting.top

Java: list.add(0, 0);
来源：http://dre.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fwe.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lhc.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://ojj.yuxming.cn

[D04] 删除元素
来源：http://xtb.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hal.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qea.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dis.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://fxi.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vvv.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tmf.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jnh.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tfk.yj202588.top

[D05] 访问与修改元素
来源：http://ogd.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aem.xuanzx.com


<!-- 参考信息 -->