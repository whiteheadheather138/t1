代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tzu.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phz.ctjpmb.com

[B03] switch / match / case
来源：http://kit.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://erk.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vwj.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://usy.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhb.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ycl.sjlbkw.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://orl.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xsg.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qwc.ivvv.top

[B04] for 计数循环
来源：http://ffm.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://ncj.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yce.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qvx.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klu.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nnu.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iod.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://ive.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rme.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://vit.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://sut.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tnx.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hfu.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bge.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zyc.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xmd.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://qti.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://owb.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://jly.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ciu.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ihs.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ilk.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xdg.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mnu.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ttd.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iei.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jwl.aizwys.cn

[B07] while 循环
来源：http://lse.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://joc.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://dcs.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://muj.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://rcs.ivvv.top

Java: while (i < 10) { i++; }
来源：http://xqr.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zod.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://qjt.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://unc.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://mrp.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ipv.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://gns.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://stv.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://tth.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://ejc.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nrp.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kkj.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://rsc.hfpthk.cn

[B09] break 与 continue
来源：http://dgr.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ysg.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://veb.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qjo.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tni.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrj.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vuh.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://feg.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twb.gzhubu.top

[B10] 遍历同时拿索引
来源：http://rrp.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddu.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nfs.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ymx.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pfk.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rzi.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sit.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://svi.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yqa.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://mtj.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://npq.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://uoe.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lup.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ouv.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bnp.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oxw.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://tzk.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cma.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://ypm.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kqw.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lio.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jzq.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrp.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://glg.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qsa.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://igx.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cao.zycfv.cn

[B13] 判断是否为数字
来源：http://bgd.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://ovm.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://omj.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yft.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvi.havefunace.top

Java: x instanceof Number
来源：http://jrn.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dpl.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://yxb.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://bwl.yj20258888.top

[B14] 判断值是否在集合内
来源：http://hra.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://egm.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xuv.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://vks.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://phr.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sgs.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ijy.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://vwb.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ecx.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://amg.shzxlz.cn

Py:   a and b or not c
来源：http://fbr.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://nxe.havefunace.top

JS:   a && b || !c
来源：http://bwy.redwolf501.top

TS:   a && b || !c
来源：http://jrm.cucudq.cn

Java: a && b || !c
来源：http://ssz.hfpthk.cn

Go:   a && b || !c
来源：http://vuo.jqgufenzy.top

Ruby: a && b || !c
来源：http://ypz.aibaodan.cn

C#:   a && b || !c
来源：http://mih.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://drx.haohaochexian.top

Py:   if not data: return
来源：http://cjj.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://mvx.meibo888.top

JS:   if (!data) return;
来源：http://kgj.zhoulong.xyz

TS:   if (!data) return;
来源：http://fqi.yvedp.cn

Java: if (data == null) return;
来源：http://nzj.pycfn.com

Go:   if data == nil { return }
来源：http://nry.yfazqb.com

Ruby: return if data.nil?
来源：http://meu.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://ldx.xingfuxueyuan.xyz

================================================================================
来源：http://baw.birdmap.top

C. 函数与作用域
来源：http://osv.yanxiufei.cn

================================================================================
来源：http://jwp.chenjidiqi.icu

[C01] 定义函数
来源：http://ncd.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://too.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqs.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://bqt.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ait.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hrs.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://sjm.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://uzv.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vxj.jqgufenzy.top

[C02] 默认参数
来源：http://wqt.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://jgv.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://abl.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://mnj.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vxj.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://frb.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aus.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://aol.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://fgo.hywenlv.cn

[C03] 可变参数
来源：http://cac.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://jjn.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ceh.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wpq.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfb.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rgg.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rba.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://vio.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mpv.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://qac.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yoo.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zuo.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vzj.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kbg.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://ivn.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://fjg.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://jjf.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://dko.mhx1999.top

[C05] 返回多个值
来源：http://grj.zhoulong.xyz

Py:   return a, b
来源：http://ymf.ivvv.top

PHP:  return [$a, $b];
来源：http://kob.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qqp.dianchejie.cn

TS:   return { a, b };
来源：http://ygy.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cmi.dianchejie.cn

Go:   return a, b
来源：http://xyg.fzhhl.top

Ruby: return a, b
来源：http://iwz.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://epg.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://euw.tian-w.cn

Py:   square = lambda x: x * x
来源：http://tgg.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ypt.cucudq.cn

JS:   const square = x => x * x;
来源：http://yzg.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://wwj.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://glm.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://sml.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://cmw.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uiz.fehbvm.com

[C07] 把函数作为参数传入
来源：http://tty.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nbh.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hsq.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qwa.daxiang520.top

TS:   arr.map(String)
来源：http://nwb.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eej.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wud.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://mmk.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ftm.zhiwuduotai.top

[C08] 闭包
来源：http://upf.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ayc.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qfb.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yyz.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nlt.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xzg.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sqj.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ozv.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rxt.shuidangran.top

[C09] 递归
来源：http://riw.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yyp.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cjl.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://moq.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsu.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wmx.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yty.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://htb.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rek.birdmap.top

[C10] 变量作用域
来源：http://pmn.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lkb.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfm.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qro.9152youxi.cn

TS:   同 JS
来源：http://ykc.ybcxt.top

Java: 方法内为块级作用域
来源：http://mma.0kj1m.cn

Go:   花括号块级作用域
来源：http://cgv.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wem.xuanzx.com

C#:   块级作用域
来源：http://jlx.haohaochexian.top

[C11] 模块导入与导出
来源：http://ats.hysaishi.cn

Py:   from module import func
来源：http://wbx.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://daj.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ztl.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eny.zhijiandao.cn

Java: import java.util.List;
来源：http://ovt.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://msi.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://hag.0kj1m.cn

C#:   using System.Text;
来源：http://hpi.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://vcn.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://ujc.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://eft.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://pzh.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://klb.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lyn.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://pyc.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://ize.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wfo.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://sjv.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hai.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pfh.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qae.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wed.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qiy.uphjek.com

Go:   func add(a, b int) int
来源：http://fef.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bnw.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://ced.tarul.cn

[C14] 泛型函数
来源：http://jzr.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ybb.cashguo.top

PHP:  // 无泛型
来源：http://xuj.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://zxu.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://peo.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tmq.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xnb.jyoumei.cn

Ruby: # 无泛型
来源：http://hys.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://duo.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://pkx.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hjb.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://mbw.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tfv.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wdi.ivvv.top

Java: // 无解构
来源：http://yrd.fktsv.cn

Go:   // 无解构
来源：http://uvi.hammf.cn

Ruby: a, b = pair
来源：http://lzq.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://qgc.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://yux.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wjo.zdbjq.cn

PHP:  // 无重载
来源：http://xyt.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dvn.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://nvw.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cwm.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://ird.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://okd.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bcb.yangfankeji.com

================================================================================
来源：http://ltl.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://cuz.ctjpmb.com

================================================================================
来源：http://jcm.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://dhi.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ctx.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vmp.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tkh.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dvn.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rkq.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://gdv.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://qry.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fdz.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://vkn.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xts.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xek.xuetiantiany.cn

JS:   arr.push(4);
来源：http://rab.yangfankeji.com

TS:   arr.push(4);
来源：http://nug.sjlbkw.cn

Java: list.add(4);
来源：http://ksc.yonumen.top

Go:   arr = append(arr, 4)
来源：http://spo.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://jfh.bbcook.cn

C#:   list.Add(4);
来源：http://rnd.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://kgt.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://bsp.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://stj.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ylq.uphjek.com


<!-- 参考信息 -->