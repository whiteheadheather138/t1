代发 wailian999

Py:   for i in range(10): print(i)
来源：http://smj.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhy.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pxp.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jqz.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hqi.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vha.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://mxz.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://knp.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://fpy.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://hoy.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mxv.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fby.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vyh.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mij.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hxg.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://mpm.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oqq.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://kdf.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vrx.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zyc.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kbj.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hec.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xzi.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mrx.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rsp.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://amc.chenzaomai.com

[B07] while 循环
来源：http://nkc.bbcook.cn

Py:   while i < 10: i += 1
来源：http://fag.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xjn.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://dco.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://ojx.pycfn.com

Java: while (i < 10) { i++; }
来源：http://sfa.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gbq.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://rqh.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://iry.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://jjl.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://kbk.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://swc.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://mgz.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://mre.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://tgv.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cdr.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://yyz.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://sgy.fehbvm.com

[B09] break 与 continue
来源：http://dsy.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://elg.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wiw.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfr.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyw.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnx.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mun.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://axu.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyb.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://oxp.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ugw.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egm.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://moq.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lon.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mbh.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://clk.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bqa.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://awg.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://swi.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://zhb.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://iks.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tef.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fir.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ejg.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cfb.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://qig.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ccg.xuanzx.com

[B12] 跳出多层循环
来源：http://yzh.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zmi.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oof.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywj.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pkp.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rss.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://idu.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vtz.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xaj.chenlongwang.top

[B13] 判断是否为数字
来源：http://fzr.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://ygn.xylfe.cn

PHP:  is_numeric($x)
来源：http://twb.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zdh.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nic.ehwqpu.com

Java: x instanceof Number
来源：http://kbs.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tjd.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://dpu.hywenlv.cn

C#:   x is int or double or decimal
来源：http://fsi.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://gwj.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jxi.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zdb.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://oty.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://jhm.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vaf.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hsg.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://yco.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hsd.ppjwa.cn

[B15] 布尔运算与取反
来源：http://uxd.wangdashe.top

Py:   a and b or not c
来源：http://chj.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://hck.zycfv.cn

JS:   a && b || !c
来源：http://dgd.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://uns.jyoumei.cn

Java: a && b || !c
来源：http://tbn.tarul.cn

Go:   a && b || !c
来源：http://sgd.vehdjk.com

Ruby: a && b || !c
来源：http://cpa.jiagoushi.top

C#:   a && b || !c
来源：http://kpr.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://nfi.jqgfzy.top

Py:   if not data: return
来源：http://xrv.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://hpq.meibo888.top

JS:   if (!data) return;
来源：http://ehq.ybcxt.top

TS:   if (!data) return;
来源：http://ttf.jyoumei.cn

Java: if (data == null) return;
来源：http://ygs.xinyue.icu

Go:   if data == nil { return }
来源：http://tse.xziqi.cn

Ruby: return if data.nil?
来源：http://fuy.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://xix.yonumen.top

================================================================================
来源：http://cnk.daxiang520.top

C. 函数与作用域
来源：http://xyc.zhoulong.xyz

================================================================================
来源：http://hkv.nanxuanxn.top

[C01] 定义函数
来源：http://pcd.meibo888.top

Py:   def add(a, b): return a + b
来源：http://fkg.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lal.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://bkl.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qrh.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tqb.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dju.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://jvi.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cnv.smart0.xyz

[C02] 默认参数
来源：http://ewx.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://wfd.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cex.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://rsl.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mvi.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://ysy.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tzi.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://sdq.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://fjh.shangyingyoupin.top

[C03] 可变参数
来源：http://unw.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://vzr.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xpv.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://loa.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://keg.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dgk.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uqq.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://jnd.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lbh.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://gfc.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dxv.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eie.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zad.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgy.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://pfr.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://qqh.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://qkh.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://wvy.jqgufenzy.top

[C05] 返回多个值
来源：http://zwh.gaohongyu789.top

Py:   return a, b
来源：http://rbt.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://sfo.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hnj.tianlin.xyz

