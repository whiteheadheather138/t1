代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dvx.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dcw.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ixz.c1oappe.top

[B04] for 计数循环
来源：http://aar.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://vih.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://enb.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jts.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tqd.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://srw.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kog.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://itn.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aie.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://yvb.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://ber.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xgr.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wrs.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kte.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lvi.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://moj.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://xxx.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nwd.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://ekd.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uuj.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pvx.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kfx.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyx.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://evb.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xpt.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lqf.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ozv.c1oappe.top

[B07] while 循环
来源：http://jaq.bbcook.cn

Py:   while i < 10: i += 1
来源：http://icl.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://poe.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://azp.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://rrm.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://pjd.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://whn.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://bsn.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://cdg.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://uue.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vnd.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qxm.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://qeh.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://ccg.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://osx.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pui.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://eru.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://axo.daxiang520.top

[B09] break 与 continue
来源：http://xph.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zvy.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ivc.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyg.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfc.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dny.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vox.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://izv.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbs.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://jxv.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dua.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qfe.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bnp.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gsg.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrc.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lgr.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vhv.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://htv.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://zkh.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://fas.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://gsx.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlg.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikf.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kwc.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://imk.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://eup.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pdg.zhongyouzk.top

[B12] 跳出多层循环
来源：http://vxy.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wxx.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gqg.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yoc.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hbd.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dwu.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://apn.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fct.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ujp.shuidangran.top

[B13] 判断是否为数字
来源：http://jfr.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://vua.xziqi.cn

PHP:  is_numeric($x)
来源：http://rze.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fpq.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://imh.jqgufenzy.top

Java: x instanceof Number
来源：http://dnq.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://obn.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://guk.fehbvm.com

C#:   x is int or double or decimal
来源：http://cay.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://ljb.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zdl.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wlf.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://zvi.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://msq.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pxu.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zit.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fnz.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zvu.mhx1999.top

[B15] 布尔运算与取反
来源：http://xik.shangyingyoupin.top

Py:   a and b or not c
来源：http://iut.shuidangran.top

PHP:  $a && $b || !$c
来源：http://wre.andypj.xyz

JS:   a && b || !c
来源：http://nzs.guannengcc.top

TS:   a && b || !c
来源：http://tpm.pengpengdd.cyou

Java: a && b || !c
来源：http://jfb.hongshengwenyu.top

Go:   a && b || !c
来源：http://lns.gotoacloud.top

Ruby: a && b || !c
来源：http://mge.shanyushiyangtech.top

C#:   a && b || !c
来源：http://ilx.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://not.zdbjq.cn

Py:   if not data: return
来源：http://kpe.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://qdn.zhiwuduotai.top

JS:   if (!data) return;
来源：http://dnt.guowangkeji.top

TS:   if (!data) return;
来源：http://pql.hongshengwenyu.top

Java: if (data == null) return;
来源：http://svj.zdqjudy.top

Go:   if data == nil { return }
来源：http://vas.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://zwc.dashuyun.cn

C#:   if (data == null) return;
来源：http://bce.andypj.xyz

================================================================================
来源：http://xuh.chenjidiqi.icu

C. 函数与作用域
来源：http://mrr.yongpay.top

================================================================================
来源：http://vnx.zycfv.cn

[C01] 定义函数
来源：http://fin.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://ody.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inw.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://dwy.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yrt.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aig.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://yci.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://duh.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pdf.tianlin.xyz

[C02] 默认参数
来源：http://amj.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://gag.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iii.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://cpv.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ldj.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://rjk.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbn.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://rob.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://yzm.dashuyun.cn

[C03] 可变参数
来源：http://bra.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://khq.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvb.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xcw.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qwt.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ter.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mgo.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gzx.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ljt.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://fgf.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xni.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xua.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ovv.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nrs.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://wio.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://tso.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://xpd.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://gfi.c1oappe.top

[C05] 返回多个值
来源：http://vwz.zhaomingkeji.xyz

