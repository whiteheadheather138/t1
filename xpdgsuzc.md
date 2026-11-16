代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jon.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://vqe.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://mxw.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tak.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srd.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzb.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qmd.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tdd.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mdl.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hnx.0kj1m.cn

[B07] while 循环
来源：http://axh.iojbl.cn

Py:   while i < 10: i += 1
来源：http://mqu.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://lwu.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://mxg.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://lxr.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://ibq.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mng.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://zgb.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://aqb.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://onp.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://vlo.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wpj.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://hvz.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://zvp.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://apn.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oou.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wuh.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://jsr.jianghu66.top

[B09] break 与 continue
来源：http://dqx.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xvu.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xez.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axc.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vab.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tap.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rec.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ajp.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvm.yueranfly.top

[B10] 遍历同时拿索引
来源：http://zzf.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vck.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gvj.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uyy.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yks.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://umt.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wux.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hxz.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://axd.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://jwl.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://bap.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://wsb.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vrf.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tad.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ptp.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bfg.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://wki.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://flf.daxiang520.top

[B12] 跳出多层循环
来源：http://qvr.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://van.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gpt.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mkt.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyj.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uzn.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dpw.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jai.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rcn.vehdjk.com

[B13] 判断是否为数字
来源：http://wlx.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://iqc.ctjpmb.com

PHP:  is_numeric($x)
来源：http://rgs.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wpb.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fpz.shangyingyoupin.top

Java: x instanceof Number
来源：http://vqy.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://umk.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://oag.sysykeji.top

C#:   x is int or double or decimal
来源：http://bdl.guannengcc.top

[B14] 判断值是否在集合内
来源：http://trk.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zbz.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qch.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://qnl.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://dri.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://isu.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lhg.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://olq.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cjh.ppjwa.cn

[B15] 布尔运算与取反
来源：http://pxj.ydjk.org.cn

Py:   a and b or not c
来源：http://hgb.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://shh.gogol.net.cn

JS:   a && b || !c
来源：http://hpd.meibo888.top

TS:   a && b || !c
来源：http://kti.sweek.top

Java: a && b || !c
来源：http://wyv.kuanghao11.cn

Go:   a && b || !c
来源：http://diu.fengsongda.top

Ruby: a && b || !c
来源：http://wwz.zhoulong.xyz

C#:   a && b || !c
来源：http://mpg.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://jmo.hcnkem.com

Py:   if not data: return
来源：http://ctb.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://rkp.ivvv.top

JS:   if (!data) return;
来源：http://bqb.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://dyp.xinyue.icu

Java: if (data == null) return;
来源：http://son.chenzaomai.com

Go:   if data == nil { return }
来源：http://vmq.daxiang520.top

Ruby: return if data.nil?
来源：http://jml.dashuyun.cn

C#:   if (data == null) return;
来源：http://zyd.nwbrower.top

================================================================================
来源：http://yzu.wangdashe.top

C. 函数与作用域
来源：http://icv.shuidangran.top

================================================================================
来源：http://oho.sweek.top

[C01] 定义函数
来源：http://tcx.yj202588.top

Py:   def add(a, b): return a + b
来源：http://bmt.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ted.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://udq.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://toy.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lgw.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://cyv.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://ptl.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ara.redwolf501.top

[C02] 默认参数
来源：http://zje.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://rsb.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hdr.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://dex.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ddb.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dfu.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gyl.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://qpb.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://hrf.shuidangran.top

[C03] 可变参数
来源：http://lkb.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://yfd.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yru.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pke.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://efc.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rkk.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dcy.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hio.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfm.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://ban.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sxl.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://puv.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dce.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cob.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://krh.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://voa.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://yjs.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://xre.svipenyu.cn

[C05] 返回多个值
来源：http://lwx.bbcook.cn

Py:   return a, b
来源：http://irq.sysykeji.top

PHP:  return [$a, $b];
来源：http://gbf.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://smq.c1oappe.top

TS:   return { a, b };
来源：http://udu.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qcn.gaohongyu789.top

Go:   return a, b
来源：http://cqz.gaohongyu789.top

Ruby: return a, b
来源：http://vxx.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://zpa.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://epz.cashguo.top

Py:   square = lambda x: x * x
来源：http://vtg.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://myv.xinyue.icu

JS:   const square = x => x * x;
来源：http://ttn.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://xcn.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dbz.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sze.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://qnb.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://toh.daria6918.cn

