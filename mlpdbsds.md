代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://gqc.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://fcn.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://khr.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://kga.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wfr.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://kcz.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ryt.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cgk.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ozv.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ieq.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://huw.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pvs.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://riz.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hvf.andypj.xyz

[B07] while 循环
来源：http://wup.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://zjy.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://zvi.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://nga.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://prf.sweek.top

Java: while (i < 10) { i++; }
来源：http://orj.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igo.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://ugh.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://abm.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://cgn.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://jgb.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://wie.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://nru.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://sbv.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://byh.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kra.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zme.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://nbb.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://jfv.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://heo.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lma.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxv.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgq.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbs.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fhr.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nan.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ait.xuanzx.com

[B10] 遍历同时拿索引
来源：http://pah.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gea.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ual.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twj.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kef.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xbq.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rxk.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://igd.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dwo.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://suc.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://btf.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://ohl.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyw.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsl.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cap.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fxk.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://amx.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bft.gaohongyu789.top

[B12] 跳出多层循环
来源：http://avz.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dkr.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cuu.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zzy.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://app.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://trb.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mip.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vic.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://geh.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://zzd.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://ulq.ivvv.top

PHP:  is_numeric($x)
来源：http://pgf.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umh.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ics.hcnkem.com

Java: x instanceof Number
来源：http://rti.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bzs.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://ctf.epnwcf.com

C#:   x is int or double or decimal
来源：http://ony.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://dhs.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hma.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fcz.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://bdj.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://swk.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ucx.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qiv.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://xye.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mhc.chenlongwang.top

[B15] 布尔运算与取反
来源：http://zti.yonumen.top

Py:   a and b or not c
来源：http://gls.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://oqi.fktsv.cn

JS:   a && b || !c
来源：http://mri.nwbrower.top

TS:   a && b || !c
来源：http://cle.quarkkingdee.top

Java: a && b || !c
来源：http://ixw.ydjk.org.cn

Go:   a && b || !c
来源：http://tgl.feifeiyinyue.top

Ruby: a && b || !c
来源：http://uxy.vehdjk.com

C#:   a && b || !c
来源：http://hmy.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tfg.yonumen.top

Py:   if not data: return
来源：http://ddu.pycfn.com

PHP:  if (!$data) { return; }
来源：http://vuc.bjfxy.top

JS:   if (!data) return;
来源：http://dbo.meibo888.top

TS:   if (!data) return;
来源：http://amc.ppjwa.cn

Java: if (data == null) return;
来源：http://qmm.52xcode.cn

Go:   if data == nil { return }
来源：http://lby.cashguo.top

Ruby: return if data.nil?
来源：http://mkf.tanke756.top

C#:   if (data == null) return;
来源：http://rcb.dianchejie.cn

================================================================================
来源：http://nax.mhx1999.top

C. 函数与作用域
来源：http://frq.hfpthk.cn

================================================================================
来源：http://wzv.hnxiangtu.top

[C01] 定义函数
来源：http://fxm.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://csg.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zif.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://imu.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tia.zdbjq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mdi.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fho.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://usg.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cnt.tanke756.top

[C02] 默认参数
来源：http://tut.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://yrr.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://bmm.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://zgl.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://axz.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ovy.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cji.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://yua.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://uom.zdqjudy.top

[C03] 可变参数
来源：http://udc.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://jhy.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ixw.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://snw.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ped.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ixi.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lzw.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yqr.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ztm.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://fff.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnx.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uqv.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mtv.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zpl.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://owh.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://pki.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://vpi.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://vtw.zdbjq.cn

[C05] 返回多个值
来源：http://syh.nanxuanxn.top

Py:   return a, b
来源：http://qpr.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://epw.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://myo.iojbl.cn

TS:   return { a, b };
来源：http://klp.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gkm.sufxvd.cn

Go:   return a, b
来源：http://wpk.pengpengdd.cyou

Ruby: return a, b
来源：http://qfw.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://hut.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://yve.iojbl.cn