Py:   return a, b
来源：http://vir.sysykeji.top

PHP:  return [$a, $b];
来源：http://tjc.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://uro.fzhhl.top

TS:   return { a, b };
来源：http://bhm.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mxg.chenzaomai.com

Go:   return a, b
来源：http://ugc.quarkkingdee.top

Ruby: return a, b
来源：http://eev.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://mbo.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://hsp.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://qnk.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://egp.yonumen.top

JS:   const square = x => x * x;
来源：http://ffg.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://rxg.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rwa.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://syq.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://wgm.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://ste.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://kkp.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iow.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://vmk.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ctw.yangfankeji.com

TS:   arr.map(String)
来源：http://eez.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jns.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yah.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://mqh.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://ypn.tanke756.top

[C08] 闭包
来源：http://cmi.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ryf.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fmi.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://euc.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yol.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tlm.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lsh.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hcz.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zvz.jiagoushi.top

[C09] 递归
来源：http://rff.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pnq.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://frh.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gop.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ped.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yti.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qjd.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://epe.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtl.daria6918.cn

[C10] 变量作用域
来源：http://fmz.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwv.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pkd.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ihq.yj20258888.top

TS:   同 JS
来源：http://pgz.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://utd.hfpthk.cn

Go:   花括号块级作用域
来源：http://udo.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cnd.quarkkingdee.top

C#:   块级作用域
来源：http://jow.smart0.xyz

[C11] 模块导入与导出
来源：http://vbd.jqgufenzy.top

Py:   from module import func
来源：http://hag.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://djr.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://vfz.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ham.hnqzz.top

Java: import java.util.List;
来源：http://kvk.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://roe.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://uxl.jqgfzy.top

C#:   using System.Text;
来源：http://ttw.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://ecx.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://yxu.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://bdd.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://crq.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://vkh.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nei.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://pmp.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://ihj.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xae.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://htt.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tag.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dim.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sxf.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blp.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://hld.aibaodan.cn

Go:   func add(a, b int) int
来源：http://oqf.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eoa.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qav.sweek.top

[C14] 泛型函数
来源：http://hkr.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ynw.ydjk.org.cn

PHP:  // 无泛型
来源：http://efd.aibaodan.cn

JS:   // 无泛型
来源：http://wmu.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tnn.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ilu.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fzd.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://lma.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eyk.daxiang520.top

[C15] 解构 / 展开参数
来源：http://ktn.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iss.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://owz.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zbn.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zue.yonumen.top

Java: // 无解构
来源：http://lhx.jiagoushi.top

Go:   // 无解构
来源：http://rle.0kj1m.cn

Ruby: a, b = pair
来源：http://iqk.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://yie.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://xux.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kah.yj20258.top

PHP:  // 无重载
来源：http://xqy.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ara.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://qmm.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bbz.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://rib.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://hkb.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gir.ybcxt.top

================================================================================
来源：http://ykv.tarul.cn

D. 数组 / 列表 / 集合
来源：http://koe.fanxiaobao.xyz

================================================================================
来源：http://fbh.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://kgv.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://bsw.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://plh.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://awb.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kwq.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oda.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://rtq.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://qrb.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ani.xinyue.icu

[D02] 追加元素到末尾
来源：http://kdj.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxc.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ezj.dianchejie.cn

JS:   arr.push(4);
来源：http://thc.gotoacloud.top

TS:   arr.push(4);
来源：http://zaa.quarkkingdee.top

Java: list.add(4);
来源：http://tst.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://nlx.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://zyi.zycfv.cn

C#:   list.Add(4);
来源：http://ime.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://vcq.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://bmj.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hap.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jtw.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://mvm.hesvh.cn

Java: list.add(0, 0);
来源：http://jfm.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://ott.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xdu.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://vff.fktsv.cn

[D04] 删除元素
来源：http://itm.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fcj.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://krk.birdmap.top


<!-- 参考信息 -->