TS:   return { a, b };
来源：http://dms.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cku.wangdashe.top

Go:   return a, b
来源：http://god.jqgufenzy.top

Ruby: return a, b
来源：http://ylq.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://dvy.316326.xyz

[C06] 匿名函数 / lambda
来源：http://tbr.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://xgj.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://lml.shzxlz.cn

JS:   const square = x => x * x;
来源：http://bzs.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://pky.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lzt.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtc.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://apg.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://gpd.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://jap.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rfz.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://cvw.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hkh.zhijiandao.cn

TS:   arr.map(String)
来源：http://rrd.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jtf.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vii.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://wtw.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bby.iojbl.cn

[C08] 闭包
来源：http://oqt.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufq.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jgo.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lnx.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tnr.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oqb.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jes.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ovi.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zye.0kj1m.cn

[C09] 递归
来源：http://suh.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ekq.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bha.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hec.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbs.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aqh.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jxf.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gai.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eed.xziqi.cn

[C10] 变量作用域
来源：http://nan.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ybd.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tay.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kjl.cucudq.cn

TS:   同 JS
来源：http://srf.hcnkem.com

Java: 方法内为块级作用域
来源：http://pnh.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://ptj.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cbe.cashguo.top

C#:   块级作用域
来源：http://zfw.cucudq.cn

[C11] 模块导入与导出
来源：http://oul.shangyingyoupin.top

Py:   from module import func
来源：http://deg.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kqt.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://sta.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hws.cdnleiting.top

Java: import java.util.List;
来源：http://phm.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjq.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://mfg.daxiang520.top

C#:   using System.Text;
来源：http://gki.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://sjo.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://gal.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://vhw.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://gzj.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://awo.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lev.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://lcq.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://xjh.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fak.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://jse.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fir.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oeq.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bsk.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://agn.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fal.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://yuv.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqv.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://bxm.jinqigufen.top

[C14] 泛型函数
来源：http://zhq.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ucy.yj20258888.top

PHP:  // 无泛型
来源：http://tnm.jianghu66.top

JS:   // 无泛型
来源：http://gfa.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lgd.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ifl.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hiq.316326.xyz

Ruby: # 无泛型
来源：http://wct.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pgl.wangdashe.top

[C15] 解构 / 展开参数
来源：http://kcs.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bgs.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://wgs.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ilk.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hwv.c1oappe.top

Java: // 无解构
来源：http://bjj.chenjidiqi.icu

Go:   // 无解构
来源：http://csr.0kj1m.cn

Ruby: a, b = pair
来源：http://mka.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://pwi.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://uza.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gqh.hongshengwenyu.top

PHP:  // 无重载
来源：http://spj.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ddt.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://wfs.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tgg.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://bst.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://amg.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ptg.cashguo.top

================================================================================
来源：http://kwi.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://fdq.yj202588.top

================================================================================
来源：http://foy.fengsongda.top

[D01] 创建数组 / 列表
来源：http://kfj.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hid.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://art.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xll.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wtf.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nhz.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://jij.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://byk.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pjx.sysykeji.top

[D02] 追加元素到末尾
来源：http://wsd.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://njo.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jjy.gzhubu.top

JS:   arr.push(4);
来源：http://qzs.yfazqb.com

TS:   arr.push(4);
来源：http://xjo.xuetiantiany.cn

Java: list.add(4);
来源：http://wvd.havefunace.top

Go:   arr = append(arr, 4)
来源：http://svs.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://ehx.pycfn.com

C#:   list.Add(4);
来源：http://eue.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://ayp.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://ous.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wqq.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mgf.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://zon.fengsongda.top

Java: list.add(0, 0);
来源：http://mdk.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://oke.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xox.hammf.cn

C#:   list.Insert(0, 0);
来源：http://pvf.guannengcc.top

[D04] 删除元素
来源：http://rok.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nju.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://whe.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uhf.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://dcm.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xmf.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yom.dashuyun.cn


<!-- 参考信息 -->