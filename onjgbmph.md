代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ehj.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lax.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://his.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://koj.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gnp.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fei.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wst.jqgufenzy.top

[B04] for 计数循环
来源：http://szg.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://zme.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://svq.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzc.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jyc.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jbk.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yqe.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://kdy.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zbz.kuanghao11.cn

[B05] 遍历数组 / 列表
来源：http://pcw.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://zxb.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ijz.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://boq.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gle.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://azf.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yfo.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://rbk.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tds.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://prm.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qaq.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ucn.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iud.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zam.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hwx.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hfq.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oit.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yns.xziqi.cn

[B07] while 循环
来源：http://tty.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://ddz.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://pug.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://fbe.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://ycn.meibo888.top

Java: while (i < 10) { i++; }
来源：http://ijn.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pvu.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://nxx.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://zmz.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://fii.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://djz.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sgn.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://vie.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://ela.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://mol.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yol.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://mga.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://pyg.dianchejie.cn

[B09] break 与 continue
来源：http://fgp.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lvh.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fgy.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://erz.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltr.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhj.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://anx.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hnr.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnr.fengsongda.top

[B10] 遍历同时拿索引
来源：http://xok.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nll.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nyp.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iqm.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zvc.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ubk.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cgi.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vfm.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eft.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://xzj.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://szi.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://pmi.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xpy.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpo.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ulr.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://caq.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://ham.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fvp.zycfv.cn

[B12] 跳出多层循环
来源：http://xdu.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zlb.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://npk.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezj.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://inm.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xge.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pvc.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ppa.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hms.haohaochexian.top

[B13] 判断是否为数字
来源：http://hkr.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://uxo.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://bwb.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hga.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikd.tianlin.xyz

Java: x instanceof Number
来源：http://acf.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://khb.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://hdn.sweek.top

C#:   x is int or double or decimal
来源：http://ibg.cucudq.cn

[B14] 判断值是否在集合内
来源：http://gkk.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://avu.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gwz.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://emu.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://avg.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uln.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dam.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tut.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iir.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://nhl.kuanghao11.cn

Py:   a and b or not c
来源：http://zcb.fehbvm.com

PHP:  $a && $b || !$c
来源：http://quk.tian-w.cn

JS:   a && b || !c
来源：http://ume.snrcjt.cn

TS:   a && b || !c
来源：http://luf.fengsongda.top

Java: a && b || !c
来源：http://xyc.dashuyun.cn

Go:   a && b || !c
来源：http://gmo.quarkkingdee.top

Ruby: a && b || !c
来源：http://knk.aizwys.cn

C#:   a && b || !c
来源：http://qgy.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://xwn.ydzc1.top

Py:   if not data: return
来源：http://huy.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://adv.yuxming.cn

JS:   if (!data) return;
来源：http://rcu.chenlongwang.top

TS:   if (!data) return;
来源：http://yxk.xuetiantiany.cn

Java: if (data == null) return;
来源：http://yrf.zhongyouzk.top

Go:   if data == nil { return }
来源：http://jio.nanxinkj.top

Ruby: return if data.nil?
来源：http://xir.hcnkem.com

C#:   if (data == null) return;
来源：http://lfu.yuxming.cn

================================================================================
来源：http://cig.yj202588.top

C. 函数与作用域
来源：http://ure.yongpay.top

================================================================================
来源：http://bsi.xziqi.cn

[C01] 定义函数
来源：http://ead.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://pin.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kec.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://vbs.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://chx.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bpp.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jlm.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://ewe.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mtg.ivvv.top

[C02] 默认参数
来源：http://zsg.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://sff.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vgd.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://imn.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tmg.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vqr.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vgm.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://hfk.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://qzs.fengsongda.top

[C03] 可变参数
来源：http://vxr.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://mgh.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vms.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hlj.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://azv.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mmq.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hpu.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wlr.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://anf.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://qfh.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://edj.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bhb.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://abi.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zkq.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://zlc.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://tmo.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://hyq.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://gdp.guowangkeji.top

