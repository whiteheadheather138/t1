代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfb.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ttd.cdnleiting.top

[B07] while 循环
来源：http://xtn.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://ooj.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gdk.sweek.top

JS:   while (i < 10) { i++; }
来源：http://hgf.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://rlf.ivvv.top

Java: while (i < 10) { i++; }
来源：http://qay.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hxv.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://hpk.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://ark.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://bln.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://soa.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gta.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://gca.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://sss.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://jir.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sej.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qck.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://ycr.ydzc1.top

[B09] break 与 continue
来源：http://iwp.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vdx.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fos.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwb.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdi.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yiq.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://enl.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zqx.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdc.sxryk.cn

[B10] 遍历同时拿索引
来源：http://cic.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kxm.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hnf.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ppf.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eah.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ipk.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://udq.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://org.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bdv.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://vtk.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://cvr.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://zsh.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mzw.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ahw.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fwy.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sgr.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://qff.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xqf.yvedp.cn

[B12] 跳出多层循环
来源：http://qso.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lxk.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnk.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://syi.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhs.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uso.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://duu.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xlp.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zzc.meibo888.top

[B13] 判断是否为数字
来源：http://idf.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://pbq.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://imp.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqm.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lmj.bjfxy.top

Java: x instanceof Number
来源：http://ukp.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnx.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://aao.shzxlz.cn

C#:   x is int or double or decimal
来源：http://mxu.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://qlz.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mlr.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bdw.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://brl.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://sdm.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vxr.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kuy.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://qlo.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mke.shzxlz.cn

[B15] 布尔运算与取反
来源：http://wbv.sufxvd.cn

Py:   a and b or not c
来源：http://kwn.bjfxy.top

PHP:  $a && $b || !$c
来源：http://gkj.svipenyu.cn

JS:   a && b || !c
来源：http://roy.kuanghao11.cn

TS:   a && b || !c
来源：http://jtn.meibo888.top

Java: a && b || !c
来源：http://xww.daria6918.cn

Go:   a && b || !c
来源：http://vom.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://mhv.ivvv.top

C#:   a && b || !c
来源：http://sha.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ibz.jqgufenzy.top

Py:   if not data: return
来源：http://bnu.uphjek.com

PHP:  if (!$data) { return; }
来源：http://dga.gzhubu.top

JS:   if (!data) return;
来源：http://vhg.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://xsf.mhx1999.top

Java: if (data == null) return;
来源：http://iuy.fehbvm.com

Go:   if data == nil { return }
来源：http://vfa.nanxinkj.top

Ruby: return if data.nil?
来源：http://krq.hnxiangtu.top

C#:   if (data == null) return;
来源：http://zft.yanxiufei.cn

================================================================================
来源：http://efo.hongshengwenyu.top

C. 函数与作用域
来源：http://szv.jqgufenzy.top

================================================================================
来源：http://qua.svipenyu.cn

[C01] 定义函数
来源：http://pnq.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://dow.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://srp.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://bri.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmb.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://zfl.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zus.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://vte.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fwm.c1oappe.top

[C02] 默认参数
来源：http://rsk.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://cmv.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xph.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://keu.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mtt.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sqh.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tzv.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://ilo.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://wmq.zhijiandao.cn

[C03] 可变参数
来源：http://csi.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://cjg.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://teu.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sfj.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://skd.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kig.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eth.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://mag.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pzb.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://ufd.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jgv.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://til.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rti.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xhn.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://zkc.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://yyn.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://sip.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://kag.uphjek.com

[C05] 返回多个值
来源：http://xhw.hammf.cn

Py:   return a, b
来源：http://hnc.hywenlv.cn

PHP:  return [$a, $b];
来源：http://boq.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://elq.zdbjq.cn

TS:   return { a, b };
来源：http://tvv.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ann.daria6918.cn

Go:   return a, b
来源：http://mog.quarkkingdee.top

Ruby: return a, b
来源：http://kzl.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://lbi.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://oau.meibo888.top

Py:   square = lambda x: x * x
来源：http://uok.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xcj.yj20258.top

JS:   const square = x => x * x;
来源：http://bno.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://smu.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ckd.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://gtn.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://mnm.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://ora.hcnkem.com

[C07] 把函数作为参数传入
来源：http://oyo.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lnj.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ndq.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zed.shangyingyoupin.top

