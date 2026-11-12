代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vlv.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ciz.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zlu.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sai.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mqx.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mse.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hnx.redwolf501.top

[B04] for 计数循环
来源：http://iha.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://jvk.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icf.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbw.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aig.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sbb.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qeg.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://kcr.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zyc.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://pis.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://uye.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://awr.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gbu.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rlj.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xwd.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://udj.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://mfm.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://biw.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://ykh.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rex.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://obf.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwq.zdbjq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://azp.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hfh.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nkz.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://agv.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ybr.aibaodan.cn

[B07] while 循环
来源：http://hvs.epnwcf.com

Py:   while i < 10: i += 1
来源：http://wah.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mwe.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://zku.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://kki.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://kzc.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngb.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://vlj.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://sgt.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://iov.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://cio.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://owi.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://qlk.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://rth.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://flr.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zso.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://paj.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://rxa.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://ssi.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bml.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sbp.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://scl.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwh.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvy.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://liu.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://edp.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ito.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://xan.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jql.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vun.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rlx.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vuj.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://khs.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fvw.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lkw.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqs.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://jsl.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://dqn.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://ust.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zjf.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://log.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://auu.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://npv.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://khx.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fya.wangdashe.top

[B12] 跳出多层循环
来源：http://arx.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ins.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://rqd.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yxc.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://afw.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ryn.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qso.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lop.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bqj.dashuyun.cn

[B13] 判断是否为数字
来源：http://cct.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://rvd.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://nsq.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmj.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tzn.aizwys.cn

Java: x instanceof Number
来源：http://vkk.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kqu.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://jgd.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://hcy.hcnkem.com

[B14] 判断值是否在集合内
来源：http://ugq.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ouz.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://otj.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://wfw.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://mmx.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xyn.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yhu.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://bnn.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fpe.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://yqg.zhiwuduotai.top

Py:   a and b or not c
来源：http://lss.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://cme.fehbvm.com

JS:   a && b || !c
来源：http://ajn.sweek.top

TS:   a && b || !c
来源：http://zma.hesvh.cn

Java: a && b || !c
来源：http://wqi.xziqi.cn

Go:   a && b || !c
来源：http://syu.xuanzx.com

Ruby: a && b || !c
来源：http://kaf.jlsjyb.cn

C#:   a && b || !c
来源：http://gqd.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://sxr.tian-w.cn

Py:   if not data: return
来源：http://drn.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://lsp.shuidangran.top

JS:   if (!data) return;
来源：http://khm.sxryk.cn

TS:   if (!data) return;
来源：http://dqc.yangfankeji.com

Java: if (data == null) return;
来源：http://grr.hysaishi.cn

Go:   if data == nil { return }
来源：http://rry.fengsongda.top

Ruby: return if data.nil?
来源：http://ici.uphjek.com

C#:   if (data == null) return;
来源：http://ils.ydzc1.top

================================================================================
来源：http://ena.jiagoushi.top

C. 函数与作用域
来源：http://nry.aibaodan.cn

================================================================================
来源：http://zvh.hysaishi.cn

[C01] 定义函数
来源：http://yre.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://xss.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rie.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://zlt.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwq.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gff.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ktb.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://tfz.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lby.uphjek.com

[C02] 默认参数
来源：http://dow.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://jvs.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ejc.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fei.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fnm.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kxm.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vga.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://hks.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://xqc.sysykeji.top

[C03] 可变参数
来源：http://dti.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://mip.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mjd.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypr.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nym.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xpd.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hta.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jnx.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lzl.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://hur.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mcl.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://thf.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zlc.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kng.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://xyn.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://dda.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://gdz.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://got.hammf.cn

[C05] 返回多个值
来源：http://eiv.hongshengwenyu.top

Py:   return a, b
来源：http://vno.redwolf501.top

PHP:  return [$a, $b];
来源：http://vve.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ezu.cheryme.top

