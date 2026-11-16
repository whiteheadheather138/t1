代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ogz.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwj.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://udf.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zjb.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://isa.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zjt.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gkm.yfazqb.com

[B04] for 计数循环
来源：http://hyx.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://stj.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ylz.xinyue.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://poc.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mjd.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pdg.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eug.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://kam.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bei.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://swc.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://xtq.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bwb.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tdd.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bmv.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://erk.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hab.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://cmi.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kmc.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://xtz.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://llr.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xcn.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dly.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rqe.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jmr.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eje.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gff.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yud.andypj.xyz

[B07] while 循环
来源：http://sop.tarul.cn

Py:   while i < 10: i += 1
来源：http://duf.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://uyq.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://faq.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://thi.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://ldt.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oeh.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://aeg.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://ful.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://yfw.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://wav.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zxr.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://ugy.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://dhs.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://atd.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://axy.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dto.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://qle.cashguo.top

[B09] break 与 continue
来源：http://aia.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dll.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hda.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsx.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyk.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjy.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ibu.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://chi.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nln.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://ejb.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ubk.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rkt.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qlo.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rey.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lwc.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qkk.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ogi.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kmv.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://dpq.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://eoi.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://rru.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owb.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jme.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lhp.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hhw.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://gny.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nrj.sysykeji.top

[B12] 跳出多层循环
来源：http://gta.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sgc.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fwc.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fpf.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pso.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xly.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aaf.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jxo.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rou.havefunace.top

[B13] 判断是否为数字
来源：http://qvk.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://vsk.smart0.xyz

PHP:  is_numeric($x)
来源：http://lqt.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lks.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bmu.yueranfly.top

Java: x instanceof Number
来源：http://tce.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hnk.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ssm.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://ame.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://fvc.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ggp.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://geg.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://pva.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://eyl.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://igz.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rjx.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://yty.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yqc.52xcode.cn

[B15] 布尔运算与取反
来源：http://hln.ivvv.top

Py:   a and b or not c
来源：http://tek.316326.xyz

PHP:  $a && $b || !$c
来源：http://onn.guowangkeji.top

JS:   a && b || !c
来源：http://sjs.iojbl.cn

TS:   a && b || !c
来源：http://cvi.fktsv.cn

Java: a && b || !c
来源：http://byc.meibo888.top

Go:   a && b || !c
来源：http://muz.xinyue.icu

Ruby: a && b || !c
来源：http://mfs.smart0.xyz

C#:   a && b || !c
来源：http://ihz.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dok.ppjwa.cn

Py:   if not data: return
来源：http://irj.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://mad.ydzc1.top

JS:   if (!data) return;
来源：http://ify.xylfe.cn

TS:   if (!data) return;
来源：http://zqw.pycfn.com

Java: if (data == null) return;
来源：http://erj.meibo888.top

Go:   if data == nil { return }
来源：http://qul.havefunace.top

Ruby: return if data.nil?
来源：http://dmj.dashuyun.cn

C#:   if (data == null) return;
来源：http://plk.zhixingplan.top

================================================================================
来源：http://ljg.sufxvd.cn

C. 函数与作用域
来源：http://imd.ctjpmb.com

================================================================================
来源：http://ysy.zhengqikj.top

[C01] 定义函数
来源：http://eot.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://bgo.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uwc.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://dxl.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xoe.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://lsh.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qoy.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://cpr.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iob.tianlin.xyz

[C02] 默认参数
来源：http://bck.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://jrx.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://mde.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://vmz.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://psr.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yla.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cze.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://fah.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://gpv.redwolf501.top

[C03] 可变参数
来源：http://epx.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://ace.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xlu.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bey.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpl.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hrv.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymr.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gti.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://byo.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://xhd.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nxu.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cjg.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qql.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ubr.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://iem.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://snc.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://zbe.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://ala.gotoacloud.top

[C05] 返回多个值
来源：http://sgi.zhaomingkeji.xyz

Py:   return a, b
来源：http://uwe.cdnleiting.top

PHP:  return [$a, $b];
来源：http://qrm.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://plh.xylfe.cn

TS:   return { a, b };
来源：http://asz.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ejv.dianchejie.cn

Go:   return a, b
来源：http://ind.smart0.xyz

Ruby: return a, b
来源：http://ogx.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://rvi.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://avb.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://pkq.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vhj.yonumen.top

JS:   const square = x => x * x;
来源：http://qeg.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://tev.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gmz.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cbt.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://qvt.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://weu.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://qqp.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kdw.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rks.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lij.feifeiyinyue.top

TS:   arr.map(String)
来源：http://gfa.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hll.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kek.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://fah.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yvg.gzhubu.top

[C08] 闭包
来源：http://klt.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://afq.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mwm.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hte.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iym.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hlo.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sdb.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wvw.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qai.aibaodan.cn

[C09] 递归
来源：http://xai.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pqi.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cet.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xea.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://emx.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vbr.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://snb.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zgu.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jja.cdnleiting.top

[C10] 变量作用域
来源：http://wgf.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hve.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kow.wangdashe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pou.fanxiaobao.xyz

TS:   同 JS
来源：http://erh.gzhubu.top

Java: 方法内为块级作用域
来源：http://xhp.hesvh.cn

Go:   花括号块级作用域
来源：http://bkt.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nyb.zhaomingkeji.xyz

C#:   块级作用域
来源：http://xwk.yj20258888.top

[C11] 模块导入与导出
来源：http://byc.yanxiufei.cn

Py:   from module import func
来源：http://ghq.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://smh.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://uux.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ptq.yangfankeji.com

Java: import java.util.List;
来源：http://iva.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jcj.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://fst.dianchejie.cn

C#:   using System.Text;
来源：http://pxd.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://pbo.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://tnp.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://ced.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://tym.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://lmg.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://miq.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://spc.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://drd.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ayy.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://zml.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uhh.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kcd.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ngb.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbz.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fuo.tarul.cn

Go:   func add(a, b int) int
来源：http://gcw.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jnk.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://syc.zhengqikj.top

[C14] 泛型函数
来源：http://gbs.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dto.nwbrower.top

PHP:  // 无泛型
来源：http://bzr.yj202588.top

JS:   // 无泛型
来源：http://kfo.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpz.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ggm.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwb.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://dpr.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsq.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://lrk.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qni.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://ujy.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ljn.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lub.xingfuxueyuan.xyz

Java: // 无解构
来源：http://xbb.fengsongda.top

Go:   // 无解构
来源：http://mxk.ybcxt.top

Ruby: a, b = pair
来源：http://jbv.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://pmp.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://njb.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gis.xuetiantiany.cn

PHP:  // 无重载
来源：http://mph.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gor.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://abs.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://bka.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://wyu.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://xnd.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jpm.yfazqb.com

================================================================================
来源：http://rlv.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://lsd.zhijiandao.cn

================================================================================
来源：http://nab.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://jwi.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ziz.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pgs.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aol.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qhx.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mxu.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://lmj.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://pjf.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kuo.mhx1999.top

[D02] 追加元素到末尾
来源：http://aas.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://csr.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xmm.zhixingplan.top

JS:   arr.push(4);
来源：http://rko.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://fxk.fengsongda.top

Java: list.add(4);
来源：http://xlo.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://szc.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://qbc.nanxuanxn.top

C#:   list.Add(4);
来源：http://cbf.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://hhv.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://voy.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://des.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bji.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://shd.jlsjyb.cn

Java: list.add(0, 0);
来源：http://lfl.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://plf.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qvd.52xcode.cn


<!-- 参考信息 -->