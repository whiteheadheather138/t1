代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mbx.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ryl.zhongyouzk.top

[B03] switch / match / case
来源：http://aqx.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hom.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fma.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://slf.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://voo.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pdt.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mki.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xob.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cuk.hywenlv.cn

[B04] for 计数循环
来源：http://nvg.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://kxf.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nji.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pek.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://irz.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iiy.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jhm.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://tfs.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kgz.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://qvp.hesvh.cn

Py:   for item in arr: print(item)
来源：http://etr.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xtw.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://oth.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://byx.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wwq.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bdo.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://fef.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mhy.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://woe.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://llg.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bes.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jnb.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mfa.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hys.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fvv.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bsn.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gyy.haohaochexian.top

[B07] while 循环
来源：http://irf.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://idf.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://dax.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://fkv.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://fgk.uphjek.com

Java: while (i < 10) { i++; }
来源：http://eed.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sfb.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://zyi.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://cni.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://rwp.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://hcg.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jpk.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://otx.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://ihj.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://bjf.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ijm.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://zbl.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://opr.wangshuangyany.cn

[B09] break 与 continue
来源：http://wuk.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hni.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iia.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xxa.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guf.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvp.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yns.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ykc.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cij.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://doy.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nwu.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hoa.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pmu.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qeh.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dqw.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cod.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ond.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kcc.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://uvg.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://hyz.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://scc.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rxb.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vzi.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hti.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qpz.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://cms.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://obf.ydzc1.top

[B12] 跳出多层循环
来源：http://gpl.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tun.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ndv.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rme.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vgo.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwk.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gad.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hsu.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dqj.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://ijg.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://ueg.fehbvm.com

PHP:  is_numeric($x)
来源：http://for.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ugc.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uph.yj20258888.top

Java: x instanceof Number
来源：http://kmt.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryb.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://mvx.mhx1999.top

C#:   x is int or double or decimal
来源：http://lsq.c1oappe.top

[B14] 判断值是否在集合内
来源：http://qld.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mtx.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ipe.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://zvs.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://ucg.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hem.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wjb.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://qid.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uca.yj20258888.top

[B15] 布尔运算与取反
来源：http://svm.zdqjudy.top

Py:   a and b or not c
来源：http://pqf.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://kjy.shangyingyoupin.top

JS:   a && b || !c
来源：http://xoi.tian-w.cn

TS:   a && b || !c
来源：http://bet.dashuyun.cn

Java: a && b || !c
来源：http://huu.yj20258.top

Go:   a && b || !c
来源：http://sdh.vehdjk.com

Ruby: a && b || !c
来源：http://tfg.ydzc1.top

C#:   a && b || !c
来源：http://mdx.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://avi.hcnkem.com

Py:   if not data: return
来源：http://qcf.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://etw.cashguo.top

JS:   if (!data) return;
来源：http://gpi.jyoumei.cn

TS:   if (!data) return;
来源：http://jfe.jinqigfzy.top

Java: if (data == null) return;
来源：http://xzz.jianghu66.top

Go:   if data == nil { return }
来源：http://ofr.hywenlv.cn

Ruby: return if data.nil?
来源：http://lnx.vehdjk.com

C#:   if (data == null) return;
来源：http://hiy.meibo888.top

================================================================================
来源：http://ihp.shuidangran.top

C. 函数与作用域
来源：http://wmh.hywenlv.cn

================================================================================
来源：http://vvc.gzhubu.top

[C01] 定义函数
来源：http://exd.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://ooy.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqh.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://boc.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqs.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nzz.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://dac.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://jqp.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ool.9152youxi.cn

[C02] 默认参数
来源：http://hgj.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://cmg.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fep.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://rpk.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vrr.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yba.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zyy.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://ihz.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://cai.haohaochexian.top

[C03] 可变参数
来源：http://ghu.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://xvv.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aqh.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qfw.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://txt.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://som.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mfk.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zho.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fvc.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://zrs.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ufw.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vnk.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://trr.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yyf.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://vtz.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://kgu.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://fev.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://giy.zhixingplan.top