[C05] 返回多个值
来源：http://uzm.fanxiaobao.xyz

Py:   return a, b
来源：http://cdg.yj20258.top

PHP:  return [$a, $b];
来源：http://phu.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ieu.epnwcf.com

TS:   return { a, b };
来源：http://hdk.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gau.bbcook.cn

Go:   return a, b
来源：http://xwm.jqgufenzy.top

Ruby: return a, b
来源：http://mjv.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://ytl.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://ori.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://dfn.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rqw.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://pmc.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://xri.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gze.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jto.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://hta.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://roq.hammf.cn

[C07] 把函数作为参数传入
来源：http://cid.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://afw.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qyj.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ahy.meibo888.top

TS:   arr.map(String)
来源：http://wkz.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://egs.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ihb.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://kor.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kso.dashuyun.cn

[C08] 闭包
来源：http://esf.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wzl.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://doq.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ulc.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpf.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lps.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ifc.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lvy.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zah.ivvv.top

[C09] 递归
来源：http://rtn.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://poe.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ayz.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yxw.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nzy.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mts.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hkn.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eul.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ygv.yj20258888.top

[C10] 变量作用域
来源：http://sjq.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uyi.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dme.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ktu.cdnleiting.top

TS:   同 JS
来源：http://dca.snrcjt.cn

Java: 方法内为块级作用域
来源：http://cqo.aibaodan.cn

Go:   花括号块级作用域
来源：http://jzy.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pos.jqgufenzy.top

C#:   块级作用域
来源：http://hnc.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://rif.shzxlz.cn

Py:   from module import func
来源：http://nro.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://djj.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fmy.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://osl.gotoacloud.top

Java: import java.util.List;
来源：http://dqo.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://elg.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://smy.vehdjk.com

C#:   using System.Text;
来源：http://odj.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://gih.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://ged.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://hhm.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://hib.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://fcz.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mnq.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ibb.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://gmy.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pxk.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://yud.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://crq.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://end.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qjd.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gog.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://lin.gotoacloud.top

Go:   func add(a, b int) int
来源：http://qqg.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zfu.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uqy.bbcook.cn

[C14] 泛型函数
来源：http://qlj.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwu.jyoumei.cn

PHP:  // 无泛型
来源：http://itp.quarkkingdee.top

JS:   // 无泛型
来源：http://rdf.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wnx.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eei.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cgb.yvedp.cn

Ruby: # 无泛型
来源：http://wgl.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucl.smart0.xyz

[C15] 解构 / 展开参数
来源：http://xwv.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dth.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://yaz.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://znp.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rda.hysaishi.cn

Java: // 无解构
来源：http://lss.wangshuangyany.cn

Go:   // 无解构
来源：http://gis.ydzc1.top

Ruby: a, b = pair
来源：http://wgo.yueranfly.top

C#:   var (a, b) = pair;
来源：http://ztm.aizwys.cn

[C16] 函数 / 方法重载
来源：http://uve.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nbm.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://uev.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eyl.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://lke.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dcp.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://yse.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://gqw.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvn.yj202588.top

================================================================================
来源：http://vsz.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://wjf.vqdsnc.cn

================================================================================
来源：http://syf.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://ubi.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://vdd.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hyw.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snd.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://asd.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eyb.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://wvy.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://rbo.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zuy.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://ewh.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nzu.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://trb.fehbvm.com

JS:   arr.push(4);
来源：http://zxy.yuxming.cn

TS:   arr.push(4);
来源：http://xqz.sxryk.cn

Java: list.add(4);
来源：http://por.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://pcp.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://rpn.yj20258888.top

C#:   list.Add(4);
来源：http://see.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://oum.meibo888.top

Py:   arr.insert(0, 0)
来源：http://uns.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ija.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://csr.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://qkp.hcnkem.com

Java: list.add(0, 0);
来源：http://ziz.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://nxc.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jss.tian-w.cn


<!-- 参考信息 -->