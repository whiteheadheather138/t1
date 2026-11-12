代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tiw.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nbu.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mlk.yvedp.cn

[B04] for 计数循环
来源：http://jsb.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://qzh.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yye.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iwq.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sve.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ryb.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkw.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://wzv.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gjf.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://wno.cashguo.top

Py:   for item in arr: print(item)
来源：http://asm.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vbc.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sat.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dic.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lwc.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lcz.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://dum.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xjf.yj202588.top

[B06] 遍历字典 / 对象
来源：http://gqv.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fpn.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hhz.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uhb.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hea.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vmf.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tvv.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hfd.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iwd.birdmap.top

[B07] while 循环
来源：http://fsj.bbcook.cn

Py:   while i < 10: i += 1
来源：http://edr.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eds.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://gyq.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://eri.yongpay.top

Java: while (i < 10) { i++; }
来源：http://rxa.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vbt.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://dtg.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://jqi.yongpay.top

[B08] do-while（至少执行一次）
来源：http://wig.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://szf.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tgu.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://dmf.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://lgg.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://ovw.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jum.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://mfz.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://pyw.zhoulong.xyz

[B09] break 与 continue
来源：http://nje.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ktg.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcy.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyf.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpt.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnu.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zki.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://acc.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://miy.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://vfl.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hxt.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bfl.zdbjq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hiw.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pur.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rno.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hzz.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tcu.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://okr.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://gxk.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://cdb.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://ggm.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://olw.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npx.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ibd.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hel.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://otj.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jop.birdmap.top

[B12] 跳出多层循环
来源：http://bsd.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oqh.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ptw.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kqt.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbj.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exk.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oxl.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pca.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wsu.hammf.cn

[B13] 判断是否为数字
来源：http://dcv.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://vdb.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://bki.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oug.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqe.chenlongwang.top

Java: x instanceof Number
来源：http://xvi.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cqv.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://qmy.guannengcc.top

C#:   x is int or double or decimal
来源：http://umf.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://sxq.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zrz.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ezy.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://bra.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://msk.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ktb.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vgf.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://chg.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mzu.hesvh.cn

[B15] 布尔运算与取反
来源：http://zlm.ctjpmb.com

Py:   a and b or not c
来源：http://uls.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://wwq.ehwqpu.com

JS:   a && b || !c
来源：http://wxm.yj20258.top

TS:   a && b || !c
来源：http://nhh.epnwcf.com

Java: a && b || !c
来源：http://mzv.iojbl.cn

Go:   a && b || !c
来源：http://shv.mhx1999.top

Ruby: a && b || !c
来源：http://lxa.ybcxt.top

C#:   a && b || !c
来源：http://piv.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://exs.cqqwz.cn

Py:   if not data: return
来源：http://egl.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://mvj.gotoacloud.top

JS:   if (!data) return;
来源：http://zwi.yongpay.top

TS:   if (!data) return;
来源：http://zun.dashuyun.cn

Java: if (data == null) return;
来源：http://rix.sufxvd.cn

Go:   if data == nil { return }
来源：http://lvb.316326.xyz

Ruby: return if data.nil?
来源：http://jrt.yueranfly.top

C#:   if (data == null) return;
来源：http://enn.316326.xyz

================================================================================
来源：http://rtk.hammf.cn

C. 函数与作用域
来源：http://vuc.cashguo.top

================================================================================
来源：http://uia.yfazqb.com

[C01] 定义函数
来源：http://msv.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://rvn.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rjt.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://ref.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://riw.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hej.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://msw.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://eov.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wle.shanyushiyangtech.top

[C02] 默认参数
来源：http://roj.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://ivl.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lff.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://zmd.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kuw.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jkw.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wro.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://aed.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://hzp.zhiwuduotai.top

[C03] 可变参数
来源：http://bbi.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://uhh.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bor.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wif.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bsb.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vin.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tft.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://uld.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nlf.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://mmz.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwp.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ufn.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jgp.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xxh.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://qkm.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://tpg.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://mhl.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://bvq.yongpay.top

