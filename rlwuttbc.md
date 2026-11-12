代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://ezj.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xdo.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gxa.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://xmc.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rvv.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://cin.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zlo.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oic.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ono.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stc.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tbi.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffw.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://txb.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mim.jinqigufen.top

[B07] while 循环
来源：http://fju.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://hbu.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://ucu.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://gyj.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://uhs.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://hbe.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lsu.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://aqg.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://llu.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://cwg.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://hjb.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qec.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://nug.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://zib.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://ybh.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yvt.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://par.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://fqq.dianchejie.cn

[B09] break 与 continue
来源：http://brf.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bzy.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eib.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uuv.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypz.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zus.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bjw.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tjo.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctd.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://lca.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://utx.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mag.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qcj.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gsn.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oll.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mmk.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qli.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lhx.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://wzd.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://vur.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://sza.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpn.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqr.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://erq.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://peg.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://lbo.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ljt.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://dux.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfp.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://psd.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrj.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcz.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwm.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qgi.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://obn.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gwr.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://cnl.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://yga.birdmap.top

PHP:  is_numeric($x)
来源：http://kpe.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ymf.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pdh.daria6918.cn

Java: x instanceof Number
来源：http://cpo.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lvw.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://moe.xuanzx.com

C#:   x is int or double or decimal
来源：http://izf.bjfxy.top

[B14] 判断值是否在集合内
来源：http://kqm.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gqa.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tlu.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://wif.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://jmp.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://clz.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqf.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://kbr.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://avr.shzxlz.cn

[B15] 布尔运算与取反
来源：http://dpg.yvedp.cn

Py:   a and b or not c
来源：http://gfr.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://evc.sxryk.cn

JS:   a && b || !c
来源：http://wbr.cheryme.top

TS:   a && b || !c
来源：http://rmp.xziqi.cn

Java: a && b || !c
来源：http://jex.daria6918.cn

Go:   a && b || !c
来源：http://qmb.kuanghao11.cn

Ruby: a && b || !c
来源：http://dcx.smart0.xyz

C#:   a && b || !c
来源：http://urt.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://rpo.zdqjudy.top

Py:   if not data: return
来源：http://msi.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://aya.chenjidiqi.icu

JS:   if (!data) return;
来源：http://bgt.hnxiangtu.top

TS:   if (!data) return;
来源：http://pja.yvedp.cn

Java: if (data == null) return;
来源：http://akm.yuanzhike.top

Go:   if data == nil { return }
来源：http://ndf.yonumen.top

Ruby: return if data.nil?
来源：http://bca.yj20258888.top

C#:   if (data == null) return;
来源：http://amp.316326.xyz

================================================================================
来源：http://bqy.bjfxy.top

C. 函数与作用域
来源：http://cqe.yueranfly.top

================================================================================
来源：http://gxu.yanxiufei.cn

[C01] 定义函数
来源：http://ryl.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://ixh.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbk.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://gel.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uic.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://uih.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xuz.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://gmd.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://odt.yvedp.cn

[C02] 默认参数
来源：http://kqa.birdmap.top

Py:   def greet(name="World"): return name
来源：http://kru.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ojs.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://ruv.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mga.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jgh.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iac.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://dbn.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://skv.fehbvm.com

[C03] 可变参数
来源：http://gvb.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://xlu.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uuh.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iap.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zez.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jco.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yey.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://qej.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tcm.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://yaz.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mwr.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhk.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xdl.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hxh.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://aiv.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://pas.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://muv.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://sgz.hesvh.cn

[C05] 返回多个值
来源：http://nqp.ehwqpu.com

Py:   return a, b
来源：http://hmb.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://pik.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uds.sweek.top

TS:   return { a, b };
来源：http://xsu.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qju.svipenyu.cn

Go:   return a, b
来源：http://wvy.svipenyu.cn

Ruby: return a, b
来源：http://ies.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://yia.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://ess.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://alf.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rho.nwbrower.top

JS:   const square = x => x * x;
来源：http://upj.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://vab.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xfh.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://clv.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://teu.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xiq.316326.xyz

