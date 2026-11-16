代发 wailian999

[B05] 遍历数组 / 列表
来源：http://nhy.hesvh.cn

Py:   for item in arr: print(item)
来源：http://ihw.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tyt.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iuw.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bck.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zbs.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://scs.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://snf.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ihp.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://vin.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kxw.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://muk.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://enk.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tis.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://thm.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mkr.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ezo.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://odh.cqqwz.cn

[B07] while 循环
来源：http://udf.cucudq.cn

Py:   while i < 10: i += 1
来源：http://brs.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dsd.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://lip.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://yqr.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://pot.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gxy.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://wfp.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://pfp.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://smg.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://xvi.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ghk.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://geh.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://xvi.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://hll.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://akz.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://eao.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://znf.bjfxy.top

[B09] break 与 continue
来源：http://xcf.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sjf.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://njo.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jew.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjj.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzn.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://juo.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wxe.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://erp.jianghu66.top

[B10] 遍历同时拿索引
来源：http://mrh.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uxb.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://btx.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fgz.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bwk.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vxc.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ydb.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ipv.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wqk.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://dup.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://oyx.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://pdm.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqv.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iss.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blh.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uhg.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://nuf.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qby.yueranfly.top

[B12] 跳出多层循环
来源：http://ssf.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xju.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://caf.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ylg.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://htx.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kak.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dgd.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzh.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gsm.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://ndu.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://mrc.hywenlv.cn

PHP:  is_numeric($x)
来源：http://qlq.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhq.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ijj.shangyingyoupin.top

Java: x instanceof Number
来源：http://luj.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ztp.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://pmm.xinyue.icu

C#:   x is int or double or decimal
来源：http://tgt.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://kye.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dwt.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yiz.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://vsl.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://kkz.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vbk.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gkq.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rbl.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jyc.meibo888.top

[B15] 布尔运算与取反
来源：http://pjv.fktsv.cn

Py:   a and b or not c
来源：http://yyn.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://lag.xylfe.cn

JS:   a && b || !c
来源：http://vtf.jiagoushi.top

TS:   a && b || !c
来源：http://vpq.nanxuanxn.top

Java: a && b || !c
来源：http://ozc.shangyingyoupin.top

Go:   a && b || !c
来源：http://jae.jyoumei.cn

Ruby: a && b || !c
来源：http://sol.uphjek.com

C#:   a && b || !c
来源：http://mth.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vsd.guannengcc.top

Py:   if not data: return
来源：http://dxi.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://qrg.yongpay.top

JS:   if (!data) return;
来源：http://zre.jqgfzy.top

TS:   if (!data) return;
来源：http://myt.sysykeji.top

Java: if (data == null) return;
来源：http://bzq.zhongyouzk.top

Go:   if data == nil { return }
来源：http://gnf.9152youxi.cn

Ruby: return if data.nil?
来源：http://yxo.ybcxt.top

C#:   if (data == null) return;
来源：http://xes.jqgufenzy.top

================================================================================
来源：http://aah.zhijiandao.cn

C. 函数与作用域
来源：http://jpc.yj202588.top

================================================================================
来源：http://inw.xuetiantiany.cn

[C01] 定义函数
来源：http://rxn.cashguo.top

Py:   def add(a, b): return a + b
来源：http://elu.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmn.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://slo.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://raa.zdbjq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wfd.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://rpy.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://dsp.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rzh.daria6918.cn

[C02] 默认参数
来源：http://cxo.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://tcu.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://swu.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ose.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sse.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zmf.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kvs.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://vma.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://jcp.andypj.xyz

[C03] 可变参数
来源：http://fum.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://sfp.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lan.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dpm.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tbs.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xzj.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fzv.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://kmv.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bko.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://qza.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nbg.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rzt.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mzi.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yln.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://rnd.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://pkb.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://xer.sweek.top

C#:   f(a: 1, b: 2)
来源：http://krm.hongshengwenyu.top

[C05] 返回多个值
来源：http://kqx.aibaodan.cn

Py:   return a, b
来源：http://jzw.cashguo.top