[C05] 返回多个值
来源：http://jkd.yangfankeji.com

Py:   return a, b
来源：http://uss.gogol.net.cn

PHP:  return [$a, $b];
来源：http://sew.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://skv.quarkkingdee.top

TS:   return { a, b };
来源：http://zzn.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ajz.dianchejie.cn

Go:   return a, b
来源：http://fhn.bbcook.cn

Ruby: return a, b
来源：http://dsd.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://ojr.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://baz.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://eja.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ewr.xinyue.icu

JS:   const square = x => x * x;
来源：http://yfb.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://kci.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wbt.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ovp.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://tgq.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lcm.fengsongda.top

[C07] 把函数作为参数传入
来源：http://aaa.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xlt.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pmc.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wia.jqgfzy.top

TS:   arr.map(String)
来源：http://djz.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dmf.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dyl.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://fci.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ksz.sweek.top

[C08] 闭包
来源：http://nwi.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://urf.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://piu.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lmy.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://igc.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://etb.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wjy.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnc.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://msc.snrcjt.cn

[C09] 递归
来源：http://qhz.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zlu.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://anp.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yez.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvy.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zfe.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://imb.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ykv.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdi.fehbvm.com

[C10] 变量作用域
来源：http://dcm.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://num.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ccd.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jts.smart0.xyz

TS:   同 JS
来源：http://nky.52xcode.cn

Java: 方法内为块级作用域
来源：http://ary.daxiang520.top

Go:   花括号块级作用域
来源：http://eda.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://anz.jinqigfzy.top

C#:   块级作用域
来源：http://wzb.cashguo.top

[C11] 模块导入与导出
来源：http://thy.bbcook.cn

Py:   from module import func
来源：http://vhp.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tiz.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lbx.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sji.hywenlv.cn

Java: import java.util.List;
来源：http://srr.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rbw.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://jnq.zhongyouzk.top

C#:   using System.Text;
来源：http://zza.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://owm.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://ybv.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://wxi.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://yzm.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://rul.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://msu.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://rxy.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://ozk.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gpb.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://dbl.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mzq.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ily.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pzs.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qog.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xoo.shuidangran.top

Go:   func add(a, b int) int
来源：http://nsx.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hqh.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ckt.yfazqb.com

[C14] 泛型函数
来源：http://pjb.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oqo.tarul.cn

PHP:  // 无泛型
来源：http://tah.shangyingyoupin.top

JS:   // 无泛型
来源：http://goo.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cmg.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rkz.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ert.quarkkingdee.top

Ruby: # 无泛型
来源：http://vto.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pau.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://sfq.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kjy.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://xwd.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ehr.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ghu.ctjpmb.com

Java: // 无解构
来源：http://xic.bbcook.cn

Go:   // 无解构
来源：http://xgl.c1oappe.top

Ruby: a, b = pair
来源：http://qpm.tarul.cn

C#:   var (a, b) = pair;
来源：http://bsh.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://nnl.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nha.fzhhl.top

PHP:  // 无重载
来源：http://gde.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilf.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://gkw.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ugy.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://jbe.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://drd.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hcc.tian-w.cn

================================================================================
来源：http://fia.cheryme.top

D. 数组 / 列表 / 集合
来源：http://hem.shuidangran.top

================================================================================
来源：http://frf.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://heh.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ibg.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ewn.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://geq.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnw.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ifk.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://gpl.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://euv.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zda.xziqi.cn

[D02] 追加元素到末尾
来源：http://rja.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uis.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbv.yangfankeji.com

JS:   arr.push(4);
来源：http://prm.xuanzx.com

TS:   arr.push(4);
来源：http://jcb.hfpthk.cn

Java: list.add(4);
来源：http://yxt.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://fkg.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://mna.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://adj.yfazqb.com

[D03] 在指定位置插入元素
来源：http://afz.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://mrn.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwd.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zcq.shuidangran.top


<!-- 参考信息 -->