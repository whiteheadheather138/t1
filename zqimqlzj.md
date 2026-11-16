代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ekn.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wbb.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tso.daxiang520.top

[B04] for 计数循环
来源：http://wgt.shanyushiyangkeji.top

Py:   for i in range(10): print(i)
来源：http://eob.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://srr.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyi.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpi.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lbu.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rwr.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://ueh.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mfw.pycfn.com

[B05] 遍历数组 / 列表
来源：http://sxv.gzhubu.top

Py:   for item in arr: print(item)
来源：http://ncr.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ahu.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tic.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://itg.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wml.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bcc.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://oui.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://phm.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://mvw.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yic.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://new.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nit.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cps.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhi.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://clv.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oqn.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://idq.wangdashe.top

[B07] while 循环
来源：http://yba.cashguo.top

Py:   while i < 10: i += 1
来源：http://loc.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nyb.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://hla.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://xrz.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://ywa.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mhv.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://flt.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://ofu.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://djd.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://xol.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jtz.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://ocu.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://qnt.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://hcd.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://oef.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://zls.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://tqt.guannengcc.top

[B09] break 与 continue
来源：http://fei.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rrz.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pjg.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjq.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqg.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocw.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fni.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xfd.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://efx.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://lsi.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ozp.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ars.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kde.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oik.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://btb.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lpo.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xij.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tyl.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://gdt.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://okp.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://blr.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://glb.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kik.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bnx.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pnf.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://qyk.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vje.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://ilr.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mor.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pqi.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ekd.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffn.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sbb.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vmo.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dwr.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lyz.vqdsnc.cn

[B13] 判断是否为数字
来源：http://hfk.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://iba.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://ovn.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://spg.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sdo.zdbjq.cn

Java: x instanceof Number
来源：http://cxv.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://die.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://jcx.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://ccx.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://fff.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://apw.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qpx.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://pwe.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://osp.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cnj.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://muf.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://rge.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fgy.zhengqikj.top

[B15] 布尔运算与取反
来源：http://vbu.ehwqpu.com

Py:   a and b or not c
来源：http://miw.xylfe.cn

PHP:  $a && $b || !$c
来源：http://vlg.zhongyouzk.top

JS:   a && b || !c
来源：http://jlr.ydjk.org.cn

TS:   a && b || !c
来源：http://jvl.shzxlz.cn

Java: a && b || !c
来源：http://osu.feifeiyinyue.top

Go:   a && b || !c
来源：http://nwh.vqdsnc.cn

Ruby: a && b || !c
来源：http://xwc.bjfxy.top

C#:   a && b || !c
来源：http://zct.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://ksy.xuetiantiany.cn

Py:   if not data: return
来源：http://xyx.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://bbo.chenlongwang.top

JS:   if (!data) return;
来源：http://jgk.hysaishi.cn

TS:   if (!data) return;
来源：http://rsq.gotoacloud.top

Java: if (data == null) return;
来源：http://kxg.shuidangran.top

Go:   if data == nil { return }
来源：http://vfh.vqdsnc.cn

Ruby: return if data.nil?
来源：http://qag.cashguo.top

C#:   if (data == null) return;
来源：http://cef.shanyushiyangtech.top

================================================================================
来源：http://mov.iojbl.cn

C. 函数与作用域
来源：http://umv.daxiang520.top

================================================================================
来源：http://jrc.fanxiaobao.xyz

[C01] 定义函数
来源：http://mqd.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://uif.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qaa.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://iqm.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dvz.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jsq.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mes.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://klv.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tle.yongpay.top

[C02] 默认参数
来源：http://hdk.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://pza.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mzd.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://qbj.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yqr.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ton.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://npc.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://oht.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://epy.xziqi.cn

[C03] 可变参数
来源：http://zed.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://ifo.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xzw.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sng.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pyx.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uct.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pyj.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://zuc.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eic.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://mba.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ohb.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hkw.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://udd.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mux.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://dgm.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://lrb.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://qbb.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://juk.hywenlv.cn

