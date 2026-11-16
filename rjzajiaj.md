代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kvu.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lnm.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nja.ctjpmb.com

[B04] for 计数循环
来源：http://hey.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://yuc.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://efy.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eqy.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aul.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xoq.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qjg.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://six.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vuv.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://ihv.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://usr.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rzt.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://joh.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xiq.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jir.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rla.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://ypt.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://chj.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://xii.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xhb.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pgh.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pip.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://izd.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bjj.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dbu.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dxw.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwl.fehbvm.com

[B07] while 循环
来源：http://nvi.shuidangran.top

Py:   while i < 10: i += 1
来源：http://csi.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://yar.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://brz.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://cve.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://uxc.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fzk.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://ejm.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://aqn.cashguo.top

[B08] do-while（至少执行一次）
来源：http://uok.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://tmo.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gwa.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://pzg.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://nei.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://yan.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wrg.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://doi.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://fbq.yueranfly.top

[B09] break 与 continue
来源：http://pqb.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zjj.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kue.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxt.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ceh.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uiz.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eko.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bow.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jic.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://fwl.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bwi.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vye.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xah.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eiu.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ebg.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qnz.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tqx.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://whg.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://rxz.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://vnm.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://uhe.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vcv.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twy.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xcs.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bqz.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://cqj.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ijo.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://ooj.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vhx.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sos.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qfs.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fzn.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sle.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tjl.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hii.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://htf.kuanghao11.cn

[B13] 判断是否为数字
来源：http://bdg.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://rsq.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://ueh.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sdr.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vto.guowangkeji.top

Java: x instanceof Number
来源：http://kgc.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://osu.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://dip.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://uwh.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://zub.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uvf.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ufg.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://pnm.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://xyk.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vud.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pbs.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://swt.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://krp.ppjwa.cn

[B15] 布尔运算与取反
来源：http://zqf.zhongyouzk.top

Py:   a and b or not c
来源：http://bjz.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://vjm.jiagoushi.top

JS:   a && b || !c
来源：http://lmq.pycfn.com

TS:   a && b || !c
来源：http://dgd.jqgfzy.top

Java: a && b || !c
来源：http://efh.yj20258888.top

Go:   a && b || !c
来源：http://lqt.hnxiangtu.top

Ruby: a && b || !c
来源：http://chx.tarul.cn

C#:   a && b || !c
来源：http://apf.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://gbi.jinyuanbaomall.cn

Py:   if not data: return
来源：http://otc.yj202588.top

PHP:  if (!$data) { return; }
来源：http://zin.tanke756.top

JS:   if (!data) return;
来源：http://uoy.yangfankeji.com

TS:   if (!data) return;
来源：http://zjp.hfpthk.cn

Java: if (data == null) return;
来源：http://iui.xylfe.cn

Go:   if data == nil { return }
来源：http://cpm.ydjk.org.cn

Ruby: return if data.nil?
来源：http://kap.yj202588.top

C#:   if (data == null) return;
来源：http://ule.sjlbkw.cn

================================================================================
来源：http://hzz.bbcook.cn

C. 函数与作用域
来源：http://srh.yuanzhike.top

================================================================================
来源：http://wkp.svipenyu.cn

[C01] 定义函数
来源：http://sta.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://vya.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ffx.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://iip.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjv.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://yjk.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://wgx.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://fqy.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wjy.yueranfly.top

[C02] 默认参数
来源：http://kce.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://yct.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bpy.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://hlv.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://jyx.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tto.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpa.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://ojq.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://cte.hammf.cn

[C03] 可变参数
来源：http://sxr.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://lbi.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hrf.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzq.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://osn.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bmy.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aui.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rin.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pip.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://wvp.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tno.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yqh.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rpu.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kuy.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://wua.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://brz.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://ujg.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://vab.hnxiangtu.top

[C05] 返回多个值
来源：http://typ.gogol.net.cn

Py:   return a, b
来源：http://zeo.ybcxt.top

