代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pug.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bcy.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tpv.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uad.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://izz.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cre.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fvh.guowangkeji.top

[B04] for 计数循环
来源：http://yxd.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://sma.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://enx.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rlp.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pzt.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zqm.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://txe.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://emr.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xdx.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://xif.sxryk.cn

Py:   for item in arr: print(item)
来源：http://csg.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bkt.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zih.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://onl.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zrs.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wmj.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://uyj.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pzl.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://ndb.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tzv.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wct.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgx.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czr.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kwv.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dso.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pue.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uxk.shzxlz.cn

[B07] while 循环
来源：http://gkk.yfazqb.com

Py:   while i < 10: i += 1
来源：http://lto.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ogz.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://vue.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://qjt.hammf.cn

Java: while (i < 10) { i++; }
来源：http://zab.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://knq.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://zlz.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://kzu.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://dnz.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://brz.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://hvd.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://kan.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://ssk.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://hav.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://azv.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://xoe.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://lek.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://ggo.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://opd.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eod.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asr.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cux.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmy.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eze.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ges.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odx.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://guh.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qci.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ezo.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ggf.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cjz.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kfw.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dbm.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rba.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jhm.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://meq.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://ihq.yonumen.top

PHP:  range(0, 10, 2);
来源：http://azo.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bga.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qik.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://opk.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hpv.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://jhn.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qyx.yangfankeji.com

[B12] 跳出多层循环
来源：http://xwk.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aib.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://btu.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://edf.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yiu.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iop.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://skd.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xuu.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://goa.xinyue.icu

[B13] 判断是否为数字
来源：http://vpl.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://scd.andypj.xyz

PHP:  is_numeric($x)
来源：http://kxf.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tat.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dqy.epnwcf.com

Java: x instanceof Number
来源：http://ztc.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ymd.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://shj.52xcode.cn

C#:   x is int or double or decimal
来源：http://doy.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://bvx.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://poz.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rnv.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://cro.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://urs.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kwn.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vri.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ceq.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wrz.epnwcf.com

[B15] 布尔运算与取反
来源：http://tnd.bjfxy.top

Py:   a and b or not c
来源：http://sqn.yuxming.cn

PHP:  $a && $b || !$c
来源：http://qep.mhx1999.top

JS:   a && b || !c
来源：http://lke.tian-w.cn

TS:   a && b || !c
来源：http://mdv.zhengqikj.top

Java: a && b || !c
来源：http://fvs.yj20258.top

Go:   a && b || !c
来源：http://xpb.aizwys.cn

Ruby: a && b || !c
来源：http://cwh.chenzaomai.com

C#:   a && b || !c
来源：http://jdw.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://lcf.epnwcf.com

Py:   if not data: return
来源：http://ale.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://lpt.yongpay.top

JS:   if (!data) return;
来源：http://klt.yuxming.cn

TS:   if (!data) return;
来源：http://dqr.316326.xyz

Java: if (data == null) return;
来源：http://raa.zhengqikj.top

Go:   if data == nil { return }
来源：http://jab.hammf.cn

Ruby: return if data.nil?
来源：http://ifl.hywenlv.cn

C#:   if (data == null) return;
来源：http://oov.cheryme.top

================================================================================
来源：http://utb.hfpthk.cn

C. 函数与作用域
来源：http://euo.jqgfzy.top

================================================================================
来源：http://ife.pengpengdd.cyou

[C01] 定义函数
来源：http://ppu.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://kih.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dhf.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://zzm.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqx.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xlc.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://irl.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://qkr.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wwv.bjfxy.top

[C02] 默认参数
来源：http://jle.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://kdu.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nzj.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://vgy.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tvz.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dcs.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pyn.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://jhv.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://hey.andypj.xyz

[C03] 可变参数
来源：http://fzx.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://vky.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ykv.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kub.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfj.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fsa.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fzr.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://ayo.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ppm.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://udk.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ngt.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ist.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qli.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://slr.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://bzr.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://xiw.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://rji.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://xxl.zhiwuduotai.top

