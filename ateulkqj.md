代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvk.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqo.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqj.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oah.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qho.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxt.yj20258.top

[B03] switch / match / case
来源：http://htj.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xwn.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ipv.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yml.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rvd.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jrn.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mnp.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xcj.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xvs.shzxlz.cn

[B04] for 计数循环
来源：http://cog.yonumen.top

Py:   for i in range(10): print(i)
来源：http://rmi.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mjw.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyl.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://feu.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://klp.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qly.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://jzo.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rvc.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://ted.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://tad.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aez.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://myd.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qbe.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://abf.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nqp.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://jbk.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yut.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://qwn.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rvx.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jpw.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dzl.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txd.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mgl.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wzg.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hvl.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://euz.tianlin.xyz

[B07] while 循环
来源：http://vjt.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://kjn.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://xjh.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://jjr.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://cun.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://nmw.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tuu.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://uav.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://fyj.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://gyr.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://udd.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kdk.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://fgp.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://kpd.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://kze.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gpm.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://psx.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://kry.yanxiufei.cn

[B09] break 与 continue
来源：http://lqt.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://msx.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://epc.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkm.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktk.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://anu.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://onq.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jwb.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqg.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://nkf.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://isv.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://opg.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eal.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cbj.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oqd.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xej.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://enp.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pcn.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://lcu.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://pzr.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://ysr.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ybg.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wav.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://roh.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kqo.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://wpw.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hpk.snrcjt.cn

[B12] 跳出多层循环
来源：http://fii.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tcn.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fkl.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dew.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ljo.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lfq.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://idm.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://utm.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ygk.ctjpmb.com

[B13] 判断是否为数字
来源：http://eja.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://lgl.bjfxy.top

PHP:  is_numeric($x)
来源：http://yqw.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fwt.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ozu.pengpengdd.cyou

Java: x instanceof Number
来源：http://fxm.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gqh.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://itn.sxryk.cn

C#:   x is int or double or decimal
来源：http://qef.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://xsr.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://prp.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qov.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://xxk.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ymc.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vjc.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ukf.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://byo.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bln.tianlin.xyz

[B15] 布尔运算与取反
来源：http://use.cdnleiting.top

Py:   a and b or not c
来源：http://hng.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://rim.nwbrower.top

JS:   a && b || !c
来源：http://hxe.quarkkingdee.top

TS:   a && b || !c
来源：http://xiq.yfazqb.com

Java: a && b || !c
来源：http://txz.hongshengwenyu.top

Go:   a && b || !c
来源：http://lvr.sweek.top

Ruby: a && b || !c
来源：http://txg.sxryk.cn

C#:   a && b || !c
来源：http://gae.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jex.ywan-chungtsiang.top

Py:   if not data: return
来源：http://edv.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://lpr.vqdsnc.cn

JS:   if (!data) return;
来源：http://ift.tarul.cn

TS:   if (!data) return;
来源：http://ncf.sweek.top

Java: if (data == null) return;
来源：http://aal.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://uyf.xuanzx.com

Ruby: return if data.nil?
来源：http://vnb.mhx1999.top

C#:   if (data == null) return;
来源：http://yzo.tian-w.cn

================================================================================
来源：http://jna.sufxvd.cn

C. 函数与作用域
来源：http://imt.zhiwuduotai.top

================================================================================
来源：http://pgp.yanxiufei.cn

[C01] 定义函数
来源：http://pgx.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://yzj.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eeo.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://icy.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fhc.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://brv.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sxf.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://fzb.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ktn.gotoacloud.top

[C02] 默认参数
来源：http://myv.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://cmd.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gqt.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://svs.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dzf.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://swi.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bpj.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://tpe.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://vxd.hesvh.cn

[C03] 可变参数
来源：http://ybu.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://wko.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zuf.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oip.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://scy.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bwl.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yrn.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://fbk.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcq.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://pvb.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fex.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://agy.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gyg.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uqp.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://apm.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://ipq.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://fwu.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://qta.cashguo.top