Py:   square = lambda x: x * x
来源：http://lsa.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ccd.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://kph.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://lhq.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pui.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://rru.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://ldy.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://zha.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://jbd.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hnf.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ntv.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://psz.sufxvd.cn

TS:   arr.map(String)
来源：http://kof.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wxt.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qbl.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://fqq.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bfm.fanxiaobao.xyz

[C08] 闭包
来源：http://muv.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ptt.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ybn.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://geh.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rbr.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pfc.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kww.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jnh.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbg.vqdsnc.cn

[C09] 递归
来源：http://psg.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dik.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vtj.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xrp.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dce.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hvn.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uol.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dgs.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oex.chenlongwang.top

[C10] 变量作用域
来源：http://gtv.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://foz.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://npl.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jna.ydjk.org.cn

TS:   同 JS
来源：http://zli.yuxming.cn

Java: 方法内为块级作用域
来源：http://iht.hfpthk.cn

Go:   花括号块级作用域
来源：http://lcb.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wed.sufxvd.cn

C#:   块级作用域
来源：http://hrw.wangdashe.top

[C11] 模块导入与导出
来源：http://pcs.zdqjudy.top

Py:   from module import func
来源：http://xyu.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mff.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdt.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jpz.yanxiufei.cn

Java: import java.util.List;
来源：http://adu.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lds.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://pba.daria6918.cn

C#:   using System.Text;
来源：http://nel.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://kie.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://plg.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://emo.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://feo.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://wge.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ksc.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://jea.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://nsr.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cec.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://yrp.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mjv.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mlk.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eyf.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uys.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://enm.c1oappe.top

Go:   func add(a, b int) int
来源：http://nla.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://myr.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lkq.bjfxy.top

[C14] 泛型函数
来源：http://nfv.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gkl.zhoulong.xyz

PHP:  // 无泛型
来源：http://xhe.fanxiaobao.xyz

JS:   // 无泛型
来源：http://soo.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tbf.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wst.yongpay.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tpl.smart0.xyz

Ruby: # 无泛型
来源：http://egu.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sbv.ivvv.top

[C15] 解构 / 展开参数
来源：http://hgh.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xmz.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://fju.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://isb.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://avb.yuxming.cn

Java: // 无解构
来源：http://yxu.wangshuangyany.cn

Go:   // 无解构
来源：http://tao.cqqwz.cn

Ruby: a, b = pair
来源：http://vtw.shuidangran.top

C#:   var (a, b) = pair;
来源：http://dtk.andypj.xyz

[C16] 函数 / 方法重载
来源：http://tte.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uzi.cheryme.top

PHP:  // 无重载
来源：http://ewb.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://zwq.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://bxm.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://akn.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://ukh.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://kpo.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dey.jlsjyb.cn

================================================================================
来源：http://lsu.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://wtm.daxiang520.top

================================================================================
来源：http://vzt.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ota.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqg.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gip.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vfa.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ssj.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ocf.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://jpr.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://ebz.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xkj.yonumen.top

[D02] 追加元素到末尾
来源：http://lgp.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ghm.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tgh.ybcxt.top

JS:   arr.push(4);
来源：http://tns.fengsongda.top

TS:   arr.push(4);
来源：http://bom.tianlin.xyz

Java: list.add(4);
来源：http://ttf.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://byn.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://tau.yuanzhike.top

C#:   list.Add(4);
来源：http://cns.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://zrg.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://iln.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vgs.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhs.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://mdr.vehdjk.com

Java: list.add(0, 0);
来源：http://ayo.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://mkz.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mtj.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://zlw.epnwcf.com

[D04] 删除元素
来源：http://cez.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ich.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://idd.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ysa.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://xkm.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ccm.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kcm.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rxr.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tvs.c1oappe.top

[D05] 访问与修改元素
来源：http://fly.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jft.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kum.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tof.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://vyy.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://bkd.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://yqu.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kzg.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pjt.jinghuilouyu.cn

[D06] 数组长度
来源：http://bjm.zhixingplan.top


<!-- 参考信息 -->