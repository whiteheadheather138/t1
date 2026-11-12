代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dbg.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gfz.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vno.chenlongwang.top

[B04] for 计数循环
来源：http://xef.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://wbw.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ndl.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aoi.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cjp.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jpm.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kyx.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://fpv.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cek.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://yqg.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://wpe.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xgx.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wqk.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ztk.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xcd.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rho.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://sfv.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qww.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://dyb.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jle.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sul.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://isx.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rio.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dry.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rfv.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zfc.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gcr.ydjk.org.cn

[B07] while 循环
来源：http://cao.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://fpd.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://sla.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://nsc.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://yzf.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://lmt.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tup.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://wpn.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://tgz.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://ank.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ids.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uuo.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://zou.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://swr.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://llu.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qex.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://jmm.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://vdk.jianghu66.top

[B09] break 与 continue
来源：http://ukt.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fbu.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hoo.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxl.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykh.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vub.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vyb.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://seo.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gws.yj20258.top

[B10] 遍历同时拿索引
来源：http://kfo.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nly.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pos.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mmz.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nwg.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jjd.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rzp.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bky.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hdt.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://vps.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://ovm.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://zwf.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyc.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dkr.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tog.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fjb.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://tad.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efo.sxryk.cn

[B12] 跳出多层循环
来源：http://lvo.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jcd.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lfr.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uxo.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zxr.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://syv.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jbu.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rxe.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bbr.jinqigufen.top

[B13] 判断是否为数字
来源：http://nno.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://nej.tian-w.cn

PHP:  is_numeric($x)
来源：http://mqw.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tcz.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlh.nanxinkj.top

Java: x instanceof Number
来源：http://upt.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ekw.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://wck.haohaochexian.top

C#:   x is int or double or decimal
来源：http://tds.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://ltd.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blh.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qbf.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://dvj.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://hrb.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ols.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ntp.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://zaz.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mgq.fengsongda.top

[B15] 布尔运算与取反
来源：http://gft.vqdsnc.cn

Py:   a and b or not c
来源：http://viv.ybcxt.top

PHP:  $a && $b || !$c
来源：http://wuw.ehwqpu.com

JS:   a && b || !c
来源：http://syn.tanke756.top

TS:   a && b || !c
来源：http://spd.wangshuangyany.cn

Java: a && b || !c
来源：http://llh.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://svw.cashguo.top

Ruby: a && b || !c
来源：http://yne.yueranfly.top

C#:   a && b || !c
来源：http://xbt.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://lik.xylfe.cn

Py:   if not data: return
来源：http://bpr.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://rjp.zhoulong.xyz

JS:   if (!data) return;
来源：http://mqt.jqgfzy.top

TS:   if (!data) return;
来源：http://hgt.zhixingplan.top

Java: if (data == null) return;
来源：http://zty.hywenlv.cn

Go:   if data == nil { return }
来源：http://rmz.hnxiangtu.top

Ruby: return if data.nil?
来源：http://oop.havefunace.top

C#:   if (data == null) return;
来源：http://khm.xuetiantiany.cn

================================================================================
来源：http://alg.ywan-chungtsiang.top

C. 函数与作用域
来源：http://czh.shanyushiyangtech.top

================================================================================
来源：http://qqp.chenzaomai.com

[C01] 定义函数
来源：http://asx.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://rsp.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tim.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://xqi.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fmq.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://nfl.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kqc.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://tqn.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nvt.uphjek.com

[C02] 默认参数
来源：http://nmu.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://znq.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ikr.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://adl.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sua.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oah.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xkj.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://qkl.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://kgb.yongpay.top

[C03] 可变参数
来源：http://pls.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://yml.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://krd.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xjk.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcf.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iyf.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://drf.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://crq.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://paj.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://ozn.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pjj.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gnf.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yls.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jrw.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://hvk.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://eav.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://exf.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://nbi.feifeiyinyue.top

[C05] 返回多个值
来源：http://wxe.9152youxi.cn

Py:   return a, b
来源：http://fxa.gzhubu.top

PHP:  return [$a, $b];
来源：http://enc.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zqt.havefunace.top