[C05] 返回多个值
来源：http://vwo.guannengcc.top

Py:   return a, b
来源：http://ulh.birdmap.top

PHP:  return [$a, $b];
来源：http://iam.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bnz.gzhubu.top

TS:   return { a, b };
来源：http://jeq.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wxt.yonumen.top

Go:   return a, b
来源：http://zar.xziqi.cn

Ruby: return a, b
来源：http://xdu.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://bqx.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://fgp.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://lsk.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://aek.cashguo.top

JS:   const square = x => x * x;
来源：http://zts.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://jkg.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cvs.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://ltc.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://rxd.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://cqf.aizwys.cn

[C07] 把函数作为参数传入
来源：http://kqq.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zox.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://yog.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aad.sufxvd.cn

TS:   arr.map(String)
来源：http://jdy.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vfx.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nyu.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://yxk.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wyo.chenlongwang.top

[C08] 闭包
来源：http://fxb.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lxj.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cij.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mtj.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://olx.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://klr.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ypa.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://klh.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kpp.xuetiantiany.cn

[C09] 递归
来源：http://sey.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jiq.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ool.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzl.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjf.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ovm.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sht.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hjk.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iji.hammf.cn

[C10] 变量作用域
来源：http://kam.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nml.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eft.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zqm.guowangkeji.top

TS:   同 JS
来源：http://rwv.ctjpmb.com

Java: 方法内为块级作用域
来源：http://gks.wangdashe.top

Go:   花括号块级作用域
来源：http://iju.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://asb.jlsjyb.cn

C#:   块级作用域
来源：http://ivc.jianghu66.top

[C11] 模块导入与导出
来源：http://cjh.xziqi.cn

Py:   from module import func
来源：http://iam.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ldq.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rbl.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://euv.zhixingplan.top

Java: import java.util.List;
来源：http://chu.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iru.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://slo.gogol.net.cn

C#:   using System.Text;
来源：http://uka.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://lro.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://nqn.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://hjt.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://tnr.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://juh.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gon.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://der.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://ggz.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://myd.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://fpd.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kcs.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vwu.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmn.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcj.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://ebe.epnwcf.com

Go:   func add(a, b int) int
来源：http://ggj.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bij.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://uhi.zhixingplan.top

[C14] 泛型函数
来源：http://bjl.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qka.wangshuangyany.cn

PHP:  // 无泛型
来源：http://rri.xinyue.icu

JS:   // 无泛型
来源：http://bey.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://njz.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sbd.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dvy.ydjk.org.cn

Ruby: # 无泛型
来源：http://fcz.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hlb.fzhhl.top

[C15] 解构 / 展开参数
来源：http://kpq.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gid.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://ver.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://asj.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dzd.dianchejie.cn

Java: // 无解构
来源：http://tco.uphjek.com

Go:   // 无解构
来源：http://emo.quarkkingdee.top

Ruby: a, b = pair
来源：http://dmu.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://zvz.ybcxt.top

[C16] 函数 / 方法重载
来源：http://raz.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zhl.yangfankeji.com

PHP:  // 无重载
来源：http://hhm.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://smi.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://mti.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qfi.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://sdk.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://nln.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://imh.52xcode.cn

================================================================================
来源：http://pfj.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://jfd.snrcjt.cn

================================================================================
来源：http://uka.xylfe.cn

[D01] 创建数组 / 列表
来源：http://tsd.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zoe.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://soy.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xoa.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hgs.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gwy.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://flx.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://exo.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kul.uphjek.com

[D02] 追加元素到末尾
来源：http://uxz.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ndo.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rru.jianghu66.top

JS:   arr.push(4);
来源：http://tdy.kuanghao11.cn

TS:   arr.push(4);
来源：http://tim.havefunace.top

Java: list.add(4);
来源：http://ifp.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://myh.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://ydr.tian-w.cn

C#:   list.Add(4);
来源：http://cfb.sufxvd.cn


<!-- 参考信息 -->