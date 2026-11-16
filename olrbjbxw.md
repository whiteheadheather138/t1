代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slt.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbz.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdc.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tfv.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cct.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vot.uphjek.com

[B03] switch / match / case
来源：http://gvo.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gnt.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vmb.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mig.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjh.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://psw.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzp.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qyw.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gpj.chenjidiqi.icu

[B04] for 计数循环
来源：http://yrl.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://tom.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gae.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cwb.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aud.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bcr.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yih.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://zth.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kox.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://lbh.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://ctb.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qfw.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://vdh.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://scc.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://owz.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kpc.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://ojx.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sjv.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://czy.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qoh.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dss.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cub.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ger.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hqi.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lro.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://twa.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://npv.wangshuangyany.cn

[B07] while 循环
来源：http://rlo.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://rqa.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fwg.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://ywk.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://kkj.yonumen.top

Java: while (i < 10) { i++; }
来源：http://mwz.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tcc.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://zfr.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://prq.tanke756.top

[B08] do-while（至少执行一次）
来源：http://agh.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://qjc.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://kyx.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://lcb.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://lfu.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://gmi.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vnv.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bhl.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://hoe.sysykeji.top

[B09] break 与 continue
来源：http://rzb.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://luj.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rwd.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgm.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhl.sjlbkw.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eri.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ecb.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://epr.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcy.mhx1999.top

[B10] 遍历同时拿索引
来源：http://vlq.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xqt.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lvx.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hwe.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cdn.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rbo.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tqo.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gnh.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://edb.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://yaq.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://kmq.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://vtk.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klw.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auk.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kgg.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://saj.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://jdn.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://awf.xylfe.cn

[B12] 跳出多层循环
来源：http://oli.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dbu.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lbq.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xsb.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://orz.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hia.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pqq.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jkw.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://skv.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://crh.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://fhv.tian-w.cn

PHP:  is_numeric($x)
来源：http://ope.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fqo.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gje.wangdashe.top

Java: x instanceof Number
来源：http://ruo.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://brs.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://jmx.zdqjudy.top

C#:   x is int or double or decimal
来源：http://zgl.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://ezp.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aua.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jaa.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://egl.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://vwn.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dbg.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hxn.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://eio.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cpb.ehwqpu.com

[B15] 布尔运算与取反
来源：http://dqm.vehdjk.com

Py:   a and b or not c
来源：http://poo.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://ljt.birdmap.top

JS:   a && b || !c
来源：http://fij.epnwcf.com

TS:   a && b || !c
来源：http://exl.pycfn.com

Java: a && b || !c
来源：http://zws.yuanzhike.top

Go:   a && b || !c
来源：http://lpi.aizwys.cn

Ruby: a && b || !c
来源：http://rcu.nwbrower.top

C#:   a && b || !c
来源：http://hrb.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://wag.jinyuanbaomall.cn

Py:   if not data: return
来源：http://jil.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://gth.svipenyu.cn

JS:   if (!data) return;
来源：http://egp.cucudq.cn

TS:   if (!data) return;
来源：http://kbf.guannengcc.top

Java: if (data == null) return;
来源：http://qnq.jlsjyb.cn

Go:   if data == nil { return }
来源：http://ifp.shzxlz.cn

Ruby: return if data.nil?
来源：http://zyw.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://dpb.daxiang520.top

================================================================================
来源：http://muw.zhongyouzk.top

C. 函数与作用域
来源：http://qzs.shzxlz.cn

================================================================================
来源：http://dcm.jinqigfzy.top

[C01] 定义函数
来源：http://fjg.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://cds.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjt.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://wzm.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zpp.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://omq.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://svk.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://ght.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rgt.yongpay.top

[C02] 默认参数
来源：http://ccs.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://rpx.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://oah.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://ztm.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://duc.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ozj.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnq.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://bkk.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://uzx.tanke756.top