PHP:  return [$a, $b];
来源：http://hbc.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://swi.chenzaomai.com

TS:   return { a, b };
来源：http://iiy.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xno.hammf.cn

Go:   return a, b
来源：http://xvd.jyoumei.cn

Ruby: return a, b
来源：http://ici.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://qed.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://jft.xziqi.cn

Py:   square = lambda x: x * x
来源：http://eks.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iua.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://mxz.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://wnh.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gje.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://loo.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://cxk.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://jef.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://tmv.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hvo.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://xfo.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://orp.redwolf501.top

TS:   arr.map(String)
来源：http://bdc.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jdk.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ukp.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://tbe.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ses.kuanghao11.cn

[C08] 闭包
来源：http://zpe.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojf.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tme.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lyo.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://phw.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xuy.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jdq.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oas.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cap.bbcook.cn

[C09] 递归
来源：http://ugh.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zoy.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpl.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sav.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asg.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fvt.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aum.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nnk.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://suu.zhixingplan.top

[C10] 变量作用域
来源：http://bht.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mcy.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pep.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vwg.fanxiaobao.xyz

TS:   同 JS
来源：http://nvq.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://udx.daria6918.cn

Go:   花括号块级作用域
来源：http://thw.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uzz.zhaomingkeji.xyz

C#:   块级作用域
来源：http://mvd.dianchejie.cn

[C11] 模块导入与导出
来源：http://mth.xuetiantiany.cn

Py:   from module import func
来源：http://wcl.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://eve.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zdz.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cke.9152youxi.cn

Java: import java.util.List;
来源：http://yln.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bnw.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://wen.zdqjudy.top

C#:   using System.Text;
来源：http://tmf.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://apm.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://wyv.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://bdk.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://jgk.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://xve.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qbv.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://lcx.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://hvr.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://soo.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://zmx.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zih.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blh.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rwo.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kpj.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xbb.iojbl.cn

Go:   func add(a, b int) int
来源：http://eqt.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bxs.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://niu.fengsongda.top

[C14] 泛型函数
来源：http://gap.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jqm.snrcjt.cn

PHP:  // 无泛型
来源：http://vcf.yueranfly.top

JS:   // 无泛型
来源：http://txm.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vud.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uem.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gun.fktsv.cn

Ruby: # 无泛型
来源：http://gvy.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ovs.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://ptx.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cgy.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://xxv.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgo.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://het.316326.xyz

Java: // 无解构
来源：http://pii.zhaomingkeji.xyz

Go:   // 无解构
来源：http://jro.gotoacloud.top

Ruby: a, b = pair
来源：http://sgs.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://mte.yueranfly.top

[C16] 函数 / 方法重载
来源：http://uxn.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nkm.jinghuilouyu.cn

PHP:  // 无重载
来源：http://gyj.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jox.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://xyi.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uyq.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://zmb.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://nod.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rsf.pycfn.com

================================================================================
来源：http://arl.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://krt.aizwys.cn

================================================================================
来源：http://dtl.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://hxp.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://sub.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://arf.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rcp.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://afe.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rii.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://zfa.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://can.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zaw.9152youxi.cn

[D02] 追加元素到末尾
来源：http://ixw.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iiw.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yzq.wangdashe.top

JS:   arr.push(4);
来源：http://juo.hfpthk.cn

TS:   arr.push(4);
来源：http://xju.hysaishi.cn

Java: list.add(4);
来源：http://prl.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://otu.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://hzq.bjfxy.top

C#:   list.Add(4);
来源：http://jqj.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://lyk.tarul.cn

Py:   arr.insert(0, 0)
来源：http://jqs.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hoj.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ujy.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://gii.zhoulong.xyz

Java: list.add(0, 0);
来源：http://lid.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pvu.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mqy.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://jwg.redwolf501.top

[D04] 删除元素
来源：http://ufz.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ode.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcf.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://god.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://hav.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://suh.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zxs.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cgj.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nlk.epnwcf.com

[D05] 访问与修改元素
来源：http://iud.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mmr.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://enn.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xor.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://swf.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://bbt.xingfuxueyuan.xyz


<!-- 参考信息 -->