PHP:  return [$a, $b];
来源：http://zra.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uoh.meibo888.top

TS:   return { a, b };
来源：http://npz.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ppr.fanxiaobao.xyz

Go:   return a, b
来源：http://yaw.zhoulong.xyz

Ruby: return a, b
来源：http://ppo.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://squ.sweek.top

[C06] 匿名函数 / lambda
来源：http://tai.gzhubu.top

Py:   square = lambda x: x * x
来源：http://ylo.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uuy.xylfe.cn

JS:   const square = x => x * x;
来源：http://tbt.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://slj.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zki.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://utm.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://eyv.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://snf.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://qsa.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nta.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://gwn.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ciu.yj20258.top

TS:   arr.map(String)
来源：http://ook.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gbx.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jcm.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://oni.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qfc.yueranfly.top

[C08] 闭包
来源：http://ksy.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jit.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nze.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hdb.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cko.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bjp.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wtl.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ace.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sug.kuanghao11.cn

[C09] 递归
来源：http://mmx.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dij.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rqi.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aof.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqn.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wsy.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://goo.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ade.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ocg.hesvh.cn

[C10] 变量作用域
来源：http://mak.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jcd.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://psc.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mum.gotoacloud.top

TS:   同 JS
来源：http://woo.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://yaq.sufxvd.cn

Go:   花括号块级作用域
来源：http://fal.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jab.hnqzz.top

C#:   块级作用域
来源：http://jiu.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://wkl.aibaodan.cn

Py:   from module import func
来源：http://pka.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ujk.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bot.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uqx.cqqwz.cn

Java: import java.util.List;
来源：http://nnv.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eow.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://dsx.gaohongyu789.top

C#:   using System.Text;
来源：http://udu.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://cqm.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://ozd.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://zic.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://urq.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://bwu.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zih.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://iug.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://qkr.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://run.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://jpe.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jdi.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inh.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bvh.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fsi.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://qzt.daria6918.cn

Go:   func add(a, b int) int
来源：http://pkt.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xje.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hqz.ydjk.org.cn

[C14] 泛型函数
来源：http://jnx.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wiz.mhx1999.top

PHP:  // 无泛型
来源：http://wzu.daxiang520.top

JS:   // 无泛型
来源：http://uca.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nhr.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ygc.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jli.chenlongwang.top

Ruby: # 无泛型
来源：http://lrd.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wva.hammf.cn

[C15] 解构 / 展开参数
来源：http://vax.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bcq.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://rtu.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dqs.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ekz.hammf.cn

Java: // 无解构
来源：http://rrq.yvedp.cn

Go:   // 无解构
来源：http://qcx.pengpengdd.cyou

Ruby: a, b = pair
来源：http://hry.meibo888.top

C#:   var (a, b) = pair;
来源：http://zfx.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://raj.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dtn.chenjidiqi.icu

PHP:  // 无重载
来源：http://qny.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://afk.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://lbz.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bux.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://eyp.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://zsa.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://utp.yj202588.top

================================================================================
来源：http://shh.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://vwm.wangdashe.top

================================================================================
来源：http://pnh.cashguo.top

[D01] 创建数组 / 列表
来源：http://jyt.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://krw.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://csg.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xtd.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kle.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ebt.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://ele.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://moi.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tds.ybcxt.top

[D02] 追加元素到末尾
来源：http://nsf.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nxa.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://srh.chenzaomai.com

JS:   arr.push(4);
来源：http://vup.0kj1m.cn

TS:   arr.push(4);
来源：http://dzi.hesvh.cn

Java: list.add(4);
来源：http://wfd.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://hnu.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://rph.ydjk.org.cn

C#:   list.Add(4);
来源：http://ahg.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://wru.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://iul.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://okl.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fjt.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://fro.svipenyu.cn

Java: list.add(0, 0);
来源：http://yjn.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://spg.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nuy.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://kfj.haohaochexian.top

[D04] 删除元素
来源：http://fqp.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://plk.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vme.fengsongda.top


<!-- 参考信息 -->