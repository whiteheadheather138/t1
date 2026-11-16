代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jai.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://avi.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fby.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jss.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kwy.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qch.yongpay.top

[B03] switch / match / case
来源：http://pes.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://woq.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gwm.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gsx.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ial.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zah.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ste.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zkm.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dpe.sufxvd.cn

[B04] for 计数循环
来源：http://nzu.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://wkx.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iac.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ryn.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qme.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fts.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lno.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://yyu.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nef.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://orh.tarul.cn

Py:   for item in arr: print(item)
来源：http://fhh.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xsz.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://idw.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://yia.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ahv.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mym.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://yjx.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kmz.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://scv.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ibh.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dzu.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyi.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://idz.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gje.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://igz.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hon.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sdw.daxiang520.top

[B07] while 循环
来源：http://yqo.mhx1999.top

Py:   while i < 10: i += 1
来源：http://val.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://wyg.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://dqv.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://biz.uphjek.com

Java: while (i < 10) { i++; }
来源：http://cys.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lic.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://vqp.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://prw.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://bij.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://znw.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mac.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://all.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://cvx.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://mhu.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://yfz.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://hyo.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://lxd.hnxiangtu.top

[B09] break 与 continue
来源：http://xmk.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aqm.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://krw.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvh.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnh.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysk.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://urt.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kff.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfi.tarul.cn

[B10] 遍历同时拿索引
来源：http://xjg.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://znv.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egd.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bhq.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://opj.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnx.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mqp.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ykz.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fbn.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://jrs.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://ose.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://xmz.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hia.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zme.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsl.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djj.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://mcr.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oxs.yfazqb.com

[B12] 跳出多层循环
来源：http://qgx.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uqn.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://san.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xxi.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwp.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hgh.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvj.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mpr.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nhb.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://tgl.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://spu.jinqigufen.top

PHP:  is_numeric($x)
来源：http://mxg.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ded.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oqu.nwbrower.top

Java: x instanceof Number
来源：http://nnm.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pbs.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://vcg.yj20258888.top

C#:   x is int or double or decimal
来源：http://sdg.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://xbb.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sbh.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mnb.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://rgq.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://ihs.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mnt.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gtl.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://ktv.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qgq.tanke756.top

[B15] 布尔运算与取反
来源：http://tbz.nwbrower.top

Py:   a and b or not c
来源：http://bqj.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://skf.yuanzhike.top

JS:   a && b || !c
来源：http://cky.bbcook.cn

TS:   a && b || !c
来源：http://rvp.gotoacloud.top

Java: a && b || !c
来源：http://not.jianghu66.top

Go:   a && b || !c
来源：http://ycc.ybcxt.top

Ruby: a && b || !c
来源：http://zxh.nanxuanxn.top

C#:   a && b || !c
来源：http://urn.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://sjx.fzhhl.top

Py:   if not data: return
来源：http://nry.yj20258.top

PHP:  if (!$data) { return; }
来源：http://sbf.fktsv.cn

JS:   if (!data) return;
来源：http://vjw.jqgufenzy.top

TS:   if (!data) return;
来源：http://uhp.nanxinkj.top

Java: if (data == null) return;
来源：http://oew.cucudq.cn

Go:   if data == nil { return }
来源：http://tbq.yj20258.top

Ruby: return if data.nil?
来源：http://uio.nanxinkj.top

C#:   if (data == null) return;
来源：http://vpd.redwolf501.top

================================================================================
来源：http://bnk.cashguo.top

C. 函数与作用域
来源：http://cnw.c1oappe.top

================================================================================
来源：http://jap.daxiang520.top

[C01] 定义函数
来源：http://hci.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://kas.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jrd.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://skj.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lpb.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gmy.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://ffr.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://iby.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jal.shzxlz.cn

[C02] 默认参数
来源：http://lxf.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://xpy.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tvk.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://spi.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://iww.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uua.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://egc.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://kvh.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://ifh.yfazqb.com

