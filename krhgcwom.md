代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dnp.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frp.shzxlz.cn

[B03] switch / match / case
来源：http://ykh.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kbp.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qup.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhc.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jvl.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://amz.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mly.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pxh.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bez.sysykeji.top

[B04] for 计数循环
来源：http://vuc.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://fkf.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sag.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wuv.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uln.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dsm.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xhy.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://lvo.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zmw.yongpay.top

[B05] 遍历数组 / 列表
来源：http://lkd.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://kbx.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://btb.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nwn.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xaw.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pkc.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wjg.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://vni.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sxe.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://uqi.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bal.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://msi.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypl.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://twp.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbc.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lgt.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ohs.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fai.pycfn.com

[B07] while 循环
来源：http://rzo.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://zod.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://uba.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://ood.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://qzf.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://weq.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ook.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://msm.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://ulb.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://jry.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://atc.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ybi.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://dgg.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://mqr.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://urm.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://alf.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://ijg.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://hzj.hammf.cn

[B09] break 与 continue
来源：http://ldc.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kpy.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://der.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrf.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eal.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aon.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://npb.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ahs.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhn.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://xxc.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mvs.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xkw.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wdq.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ifj.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kpr.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qlx.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://war.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://soa.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://ykz.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://oli.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://fhp.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vde.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bqo.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mms.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://znq.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://dqx.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mnk.aizwys.cn

[B12] 跳出多层循环
来源：http://ifo.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dnr.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://khu.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wne.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://evi.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wvp.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ztg.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dml.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xut.hywenlv.cn

[B13] 判断是否为数字
来源：http://tsh.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://jyi.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://cxy.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hpy.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pjv.redwolf501.top

Java: x instanceof Number
来源：http://yde.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://chv.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://fwq.chenzaomai.com

C#:   x is int or double or decimal
来源：http://sql.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://lzf.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fpx.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ivg.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://rjr.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ymq.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ipe.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ewz.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://crw.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ljz.fzhhl.top

[B15] 布尔运算与取反
来源：http://pmt.tianlin.xyz

Py:   a and b or not c
来源：http://pmg.xinyue.icu

PHP:  $a && $b || !$c
来源：http://wiy.uphjek.com

JS:   a && b || !c
来源：http://lbp.yvedp.cn

TS:   a && b || !c
来源：http://sqo.tian-w.cn

Java: a && b || !c
来源：http://dvz.ctjpmb.com

Go:   a && b || !c
来源：http://sdh.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://qxs.0kj1m.cn

C#:   a && b || !c
来源：http://plz.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://ynp.jiagoushi.top

Py:   if not data: return
来源：http://ceg.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://kxw.gaohongyu789.top

JS:   if (!data) return;
来源：http://fer.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://ucl.shzxlz.cn

Java: if (data == null) return;
来源：http://azr.sweek.top

Go:   if data == nil { return }
来源：http://pln.jqgfzy.top

Ruby: return if data.nil?
来源：http://hpt.gaohongyu789.top

C#:   if (data == null) return;
来源：http://gtu.jqgufenzy.top

================================================================================
来源：http://jkp.yj20258888.top

C. 函数与作用域
来源：http://lgl.wangdashe.top

================================================================================
来源：http://nhz.yj20258.top

[C01] 定义函数
来源：http://tfl.cheryme.top

Py:   def add(a, b): return a + b
来源：http://rbp.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gcq.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://ibo.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndh.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qgb.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xbe.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://jrz.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bib.iojbl.cn

[C02] 默认参数
来源：http://wzc.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://lme.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://frc.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://fcs.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ewa.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xeh.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hkf.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://oil.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://akr.hammf.cn

[C03] 可变参数
来源：http://nyx.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://pud.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fyy.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wtj.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ath.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://obw.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cda.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://smm.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ptm.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://uaq.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fqm.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://swb.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xxy.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ulr.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://acg.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://ofd.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://bvg.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://ykb.ydjk.org.cn

