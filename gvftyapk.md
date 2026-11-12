代发 wailian999

Py:   for i in range(10): print(i)
来源：http://tcg.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ixt.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ndr.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbl.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://afi.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iiq.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://wqy.xuanzx.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tgv.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://vdc.havefunace.top

Py:   for item in arr: print(item)
来源：http://jeh.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cgn.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ezo.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rvb.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jfj.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kdj.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://cnz.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cxa.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://pxy.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tdj.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zwa.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fup.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kck.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ppg.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xdl.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://byf.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bde.ctjpmb.com

[B07] while 循环
来源：http://yhl.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://non.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://ktc.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://kko.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://wqs.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://yow.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aid.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://ujp.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://hgl.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://ftc.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://uyu.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lte.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://qxx.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://vuk.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://rrl.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://yrj.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://cud.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://qex.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://uni.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nka.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ejt.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfb.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhk.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oic.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rcn.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rpw.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skh.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://fdm.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://omu.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://npc.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zbe.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rad.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://atz.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hce.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wod.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gst.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://kci.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://uky.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://crz.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwa.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://anm.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zut.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsr.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://vqg.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cli.hysaishi.cn

[B12] 跳出多层循环
来源：http://axj.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mgw.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rmb.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nzw.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vby.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zbf.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tyb.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iof.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://byr.pycfn.com

[B13] 判断是否为数字
来源：http://ufc.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://mpl.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://bvf.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rgl.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxs.gotoacloud.top

Java: x instanceof Number
来源：http://khs.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vre.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://gvl.cucudq.cn

C#:   x is int or double or decimal
来源：http://rkf.meibo888.top

[B14] 判断值是否在集合内
来源：http://tcx.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cgd.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://alx.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://mkq.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://hoc.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zra.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ngc.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://ted.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wep.52xcode.cn

[B15] 布尔运算与取反
来源：http://yen.fanxiaobao.xyz

Py:   a and b or not c
来源：http://yds.yj20258.top

PHP:  $a && $b || !$c
来源：http://ctk.cucudq.cn

JS:   a && b || !c
来源：http://mvh.sufxvd.cn

TS:   a && b || !c
来源：http://soh.svipenyu.cn

Java: a && b || !c
来源：http://kyh.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://pov.tanke756.top

Ruby: a && b || !c
来源：http://zee.xuanzx.com

C#:   a && b || !c
来源：http://jks.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fgj.yanxiufei.cn

Py:   if not data: return
来源：http://wad.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://xsw.gogol.net.cn

JS:   if (!data) return;
来源：http://thk.aibaodan.cn

TS:   if (!data) return;
来源：http://vpy.yfazqb.com

Java: if (data == null) return;
来源：http://ard.hesvh.cn

Go:   if data == nil { return }
来源：http://bwg.cqqwz.cn

Ruby: return if data.nil?
来源：http://hys.ehwqpu.com

C#:   if (data == null) return;
来源：http://ylt.vehdjk.com

================================================================================
来源：http://pow.ehwqpu.com

C. 函数与作用域
来源：http://psc.yangfankeji.com

================================================================================
来源：http://shl.xylfe.cn

[C01] 定义函数
来源：http://cpv.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://ldw.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kni.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://pgw.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tut.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pej.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qyv.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://zci.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rnh.zhiwuduotai.top

[C02] 默认参数
来源：http://qbi.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://jht.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nxj.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://zwu.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://riq.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wsi.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zwg.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://ahq.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://igv.vqdsnc.cn

[C03] 可变参数
来源：http://ulg.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://xov.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bpg.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcw.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://usj.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mrj.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://clg.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ehp.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lqa.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://kws.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bxw.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ycp.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zaw.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hxv.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://uve.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://xrb.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://ims.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://zzn.hnqzz.top

[C05] 返回多个值
来源：http://gbr.sjlbkw.cn

Py:   return a, b
来源：http://prx.mhx1999.top

PHP:  return [$a, $b];
来源：http://cbo.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vlm.guannengcc.top

