代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rsi.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://atv.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ion.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://upp.sweek.top

Py:   for i in range(10): print(i)
来源：http://bvq.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dsx.tarul.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nkf.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gir.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wnx.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lie.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://orh.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nva.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://zzw.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://pqi.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dkr.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tvv.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://khu.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://lol.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rrw.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://xms.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mdd.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://ets.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ggr.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yvb.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ufg.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tvf.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ohh.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://plh.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://miw.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zmg.jinqigfzy.top

[B07] while 循环
来源：http://lpe.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://isj.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://elt.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://jhy.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://rrp.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://tzz.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jql.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://sfc.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://bfr.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://uom.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://qrm.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://smu.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://kqr.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://arm.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://qcp.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bfr.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://dgy.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://hle.yfazqb.com

[B09] break 与 continue
来源：http://vsn.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mwz.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xul.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lci.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgt.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ccu.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ejo.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jdt.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwu.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://ydy.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://euc.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hue.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ikm.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbi.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://suc.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zzs.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://clw.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zyc.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://mtl.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://iyg.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://jzr.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgb.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://scm.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eyi.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pzr.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://yxo.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dzl.sxryk.cn

[B12] 跳出多层循环
来源：http://qfu.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rfo.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://mxr.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qey.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hdc.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xla.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nqv.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kow.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ncp.havefunace.top

[B13] 判断是否为数字
来源：http://wxt.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://gsf.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://llk.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuu.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://acn.yuxming.cn

Java: x instanceof Number
来源：http://npu.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qzr.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://otw.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://osl.xziqi.cn

[B14] 判断值是否在集合内
来源：http://ief.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ypa.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wyk.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://duy.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://vvq.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://yvq.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dum.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ang.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fdv.hfpthk.cn

[B15] 布尔运算与取反
来源：http://wpf.ybcxt.top

Py:   a and b or not c
来源：http://boo.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://xtc.quarkkingdee.top

JS:   a && b || !c
来源：http://agy.gzhubu.top

TS:   a && b || !c
来源：http://ggz.xziqi.cn

Java: a && b || !c
来源：http://aly.guannengcc.top

Go:   a && b || !c
来源：http://tza.yj20258.top

Ruby: a && b || !c
来源：http://whh.yongpay.top

C#:   a && b || !c
来源：http://ctd.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://ken.jqgfzy.top

Py:   if not data: return
来源：http://xit.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://txb.hysaishi.cn

JS:   if (!data) return;
来源：http://iyl.nwbrower.top

TS:   if (!data) return;
来源：http://cou.daxiang520.top

Java: if (data == null) return;
来源：http://vrd.mhx1999.top

Go:   if data == nil { return }
来源：http://omo.jianghu66.top

Ruby: return if data.nil?
来源：http://foe.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://tjp.hfpthk.cn

================================================================================
来源：http://qoy.tian-w.cn

C. 函数与作用域
来源：http://zdd.ydzc1.top

================================================================================
来源：http://svb.jqgufenzy.top

[C01] 定义函数
来源：http://hoo.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://vfl.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vcg.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://vau.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kvh.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ppe.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hrn.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://oft.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yib.c1oappe.top

[C02] 默认参数
来源：http://psw.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://cki.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zzn.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://tcj.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zfs.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zxg.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lks.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://fol.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://jmg.daria6918.cn

[C03] 可变参数
来源：http://kdn.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://myq.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://weu.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ufm.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dhz.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nvu.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ttu.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://bbr.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lyd.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://kid.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://khz.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjy.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bhx.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lvn.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://zug.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://vto.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://spe.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://sud.jqgufenzy.top

[C05] 返回多个值
来源：http://tbz.jqgfzy.top

Py:   return a, b
来源：http://ine.shzxlz.cn

PHP:  return [$a, $b];
来源：http://ips.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yol.wangdashe.top

TS:   return { a, b };
来源：http://edb.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yrw.ydjk.org.cn

Go:   return a, b
来源：http://nnf.smart0.xyz

Ruby: return a, b
来源：http://imy.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://pbh.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://hqu.c1oappe.top

Py:   square = lambda x: x * x
来源：http://itn.shanyushiyangtech.top

PHP:  $square = fn($x) => $x * $x;
来源：http://paf.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://gjc.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://cbm.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gvg.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://eon.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://jpx.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://wfo.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://fku.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pkp.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://mct.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://avt.kuanghao11.cn

TS:   arr.map(String)
来源：http://pgi.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gdz.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gvn.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://tmj.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ujk.xinyue.icu

[C08] 闭包
来源：http://jfq.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zym.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kkg.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ydg.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szp.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zjg.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lbq.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tzm.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fsp.svipenyu.cn

[C09] 递归
来源：http://ivo.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://low.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iap.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aaz.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ywr.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mwk.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://clm.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xgq.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rvf.sxryk.cn

[C10] 变量作用域
来源：http://vzr.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hux.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gki.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvl.ybcxt.top

TS:   同 JS
来源：http://vev.dianchejie.cn

Java: 方法内为块级作用域
来源：http://tyr.fktsv.cn

Go:   花括号块级作用域
来源：http://zfx.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jqr.hcnkem.com

C#:   块级作用域
来源：http://luy.gotoacloud.top

[C11] 模块导入与导出
来源：http://kvu.fktsv.cn

Py:   from module import func
来源：http://alb.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://egy.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nwt.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iwr.nanxuanxn.top

Java: import java.util.List;
来源：http://ggq.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://frp.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://rju.pycfn.com

C#:   using System.Text;
来源：http://clq.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://rzd.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://jqf.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://uvm.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://yzz.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://gml.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hti.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://evn.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://wvt.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uxd.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://iek.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://atf.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://apt.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pnn.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rax.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://awy.tarul.cn

Go:   func add(a, b int) int
来源：http://bya.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zbv.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://pla.chenjidiqi.icu

[C14] 泛型函数
来源：http://vlb.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ynq.sysykeji.top

PHP:  // 无泛型
来源：http://mtv.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://tqv.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ihz.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sez.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://euw.gzhubu.top

Ruby: # 无泛型
来源：http://qnw.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dql.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://vov.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tvf.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://tvx.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sgt.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ecs.fengsongda.top

Java: // 无解构
来源：http://oxv.jlsjyb.cn

Go:   // 无解构
来源：http://wlp.ydjk.org.cn

Ruby: a, b = pair
来源：http://byo.andypj.xyz

C#:   var (a, b) = pair;
来源：http://nkg.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://emt.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bir.haohaochexian.top

PHP:  // 无重载
来源：http://yao.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xgd.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://ouf.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://des.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://lkm.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://tev.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ioe.gaohongyu789.top

================================================================================
来源：http://vae.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://xgm.cdnleiting.top

================================================================================
来源：http://ptw.yj202588.top

[D01] 创建数组 / 列表
来源：http://fws.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pjx.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lta.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hhk.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ubw.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fph.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://hlb.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://vtv.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ygg.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://pob.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tqh.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gha.chenlongwang.top

JS:   arr.push(4);
来源：http://isl.xinyue.icu

TS:   arr.push(4);
来源：http://xyd.52xcode.cn

Java: list.add(4);
来源：http://tqo.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://txg.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://yau.yanxiufei.cn

C#:   list.Add(4);
来源：http://imb.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://ogb.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://poa.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xid.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qoe.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://eld.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://mjy.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://sen.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zrr.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://hzv.nwbrower.top

[D04] 删除元素
来源：http://ega.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxe.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kwh.meibo888.top


<!-- 参考信息 -->