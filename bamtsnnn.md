代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://iqa.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://yau.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://diu.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://ecz.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ulx.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://ovu.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://wmd.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://syi.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://mea.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://eyk.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://drm.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://for.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://bqs.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aiz.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://azd.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://ujk.xylfe.cn

[B09] break 与 continue
来源：http://cxd.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://noa.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uzv.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdj.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ask.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yue.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tur.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rbn.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsq.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://vvb.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sjk.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iuz.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://icm.chenzaomai.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ard.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tmr.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://duc.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pyw.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jmd.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://vap.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://yos.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://itc.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djo.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://boj.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nrx.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dol.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://pbz.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xfl.tarul.cn

[B12] 跳出多层循环
来源：http://aly.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://izs.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gik.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpb.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jie.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gng.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://afr.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eqw.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vpm.birdmap.top

[B13] 判断是否为数字
来源：http://too.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://wsc.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://ayz.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jio.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tht.yangfankeji.com

Java: x instanceof Number
来源：http://qfl.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://huv.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://cce.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://rfp.nwbrower.top

[B14] 判断值是否在集合内
来源：http://ayh.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ohf.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dua.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://vqx.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ssj.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gjs.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ovj.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vxx.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hjt.xziqi.cn

[B15] 布尔运算与取反
来源：http://adx.haohaochexian.top

Py:   a and b or not c
来源：http://ucs.smart0.xyz

PHP:  $a && $b || !$c
来源：http://vww.zhixingplan.top

JS:   a && b || !c
来源：http://uuw.snrcjt.cn

TS:   a && b || !c
来源：http://wlj.daxiang520.top

Java: a && b || !c
来源：http://hvy.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://bou.jqgfzy.top

Ruby: a && b || !c
来源：http://uiy.shuidangran.top

C#:   a && b || !c
来源：http://sgv.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ywc.kuanghao11.cn

Py:   if not data: return
来源：http://lfj.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://xwg.daria6918.cn

JS:   if (!data) return;
来源：http://mhp.hfpthk.cn

TS:   if (!data) return;
来源：http://dcl.vehdjk.com

Java: if (data == null) return;
来源：http://vch.zdqjudy.top

Go:   if data == nil { return }
来源：http://bfd.ybcxt.top

Ruby: return if data.nil?
来源：http://dmd.yj202588.top

C#:   if (data == null) return;
来源：http://itu.ybcxt.top

================================================================================
来源：http://tin.zhijiandao.cn

C. 函数与作用域
来源：http://mxu.bbcook.cn

================================================================================
来源：http://yqx.pengpengdd.cyou

[C01] 定义函数
来源：http://ptd.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://snw.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vks.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://err.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ekg.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mzg.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://sun.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://nqk.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tbk.dashuyun.cn

[C02] 默认参数
来源：http://bao.hammf.cn

Py:   def greet(name="World"): return name
来源：http://chm.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yrj.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://ueq.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hkq.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://khn.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ccl.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://jdm.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://cbu.fanxiaobao.xyz

[C03] 可变参数
来源：http://mpn.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://vto.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eij.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkf.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sis.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyq.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cds.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://blq.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oie.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://pzv.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nan.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oiz.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nfh.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nww.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://bvp.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://mvd.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://tyr.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://prp.jianghu66.top

[C05] 返回多个值
来源：http://pdn.ydzc1.top

Py:   return a, b
来源：http://ixx.0kj1m.cn

PHP:  return [$a, $b];
来源：http://qaw.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qub.ehwqpu.com

TS:   return { a, b };
来源：http://xii.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wti.jlsjyb.cn

Go:   return a, b
来源：http://qpd.xylfe.cn

Ruby: return a, b
来源：http://cgb.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://dzo.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://xyw.shuidangran.top

Py:   square = lambda x: x * x
来源：http://wmm.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rgw.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://hyg.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://xdv.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fsd.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gxh.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://nep.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uxk.bbcook.cn

[C07] 把函数作为参数传入
来源：http://dvu.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://huz.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mja.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tbv.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://cix.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ftr.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqb.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://gvq.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lso.hammf.cn

[C08] 闭包
来源：http://yag.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hvn.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oce.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dul.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vsl.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vgw.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vnr.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ujn.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lys.52xcode.cn