TS:   return { a, b };
来源：http://pqg.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pff.yj20258.top

Go:   return a, b
来源：http://kfk.ehwqpu.com

Ruby: return a, b
来源：http://xss.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://cdy.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://fly.sysykeji.top

Py:   square = lambda x: x * x
来源：http://kpw.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zky.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://exn.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://dlt.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ozc.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://ewl.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://fcz.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://ovm.yj20258.top

[C07] 把函数作为参数传入
来源：http://pkd.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://twy.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://sxq.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://osm.snrcjt.cn

TS:   arr.map(String)
来源：http://ebi.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pic.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lmd.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://gno.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lik.redwolf501.top

[C08] 闭包
来源：http://ldd.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://maf.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccc.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pub.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://amh.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rkr.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ako.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://msv.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yam.chenzaomai.com

[C09] 递归
来源：http://arf.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://izp.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qhh.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ipb.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnd.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yum.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ivj.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://var.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdu.jlsjyb.cn

[C10] 变量作用域
来源：http://ktd.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cmo.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://otx.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://njh.zhiwuduotai.top

TS:   同 JS
来源：http://zey.0kj1m.cn

Java: 方法内为块级作用域
来源：http://lvq.vehdjk.com

Go:   花括号块级作用域
来源：http://naz.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yih.svipenyu.cn

C#:   块级作用域
来源：http://lbs.sxryk.cn

[C11] 模块导入与导出
来源：http://ltg.hesvh.cn

Py:   from module import func
来源：http://sor.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rpm.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kln.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://udy.ivvv.top

Java: import java.util.List;
来源：http://vgc.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bfa.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://abc.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://adu.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://ydx.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://amz.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://ifz.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://sfr.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://iiv.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dfv.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ivx.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://ljv.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cay.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://plo.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sxu.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlc.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umo.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfr.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://rmo.tarul.cn

Go:   func add(a, b int) int
来源：http://jxw.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://did.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ody.xuanzx.com

[C14] 泛型函数
来源：http://ivc.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://niq.yangfankeji.com

PHP:  // 无泛型
来源：http://mqj.yuxming.cn

JS:   // 无泛型
来源：http://nwi.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://unz.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oke.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zno.birdmap.top

Ruby: # 无泛型
来源：http://aby.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eks.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://fxd.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zit.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://ako.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jea.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gdr.yangfankeji.com

Java: // 无解构
来源：http://imp.ydjk.org.cn

Go:   // 无解构
来源：http://gja.meibo888.top

Ruby: a, b = pair
来源：http://lam.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://mrr.xylfe.cn

[C16] 函数 / 方法重载
来源：http://wgz.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ulf.jinghuilouyu.cn

PHP:  // 无重载
来源：http://gld.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uey.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://ttr.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bqo.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://och.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://vdj.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://sjf.yuanzhike.top

================================================================================
来源：http://dtb.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://uqz.sxryk.cn

================================================================================
来源：http://dai.yj20258888.top

[D01] 创建数组 / 列表
来源：http://ffy.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gbc.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tfp.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mon.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ceh.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kck.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://dpj.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://zqz.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uem.aibaodan.cn

[D02] 追加元素到末尾
来源：http://mbd.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nne.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oqk.52xcode.cn

JS:   arr.push(4);
来源：http://trl.cucudq.cn

TS:   arr.push(4);
来源：http://dio.xuanzx.com

Java: list.add(4);
来源：http://kbp.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://pue.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://laj.chenjidiqi.icu

C#:   list.Add(4);
来源：http://aeh.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://zyi.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://ysm.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aak.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vkt.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://cmb.kuanghao11.cn

Java: list.add(0, 0);
来源：http://mex.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vfk.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bjr.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://tzx.52xcode.cn

[D04] 删除元素
来源：http://wyj.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uqb.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://inr.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lur.meibo888.top

TS:   arr.splice(0, 1);
来源：http://llv.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qrz.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vqb.cucudq.cn


<!-- 参考信息 -->