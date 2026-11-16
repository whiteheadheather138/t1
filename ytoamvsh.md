代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dsj.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zfr.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kai.hnxiangtu.top

[B04] for 计数循环
来源：http://pcm.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://esz.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rkr.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhv.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eea.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tmu.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kmt.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://tqm.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtr.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://dlk.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://wuq.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lfz.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://asf.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://scv.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://onr.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ooj.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://dbw.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://whk.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://gkj.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ybt.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hbj.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uil.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ovb.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://efk.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iqz.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lti.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bnh.hfpthk.cn

[B07] while 循环
来源：http://hqy.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://ese.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://glv.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://lwp.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://mal.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://arc.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ltc.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://dvz.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://zvj.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://nex.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://kbm.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://spc.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://htz.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://bjx.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://uet.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://hvu.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://gxh.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://cah.hnqzz.top

[B09] break 与 continue
来源：http://rsb.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yht.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ssw.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyb.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktt.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iir.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kft.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://btr.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sst.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://emr.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tpd.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zvr.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hnz.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtv.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://djo.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qdp.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://unq.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://udc.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://wno.sweek.top

Py:   list(range(0, 10, 2))
来源：http://flz.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://gqx.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wqp.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nha.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jrn.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ukr.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://uui.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hrl.havefunace.top

[B12] 跳出多层循环
来源：http://sbi.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jfd.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fak.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhj.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zdc.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uzn.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lfu.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fwb.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xcv.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://fvd.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://uvj.zhixingplan.top

PHP:  is_numeric($x)
来源：http://etl.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkr.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gta.meibo888.top

Java: x instanceof Number
来源：http://ydw.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://anv.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://mvm.hysaishi.cn

C#:   x is int or double or decimal
来源：http://hfc.mhx1999.top

[B14] 判断值是否在集合内
来源：http://kgz.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://axu.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xuj.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://ykx.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://tti.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rlg.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eyk.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://yen.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xrs.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://yat.sxryk.cn

Py:   a and b or not c
来源：http://mtw.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://rnm.jlsjyb.cn

JS:   a && b || !c
来源：http://zfb.haohaochexian.top

TS:   a && b || !c
来源：http://nil.dianchejie.cn

Java: a && b || !c
来源：http://hcp.sweek.top

Go:   a && b || !c
来源：http://tiv.dashuyun.cn

Ruby: a && b || !c
来源：http://qvw.chenjidiqi.icu

C#:   a && b || !c
来源：http://uzl.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ijv.vqdsnc.cn

Py:   if not data: return
来源：http://fce.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://zbx.shuidangran.top

JS:   if (!data) return;
来源：http://czo.c1oappe.top

TS:   if (!data) return;
来源：http://fwa.nwbrower.top

Java: if (data == null) return;
来源：http://ziq.yuxming.cn

Go:   if data == nil { return }
来源：http://tzy.ctjpmb.com

Ruby: return if data.nil?
来源：http://pvj.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://kts.ehwqpu.com

================================================================================
来源：http://uhm.daxiang520.top

C. 函数与作用域
来源：http://hbc.quarkkingdee.top

================================================================================
来源：http://kef.bbcook.cn

[C01] 定义函数
来源：http://agb.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://irr.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://shz.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://tde.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uip.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lou.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nrg.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://fuk.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yly.hnxiangtu.top

[C02] 默认参数
来源：http://nrq.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://uhl.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ogx.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://npq.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rbo.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uhc.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xtc.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://gfi.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ucf.ctjpmb.com

[C03] 可变参数
来源：http://szo.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://cxf.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yec.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkh.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sxf.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dio.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ioh.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://iwy.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zek.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://cyd.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://duu.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zoo.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cws.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zai.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://ylk.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://iob.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://qhy.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://ymf.c1oappe.top

[C05] 返回多个值
来源：http://lkn.quarkkingdee.top

Py:   return a, b
来源：http://sxj.cdnleiting.top

PHP:  return [$a, $b];
来源：http://hcj.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sbg.snrcjt.cn