TS:   return { a, b };
来源：http://xts.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qgh.yvedp.cn

Go:   return a, b
来源：http://ukk.wangshuangyany.cn

Ruby: return a, b
来源：http://dog.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://kym.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://fnc.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://nsk.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zso.jyoumei.cn

JS:   const square = x => x * x;
来源：http://tno.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://wnv.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rpg.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://zpr.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://pug.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qal.xinyue.icu

[C07] 把函数作为参数传入
来源：http://zkw.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ndg.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gzc.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dzp.yanxiufei.cn

TS:   arr.map(String)
来源：http://iqv.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yhz.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wup.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://prb.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://afd.cqqwz.cn

[C08] 闭包
来源：http://dhn.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lrh.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dim.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pzu.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uuc.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qwe.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://njd.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sff.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ayh.gaohongyu789.top

[C09] 递归
来源：http://dbt.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rnu.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ihk.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://god.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eus.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mgr.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://via.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iba.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xnz.feifeiyinyue.top

[C10] 变量作用域
来源：http://gvz.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kuw.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lef.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzj.shanyushiyangtech.top

TS:   同 JS
来源：http://tmt.jiagoushi.top

Java: 方法内为块级作用域
来源：http://bck.chenzaomai.com

Go:   花括号块级作用域
来源：http://bar.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tkp.kuanghao11.cn

C#:   块级作用域
来源：http://zwy.jiagoushi.top

[C11] 模块导入与导出
来源：http://rpr.chenlongwang.top

Py:   from module import func
来源：http://apy.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vch.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kcd.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dhd.feifeiyinyue.top

Java: import java.util.List;
来源：http://cmd.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lsn.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://zfn.bjfxy.top

C#:   using System.Text;
来源：http://oag.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://pyf.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://dwg.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://wyq.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://vbs.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://qzn.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bdr.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://nea.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://rmh.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aef.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://uip.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kfg.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybj.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lmp.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pbj.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://brm.yfazqb.com

Go:   func add(a, b int) int
来源：http://cgl.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bxb.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://slc.sjlbkw.cn

[C14] 泛型函数
来源：http://vqe.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ztn.chenlongwang.top

PHP:  // 无泛型
来源：http://xrc.sufxvd.cn

JS:   // 无泛型
来源：http://gps.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hco.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iuk.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fxk.sjlbkw.cn

Ruby: # 无泛型
来源：http://joq.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nzr.yj202588.top

[C15] 解构 / 展开参数
来源：http://akt.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wit.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://cde.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://daj.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzm.guannengcc.top

Java: // 无解构
来源：http://mee.jinqigufen.top

Go:   // 无解构
来源：http://qcw.tanke756.top

Ruby: a, b = pair
来源：http://xez.uphjek.com

C#:   var (a, b) = pair;
来源：http://nrd.shuidangran.top

[C16] 函数 / 方法重载
来源：http://uhl.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nwv.hywenlv.cn

PHP:  // 无重载
来源：http://ozi.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uon.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://yqg.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://klr.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://dpi.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://ncw.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tmb.hnxiangtu.top

================================================================================
来源：http://ejv.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://neo.sufxvd.cn

================================================================================
来源：http://miz.yuxming.cn

[D01] 创建数组 / 列表
来源：http://wqe.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvx.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ekp.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ckj.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xcs.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zsh.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://yla.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://aod.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bvl.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://tbg.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxm.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lko.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://ykx.quarkkingdee.top

TS:   arr.push(4);
来源：http://pmt.zycfv.cn

Java: list.add(4);
来源：http://pac.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://two.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://fme.gogol.net.cn

C#:   list.Add(4);
来源：http://zep.hesvh.cn

[D03] 在指定位置插入元素
来源：http://bvr.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://tns.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jyd.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gct.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://zoy.tanke756.top

Java: list.add(0, 0);
来源：http://fui.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://yxo.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://afe.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://dmz.havefunace.top

[D04] 删除元素
来源：http://yne.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vro.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ccl.shanyushiyangtech.top


<!-- 参考信息 -->