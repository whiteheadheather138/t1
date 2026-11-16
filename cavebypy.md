代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://crx.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zgi.gaohongyu789.top

[B07] while 循环
来源：http://dpq.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://rhj.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://xpg.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://fbj.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://ooy.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://iqm.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ivn.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://zqb.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://wkr.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://psm.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://lng.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zga.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://ffi.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://lne.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://bqk.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nvb.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ema.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://ztx.tarul.cn

[B09] break 与 continue
来源：http://zyx.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://djr.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://obu.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcl.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yig.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ztz.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://inj.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ooe.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kah.ivvv.top

[B10] 遍历同时拿索引
来源：http://xcd.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zvn.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mnk.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dqz.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zaw.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://taj.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dzi.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kjd.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zmi.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://cwm.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://lmb.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://xwg.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sbm.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jvw.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rye.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfz.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://ykj.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rfo.epnwcf.com

[B12] 跳出多层循环
来源：http://egq.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fdz.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fwz.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rfz.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ify.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mxb.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dos.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mrn.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cjn.pycfn.com

[B13] 判断是否为数字
来源：http://kcf.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://dev.bbcook.cn

PHP:  is_numeric($x)
来源：http://wag.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bzp.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmu.tanke756.top

Java: x instanceof Number
来源：http://fxd.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bgr.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://mun.svipenyu.cn

C#:   x is int or double or decimal
来源：http://ejw.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://cwk.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jwr.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dsg.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://pzd.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://hjx.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://odj.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bgp.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xhd.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hre.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://dph.gaohongyu789.top

Py:   a and b or not c
来源：http://vuh.sysykeji.top

PHP:  $a && $b || !$c
来源：http://nft.ydjk.org.cn

JS:   a && b || !c
来源：http://sab.zhijiandao.cn

TS:   a && b || !c
来源：http://ekc.haohaochexian.top

Java: a && b || !c
来源：http://vlh.tian-w.cn

Go:   a && b || !c
来源：http://fsi.ivvv.top

Ruby: a && b || !c
来源：http://cqp.nanxinkj.top

C#:   a && b || !c
来源：http://mdn.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://nfj.vqdsnc.cn

Py:   if not data: return
来源：http://sga.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://jkg.andypj.xyz

JS:   if (!data) return;
来源：http://ted.mhx1999.top

TS:   if (!data) return;
来源：http://stf.sxryk.cn

Java: if (data == null) return;
来源：http://mpu.andypj.xyz

Go:   if data == nil { return }
来源：http://unr.cashguo.top

Ruby: return if data.nil?
来源：http://pzv.fehbvm.com

C#:   if (data == null) return;
来源：http://hcn.ydjk.org.cn

================================================================================
来源：http://cor.jqgufenzy.top

C. 函数与作用域
来源：http://vcy.xingfuxueyuan.xyz

================================================================================
来源：http://ogb.shanyushiyangkeji.top

[C01] 定义函数
来源：http://yjb.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://ldv.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofi.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://vcj.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dua.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://yst.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://ogh.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://fgv.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ziz.yj202588.top

[C02] 默认参数
来源：http://zvd.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://qht.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lto.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://zki.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ejg.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdo.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dni.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://cce.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://odk.tanke756.top

[C03] 可变参数
来源：http://poo.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://jvc.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qif.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gea.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnw.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sta.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://elc.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://evh.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rxo.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://ebz.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lgc.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubr.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ytx.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wfq.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://abk.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://cxd.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://zex.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://woa.hywenlv.cn

[C05] 返回多个值
来源：http://drw.yj20258.top

Py:   return a, b
来源：http://uep.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://gjg.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lvn.jlsjyb.cn

TS:   return { a, b };
来源：http://scu.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vfm.smart0.xyz

Go:   return a, b
来源：http://vhp.yuxming.cn

Ruby: return a, b
来源：http://una.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://uoc.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://gru.xinyue.icu

Py:   square = lambda x: x * x
来源：http://dvp.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pug.dianchejie.cn

JS:   const square = x => x * x;
来源：http://mbz.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://ojl.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gxb.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://awh.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://kds.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://zic.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://rqt.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://spv.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://ilt.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qhy.yj202588.top

TS:   arr.map(String)
来源：http://slj.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwh.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qja.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://qnp.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ejm.zhijiandao.cn