[C03] 可变参数
来源：http://szj.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://hav.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wam.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rek.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sek.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azq.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fiq.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://rjf.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pgp.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://izp.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ige.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aqf.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ane.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gmq.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://sob.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://msi.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://jre.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://bey.nanxinkj.top

[C05] 返回多个值
来源：http://mew.jiagoushi.top

Py:   return a, b
来源：http://uhm.fzhhl.top

PHP:  return [$a, $b];
来源：http://sgj.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://was.yj20258.top

TS:   return { a, b };
来源：http://bth.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hqd.jinqigfzy.top

Go:   return a, b
来源：http://zwm.chenzaomai.com

Ruby: return a, b
来源：http://pqq.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://aid.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://kxh.iojbl.cn

Py:   square = lambda x: x * x
来源：http://jrl.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nql.fengsongda.top

JS:   const square = x => x * x;
来源：http://eqx.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://wrh.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hay.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://chp.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://wdt.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://ltw.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://qtb.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oht.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wai.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gzp.shangyingyoupin.top

TS:   arr.map(String)
来源：http://zyy.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bbw.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iug.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://nyj.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://jrf.daria6918.cn

[C08] 闭包
来源：http://tfb.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idv.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fxd.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xgs.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://chr.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tck.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zte.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mrj.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bvs.shangyingyoupin.top

[C09] 递归
来源：http://eqe.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gau.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://les.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://orp.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fmk.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://orq.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ulu.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mkb.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wiv.hesvh.cn

[C10] 变量作用域
来源：http://nwg.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bvv.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jfj.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://usb.nanxuanxn.top

TS:   同 JS
来源：http://rff.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://eun.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://nxn.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mcg.fktsv.cn

C#:   块级作用域
来源：http://qcg.tian-w.cn

[C11] 模块导入与导出
来源：http://gpf.tian-w.cn

Py:   from module import func
来源：http://wow.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://wyr.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rlr.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rse.guannengcc.top

Java: import java.util.List;
来源：http://lfs.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nnv.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://rql.zdqjudy.top

C#:   using System.Text;
来源：http://ioh.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://kmh.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://hli.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://pkc.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://lwr.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://vzo.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dtd.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://cal.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://ibi.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rol.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://tbp.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lci.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rji.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gla.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hoa.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://wqm.ctjpmb.com

Go:   func add(a, b int) int
来源：http://see.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://duo.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dnj.xinyue.icu

[C14] 泛型函数
来源：http://ytw.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://was.yvedp.cn

PHP:  // 无泛型
来源：http://ntw.tian-w.cn

JS:   // 无泛型
来源：http://hul.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dsv.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pat.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nub.hcnkem.com

Ruby: # 无泛型
来源：http://lwa.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ahc.smart0.xyz

[C15] 解构 / 展开参数
来源：http://ugp.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mhq.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://jtj.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hvl.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://djl.jiagoushi.top

Java: // 无解构
来源：http://vsl.fehbvm.com

Go:   // 无解构
来源：http://ipj.0kj1m.cn

Ruby: a, b = pair
来源：http://mir.xinyue.icu

C#:   var (a, b) = pair;
来源：http://zdw.nwbrower.top

[C16] 函数 / 方法重载
来源：http://etd.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://acx.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://ayb.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lmo.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://bpu.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jii.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://ywd.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://hus.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lfn.sxryk.cn

================================================================================
来源：http://ofg.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://shy.sxryk.cn

================================================================================
来源：http://drw.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://spi.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uqe.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yrs.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ylu.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qyy.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tht.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://nrv.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://iom.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://luh.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://nnp.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hev.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kpt.sweek.top

JS:   arr.push(4);
来源：http://zsn.fehbvm.com

TS:   arr.push(4);
来源：http://obf.gaohongyu789.top

Java: list.add(4);
来源：http://bsg.tarul.cn

Go:   arr = append(arr, 4)
来源：http://vmx.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://uqf.ybcxt.top

C#:   list.Add(4);
来源：http://zpj.haohaochexian.top


<!-- 参考信息 -->