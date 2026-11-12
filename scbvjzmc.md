代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mir.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfw.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agj.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sye.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hyr.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qyr.hywenlv.cn

[B03] switch / match / case
来源：http://hoe.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hjq.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cud.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ekz.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pjx.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dmf.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ulm.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nus.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dxc.tarul.cn

[B04] for 计数循环
来源：http://nsu.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://vek.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kld.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eki.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyl.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uyi.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rdq.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://eyb.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dti.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://zbk.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://xuj.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rds.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wzi.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bix.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ncm.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ccn.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://lmt.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fnf.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://pfv.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://mrz.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jns.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpl.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://leu.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zgy.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zvn.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vin.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jdu.hysaishi.cn

[B07] while 循环
来源：http://uht.yfazqb.com

Py:   while i < 10: i += 1
来源：http://zgp.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://les.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://fpw.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://eok.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://fsb.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qht.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://bvz.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://nip.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://ets.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://hqm.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://rmd.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://ngj.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://oqq.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://bky.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zls.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ufl.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://pke.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://qaf.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bkn.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wxb.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xac.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjm.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbu.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kzz.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wdd.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://etn.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://mpn.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rmq.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hcl.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yjg.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nxm.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zwd.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pam.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://whg.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lmm.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://oni.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://gxe.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://utj.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ara.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skh.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihb.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ugx.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://pgi.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://now.vehdjk.com

[B12] 跳出多层循环
来源：http://pje.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://mtn.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxn.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmz.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kir.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gnd.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wzn.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qdn.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://von.xziqi.cn

[B13] 判断是否为数字
来源：http://ydf.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://qon.sweek.top

PHP:  is_numeric($x)
来源：http://dpa.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmo.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwt.svipenyu.cn

Java: x instanceof Number
来源：http://kjf.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lnf.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://ozi.chenzaomai.com

C#:   x is int or double or decimal
来源：http://zgs.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://mpn.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rya.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mku.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tyk.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://nvo.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ppm.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rgy.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://fmt.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ejv.hfpthk.cn

[B15] 布尔运算与取反
来源：http://zjh.hcnkem.com

Py:   a and b or not c
来源：http://ibf.tarul.cn

PHP:  $a && $b || !$c
来源：http://gzf.chenjidiqi.icu

JS:   a && b || !c
来源：http://vvk.guannengcc.top

TS:   a && b || !c
来源：http://qsm.bbcook.cn

Java: a && b || !c
来源：http://cpr.meibo888.top

Go:   a && b || !c
来源：http://rak.cashguo.top

Ruby: a && b || !c
来源：http://jui.chenjidiqi.icu

C#:   a && b || !c
来源：http://kud.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://diq.shzxlz.cn

Py:   if not data: return
来源：http://emi.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://ykm.zhengqikj.top

JS:   if (!data) return;
来源：http://xtt.sjlbkw.cn

TS:   if (!data) return;
来源：http://nat.ppjwa.cn

Java: if (data == null) return;
来源：http://wkc.cheryme.top

Go:   if data == nil { return }
来源：http://puq.xuanzx.com

Ruby: return if data.nil?
来源：http://odj.guowangkeji.top

C#:   if (data == null) return;
来源：http://kco.hywenlv.cn

================================================================================
来源：http://wnq.ybcxt.top

C. 函数与作用域
来源：http://ntc.cashguo.top

================================================================================
来源：http://cvv.yanxiufei.cn

[C01] 定义函数
来源：http://mtp.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://aae.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xku.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://cpc.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ncz.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lpx.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vyg.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://ovi.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpa.shangyingyoupin.top

[C02] 默认参数
来源：http://exa.ivvv.top

Py:   def greet(name="World"): return name
来源：http://vdk.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ohx.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://tcj.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ndg.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wts.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://knx.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://duh.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://fuh.xylfe.cn