TS:   arr.map(String)
来源：http://kms.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bee.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zyk.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://ozo.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fco.vqdsnc.cn

[C08] 闭包
来源：http://pgs.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nmw.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eay.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://grg.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sda.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kgc.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ewi.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ktp.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fhk.yongpay.top

[C09] 递归
来源：http://yib.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uqs.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lzd.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zgd.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gto.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsf.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lgq.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xnp.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gpm.zhixingplan.top

[C10] 变量作用域
来源：http://kkm.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hgo.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qcl.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pgg.ybcxt.top

TS:   同 JS
来源：http://sjb.smart0.xyz

Java: 方法内为块级作用域
来源：http://ges.bjfxy.top

Go:   花括号块级作用域
来源：http://ech.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://szr.yfazqb.com

C#:   块级作用域
来源：http://lba.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://edl.snrcjt.cn

Py:   from module import func
来源：http://vcc.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vvv.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://coq.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hgr.tianlin.xyz

Java: import java.util.List;
来源：http://lof.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mzs.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://nyu.gotoacloud.top

C#:   using System.Text;
来源：http://hqj.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://ibj.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://fhm.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://xdj.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://odo.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://oyq.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jip.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://bdm.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://xat.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dsq.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://kgy.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sua.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqy.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gta.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iow.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://sbf.vehdjk.com

Go:   func add(a, b int) int
来源：http://koz.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fae.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://odl.tanke756.top

[C14] 泛型函数
来源：http://fao.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fkx.kuanghao11.cn

PHP:  // 无泛型
来源：http://qlk.hcnkem.com

JS:   // 无泛型
来源：http://pfw.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fvn.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bsc.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rin.hongshengwenyu.top

Ruby: # 无泛型
来源：http://hkx.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yub.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://qpc.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://prz.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://csj.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oms.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://odz.0kj1m.cn

Java: // 无解构
来源：http://cma.xziqi.cn

Go:   // 无解构
来源：http://dyi.chenzaomai.com

Ruby: a, b = pair
来源：http://dsb.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://jdb.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://ege.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fpb.mhx1999.top

PHP:  // 无重载
来源：http://qxa.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://btu.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://soz.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xgd.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://dlh.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://udm.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wfg.ydjk.org.cn

================================================================================
来源：http://syn.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://oaw.cheryme.top

================================================================================
来源：http://lcp.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://sch.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oou.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kjo.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cgy.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xiu.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cca.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://azg.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://wog.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjy.meibo888.top

[D02] 追加元素到末尾
来源：http://dft.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://euv.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fos.0kj1m.cn

JS:   arr.push(4);
来源：http://hxj.zdqjudy.top

TS:   arr.push(4);
来源：http://hsn.zdqjudy.top

Java: list.add(4);
来源：http://pwj.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://con.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://kqf.dianchejie.cn

C#:   list.Add(4);
来源：http://ivj.hcnkem.com

[D03] 在指定位置插入元素
来源：http://tuo.hammf.cn

Py:   arr.insert(0, 0)
来源：http://mpz.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://svx.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xgj.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://fxm.hnxiangtu.top

Java: list.add(0, 0);
来源：http://owd.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://xft.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kft.tanke756.top

C#:   list.Insert(0, 0);
来源：http://gzw.jyoumei.cn

[D04] 删除元素
来源：http://ixc.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fuk.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oma.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tpk.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://wbc.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ecd.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yqi.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kme.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ddv.gogol.net.cn

[D05] 访问与修改元素
来源：http://khf.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cgi.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yjh.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fhh.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://kwg.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://ncp.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://bxk.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lja.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acm.xuetiantiany.cn

[D06] 数组长度
来源：http://jvz.yfazqb.com

Py:   len(arr)
来源：http://ogj.vehdjk.com

PHP:  count($arr);
来源：http://jnh.sweek.top

JS:   arr.length
来源：http://ahp.vqdsnc.cn

TS:   arr.length
来源：http://rem.kuanghao11.cn

Java: list.size();
来源：http://stl.ybcxt.top

Go:   len(arr)
来源：http://msg.xuanzx.com

Ruby: arr.length; arr.size
来源：http://mzi.zhaomingkeji.xyz

C#:   list.Count;
来源：http://utf.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://nyb.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://alu.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://ybj.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://afy.zhiwuduotai.top


<!-- 参考信息 -->