[C07] 把函数作为参数传入
来源：http://hkx.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hrd.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cao.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zbw.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://bwa.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qcm.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://umx.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://pwp.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yjs.wangdashe.top

[C08] 闭包
来源：http://nfk.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ygf.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vhl.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://abh.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptn.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bet.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xir.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lqc.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://slq.gogol.net.cn

[C09] 递归
来源：http://hnu.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dxq.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://apc.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uwf.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sms.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uzh.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tgu.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bcs.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdp.sweek.top

[C10] 变量作用域
来源：http://hpj.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vio.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yor.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tgz.shangyingyoupin.top

TS:   同 JS
来源：http://pkp.guowangkeji.top

Java: 方法内为块级作用域
来源：http://sve.316326.xyz

Go:   花括号块级作用域
来源：http://cvd.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eng.andypj.xyz

C#:   块级作用域
来源：http://gpf.hywenlv.cn

[C11] 模块导入与导出
来源：http://stq.pengpengdd.cyou

Py:   from module import func
来源：http://kpr.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ngg.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvl.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sfs.ctjpmb.com

Java: import java.util.List;
来源：http://tua.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wma.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://eqj.vehdjk.com

C#:   using System.Text;
来源：http://vym.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://xtw.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://oop.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://xrr.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://ayy.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://art.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zqs.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://ziw.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://jno.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tfy.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://vcs.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pyq.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zbh.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mdq.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yuz.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://nfj.epnwcf.com

Go:   func add(a, b int) int
来源：http://tvs.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nwj.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ifm.quarkkingdee.top

[C14] 泛型函数
来源：http://hsk.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nnv.shangyingyoupin.top

PHP:  // 无泛型
来源：http://mlw.hongshengwenyu.top

JS:   // 无泛型
来源：http://xue.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ufn.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://agq.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjs.xylfe.cn

Ruby: # 无泛型
来源：http://fat.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hqp.tian-w.cn

[C15] 解构 / 展开参数
来源：http://ery.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhd.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://jhj.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ory.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://slw.xylfe.cn

Java: // 无解构
来源：http://zkf.hesvh.cn

Go:   // 无解构
来源：http://iip.tarul.cn

Ruby: a, b = pair
来源：http://dkm.hcnkem.com

C#:   var (a, b) = pair;
来源：http://sfc.xylfe.cn

[C16] 函数 / 方法重载
来源：http://wqw.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rix.chenjidiqi.icu

PHP:  // 无重载
来源：http://smj.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qah.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://ctn.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zxp.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://dht.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://ody.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bla.aibaodan.cn

================================================================================
来源：http://fnp.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://zrb.ctjpmb.com

================================================================================
来源：http://iho.bjfxy.top

[D01] 创建数组 / 列表
来源：http://hxw.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rir.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gkt.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://utf.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xdc.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xtq.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://zob.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://vdo.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xji.yuanzhike.top

[D02] 追加元素到末尾
来源：http://dhx.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tha.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyx.pengpengdd.cyou

JS:   arr.push(4);
来源：http://mxt.cheryme.top

TS:   arr.push(4);
来源：http://pbd.vehdjk.com

Java: list.add(4);
来源：http://mug.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://qwl.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://mey.jinqigufen.top

C#:   list.Add(4);
来源：http://kts.yonumen.top

[D03] 在指定位置插入元素
来源：http://amc.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://loa.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vrv.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vey.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://zij.jqgufenzy.top

Java: list.add(0, 0);
来源：http://cre.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fiy.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lpn.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://gna.hammf.cn

[D04] 删除元素
来源：http://uww.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dmh.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://okr.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://osu.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://gcp.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oed.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://duv.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ssb.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gph.jyoumei.cn

[D05] 访问与修改元素
来源：http://foi.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bus.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zlz.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tic.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://eoo.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://kca.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://apn.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qms.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rww.pengpengdd.cyou

[D06] 数组长度
来源：http://frb.jinghuilouyu.cn


<!-- 参考信息 -->