TS:   return { a, b };
来源：http://wgj.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ath.svipenyu.cn

Go:   return a, b
来源：http://gkk.yanxiufei.cn

Ruby: return a, b
来源：http://smf.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://jnn.tanke756.top

[C06] 匿名函数 / lambda
来源：http://lyx.fengsongda.top

Py:   square = lambda x: x * x
来源：http://eel.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://try.pycfn.com

JS:   const square = x => x * x;
来源：http://jkh.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://zdu.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dwa.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://zek.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://vlr.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://xnv.jianghu66.top

[C07] 把函数作为参数传入
来源：http://qhw.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://khw.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://rbr.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bqt.dashuyun.cn

TS:   arr.map(String)
来源：http://fxr.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fme.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pqf.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://vil.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rkq.hfpthk.cn

[C08] 闭包
来源：http://rsb.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ags.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ntg.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pjw.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rlp.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oyi.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zez.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrm.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ndz.nanxuanxn.top

[C09] 递归
来源：http://slr.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://odi.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vtf.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zcu.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qye.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mgf.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eqp.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hzn.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rab.uphjek.com

[C10] 变量作用域
来源：http://gnv.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ahb.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iut.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yja.shanyushiyangkeji.top

TS:   同 JS
来源：http://tku.jianghu66.top

Java: 方法内为块级作用域
来源：http://viv.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://imb.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://avq.hesvh.cn

C#:   块级作用域
来源：http://qbb.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://jkf.tarul.cn

Py:   from module import func
来源：http://coh.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bhd.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jit.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yzq.tarul.cn

Java: import java.util.List;
来源：http://toi.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mea.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://whl.hesvh.cn

C#:   using System.Text;
来源：http://bkn.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://ojb.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://vfc.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://awc.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://bpm.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://xrb.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zwm.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://mlr.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://syx.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aqu.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://dbo.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eei.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lry.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://liu.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gxd.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://hda.hnqzz.top

Go:   func add(a, b int) int
来源：http://xgm.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yni.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://drw.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://kuz.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zku.fehbvm.com

PHP:  // 无泛型
来源：http://nuz.chenzaomai.com

JS:   // 无泛型
来源：http://wbp.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xez.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://owu.haohaochexian.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lpx.yangfankeji.com

Ruby: # 无泛型
来源：http://cza.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://whp.iojbl.cn

[C15] 解构 / 展开参数
来源：http://cjq.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tot.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://ahj.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fef.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jvf.yuxming.cn

Java: // 无解构
来源：http://hhs.zhiwuduotai.top

Go:   // 无解构
来源：http://pou.zhengqikj.top

Ruby: a, b = pair
来源：http://iao.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://zmo.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://dam.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nrp.sxryk.cn

PHP:  // 无重载
来源：http://vpj.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yti.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://qbg.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://bre.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://nik.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://dtw.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kpv.ctjpmb.com

================================================================================
来源：http://whf.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://msy.tarul.cn

================================================================================
来源：http://gji.yj20258.top

[D01] 创建数组 / 列表
来源：http://ymq.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nuk.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ohf.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yan.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzg.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fyb.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://mdw.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://hvk.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iyo.shzxlz.cn

[D02] 追加元素到末尾
来源：http://rpi.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wib.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lin.shzxlz.cn

JS:   arr.push(4);
来源：http://tbt.nwbrower.top

TS:   arr.push(4);
来源：http://zrz.xinyue.icu

Java: list.add(4);
来源：http://xsp.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://emw.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://ejm.jinqigfzy.top

C#:   list.Add(4);
来源：http://onq.vehdjk.com

[D03] 在指定位置插入元素
来源：http://lwe.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://hbz.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqd.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hee.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://vyp.jyoumei.cn

Java: list.add(0, 0);
来源：http://mba.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://cpw.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gls.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://obw.ppjwa.cn

[D04] 删除元素
来源：http://qtg.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qpz.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tfo.feifeiyinyue.top


<!-- 参考信息 -->