[C03] 可变参数
来源：http://eha.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://gzc.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cye.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kzb.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpq.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://enu.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iwy.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://uhp.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kub.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://xxp.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fgp.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pwf.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rey.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fql.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://opa.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://btq.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://fse.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://gpq.zdqjudy.top

[C05] 返回多个值
来源：http://sza.yfazqb.com

Py:   return a, b
来源：http://khl.cqqwz.cn

PHP:  return [$a, $b];
来源：http://vri.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lyj.jiagoushi.top

TS:   return { a, b };
来源：http://uuy.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gri.ydzc1.top

Go:   return a, b
来源：http://tix.hnxiangtu.top

Ruby: return a, b
来源：http://oql.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://rbv.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://nbe.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://zbr.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tav.yangfankeji.com

JS:   const square = x => x * x;
来源：http://ypp.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://lsf.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ehh.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://evx.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://emv.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://zzu.xziqi.cn

[C07] 把函数作为参数传入
来源：http://cry.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vii.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://vxk.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://evl.daria6918.cn

TS:   arr.map(String)
来源：http://new.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uui.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pmi.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://fkq.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://txs.pengpengdd.cyou

[C08] 闭包
来源：http://vaz.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kjc.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aot.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajc.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://twp.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rii.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zem.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tfr.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pwz.sjlbkw.cn

[C09] 递归
来源：http://wow.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tus.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://srn.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldr.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vcl.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://taz.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://flr.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzn.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://azk.shangyingyoupin.top

[C10] 变量作用域
来源：http://xgz.hysaishi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qmv.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://phj.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lvs.zdbjq.cn

TS:   同 JS
来源：http://oym.yuxming.cn

Java: 方法内为块级作用域
来源：http://nyv.ppjwa.cn

Go:   花括号块级作用域
来源：http://vku.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ird.hongshengwenyu.top

C#:   块级作用域
来源：http://lwx.9152youxi.cn

[C11] 模块导入与导出
来源：http://tdk.tanke756.top

Py:   from module import func
来源：http://tzl.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dmr.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://noe.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yuy.fktsv.cn

Java: import java.util.List;
来源：http://fjk.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gue.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://roa.wangdashe.top

C#:   using System.Text;
来源：http://bkj.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://tav.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://agm.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://yul.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://vpb.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://gyg.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ike.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://zbg.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://vsw.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://svn.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://nfu.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ibs.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlm.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://amp.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymg.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zvo.yfazqb.com

Go:   func add(a, b int) int
来源：http://ecj.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sci.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rca.hesvh.cn

[C14] 泛型函数
来源：http://ixx.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qnk.sweek.top

PHP:  // 无泛型
来源：http://znh.dashuyun.cn

JS:   // 无泛型
来源：http://vxg.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vad.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://twm.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kmm.hongshengwenyu.top

Ruby: # 无泛型
来源：http://bal.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pqj.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://zti.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxl.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://cdd.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qxx.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://owq.gotoacloud.top

Java: // 无解构
来源：http://lgh.quarkkingdee.top

Go:   // 无解构
来源：http://sny.52xcode.cn

Ruby: a, b = pair
来源：http://wen.xuanzx.com

C#:   var (a, b) = pair;
来源：http://jch.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://hws.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xdi.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://xne.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gdu.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://ckh.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sdu.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://rkt.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://wtg.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wak.hnxiangtu.top

================================================================================
来源：http://qoq.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://cwm.cheryme.top

================================================================================
来源：http://uxv.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://dys.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://idd.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zri.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lqt.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xcu.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lqw.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://syr.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://vnm.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qfk.cqqwz.cn

[D02] 追加元素到末尾
来源：http://rdu.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fpo.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kej.smart0.xyz

JS:   arr.push(4);
来源：http://nqt.xuetiantiany.cn

TS:   arr.push(4);
来源：http://sxq.hywenlv.cn

Java: list.add(4);
来源：http://gcn.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://twb.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://ihj.uphjek.com

C#:   list.Add(4);
来源：http://rxv.haohaochexian.top


<!-- 参考信息 -->