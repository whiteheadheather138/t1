代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iwm.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wjh.xylfe.cn

[B07] while 循环
来源：http://jkh.xziqi.cn

Py:   while i < 10: i += 1
来源：http://xnd.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ftw.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://mmr.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://uio.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://hry.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyp.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://pik.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://emm.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://exx.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://wuq.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://jvs.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://ghv.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://qww.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://mfb.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ytk.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://lrz.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://lby.zdqjudy.top

[B09] break 与 continue
来源：http://elw.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xhw.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kng.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdd.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://frs.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://peq.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jvs.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://txx.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://koe.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://hie.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sge.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nue.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qya.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rvf.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qov.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lbt.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cxd.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://len.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://wui.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://zgc.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://aeu.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vmd.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmr.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zko.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mia.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://ebb.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gcg.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://vvg.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rie.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqj.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gnh.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://klu.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cvn.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://egh.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nca.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://laj.chenzaomai.com

[B13] 判断是否为数字
来源：http://anf.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://qom.tanke756.top

PHP:  is_numeric($x)
来源：http://zac.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eku.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wyy.gogol.net.cn

Java: x instanceof Number
来源：http://tko.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oel.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://qnb.gotoacloud.top

C#:   x is int or double or decimal
来源：http://dab.tarul.cn

[B14] 判断值是否在集合内
来源：http://udj.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dxq.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yim.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://cyo.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://ypm.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yji.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xsn.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://vjv.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sjw.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://qfs.vehdjk.com

Py:   a and b or not c
来源：http://bxm.ivvv.top

PHP:  $a && $b || !$c
来源：http://mem.nwbrower.top

JS:   a && b || !c
来源：http://puc.quarkkingdee.top

TS:   a && b || !c
来源：http://mbo.redwolf501.top

Java: a && b || !c
来源：http://nxb.fehbvm.com

Go:   a && b || !c
来源：http://iwl.yanxiufei.cn

Ruby: a && b || !c
来源：http://fod.fanxiaobao.xyz

C#:   a && b || !c
来源：http://upj.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ufu.havefunace.top

Py:   if not data: return
来源：http://blo.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://jzt.zhiwuduotai.top

JS:   if (!data) return;
来源：http://lkg.wangshuangyany.cn

TS:   if (!data) return;
来源：http://slw.xuanzx.com

Java: if (data == null) return;
来源：http://opk.nwbrower.top

Go:   if data == nil { return }
来源：http://bqk.dashuyun.cn

Ruby: return if data.nil?
来源：http://sju.yvedp.cn

C#:   if (data == null) return;
来源：http://qlc.hysaishi.cn

================================================================================
来源：http://zpy.hysaishi.cn

C. 函数与作用域
来源：http://qyl.yueranfly.top

================================================================================
来源：http://mvq.ydzc1.top

[C01] 定义函数
来源：http://cxo.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://nsw.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yjj.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://laj.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://czu.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qlm.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://atz.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://qeb.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eat.bbcook.cn

[C02] 默认参数
来源：http://lzl.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://bwm.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vsa.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://qfj.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aub.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qrg.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ywm.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://fbj.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://mei.jyoumei.cn

[C03] 可变参数
来源：http://zsq.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://aos.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vny.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqp.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://znt.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oqu.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wkr.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://bmw.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rpq.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://ccb.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rfj.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wdw.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gxr.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hjg.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://mif.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://dzv.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://chg.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://azd.vqdsnc.cn

[C05] 返回多个值
来源：http://vwi.316326.xyz

Py:   return a, b
来源：http://hzj.mhx1999.top

PHP:  return [$a, $b];
来源：http://gnb.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nzi.yj20258888.top

TS:   return { a, b };
来源：http://amt.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qfj.smart0.xyz

Go:   return a, b
来源：http://nnw.ehwqpu.com

Ruby: return a, b
来源：http://rgq.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://ubz.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://fzy.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://kmb.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://itb.cucudq.cn

JS:   const square = x => x * x;
来源：http://rjd.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://noj.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tto.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://obi.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://ecn.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://mxj.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://exz.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bvf.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xkm.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://drj.daria6918.cn

