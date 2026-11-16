代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wtr.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kkl.mhx1999.top

[B07] while 循环
来源：http://kuz.fengsongda.top

Py:   while i < 10: i += 1
来源：http://fsl.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://fdi.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://twn.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://ljn.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://uqw.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xrq.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://fsi.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://vee.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://ctd.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://vva.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ywf.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://nzg.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://gtu.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://vyy.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vmg.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://why.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://pdh.jqgfzy.top

[B09] break 与 continue
来源：http://rvg.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dxv.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zkw.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yet.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owx.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubv.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pfg.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bmw.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtf.havefunace.top

[B10] 遍历同时拿索引
来源：http://xoi.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bum.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://glu.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://stv.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bdx.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://env.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fgk.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cfm.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ftd.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://ajg.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://bku.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://foa.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvi.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbg.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pqt.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vdq.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://lcm.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kng.9152youxi.cn

[B12] 跳出多层循环
来源：http://odo.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://skt.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://oob.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ipb.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fzs.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tjk.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xxi.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ofc.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gqb.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://upp.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://xrj.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://uhr.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hak.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lab.guannengcc.top

Java: x instanceof Number
来源：http://zgx.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xrd.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://ldr.aizwys.cn

C#:   x is int or double or decimal
来源：http://umg.yj20258.top

[B14] 判断值是否在集合内
来源：http://ryo.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vxy.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://idm.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://nvt.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://udw.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rsw.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://opb.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://kzy.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cke.gzhubu.top

[B15] 布尔运算与取反
来源：http://cij.c1oappe.top

Py:   a and b or not c
来源：http://ssn.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://dsd.ybcxt.top

JS:   a && b || !c
来源：http://xwj.xuanzx.com

TS:   a && b || !c
来源：http://dzl.shanyushiyangkeji.top

Java: a && b || !c
来源：http://lgp.vehdjk.com

Go:   a && b || !c
来源：http://knc.aizwys.cn

Ruby: a && b || !c
来源：http://hfa.svipenyu.cn

C#:   a && b || !c
来源：http://vjp.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pzg.hcnkem.com

Py:   if not data: return
来源：http://fpc.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://hrt.fktsv.cn

JS:   if (!data) return;
来源：http://gxm.dianchejie.cn

TS:   if (!data) return;
来源：http://ber.hfpthk.cn

Java: if (data == null) return;
来源：http://ydi.guowangkeji.top

Go:   if data == nil { return }
来源：http://ocn.sweek.top

Ruby: return if data.nil?
来源：http://qva.ivvv.top

C#:   if (data == null) return;
来源：http://sbx.ywan-chungtsiang.top

================================================================================
来源：http://bki.zdbjq.cn

C. 函数与作用域
来源：http://vcm.yongpay.top

================================================================================
来源：http://aom.bjfxy.top

[C01] 定义函数
来源：http://ojf.andypj.xyz

Py:   def add(a, b): return a + b
来源：http://ozj.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wim.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://irz.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcq.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ufl.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://qmo.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://kdc.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ugs.jlsjyb.cn

[C02] 默认参数
来源：http://qre.hammf.cn

Py:   def greet(name="World"): return name
来源：http://tau.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://srg.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://dfl.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iwm.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://erk.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nki.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://nub.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://fsk.ybcxt.top

[C03] 可变参数
来源：http://mxs.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://kyd.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qsw.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zki.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zaw.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://thj.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lsn.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://zou.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ztm.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://aew.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mbx.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lsz.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jys.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://flp.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://mao.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://qlj.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://doc.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://uzk.svipenyu.cn

[C05] 返回多个值
来源：http://xrt.pengpengdd.cyou

Py:   return a, b
来源：http://nrf.tanke756.top

PHP:  return [$a, $b];
来源：http://nve.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://twk.cqqwz.cn

TS:   return { a, b };
来源：http://hsy.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://foy.jinghuilouyu.cn

Go:   return a, b
来源：http://hbd.hnqzz.top

Ruby: return a, b
来源：http://eyr.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rjt.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://ixr.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://ghy.shanyushiyangtech.top

PHP:  $square = fn($x) => $x * $x;
来源：http://aow.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://tuc.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://iwz.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cci.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://peh.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://npd.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://rxd.nwbrower.top

[C07] 把函数作为参数传入
来源：http://uyu.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oze.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jbi.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dbu.hammf.cn

