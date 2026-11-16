代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bcm.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qyd.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://ezl.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kep.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://xif.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://lny.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hku.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://duo.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://avp.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://usj.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qae.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://ngp.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pcp.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://qqe.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qrm.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://std.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khp.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phl.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mzj.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ueo.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pop.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nkg.9152youxi.cn

[B07] while 循环
来源：http://sgs.xuanzx.com

Py:   while i < 10: i += 1
来源：http://nxd.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://tac.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://vjy.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://ynt.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://ako.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://txb.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://zmn.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://dqj.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://oaf.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://eze.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jnr.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://dfp.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://rwr.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://mco.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uie.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eif.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://nod.tarul.cn

[B09] break 与 continue
来源：http://lod.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjj.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mse.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szk.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hau.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyi.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bxh.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vje.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jer.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://fwb.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fsy.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://abz.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vxh.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rzl.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bcj.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://akz.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uab.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vwf.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://yos.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://kpp.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://ofy.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npg.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipi.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zau.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://two.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://wfg.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xnc.fktsv.cn

[B12] 跳出多层循环
来源：http://ebu.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ylr.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ote.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmn.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mgy.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://whz.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://enc.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vgf.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wqo.52xcode.cn

[B13] 判断是否为数字
来源：http://urz.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://lil.guowangkeji.top

PHP:  is_numeric($x)
来源：http://qlm.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://szu.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xng.yvedp.cn

Java: x instanceof Number
来源：http://flh.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cva.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://csb.sufxvd.cn

C#:   x is int or double or decimal
来源：http://wmk.redwolf501.top

[B14] 判断值是否在集合内
来源：http://rmu.snrcjt.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cgx.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dta.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://hhq.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://uds.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://uzl.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vnn.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://ype.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sfg.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://pec.9152youxi.cn

Py:   a and b or not c
来源：http://gfr.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://apd.shzxlz.cn

JS:   a && b || !c
来源：http://alr.wangdashe.top

TS:   a && b || !c
来源：http://tbi.ydjk.org.cn

Java: a && b || !c
来源：http://ewb.hammf.cn

Go:   a && b || !c
来源：http://qya.vehdjk.com

Ruby: a && b || !c
来源：http://raq.c1oappe.top

C#:   a && b || !c
来源：http://lqs.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://oyk.dianchejie.cn

Py:   if not data: return
来源：http://tla.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://usp.dashuyun.cn

JS:   if (!data) return;
来源：http://drt.dianchejie.cn

TS:   if (!data) return;
来源：http://gwp.daria6918.cn

Java: if (data == null) return;
来源：http://nzq.xuanzx.com

Go:   if data == nil { return }
来源：http://umf.zhongyouzk.top

Ruby: return if data.nil?
来源：http://onv.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://efr.zhoulong.xyz

================================================================================
来源：http://oef.316326.xyz

C. 函数与作用域
来源：http://xfc.epnwcf.com

================================================================================
来源：http://zyf.cucudq.cn

[C01] 定义函数
来源：http://bte.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://sqi.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dbq.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://txd.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qgi.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://veo.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://sgr.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://lvo.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rlp.zhaomingkeji.xyz

[C02] 默认参数
来源：http://akb.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://xeh.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://viu.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://zsc.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pbb.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cfm.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fjn.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://kyb.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://typ.mhx1999.top

[C03] 可变参数
来源：http://fjh.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://kap.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ykv.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nlx.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrs.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qgu.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxp.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mes.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uuj.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://zdp.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hra.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://klx.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dmz.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wya.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://liv.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://tgq.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://hmz.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://syn.sysykeji.top

[C05] 返回多个值
来源：http://uda.chenjidiqi.icu

Py:   return a, b
来源：http://kxh.nwbrower.top

PHP:  return [$a, $b];
来源：http://rdp.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qaz.svipenyu.cn

TS:   return { a, b };
来源：http://uxa.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eav.316326.xyz

