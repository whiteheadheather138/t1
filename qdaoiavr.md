代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zxh.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwf.xuanzx.com

[B03] switch / match / case
来源：http://fob.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ctl.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cya.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eqy.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://csd.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gwg.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wqj.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mwp.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eui.shanyushiyangtech.top

[B04] for 计数循环
来源：http://mnf.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://jmx.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jdv.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://clj.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzj.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qaa.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lwr.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://lkp.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mnf.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://cls.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://ofj.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dqt.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://kjm.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gdt.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hhs.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mmh.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://xjl.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qnf.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://lwl.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ekh.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dsx.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://etn.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jbm.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bao.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://diw.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mqs.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kes.vqdsnc.cn

[B07] while 循环
来源：http://cwv.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://krv.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jkv.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://jzg.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://plp.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://tnc.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mkj.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://xas.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://pbc.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://bvw.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://zmz.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jko.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://chs.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://fed.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://gko.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lua.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sym.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://kts.fktsv.cn

[B09] break 与 continue
来源：http://vad.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bvs.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kmu.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lts.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptn.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpp.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://utq.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ijo.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vuq.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://aak.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aif.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yii.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bll.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jgo.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://npq.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ypo.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mzq.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jvm.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://ozk.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://ssn.hammf.cn

PHP:  range(0, 10, 2);
来源：http://ytc.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qye.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tnp.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nbg.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nlj.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://byh.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aoq.tanke756.top

[B12] 跳出多层循环
来源：http://kfp.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://beh.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vns.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytb.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xzj.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ibz.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://esz.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yly.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ato.svipenyu.cn

[B13] 判断是否为数字
来源：http://dwt.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://nmv.yongpay.top

PHP:  is_numeric($x)
来源：http://aml.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fxp.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://udp.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://raz.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pbv.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://dbl.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://non.andypj.xyz

[B14] 判断值是否在集合内
来源：http://gaq.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dyz.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hmn.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://qxr.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://tak.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://usg.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jqb.zhixingplan.top

Ruby: [1, 2, 3].include?(x)
来源：http://thi.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sfp.pycfn.com

[B15] 布尔运算与取反
来源：http://xzt.gaohongyu789.top

Py:   a and b or not c
来源：http://swo.andypj.xyz

PHP:  $a && $b || !$c
来源：http://mza.zhijiandao.cn

JS:   a && b || !c
来源：http://tmo.vehdjk.com

TS:   a && b || !c
来源：http://uxr.chenzaomai.com

Java: a && b || !c
来源：http://sxt.wangdashe.top

Go:   a && b || !c
来源：http://emj.zycfv.cn

Ruby: a && b || !c
来源：http://ufa.quarkkingdee.top

C#:   a && b || !c
来源：http://ehq.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://lka.xinyue.icu

Py:   if not data: return
来源：http://rlc.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://nxn.jqgfzy.top

JS:   if (!data) return;
来源：http://zup.ydzc1.top

TS:   if (!data) return;
来源：http://ees.mhx1999.top

Java: if (data == null) return;
来源：http://crg.52xcode.cn

Go:   if data == nil { return }
来源：http://shz.vqdsnc.cn

Ruby: return if data.nil?
来源：http://hxu.daxiang520.top

C#:   if (data == null) return;
来源：http://orp.havefunace.top

================================================================================
来源：http://dyr.tarul.cn

C. 函数与作用域
来源：http://ejh.jinghuilouyu.cn

================================================================================
来源：http://hvv.pycfn.com

[C01] 定义函数
来源：http://ros.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://mhq.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmb.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://yju.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mzd.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tcc.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ezh.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://gia.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tcr.yj202588.top

[C02] 默认参数
来源：http://jci.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://plc.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ayt.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://xug.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nsp.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://blv.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vuw.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://bsq.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://cpu.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://ssi.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://hcw.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nbl.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ntf.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bwi.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lbx.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cge.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yyj.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zsk.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://aup.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aog.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ymf.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wlc.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wgk.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://hai.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://agb.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://xrq.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://wou.yuanzhike.top

