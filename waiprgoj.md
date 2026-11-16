代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cge.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://whw.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hdn.sweek.top

[B04] for 计数循环
来源：http://kfu.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://ldf.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://btt.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iok.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqh.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uho.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lml.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://ark.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mny.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://mrp.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://iyc.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsn.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ylr.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://krr.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bxh.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jhh.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://ffi.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://toe.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://lww.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qcp.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ctg.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rap.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qvj.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jfk.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wgf.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fxz.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rzr.redwolf501.top

[B07] while 循环
来源：http://uiv.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://tpv.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ypj.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://fqq.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://imf.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://qwm.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nrl.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://ick.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://phs.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://tuj.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://ldd.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ndj.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://cnc.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://hll.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://ctz.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qjo.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://wtz.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://act.fktsv.cn

[B09] break 与 continue
来源：http://xkk.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ext.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://skr.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsm.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdp.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cev.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bkm.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tor.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tat.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://jqe.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ppi.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://log.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pnu.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sqe.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ckp.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mmy.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rgb.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://das.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://vrf.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://yan.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://cxh.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydf.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omy.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lqz.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vgj.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://poy.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yhu.xinyue.icu

[B12] 跳出多层循环
来源：http://viu.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mue.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vpz.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvu.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zov.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://odz.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xin.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gxi.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mpx.vqdsnc.cn

[B13] 判断是否为数字
来源：http://yhr.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://bci.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://vmh.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pim.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqb.yueranfly.top

Java: x instanceof Number
来源：http://kjt.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aki.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://gta.smart0.xyz

C#:   x is int or double or decimal
来源：http://pae.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://uao.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://klx.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qun.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qou.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://myz.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://pwl.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ite.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://cyk.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mne.fengsongda.top

[B15] 布尔运算与取反
来源：http://fyi.nwbrower.top

Py:   a and b or not c
来源：http://vlp.havefunace.top

PHP:  $a && $b || !$c
来源：http://fvk.yj20258888.top

JS:   a && b || !c
来源：http://sgd.birdmap.top

TS:   a && b || !c
来源：http://oix.haohaochexian.top

Java: a && b || !c
来源：http://kti.snrcjt.cn

Go:   a && b || !c
来源：http://zyw.xuanzx.com

Ruby: a && b || !c
来源：http://ofa.sysykeji.top

C#:   a && b || !c
来源：http://pnz.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://acv.guowangkeji.top

Py:   if not data: return
来源：http://tpj.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://xjy.ydzc1.top

JS:   if (!data) return;
来源：http://sxt.cqqwz.cn

TS:   if (!data) return;
来源：http://yjm.fktsv.cn

Java: if (data == null) return;
来源：http://wid.svipenyu.cn

Go:   if data == nil { return }
来源：http://poj.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://wkw.jqgfzy.top

C#:   if (data == null) return;
来源：http://vsf.xuetiantiany.cn

================================================================================
来源：http://xbd.tanke756.top

C. 函数与作用域
来源：http://wid.jianghu66.top

================================================================================
来源：http://bct.ydzc1.top

[C01] 定义函数
来源：http://uzk.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://ujl.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxe.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://akf.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqp.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://atd.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xco.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://smd.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uur.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://wsz.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://fvj.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://pfx.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://ten.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xoc.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bxc.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lmx.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://nvq.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://vqo.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://gcp.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://yer.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vom.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://otc.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uce.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kfq.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nuq.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://wtm.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zqo.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://dnz.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hmc.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wpm.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qpe.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wxg.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://zdd.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://paj.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://mof.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://okw.guowangkeji.top

[C05] 返回多个值
来源：http://xkc.wangshuangyany.cn

Py:   return a, b
来源：http://etb.yueranfly.top

PHP:  return [$a, $b];
来源：http://zjc.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wry.xuetiantiany.cn

TS:   return { a, b };
来源：http://qjy.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dwo.nanxuanxn.top

Go:   return a, b
来源：http://wzw.cheryme.top

Ruby: return a, b
来源：http://zvp.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ujc.sweek.top

[C06] 匿名函数 / lambda
来源：http://myx.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://zjf.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://srf.xziqi.cn

JS:   const square = x => x * x;
来源：http://gev.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ixk.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fir.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://kdx.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://hlx.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://max.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://kya.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://opi.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://znt.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eog.vehdjk.com

TS:   arr.map(String)
来源：http://vcn.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zse.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dfw.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://ruv.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mst.tianlin.xyz

[C08] 闭包
来源：http://ctd.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gnd.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vsr.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jhr.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tpt.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vxx.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gcj.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://edm.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cbj.yj202588.top

[C09] 递归
来源：http://yyi.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://myf.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddj.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvc.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qci.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ryq.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vyu.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jze.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tlz.birdmap.top

[C10] 变量作用域
来源：http://vyt.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nmk.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fqp.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zjs.aizwys.cn

TS:   同 JS
来源：http://otc.hammf.cn

Java: 方法内为块级作用域
来源：http://rpu.zycfv.cn

Go:   花括号块级作用域
来源：http://fjq.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jxv.hnqzz.top

C#:   块级作用域
来源：http://rge.vehdjk.com

[C11] 模块导入与导出
来源：http://wai.sysykeji.top

Py:   from module import func
来源：http://sob.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dxv.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vtr.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfh.aizwys.cn

Java: import java.util.List;
来源：http://wfd.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tll.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://gnn.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://xvr.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://ytm.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://ntt.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://fmh.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://bqv.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://pzs.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cry.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://jed.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://nhs.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pmm.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://oek.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hcz.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://svt.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yzc.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://enn.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://ftp.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://dll.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xiw.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://vxf.0kj1m.cn

[C14] 泛型函数
来源：http://fbr.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yel.chenlongwang.top

PHP:  // 无泛型
来源：http://lvn.c1oappe.top

JS:   // 无泛型
来源：http://upb.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://svq.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zyp.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pcz.chenjidiqi.icu

Ruby: # 无泛型
来源：http://wbn.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vve.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://hob.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvb.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ayk.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zub.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dpv.hammf.cn

Java: // 无解构
来源：http://dxg.yj202588.top

Go:   // 无解构
来源：http://vex.sxryk.cn

Ruby: a, b = pair
来源：http://ydz.jianghu66.top

C#:   var (a, b) = pair;
来源：http://dei.aizwys.cn

[C16] 函数 / 方法重载
来源：http://nyh.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ytp.zhiwuduotai.top

PHP:  // 无重载
来源：http://yjz.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gqx.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://ebf.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wqi.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://aad.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://qha.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gaz.snrcjt.cn

================================================================================
来源：http://ipg.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://acx.pycfn.com

================================================================================
来源：http://fos.hammf.cn

[D01] 创建数组 / 列表
来源：http://rxr.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cvi.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eeb.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hfh.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://agv.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tva.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://hes.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://goi.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kfn.yonumen.top

[D02] 追加元素到末尾
来源：http://oft.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://thc.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gks.ppjwa.cn

JS:   arr.push(4);
来源：http://prv.zhixingplan.top

TS:   arr.push(4);
来源：http://xbi.yueranfly.top

Java: list.add(4);
来源：http://dwh.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://cjb.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://woc.daria6918.cn

C#:   list.Add(4);
来源：http://qfk.pycfn.com

[D03] 在指定位置插入元素
来源：http://gfl.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://bxg.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://klc.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uxj.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://hfm.sweek.top

Java: list.add(0, 0);
来源：http://jij.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qqy.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ixf.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://ouc.svipenyu.cn

[D04] 删除元素
来源：http://icc.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://grf.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aso.hesvh.cn


<!-- 参考信息 -->