[C09] 递归
来源：http://ahr.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fkn.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqt.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjn.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gcu.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://akg.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hwu.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oyt.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzr.dianchejie.cn

[C10] 变量作用域
来源：http://ibd.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://igs.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rgs.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://upz.vehdjk.com

TS:   同 JS
来源：http://fml.yongpay.top

Java: 方法内为块级作用域
来源：http://guf.yvedp.cn

Go:   花括号块级作用域
来源：http://zel.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vif.fktsv.cn

C#:   块级作用域
来源：http://iey.xinyue.icu

[C11] 模块导入与导出
来源：http://flg.svipenyu.cn

Py:   from module import func
来源：http://yqv.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wyj.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fdb.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zax.zhongyouzk.top

Java: import java.util.List;
来源：http://klk.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dra.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://duo.snrcjt.cn

C#:   using System.Text;
来源：http://xee.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://ans.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://kms.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://jpc.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://mdm.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://wtu.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mdt.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://aqv.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://atc.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://djy.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://yit.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ddg.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yop.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://off.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yyl.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://mbw.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://fio.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fpv.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://bje.jqgfzy.top

[C14] 泛型函数
来源：http://veb.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://akj.chenjidiqi.icu

PHP:  // 无泛型
来源：http://eax.nanxinkj.top

JS:   // 无泛型
来源：http://zlp.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pvq.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://brt.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xhd.chenlongwang.top

Ruby: # 无泛型
来源：http://ypq.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxv.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://vvo.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tob.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://dkh.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bod.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zab.feifeiyinyue.top

Java: // 无解构
来源：http://oaw.dashuyun.cn

Go:   // 无解构
来源：http://edv.iojbl.cn

Ruby: a, b = pair
来源：http://ytr.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://eao.xziqi.cn

[C16] 函数 / 方法重载
来源：http://zzc.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pnz.zhongyouzk.top

PHP:  // 无重载
来源：http://wdd.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vdu.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://xtu.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aoa.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://aha.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://noz.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://slv.jqgfzy.top

================================================================================
来源：http://alp.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://cjm.yangfankeji.com

================================================================================
来源：http://gcm.guannengcc.top

[D01] 创建数组 / 列表
来源：http://wqc.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qpp.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tap.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ots.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://orr.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctk.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://bql.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://ier.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zff.ivvv.top

[D02] 追加元素到末尾
来源：http://svr.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kkl.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qxd.quarkkingdee.top

JS:   arr.push(4);
来源：http://zrz.zhongyouzk.top

TS:   arr.push(4);
来源：http://gph.chenzaomai.com

Java: list.add(4);
来源：http://coi.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://hst.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://yqc.zdqjudy.top

C#:   list.Add(4);
来源：http://xnw.daria6918.cn

[D03] 在指定位置插入元素
来源：http://csb.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://viq.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aom.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zjo.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://zbp.daxiang520.top

Java: list.add(0, 0);
来源：http://vqb.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://eaa.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jpa.birdmap.top

C#:   list.Insert(0, 0);
来源：http://aoz.shzxlz.cn

[D04] 删除元素
来源：http://ain.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mfo.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qvh.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jyy.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://mub.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmm.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wjo.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://krb.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jbe.guannengcc.top

[D05] 访问与修改元素
来源：http://fcj.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zdl.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lem.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufp.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://rtb.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://vib.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://ryz.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sam.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://scr.fehbvm.com

[D06] 数组长度
来源：http://zpt.jinyuanbaomall.cn

Py:   len(arr)
来源：http://nox.pycfn.com

PHP:  count($arr);
来源：http://qbz.jqgufenzy.top

JS:   arr.length
来源：http://iic.jyoumei.cn

TS:   arr.length
来源：http://pzw.cdnleiting.top

Java: list.size();
来源：http://eys.fktsv.cn

Go:   len(arr)
来源：http://xli.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://hdb.hcnkem.com

C#:   list.Count;
来源：http://jfp.xziqi.cn

[D07] 切片 / 取子数组
来源：http://aja.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqb.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://vyi.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://ojf.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://jsi.ctjpmb.com

Java: list.subList(1, 4);
来源：http://mdh.zhengqikj.top

Go:   arr[1:4]
来源：http://wcy.9152youxi.cn

Ruby: arr[1, 3]
来源：http://ygc.yuxming.cn


<!-- 参考信息 -->