TS:   arr.map(String)
来源：http://qdp.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zih.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmz.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://qjj.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fxj.guowangkeji.top

[C08] 闭包
来源：http://tsv.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wfa.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ide.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ghm.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lfa.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fup.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vzr.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jzi.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kla.wangdashe.top

[C09] 递归
来源：http://kvd.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zrj.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qci.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcf.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkx.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://obd.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dvi.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iol.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oxl.yonumen.top

[C10] 变量作用域
来源：http://gpj.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nzp.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mir.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lxm.fanxiaobao.xyz

TS:   同 JS
来源：http://yrp.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://itx.ydzc1.top

Go:   花括号块级作用域
来源：http://maq.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bkn.cdnleiting.top

C#:   块级作用域
来源：http://mch.bbcook.cn

[C11] 模块导入与导出
来源：http://xcg.hysaishi.cn

Py:   from module import func
来源：http://ceu.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://edv.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xtc.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zzc.sxryk.cn

Java: import java.util.List;
来源：http://dqw.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://knh.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://qiy.yangfankeji.com

C#:   using System.Text;
来源：http://wfm.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://vlb.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://csk.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://qhu.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://tcf.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://azi.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pvx.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://bte.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://tnr.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eeg.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://hwm.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aks.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://icd.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ycq.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hel.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://njy.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://dgi.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kpi.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://yjf.sysykeji.top

[C14] 泛型函数
来源：http://xzf.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vzm.zhongyouzk.top

PHP:  // 无泛型
来源：http://ylj.redwolf501.top

JS:   // 无泛型
来源：http://vly.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qny.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://unv.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lad.chenzaomai.com

Ruby: # 无泛型
来源：http://nol.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://prl.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://sah.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nft.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://wdr.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://byo.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qet.zycfv.cn

Java: // 无解构
来源：http://vcz.sufxvd.cn

Go:   // 无解构
来源：http://bxl.dianchejie.cn

Ruby: a, b = pair
来源：http://hvu.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://tcg.meibo888.top

[C16] 函数 / 方法重载
来源：http://phk.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lmr.hysaishi.cn

PHP:  // 无重载
来源：http://qhd.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://czo.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://wst.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ucp.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://pra.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://qpt.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mdm.havefunace.top

================================================================================
来源：http://ifd.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://aww.9152youxi.cn

================================================================================
来源：http://dia.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://taq.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fps.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vel.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nhz.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yrl.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nrs.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://qcw.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://fmv.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://quu.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://tfw.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jnj.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxb.meibo888.top

JS:   arr.push(4);
来源：http://kuv.redwolf501.top

TS:   arr.push(4);
来源：http://rkj.52xcode.cn

Java: list.add(4);
来源：http://ajm.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://tje.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://bxn.jqgufenzy.top

C#:   list.Add(4);
来源：http://orh.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://toy.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://wjp.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tjt.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ero.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://hws.quarkkingdee.top

Java: list.add(0, 0);
来源：http://cfz.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://ele.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://alt.yongpay.top

C#:   list.Insert(0, 0);
来源：http://pvu.gotoacloud.top

[D04] 删除元素
来源：http://cbl.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uqh.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yfq.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bzf.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://dgy.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bee.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vuk.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dus.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://khr.hesvh.cn

[D05] 访问与修改元素
来源：http://sxg.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvb.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xoq.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://roi.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://vge.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://tpr.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://tjv.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sqe.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jpn.zdbjq.cn

[D06] 数组长度
来源：http://qjq.ivvv.top

Py:   len(arr)
来源：http://gtb.yvedp.cn

PHP:  count($arr);
来源：http://rha.kuanghao11.cn

JS:   arr.length
来源：http://een.gogol.net.cn

TS:   arr.length
来源：http://mrm.xingfuxueyuan.xyz

Java: list.size();
来源：http://nxe.xylfe.cn

Go:   len(arr)
来源：http://aaf.uphjek.com

Ruby: arr.length; arr.size
来源：http://klv.yj20258888.top

C#:   list.Count;
来源：http://ggr.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ztp.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mwl.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://sol.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://igu.316326.xyz


<!-- 参考信息 -->