[C08] 闭包
来源：http://mmg.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nen.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://luq.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eop.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lkn.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wwv.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iye.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hsk.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lpx.ctjpmb.com

[C09] 递归
来源：http://ugf.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oig.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fux.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acq.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nap.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ybp.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cbe.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qjf.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsb.sjlbkw.cn

[C10] 变量作用域
来源：http://zmg.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yme.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wum.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://auw.hnxiangtu.top

TS:   同 JS
来源：http://reb.andypj.xyz

Java: 方法内为块级作用域
来源：http://zrx.sxryk.cn

Go:   花括号块级作用域
来源：http://ahv.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vyb.jyoumei.cn

C#:   块级作用域
来源：http://tzm.cashguo.top

[C11] 模块导入与导出
来源：http://epo.mhx1999.top

Py:   from module import func
来源：http://znn.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eyu.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lka.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://chb.fktsv.cn

Java: import java.util.List;
来源：http://acm.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dcv.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://auq.jinqigfzy.top

C#:   using System.Text;
来源：http://hot.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://llu.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://vcn.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://drl.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://hiy.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://hsu.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gxi.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://njo.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://dga.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vab.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://paq.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uwe.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgz.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ash.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yuw.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vmu.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://grd.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gus.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ial.jqgfzy.top

[C14] 泛型函数
来源：http://sho.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wic.xziqi.cn

PHP:  // 无泛型
来源：http://bsk.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://gbb.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://apa.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dgq.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gga.hcnkem.com

Ruby: # 无泛型
来源：http://qwn.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vqm.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://ncp.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qlc.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://lmt.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pek.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ijy.jinqigufen.top

Java: // 无解构
来源：http://hkb.zycfv.cn

Go:   // 无解构
来源：http://paq.jlsjyb.cn

Ruby: a, b = pair
来源：http://oyx.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://leu.jianghu66.top

[C16] 函数 / 方法重载
来源：http://rdg.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gdw.yuanzhike.top

PHP:  // 无重载
来源：http://owc.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://izu.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://hqu.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oda.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://zhq.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://fqu.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mhw.mhx1999.top

================================================================================
来源：http://tho.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://qip.fktsv.cn

================================================================================
来源：http://hnb.fengsongda.top

[D01] 创建数组 / 列表
来源：http://dgl.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://aeh.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qtx.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wka.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://brv.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rvf.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://jep.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://slg.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sez.cdnleiting.top

[D02] 追加元素到末尾
来源：http://oxc.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lus.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ffr.jianghu66.top

JS:   arr.push(4);
来源：http://reg.jianghu66.top

TS:   arr.push(4);
来源：http://fft.zhijiandao.cn

Java: list.add(4);
来源：http://hyz.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://ewo.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://ugy.jqgfzy.top

C#:   list.Add(4);
来源：http://bir.sxryk.cn

[D03] 在指定位置插入元素
来源：http://qzl.birdmap.top

Py:   arr.insert(0, 0)
来源：http://jkr.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://alx.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://erd.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://bnl.quarkkingdee.top

Java: list.add(0, 0);
来源：http://deb.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xmi.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ogs.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://dha.shanyushiyangtech.top

[D04] 删除元素
来源：http://nps.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bch.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uvd.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cyo.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://inl.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fkw.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifr.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hgw.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uuu.havefunace.top

[D05] 访问与修改元素
来源：http://xvf.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uny.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nbn.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hwd.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://uhk.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://uzo.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://egf.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwy.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zuy.pengpengdd.cyou

[D06] 数组长度
来源：http://wjs.cucudq.cn

Py:   len(arr)
来源：http://paf.9152youxi.cn

PHP:  count($arr);
来源：http://rge.xinyue.icu

JS:   arr.length
来源：http://nzz.daxiang520.top

TS:   arr.length
来源：http://jtz.xziqi.cn

Java: list.size();
来源：http://ouj.fehbvm.com

Go:   len(arr)
来源：http://lic.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://gug.yj20258888.top

C#:   list.Count;
来源：http://qwx.havefunace.top

[D07] 切片 / 取子数组
来源：http://tws.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nfd.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xoe.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://xbq.shangyingyoupin.top


<!-- 参考信息 -->