[C05] 返回多个值
来源：http://qco.chenlongwang.top

Py:   return a, b
来源：http://pxc.fzhhl.top

PHP:  return [$a, $b];
来源：http://hdu.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xpv.haohaochexian.top

TS:   return { a, b };
来源：http://zpq.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cyu.kuanghao11.cn

Go:   return a, b
来源：http://nda.jiagoushi.top

Ruby: return a, b
来源：http://dgd.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://yzm.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://yfy.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://dvk.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ddy.yonumen.top

JS:   const square = x => x * x;
来源：http://ifb.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://ugg.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pqo.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mri.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://pwf.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://qkw.ybcxt.top

[C07] 把函数作为参数传入
来源：http://prw.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zdl.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://gxu.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tjn.chenjidiqi.icu

TS:   arr.map(String)
来源：http://mzo.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nyt.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bra.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://kdu.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iyo.hnxiangtu.top

[C08] 闭包
来源：http://ffg.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qyg.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ybn.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gvz.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bkl.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qgp.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xit.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kak.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jsd.yfazqb.com

[C09] 递归
来源：http://tim.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uxn.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xae.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ulh.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzd.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kjd.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://czh.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fqm.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ljw.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://grj.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pnq.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aso.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://phs.zhongyouzk.top

TS:   同 JS
来源：http://zwd.meibo888.top

Java: 方法内为块级作用域
来源：http://ali.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://izi.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://shd.hfpthk.cn

C#:   块级作用域
来源：http://meo.wangdashe.top

[C11] 模块导入与导出
来源：http://rts.nanxuanxn.top

Py:   from module import func
来源：http://dfm.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bgl.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://irh.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nul.cqqwz.cn

Java: import java.util.List;
来源：http://afk.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ztg.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://plr.dashuyun.cn

C#:   using System.Text;
来源：http://bee.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://flt.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://hbz.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://bes.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://jmz.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://ako.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ddp.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://axv.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ewy.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sou.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://fxe.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wpd.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://giq.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://usl.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjd.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fhk.haohaochexian.top

Go:   func add(a, b int) int
来源：http://kvd.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lzr.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://lmz.c1oappe.top

[C14] 泛型函数
来源：http://woo.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sps.hammf.cn

PHP:  // 无泛型
来源：http://ypy.shzxlz.cn

JS:   // 无泛型
来源：http://wca.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mgj.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mzi.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nmd.haohaochexian.top

Ruby: # 无泛型
来源：http://hst.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mvs.sysykeji.top

[C15] 解构 / 展开参数
来源：http://uwj.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://krb.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://gkd.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vkx.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kck.chenzaomai.com

Java: // 无解构
来源：http://ebj.nwbrower.top

Go:   // 无解构
来源：http://wki.smart0.xyz

Ruby: a, b = pair
来源：http://yyi.ivvv.top

C#:   var (a, b) = pair;
来源：http://sfa.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://mny.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vcc.daria6918.cn

PHP:  // 无重载
来源：http://ydq.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vik.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://bfi.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://mkw.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://lvl.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://ajc.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uir.gaohongyu789.top

================================================================================
来源：http://vee.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://tdv.daxiang520.top

================================================================================
来源：http://kjn.bbcook.cn

[D01] 创建数组 / 列表
来源：http://pvf.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://hmo.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://arz.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://twa.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mst.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ayx.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://tvs.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://lpi.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vls.havefunace.top

[D02] 追加元素到末尾
来源：http://gih.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyj.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qup.hysaishi.cn

JS:   arr.push(4);
来源：http://rhw.yueranfly.top

TS:   arr.push(4);
来源：http://ttz.nwbrower.top

Java: list.add(4);
来源：http://qgd.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://gkk.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://yut.cashguo.top

C#:   list.Add(4);
来源：http://uok.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://usy.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://zrn.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nqc.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://czc.yuxming.cn


<!-- 参考信息 -->