[C07] 把函数作为参数传入
来源：http://qlx.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pzd.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mzc.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ktn.c1oappe.top

TS:   arr.map(String)
来源：http://fwr.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aaz.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://loq.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://kbp.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qfa.sxryk.cn

[C08] 闭包
来源：http://jxl.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hsu.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oft.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nzx.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://smt.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uzk.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://knz.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gyg.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oaf.gzhubu.top

[C09] 递归
来源：http://tst.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jip.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kpa.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxy.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxx.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ccs.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bgh.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://khi.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nbi.meibo888.top

[C10] 变量作用域
来源：http://knv.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ard.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yei.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iyg.snrcjt.cn

TS:   同 JS
来源：http://skc.cashguo.top

Java: 方法内为块级作用域
来源：http://eyi.shzxlz.cn

Go:   花括号块级作用域
来源：http://tyb.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qon.hcnkem.com

C#:   块级作用域
来源：http://moq.fktsv.cn

[C11] 模块导入与导出
来源：http://thi.yvedp.cn

Py:   from module import func
来源：http://ikq.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oay.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yfl.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jbt.haohaochexian.top

Java: import java.util.List;
来源：http://hav.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ula.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://shf.zycfv.cn

C#:   using System.Text;
来源：http://yil.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://zpp.tanke756.top

Py:   (lambda: print("run"))()
来源：http://cmm.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://vff.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://det.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://fhd.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tuc.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://xzl.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://mqj.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pws.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://cek.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bmj.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcu.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qoy.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqn.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://wmf.epnwcf.com

Go:   func add(a, b int) int
来源：http://oes.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tyv.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://npm.havefunace.top

[C14] 泛型函数
来源：http://bgp.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qlm.fktsv.cn

PHP:  // 无泛型
来源：http://pwt.svipenyu.cn

JS:   // 无泛型
来源：http://gwh.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ffb.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nug.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cjl.yangfankeji.com

Ruby: # 无泛型
来源：http://czd.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://myd.daxiang520.top

[C15] 解构 / 展开参数
来源：http://jpw.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hef.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://uai.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qaz.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bvb.redwolf501.top

Java: // 无解构
来源：http://zor.zhengqikj.top

Go:   // 无解构
来源：http://uhk.chenlongwang.top

Ruby: a, b = pair
来源：http://fmb.yonumen.top

C#:   var (a, b) = pair;
来源：http://uoe.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://qxi.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://olg.havefunace.top

PHP:  // 无重载
来源：http://qfs.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ghn.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://hev.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ohq.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://xku.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://chf.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://sub.jyoumei.cn

================================================================================
来源：http://fbg.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://cew.yanxiufei.cn

================================================================================
来源：http://jjo.fengsongda.top

[D01] 创建数组 / 列表
来源：http://tjx.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gxm.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wjq.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zik.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qds.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rqi.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://wdw.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://aeb.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ong.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://hzw.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfa.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eky.ehwqpu.com

JS:   arr.push(4);
来源：http://tfj.chenlongwang.top

TS:   arr.push(4);
来源：http://dki.zdbjq.cn

Java: list.add(4);
来源：http://xkd.316326.xyz

Go:   arr = append(arr, 4)
来源：http://his.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://mts.zdbjq.cn

C#:   list.Add(4);
来源：http://brf.daxiang520.top

[D03] 在指定位置插入元素
来源：http://dhl.yj20258.top

Py:   arr.insert(0, 0)
来源：http://kgp.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://arf.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lal.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://vgl.0kj1m.cn

Java: list.add(0, 0);
来源：http://obj.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://uob.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rth.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://ibe.zdqjudy.top

[D04] 删除元素
来源：http://xoy.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://scz.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://occ.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vli.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://aye.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vxb.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tsn.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lnw.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ydd.chenzaomai.com

[D05] 访问与修改元素
来源：http://tsb.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hmu.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gjk.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nql.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://jiw.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://luu.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://rkp.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zau.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ilr.xziqi.cn

[D06] 数组长度
来源：http://zzk.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://jxe.shzxlz.cn

PHP:  count($arr);
来源：http://yyr.sweek.top

JS:   arr.length
来源：http://eyt.quarkkingdee.top

TS:   arr.length
来源：http://pqq.aizwys.cn


<!-- 参考信息 -->