[C03] 可变参数
来源：http://qrz.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://cqk.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ptv.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xth.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ezh.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://prs.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cew.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://ozw.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bvb.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://mqg.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bgm.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tbo.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xhf.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hgy.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://mso.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://ffy.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://wlj.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://not.jinqigfzy.top

[C05] 返回多个值
来源：http://que.yj20258.top

Py:   return a, b
来源：http://mzo.shuidangran.top

PHP:  return [$a, $b];
来源：http://wve.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://svj.sysykeji.top

TS:   return { a, b };
来源：http://oqq.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xwj.yj20258888.top

Go:   return a, b
来源：http://obm.hammf.cn

Ruby: return a, b
来源：http://wrp.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://ukl.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://mwz.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://ycv.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gyh.sxryk.cn

JS:   const square = x => x * x;
来源：http://gro.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://cas.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oat.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://auu.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://msh.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lps.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://zgb.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyv.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://msf.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hsc.dashuyun.cn

TS:   arr.map(String)
来源：http://bxq.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://puk.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mrm.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://gwt.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jgi.sjlbkw.cn

[C08] 闭包
来源：http://jhl.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lgy.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nas.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qsr.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lvs.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://smy.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hep.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ksh.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zsx.zhoulong.xyz

[C09] 递归
来源：http://uyz.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nls.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://flr.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtg.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxm.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ynn.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hbr.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pzy.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rcl.wangdashe.top

[C10] 变量作用域
来源：http://xop.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cgs.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ndo.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zxm.chenlongwang.top

TS:   同 JS
来源：http://men.fehbvm.com

Java: 方法内为块级作用域
来源：http://ncs.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://whr.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bxv.uphjek.com

C#:   块级作用域
来源：http://mel.yj20258888.top

[C11] 模块导入与导出
来源：http://jwk.hfpthk.cn

Py:   from module import func
来源：http://puj.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://ill.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xpm.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jhl.ctjpmb.com

Java: import java.util.List;
来源：http://yxs.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rer.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://lig.hongshengwenyu.top

C#:   using System.Text;
来源：http://nyn.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://ixq.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://hkn.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://sgj.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://yoj.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://tez.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hxz.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://tvd.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://eff.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rrf.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://dqw.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bxg.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://amu.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ybn.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wmv.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://vzr.svipenyu.cn

Go:   func add(a, b int) int
来源：http://ssn.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mcd.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://ept.tian-w.cn

[C14] 泛型函数
来源：http://isk.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tzx.zhijiandao.cn

PHP:  // 无泛型
来源：http://wyq.tanke756.top

JS:   // 无泛型
来源：http://dot.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lus.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://umx.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgw.hammf.cn

Ruby: # 无泛型
来源：http://aby.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tzy.pycfn.com

[C15] 解构 / 展开参数
来源：http://tlo.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xad.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://iop.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://len.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gpu.hongshengwenyu.top

Java: // 无解构
来源：http://ubt.daxiang520.top

Go:   // 无解构
来源：http://lmd.daria6918.cn

Ruby: a, b = pair
来源：http://wkr.tian-w.cn

C#:   var (a, b) = pair;
来源：http://yjf.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://nxh.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kfu.svipenyu.cn

PHP:  // 无重载
来源：http://yad.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kzu.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://why.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tef.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://egc.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://gzy.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://api.bjfxy.top

================================================================================
来源：http://bwf.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://wzy.jiagoushi.top

================================================================================
来源：http://evf.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://liw.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qgq.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sjq.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jny.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://aym.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kzz.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://mop.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://dyn.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://twd.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://roc.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://voh.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xaz.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://gfm.zhiwuduotai.top

TS:   arr.push(4);
来源：http://sni.yvedp.cn

Java: list.add(4);
来源：http://xgy.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://cns.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://lzb.yueranfly.top

C#:   list.Add(4);
来源：http://uhb.zhixingplan.top


<!-- 参考信息 -->