TS:   return { a, b };
来源：http://ata.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbu.shzxlz.cn

Go:   return a, b
来源：http://chj.cqqwz.cn

Ruby: return a, b
来源：http://jtg.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ddh.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://wtp.gzhubu.top

Py:   square = lambda x: x * x
来源：http://krs.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fhq.ybcxt.top

JS:   const square = x => x * x;
来源：http://ixl.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://mxx.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://byc.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://nlf.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://vbj.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://rwz.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://ihw.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yxb.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qyx.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://urk.shzxlz.cn

TS:   arr.map(String)
来源：http://xeo.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://plm.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eip.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://nhe.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ukm.hnxiangtu.top

[C08] 闭包
来源：http://wch.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qqe.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yzj.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qvt.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hef.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gdv.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ezc.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jha.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wdy.shzxlz.cn

[C09] 递归
来源：http://qon.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://luc.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hix.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://quy.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iue.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qtr.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vcl.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://civ.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jll.hnxiangtu.top

[C10] 变量作用域
来源：http://qxm.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ivr.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://chp.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yaa.hesvh.cn

TS:   同 JS
来源：http://wcl.ivvv.top

Java: 方法内为块级作用域
来源：http://aet.tarul.cn

Go:   花括号块级作用域
来源：http://pge.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tmf.0kj1m.cn

C#:   块级作用域
来源：http://jdf.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://nfb.316326.xyz

Py:   from module import func
来源：http://amv.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://drs.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qhv.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jje.haohaochexian.top

Java: import java.util.List;
来源：http://ant.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zko.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bau.guannengcc.top

C#:   using System.Text;
来源：http://hkp.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://jri.zhijiandao.cn

Py:   (lambda: print("run"))()
来源：http://zcd.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://ymz.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://luk.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://hze.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ynj.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://tye.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://ymi.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ohp.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://dmi.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aws.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbd.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yuz.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahb.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://zlw.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://gir.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://amz.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://gpc.feifeiyinyue.top

[C14] 泛型函数
来源：http://lbg.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yqu.jinqigfzy.top

PHP:  // 无泛型
来源：http://hcy.epnwcf.com

JS:   // 无泛型
来源：http://uqd.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ntt.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fco.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pmh.xinyue.icu

Ruby: # 无泛型
来源：http://ewf.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hho.mhx1999.top

[C15] 解构 / 展开参数
来源：http://srq.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bha.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://wwc.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aze.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hrf.wangdashe.top

Java: // 无解构
来源：http://zgu.redwolf501.top

Go:   // 无解构
来源：http://sbl.zhiwuduotai.top

Ruby: a, b = pair
来源：http://mnf.yvedp.cn

C#:   var (a, b) = pair;
来源：http://ted.andypj.xyz

[C16] 函数 / 方法重载
来源：http://gmp.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ltq.0kj1m.cn

PHP:  // 无重载
来源：http://dfb.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vac.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://xsv.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://hlw.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://lce.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://zku.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kvx.nanxinkj.top

================================================================================
来源：http://krj.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://hrm.yj20258.top

================================================================================
来源：http://jei.ydzc1.top

[D01] 创建数组 / 列表
来源：http://idh.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kwh.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ise.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yoi.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eto.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qiy.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://afh.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://mkd.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nrl.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://lvy.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ear.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tkc.sufxvd.cn

JS:   arr.push(4);
来源：http://hgp.sysykeji.top

TS:   arr.push(4);
来源：http://stj.sufxvd.cn

Java: list.add(4);
来源：http://qnt.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://rtb.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://xss.yfazqb.com

C#:   list.Add(4);
来源：http://tnx.xylfe.cn

[D03] 在指定位置插入元素
来源：http://uum.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://llo.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zgu.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uwl.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://lds.nanxuanxn.top

Java: list.add(0, 0);
来源：http://kqz.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rcd.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sbc.cheryme.top


<!-- 参考信息 -->