[C05] 返回多个值
来源：http://ibv.snrcjt.cn

Py:   return a, b
来源：http://vgi.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://osr.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pwu.aibaodan.cn

TS:   return { a, b };
来源：http://zso.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qyk.cheryme.top

Go:   return a, b
来源：http://jlq.ehwqpu.com

Ruby: return a, b
来源：http://zkf.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vhd.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://tdj.fehbvm.com

Py:   square = lambda x: x * x
来源：http://gro.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nsb.dianchejie.cn

JS:   const square = x => x * x;
来源：http://ara.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://kme.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tcw.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ylb.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://pfx.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ovz.hnqzz.top

[C07] 把函数作为参数传入
来源：http://cct.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uhk.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xmj.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wat.yanxiufei.cn

TS:   arr.map(String)
来源：http://lzx.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bor.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kbl.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://pka.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fmy.jinyuanbaomall.cn

[C08] 闭包
来源：http://pbo.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vrc.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://umd.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lkd.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pko.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gca.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dye.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://plv.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eew.cheryme.top

[C09] 递归
来源：http://tke.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yju.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mli.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hef.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgt.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hve.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pnj.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhw.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vlz.yuanzhike.top

[C10] 变量作用域
来源：http://oua.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mzn.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hfj.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cgl.shanyushiyangtech.top

TS:   同 JS
来源：http://rbk.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://lwk.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://rsz.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uuj.guannengcc.top

C#:   块级作用域
来源：http://dnd.yj20258888.top

[C11] 模块导入与导出
来源：http://jlj.fanxiaobao.xyz

Py:   from module import func
来源：http://syd.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xxx.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ikr.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhw.chenlongwang.top

Java: import java.util.List;
来源：http://hka.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lvw.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://seb.shangyingyoupin.top

C#:   using System.Text;
来源：http://swt.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://wva.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://ufi.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://zbh.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://fgw.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://vhi.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tqz.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://muw.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://xwe.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://auu.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://qsm.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqe.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oms.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yhg.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aiy.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://uct.hfpthk.cn

Go:   func add(a, b int) int
来源：http://evn.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qdd.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://czj.jinqigfzy.top

[C14] 泛型函数
来源：http://kkv.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eys.haohaochexian.top

PHP:  // 无泛型
来源：http://opd.epnwcf.com

JS:   // 无泛型
来源：http://xjc.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://con.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://osr.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://evt.xuetiantiany.cn

Ruby: # 无泛型
来源：http://hsd.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dej.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://mve.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xgx.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://ktw.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ogl.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yye.bjfxy.top

Java: // 无解构
来源：http://fas.cucudq.cn

Go:   // 无解构
来源：http://tye.jiagoushi.top

Ruby: a, b = pair
来源：http://ppt.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://bix.ybcxt.top

[C16] 函数 / 方法重载
来源：http://bke.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://err.jyoumei.cn

PHP:  // 无重载
来源：http://zfi.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tyj.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://hwv.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://woi.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://vcj.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://goa.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://txx.shangyingyoupin.top

================================================================================
来源：http://gcv.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://xvn.yuxming.cn

================================================================================
来源：http://jqf.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://wuw.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://spm.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sii.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vhb.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qaz.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pkv.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://ebl.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://pug.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pbm.cucudq.cn

[D02] 追加元素到末尾
来源：http://ddq.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zzb.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tjs.cucudq.cn

JS:   arr.push(4);
来源：http://nax.zycfv.cn

TS:   arr.push(4);
来源：http://boj.yanxiufei.cn

Java: list.add(4);
来源：http://fxf.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://tqt.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://swe.bbcook.cn

C#:   list.Add(4);
来源：http://ulh.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://dkd.yonumen.top

Py:   arr.insert(0, 0)
来源：http://gmz.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mgb.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sap.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://jok.ctjpmb.com

Java: list.add(0, 0);
来源：http://zjq.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ktr.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xgb.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://kck.bjfxy.top

[D04] 删除元素
来源：http://omj.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lwy.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lhr.jianghu66.top


<!-- 参考信息 -->