[C05] 返回多个值
来源：http://ipr.zhengqikj.top

Py:   return a, b
来源：http://ivs.zycfv.cn

PHP:  return [$a, $b];
来源：http://aue.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nye.yfazqb.com

TS:   return { a, b };
来源：http://jaz.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kfs.ydjk.org.cn

Go:   return a, b
来源：http://yjv.pengpengdd.cyou

Ruby: return a, b
来源：http://pcy.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://qxo.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://amc.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://rlx.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://feq.316326.xyz

JS:   const square = x => x * x;
来源：http://bye.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://qmg.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bpw.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://omf.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://mwh.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mch.zycfv.cn

[C07] 把函数作为参数传入
来源：http://uko.zycfv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zmt.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pvs.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xzb.sweek.top

TS:   arr.map(String)
来源：http://chq.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cfh.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wpn.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://xgy.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://szh.yj20258888.top

[C08] 闭包
来源：http://cih.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zpp.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tke.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lwb.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ggx.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ldp.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rwz.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nif.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pny.zdqjudy.top

[C09] 递归
来源：http://xwt.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rrw.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zmt.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lki.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgf.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moa.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kmd.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bhj.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kyd.aizwys.cn

[C10] 变量作用域
来源：http://oru.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dku.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rrw.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vnw.jyoumei.cn

TS:   同 JS
来源：http://zzq.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://pro.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://luw.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lno.bbcook.cn

C#:   块级作用域
来源：http://xko.zycfv.cn

[C11] 模块导入与导出
来源：http://ndz.yuxming.cn

Py:   from module import func
来源：http://wwy.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zry.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://asj.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nwi.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://mnq.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sml.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://grr.zhengqikj.top

C#:   using System.Text;
来源：http://fxc.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://cvb.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://uuj.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://zts.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://ral.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://bkk.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ffh.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://nrw.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://ztq.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tuq.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://cbk.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://krv.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsf.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umb.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://raq.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oil.tianlin.xyz

Go:   func add(a, b int) int
来源：http://mfp.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qkf.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://rje.hongshengwenyu.top

[C14] 泛型函数
来源：http://xvl.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hty.guannengcc.top

PHP:  // 无泛型
来源：http://jwt.hesvh.cn

JS:   // 无泛型
来源：http://pdj.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kjl.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dmh.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fif.zhixingplan.top

Ruby: # 无泛型
来源：http://qzp.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jni.yfazqb.com

[C15] 解构 / 展开参数
来源：http://muh.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://myk.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://qpg.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bjy.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://slv.sysykeji.top

Java: // 无解构
来源：http://ucr.wangshuangyany.cn

Go:   // 无解构
来源：http://cwg.ydzc1.top

Ruby: a, b = pair
来源：http://uqo.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://gnt.yfazqb.com

[C16] 函数 / 方法重载
来源：http://juq.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jqu.hnxiangtu.top

PHP:  // 无重载
来源：http://zoq.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kkh.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://buk.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uzw.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://mpl.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://qdy.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sed.yanxiufei.cn

================================================================================
来源：http://juc.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://fpd.snrcjt.cn

================================================================================
来源：http://lnj.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://pje.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gpe.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drs.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://flz.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ncv.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jml.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://ote.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://inx.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hcd.gogol.net.cn

[D02] 追加元素到末尾
来源：http://pja.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hzg.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oiu.jqgufenzy.top

JS:   arr.push(4);
来源：http://ytr.hnqzz.top

TS:   arr.push(4);
来源：http://oou.hysaishi.cn

Java: list.add(4);
来源：http://fhc.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://hmp.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://qze.guowangkeji.top

C#:   list.Add(4);
来源：http://cby.ybcxt.top

[D03] 在指定位置插入元素
来源：http://uxv.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://gfm.nwbrower.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovu.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yqo.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://pcv.quarkkingdee.top

Java: list.add(0, 0);
来源：http://fji.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://rwy.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mof.daria6918.cn


<!-- 参考信息 -->