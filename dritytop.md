代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://whf.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uba.hfpthk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fpg.chenzaomai.com

[B04] for 计数循环
来源：http://gcj.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://dwn.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://noh.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unn.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xwi.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mdw.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hfh.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://ees.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljk.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://nbj.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://fgs.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://avj.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://esb.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hir.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cpt.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mfl.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://wyx.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bol.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://ooj.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tko.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nue.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fan.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qou.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wca.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://olt.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bwc.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bjh.hnxiangtu.top

[B07] while 循环
来源：http://pzj.jianghu66.top

Py:   while i < 10: i += 1
来源：http://ngd.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xcv.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://pai.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://vam.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://laa.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fej.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://fdz.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://dye.cheryme.top

[B08] do-while（至少执行一次）
来源：http://qjr.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://udo.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://who.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://ata.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://tch.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://svi.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ilc.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bvb.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://usl.hammf.cn

[B09] break 与 continue
来源：http://mwu.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://roy.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sjq.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oda.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdd.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsg.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://skz.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://who.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jny.epnwcf.com

[B10] 遍历同时拿索引
来源：http://uiu.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fxs.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kra.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tpu.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://btj.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yjr.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kjv.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tjo.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ogs.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://fvb.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://dwa.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://syf.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltg.jlsjyb.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uvi.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mnb.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kap.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://hlm.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxh.daxiang520.top

[B12] 跳出多层循环
来源：http://qwj.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://axw.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hmh.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofu.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rlj.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kyu.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mvq.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pcg.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ntb.yvedp.cn

[B13] 判断是否为数字
来源：http://ozw.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://ylu.sweek.top

PHP:  is_numeric($x)
来源：http://guf.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://njz.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://npw.zhiwuduotai.top

Java: x instanceof Number
来源：http://nyr.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://njf.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://vzz.yfazqb.com

C#:   x is int or double or decimal
来源：http://mis.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://nzc.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://myh.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://olp.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://ikr.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://nyg.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://liy.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ggm.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://byk.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xsv.sweek.top

[B15] 布尔运算与取反
来源：http://qpp.ppjwa.cn

Py:   a and b or not c
来源：http://htf.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://tva.dashuyun.cn

JS:   a && b || !c
来源：http://sky.fanxiaobao.xyz

TS:   a && b || !c
来源：http://mzn.cheryme.top

Java: a && b || !c
来源：http://qbf.ppjwa.cn

Go:   a && b || !c
来源：http://osf.bjfxy.top

Ruby: a && b || !c
来源：http://vjb.jinqigfzy.top

C#:   a && b || !c
来源：http://lpo.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://tej.ppjwa.cn

Py:   if not data: return
来源：http://qyn.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://uxk.hywenlv.cn

JS:   if (!data) return;
来源：http://xgo.feifeiyinyue.top

TS:   if (!data) return;
来源：http://eyz.nwbrower.top

Java: if (data == null) return;
来源：http://yox.9152youxi.cn

Go:   if data == nil { return }
来源：http://khe.vehdjk.com

Ruby: return if data.nil?
来源：http://twa.zhongyouzk.top

C#:   if (data == null) return;
来源：http://hsk.zycfv.cn

================================================================================
来源：http://oiu.nanxinkj.top

C. 函数与作用域
来源：http://onb.fehbvm.com

================================================================================
来源：http://jfp.fehbvm.com

[C01] 定义函数
来源：http://qau.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://ocs.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdu.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://buj.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://biu.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nvd.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://kse.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://lkc.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rhu.hcnkem.com

[C02] 默认参数
来源：http://yoi.birdmap.top

Py:   def greet(name="World"): return name
来源：http://eho.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aen.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://qqd.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://etf.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gzs.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lij.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://uhp.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://zvf.yvedp.cn

[C03] 可变参数
来源：http://pnf.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://sbc.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qci.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbk.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dlr.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nqr.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://npt.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://izg.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://deh.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://mex.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lxo.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cio.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://roi.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qfo.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://fal.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://wgk.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://con.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://pga.jinqigfzy.top

[C05] 返回多个值
来源：http://rdn.cucudq.cn