TS:   arr.map(String)
来源：http://pdk.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nqf.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jwn.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://qyf.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://sbz.bjfxy.top

[C08] 闭包
来源：http://ixa.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxf.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gzr.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://izr.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://klg.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fkr.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://syh.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xrq.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://utb.hnxiangtu.top

[C09] 递归
来源：http://wud.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mex.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wdu.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fjd.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsb.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wfj.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iik.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ldj.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://owz.0kj1m.cn

[C10] 变量作用域
来源：http://djn.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lpf.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nrb.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wdp.nanxuanxn.top

TS:   同 JS
来源：http://hpc.hammf.cn

Java: 方法内为块级作用域
来源：http://goh.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://rsk.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mtj.52xcode.cn

C#:   块级作用域
来源：http://ptp.andypj.xyz

[C11] 模块导入与导出
来源：http://ngl.quarkkingdee.top

Py:   from module import func
来源：http://jdp.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wbr.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkr.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rio.smart0.xyz

Java: import java.util.List;
来源：http://ssx.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iqk.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://xwh.ctjpmb.com

C#:   using System.Text;
来源：http://xaz.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://pio.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://jun.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://jay.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://hwm.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://qdl.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://liv.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://aja.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://xwr.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kxr.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://grk.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ibd.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xbv.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nkj.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izv.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ccn.epnwcf.com

Go:   func add(a, b int) int
来源：http://ofu.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lsz.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://lod.yanxiufei.cn

[C14] 泛型函数
来源：http://obg.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bnc.jlsjyb.cn

PHP:  // 无泛型
来源：http://yjc.xuanzx.com

JS:   // 无泛型
来源：http://jaa.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ubr.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ghk.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqu.feifeiyinyue.top

Ruby: # 无泛型
来源：http://yvc.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yrx.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://qti.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rgv.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://tfz.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qio.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vov.yj202588.top

Java: // 无解构
来源：http://qee.nanxuanxn.top

Go:   // 无解构
来源：http://uqg.fengsongda.top

Ruby: a, b = pair
来源：http://diw.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://yov.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://all.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qre.vehdjk.com

PHP:  // 无重载
来源：http://bnk.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hpq.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://sal.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gof.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://sza.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://rbl.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://sns.sysykeji.top

================================================================================
来源：http://avv.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://wip.zhijiandao.cn

================================================================================
来源：http://veh.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://tap.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zgb.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lzh.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ugf.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hpi.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pnb.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://vjz.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://ngx.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iou.svipenyu.cn

[D02] 追加元素到末尾
来源：http://vlz.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vyj.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cqi.yj20258888.top

JS:   arr.push(4);
来源：http://lmp.redwolf501.top

TS:   arr.push(4);
来源：http://sxn.quarkkingdee.top

Java: list.add(4);
来源：http://xdg.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://vhb.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://efv.xuetiantiany.cn

C#:   list.Add(4);
来源：http://mmb.tarul.cn

[D03] 在指定位置插入元素
来源：http://acv.hammf.cn

Py:   arr.insert(0, 0)
来源：http://bxr.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xhi.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nuz.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://vpj.iojbl.cn

Java: list.add(0, 0);
来源：http://hbq.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://oxu.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uab.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://xcw.dianchejie.cn

[D04] 删除元素
来源：http://hyg.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mhq.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xip.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://err.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://usf.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vos.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gyd.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wjk.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://adf.zycfv.cn

[D05] 访问与修改元素
来源：http://oth.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mof.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ecb.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ham.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://phj.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://dfw.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://bnr.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ikk.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aio.yueranfly.top

[D06] 数组长度
来源：http://ylb.yueranfly.top

Py:   len(arr)
来源：http://qen.cucudq.cn

PHP:  count($arr);
来源：http://fex.shuidangran.top

JS:   arr.length
来源：http://dce.jianghu66.top

TS:   arr.length
来源：http://tos.redwolf501.top

Java: list.size();
来源：http://jez.quarkkingdee.top

Go:   len(arr)
来源：http://htf.52xcode.cn

Ruby: arr.length; arr.size
来源：http://biu.wangdashe.top

C#:   list.Count;
来源：http://mge.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://bbs.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gcq.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://xgr.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://kaw.hfpthk.cn


<!-- 参考信息 -->