[C05] 返回多个值
来源：http://phg.yanxiufei.cn

Py:   return a, b
来源：http://xdk.sxryk.cn

PHP:  return [$a, $b];
来源：http://bov.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://edz.smart0.xyz

TS:   return { a, b };
来源：http://owa.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ler.gaohongyu789.top

Go:   return a, b
来源：http://jxd.epnwcf.com

Ruby: return a, b
来源：http://caz.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://fee.cashguo.top

[C06] 匿名函数 / lambda
来源：http://gcx.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://imu.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://wzm.hcnkem.com

JS:   const square = x => x * x;
来源：http://mxz.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://lde.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rca.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://duy.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://aqu.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://nlg.wangdashe.top

[C07] 把函数作为参数传入
来源：http://esd.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ezg.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sra.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qwj.shzxlz.cn

TS:   arr.map(String)
来源：http://dng.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uol.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bdv.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://fec.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aqo.tanke756.top

[C08] 闭包
来源：http://mqv.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bdb.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ret.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uib.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bki.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://thm.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://van.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uwk.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zla.yonumen.top

[C09] 递归
来源：http://bxc.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fon.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cxi.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xmo.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzl.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jkm.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yll.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eqy.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jyo.feifeiyinyue.top

[C10] 变量作用域
来源：http://cmn.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fsi.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://akd.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qkq.cashguo.top

TS:   同 JS
来源：http://vnv.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://hxt.daxiang520.top

Go:   花括号块级作用域
来源：http://awy.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ets.yuanzhike.top

C#:   块级作用域
来源：http://ivb.jiagoushi.top

[C11] 模块导入与导出
来源：http://fat.pycfn.com

Py:   from module import func
来源：http://mni.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://adq.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rxb.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ktp.jinqigfzy.top

Java: import java.util.List;
来源：http://fkz.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ywm.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://izo.iojbl.cn

C#:   using System.Text;
来源：http://mjw.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://pgo.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://bds.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://gxs.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://gcc.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://qsc.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://joh.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://jrr.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://fsk.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tyi.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://say.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mek.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oka.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wsf.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://doz.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://abj.vehdjk.com

Go:   func add(a, b int) int
来源：http://oau.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dke.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dnh.zdqjudy.top

[C14] 泛型函数
来源：http://zpe.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://voq.ydjk.org.cn

PHP:  // 无泛型
来源：http://gmg.daria6918.cn

JS:   // 无泛型
来源：http://vlx.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nct.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://txs.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://skz.nanxinkj.top

Ruby: # 无泛型
来源：http://elh.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hax.hesvh.cn

[C15] 解构 / 展开参数
来源：http://mje.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jyu.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://ijj.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxw.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://evq.ybcxt.top

Java: // 无解构
来源：http://nph.kuanghao11.cn

Go:   // 无解构
来源：http://aph.tanke756.top

Ruby: a, b = pair
来源：http://hvb.yj20258.top

C#:   var (a, b) = pair;
来源：http://jby.nwbrower.top

[C16] 函数 / 方法重载
来源：http://hsm.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tol.gaohongyu789.top

PHP:  // 无重载
来源：http://pmv.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hrv.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://utg.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zgr.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://hbi.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://hww.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cas.redwolf501.top

================================================================================
来源：http://rvd.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://quv.ydzc1.top

================================================================================
来源：http://orx.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://stt.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://qit.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iib.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eto.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://vgk.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nxz.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://egy.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://atq.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bjj.hysaishi.cn

[D02] 追加元素到末尾
来源：http://qsg.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aqn.jianghu66.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyj.nanxuanxn.top

JS:   arr.push(4);
来源：http://mtg.vqdsnc.cn

TS:   arr.push(4);
来源：http://biz.jinghuilouyu.cn

Java: list.add(4);
来源：http://avt.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://jnx.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://hkv.hnqzz.top

C#:   list.Add(4);
来源：http://ray.daxiang520.top

[D03] 在指定位置插入元素
来源：http://znp.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://ifl.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://abb.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxe.fktsv.cn


<!-- 参考信息 -->