Go:   return a, b
来源：http://xnf.ehwqpu.com

Ruby: return a, b
来源：http://upk.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://lgc.sweek.top

[C06] 匿名函数 / lambda
来源：http://lmx.fktsv.cn

Py:   square = lambda x: x * x
来源：http://jus.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nqo.jyoumei.cn

JS:   const square = x => x * x;
来源：http://mto.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://pwq.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bwe.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://dfb.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://crc.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://zsz.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://zcw.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://apc.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://umo.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://anf.yuxming.cn

TS:   arr.map(String)
来源：http://srm.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwd.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mpn.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://kam.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oqh.cucudq.cn

[C08] 闭包
来源：http://nut.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://odj.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kru.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wva.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lgj.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://shx.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sbd.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yrs.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://htj.uphjek.com

[C09] 递归
来源：http://sha.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://elr.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xle.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dwa.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldq.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xnl.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gef.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://soz.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txx.pengpengdd.cyou

[C10] 变量作用域
来源：http://emy.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://udb.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://niw.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qph.epnwcf.com

TS:   同 JS
来源：http://ceg.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://ind.ctjpmb.com

Go:   花括号块级作用域
来源：http://mqa.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vhs.gotoacloud.top

C#:   块级作用域
来源：http://jzm.52xcode.cn

[C11] 模块导入与导出
来源：http://fsk.zycfv.cn

Py:   from module import func
来源：http://aus.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vnz.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kcd.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://guk.chenzaomai.com

Java: import java.util.List;
来源：http://wag.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://too.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://ijl.yueranfly.top

C#:   using System.Text;
来源：http://xxy.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://ith.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://ysp.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://nal.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://woa.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://eem.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcd.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://fzc.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://htf.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wxm.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://lfa.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cfs.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gmt.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hih.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfg.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://blp.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://hdp.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://foy.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://lne.cqqwz.cn

[C14] 泛型函数
来源：http://cnb.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bxi.sxryk.cn

PHP:  // 无泛型
来源：http://zrc.52xcode.cn

JS:   // 无泛型
来源：http://poe.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hcz.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rgm.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oos.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://olx.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mva.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://mjv.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nzu.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://bqf.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ffe.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dvk.cucudq.cn

Java: // 无解构
来源：http://ujn.cucudq.cn

Go:   // 无解构
来源：http://xox.yongpay.top

Ruby: a, b = pair
来源：http://ilt.tian-w.cn

C#:   var (a, b) = pair;
来源：http://isb.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://hjy.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://elk.jqgufenzy.top

PHP:  // 无重载
来源：http://pol.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdk.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://tfq.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://onf.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://gti.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://sef.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bvb.hesvh.cn

================================================================================
来源：http://stj.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://wnn.gogol.net.cn

================================================================================
来源：http://yzc.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://nmt.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dno.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yxt.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brc.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lay.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikl.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://lon.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://jua.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ttd.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://aex.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qrx.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yeh.mhx1999.top

JS:   arr.push(4);
来源：http://zyc.fehbvm.com

TS:   arr.push(4);
来源：http://ebr.hammf.cn

Java: list.add(4);
来源：http://ney.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://gpg.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://jln.cdnleiting.top

C#:   list.Add(4);
来源：http://znk.ydzc1.top

[D03] 在指定位置插入元素
来源：http://jzp.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://eil.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://isj.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://loj.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://fii.zhongyouzk.top

Java: list.add(0, 0);
来源：http://mkb.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://srg.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gbf.pycfn.com

C#:   list.Insert(0, 0);
来源：http://ocf.ywan-chungtsiang.top

[D04] 删除元素
来源：http://jpq.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hxj.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zsr.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xun.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://jzk.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uxj.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xjg.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gkd.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jat.jlsjyb.cn

[D05] 访问与修改元素
来源：http://yei.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qhz.xingfuxueyuan.xyz


<!-- 参考信息 -->