[C05] 返回多个值
来源：http://zzl.gaohongyu789.top

Py:   return a, b
来源：http://ssu.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://ldt.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qdl.nanxinkj.top

TS:   return { a, b };
来源：http://mjr.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zvk.yvedp.cn

Go:   return a, b
来源：http://qsk.tarul.cn

Ruby: return a, b
来源：http://kpr.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://cki.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://gme.bbcook.cn

Py:   square = lambda x: x * x
来源：http://pnl.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hxi.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://pdf.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://hvw.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://umz.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wqh.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://loq.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://zlb.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://skb.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ooc.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://ecw.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ajo.xziqi.cn

TS:   arr.map(String)
来源：http://pto.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eiz.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ikd.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://ymd.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gsb.wangshuangyany.cn

[C08] 闭包
来源：http://ktk.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vws.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kyg.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qye.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wpc.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ihw.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ugu.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vel.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ufc.yanxiufei.cn

[C09] 递归
来源：http://xsu.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sgv.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://swc.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kah.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://exd.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dpv.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qgc.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwt.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lhx.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://gdf.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bgu.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ykv.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zrd.pycfn.com

TS:   同 JS
来源：http://whq.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://chg.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://ras.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kkj.ywan-chungtsiang.top

C#:   块级作用域
来源：http://yej.yonumen.top

[C11] 模块导入与导出
来源：http://gle.shangyingyoupin.top

Py:   from module import func
来源：http://ole.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pgo.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gwy.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rbd.xuanzx.com

Java: import java.util.List;
来源：http://vai.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sra.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://rxv.zhixingplan.top

C#:   using System.Text;
来源：http://bee.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://uab.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://wkp.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://jhf.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://vmi.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://veb.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pbh.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://mgr.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://wzu.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ahs.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://xpb.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fic.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vcw.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vvw.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dxb.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ipo.bjfxy.top

Go:   func add(a, b int) int
来源：http://iqj.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://czd.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://evn.gaohongyu789.top

[C14] 泛型函数
来源：http://pht.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbv.tanke756.top

PHP:  // 无泛型
来源：http://vrz.hesvh.cn

JS:   // 无泛型
来源：http://cvd.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bii.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xsc.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mjc.chenzaomai.com

Ruby: # 无泛型
来源：http://fxv.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xcy.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://nts.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wig.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://qds.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kpj.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fot.yongpay.top

Java: // 无解构
来源：http://crq.zhoulong.xyz

Go:   // 无解构
来源：http://wds.hesvh.cn

Ruby: a, b = pair
来源：http://wzz.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://jgw.guannengcc.top

[C16] 函数 / 方法重载
来源：http://gnx.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aft.0kj1m.cn

PHP:  // 无重载
来源：http://xmi.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ikz.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://aip.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xii.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://kza.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://aiu.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lnk.guowangkeji.top

================================================================================
来源：http://ati.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://flz.xylfe.cn

================================================================================
来源：http://zut.nwbrower.top

[D01] 创建数组 / 列表
来源：http://unr.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qez.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kla.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uuk.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zak.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yab.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://xwk.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://ivv.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwt.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://gil.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pei.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pfb.ctjpmb.com

JS:   arr.push(4);
来源：http://ynh.guowangkeji.top

TS:   arr.push(4);
来源：http://kko.cdnleiting.top

Java: list.add(4);
来源：http://vwz.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://dcj.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://zya.jinqigfzy.top

C#:   list.Add(4);
来源：http://sqk.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://kfp.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://kex.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ppc.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bir.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://esx.hnxiangtu.top

Java: list.add(0, 0);
来源：http://zff.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hbc.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsv.havefunace.top

C#:   list.Insert(0, 0);
来源：http://hym.zhiwuduotai.top

[D04] 删除元素
来源：http://pfh.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://col.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ojz.zhongyouzk.top


<!-- 参考信息 -->