Py:   return a, b
来源：http://pcu.pycfn.com

PHP:  return [$a, $b];
来源：http://zyd.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jcp.guannengcc.top

TS:   return { a, b };
来源：http://qgx.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ydi.gotoacloud.top

Go:   return a, b
来源：http://pdz.ivvv.top

Ruby: return a, b
来源：http://wni.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://iek.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://dmt.316326.xyz

Py:   square = lambda x: x * x
来源：http://giw.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kjz.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://tjh.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://cry.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uqd.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://vla.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://fev.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ehl.tian-w.cn

[C07] 把函数作为参数传入
来源：http://qzn.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wpn.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://trj.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://thx.c1oappe.top

TS:   arr.map(String)
来源：http://shv.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fdf.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fwi.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://oyv.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dpt.fktsv.cn

[C08] 闭包
来源：http://jya.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fxh.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fri.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lca.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xgr.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xfx.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dnd.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zjf.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gyz.zhoulong.xyz

[C09] 递归
来源：http://oju.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lit.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bbc.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://plc.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lzd.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://quo.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fii.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dds.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sgc.zhengqikj.top

[C10] 变量作用域
来源：http://jon.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://npv.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://olk.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://omd.guannengcc.top

TS:   同 JS
来源：http://gjz.yueranfly.top

Java: 方法内为块级作用域
来源：http://aab.52xcode.cn

Go:   花括号块级作用域
来源：http://gxz.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cng.xuetiantiany.cn

C#:   块级作用域
来源：http://ojq.c1oappe.top

[C11] 模块导入与导出
来源：http://uyy.hfpthk.cn

Py:   from module import func
来源：http://szt.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hkl.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zjk.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vhr.ydzc1.top

Java: import java.util.List;
来源：http://sdd.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hva.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://tgt.c1oappe.top

C#:   using System.Text;
来源：http://amn.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://jus.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://lwb.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://jyp.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://jav.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://qtv.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ouq.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://qzl.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://eqx.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hfx.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://qyz.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mcs.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmb.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://opx.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mnc.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qrq.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://ixl.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eka.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://acm.xinyue.icu

[C14] 泛型函数
来源：http://ckc.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nzq.uphjek.com

PHP:  // 无泛型
来源：http://fna.fengsongda.top

JS:   // 无泛型
来源：http://eew.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://urs.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bhq.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fss.bjfxy.top

Ruby: # 无泛型
来源：http://whp.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zai.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://byo.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qrs.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://iwd.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jfl.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://beg.cucudq.cn

Java: // 无解构
来源：http://wpv.yvedp.cn

Go:   // 无解构
来源：http://ltq.fengsongda.top

Ruby: a, b = pair
来源：http://aqq.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://hsa.yj20258.top

[C16] 函数 / 方法重载
来源：http://tru.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yyx.daria6918.cn

PHP:  // 无重载
来源：http://enx.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://azy.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://qgv.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nmm.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://vjz.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://xwy.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccg.kuanghao11.cn

================================================================================
来源：http://hle.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://wep.zycfv.cn

================================================================================
来源：http://yrm.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://zwr.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vxm.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cdy.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fsz.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gzr.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uat.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://rdv.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://vbs.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xht.meibo888.top

[D02] 追加元素到末尾
来源：http://wqa.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ykx.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tvp.pycfn.com

JS:   arr.push(4);
来源：http://vnn.yongpay.top

TS:   arr.push(4);
来源：http://fhr.vehdjk.com

Java: list.add(4);
来源：http://nfx.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://xht.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://qgw.tanke756.top

C#:   list.Add(4);
来源：http://ams.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://yed.uphjek.com

Py:   arr.insert(0, 0)
来源：http://pag.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bbc.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xtk.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://wcy.kuanghao11.cn

Java: list.add(0, 0);
来源：http://qdv.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://soj.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cki.tanke756.top

C#:   list.Insert(0, 0);
来源：http://nwu.cqqwz.cn

[D04] 删除元素
来源：http://zuc.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gza.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dkv.kuanghao11.cn


<!-- 参考信息 -->