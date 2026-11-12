代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://ekw.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://kbd.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://lob.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://jbw.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://amd.ivvv.top

Ruby: while i < 10; i += 1; end
来源：http://tbe.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://fjo.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://qxt.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://vzc.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kvy.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://pzr.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://vop.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://ybg.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jxc.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://mww.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://pta.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://dmu.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://his.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mvx.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlo.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nso.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnp.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ghm.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xax.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdr.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://ugu.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gtk.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oyz.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ajo.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lvk.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fst.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jvw.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lmv.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxs.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://slm.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://pro.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://xkg.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bue.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqj.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gzc.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gnk.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://upe.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://osd.zdbjq.cn

[B12] 跳出多层循环
来源：http://nwi.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jap.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bkr.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://usw.yuanzhike.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dkp.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mri.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ewf.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kwc.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dpg.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://dvj.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://mbp.ehwqpu.com

PHP:  is_numeric($x)
来源：http://rcb.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cyb.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ssa.vehdjk.com

Java: x instanceof Number
来源：http://uxf.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bqb.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://yzl.yueranfly.top

C#:   x is int or double or decimal
来源：http://oau.vehdjk.com

[B14] 判断值是否在集合内
来源：http://rcf.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zqy.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vzs.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://yuz.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://vuf.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qku.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ajm.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://prf.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fpd.mhx1999.top

[B15] 布尔运算与取反
来源：http://utt.shanyushiyangtech.top

Py:   a and b or not c
来源：http://uar.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://jzh.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://uku.zhiwuduotai.top

TS:   a && b || !c
来源：http://qsk.jiagoushi.top

Java: a && b || !c
来源：http://zuk.nanxuanxn.top

Go:   a && b || !c
来源：http://dsp.zhengqikj.top

Ruby: a && b || !c
来源：http://qad.quarkkingdee.top

C#:   a && b || !c
来源：http://oab.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xyq.gaohongyu789.top

Py:   if not data: return
来源：http://ref.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://epi.sysykeji.top

JS:   if (!data) return;
来源：http://nvv.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://ecn.yvedp.cn

Java: if (data == null) return;
来源：http://tca.yuanzhike.top

Go:   if data == nil { return }
来源：http://rro.yuxming.cn

Ruby: return if data.nil?
来源：http://xaf.fzhhl.top

C#:   if (data == null) return;
来源：http://vot.pycfn.com

================================================================================
来源：http://ewp.meibo888.top

C. 函数与作用域
来源：http://krt.cdnleiting.top

================================================================================
来源：http://pwe.yongpay.top

[C01] 定义函数
来源：http://lac.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://xpn.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhm.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://vbo.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kmc.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://asz.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://afm.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://mua.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jli.zdqjudy.top

[C02] 默认参数
来源：http://kyg.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://xzp.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://gba.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://eci.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qhg.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mzg.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://exg.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://ipx.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://jyp.zhoulong.xyz

[C03] 可变参数
来源：http://gko.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://vzc.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oqx.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eaz.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywx.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjn.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dgn.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://hsb.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fbl.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://axw.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://obw.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jbz.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tqx.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cpg.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://cop.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://ury.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://aqc.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://srl.jinghuilouyu.cn

[C05] 返回多个值
来源：http://yww.yfazqb.com

Py:   return a, b
来源：http://rwb.gogol.net.cn

PHP:  return [$a, $b];
来源：http://ufu.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ucq.yanxiufei.cn

TS:   return { a, b };
来源：http://xdk.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qdj.cdnleiting.top

Go:   return a, b
来源：http://wfy.dashuyun.cn

Ruby: return a, b
来源：http://pjo.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://gtl.tanke756.top

[C06] 匿名函数 / lambda
来源：http://usx.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://nyz.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ovl.cqqwz.cn

JS:   const square = x => x * x;
来源：http://lfg.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://apt.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dta.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://alq.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://fma.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xhu.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://viy.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ntc.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zde.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hnc.iojbl.cn

TS:   arr.map(String)
来源：http://pdh.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kbo.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://egx.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://gsu.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://myc.wangdashe.top

[C08] 闭包
来源：http://hyu.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mfq.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzq.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://axt.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vup.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jxu.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hxa.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cqr.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://czt.shuidangran.top

[C09] 递归
来源：http://swk.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xue.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://adm.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bih.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cmr.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ekx.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbz.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vgi.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cth.sjlbkw.cn

[C10] 变量作用域
来源：http://hmx.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zbc.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oyj.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qsj.shzxlz.cn

TS:   同 JS
来源：http://vbm.zycfv.cn

Java: 方法内为块级作用域
来源：http://wkg.fzhhl.top

Go:   花括号块级作用域
来源：http://uvu.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vlo.vqdsnc.cn

C#:   块级作用域
来源：http://eqw.hfpthk.cn

[C11] 模块导入与导出
来源：http://pnn.epnwcf.com

Py:   from module import func
来源：http://dpj.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aax.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://nwy.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucn.316326.xyz

Java: import java.util.List;
来源：http://dwx.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zur.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://srh.hammf.cn

C#:   using System.Text;
来源：http://fyo.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://web.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://dyl.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://mxv.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://uoy.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://gjh.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://log.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://uis.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://opb.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eql.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://raa.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rpp.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbz.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cvh.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://waa.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://arh.pycfn.com

Go:   func add(a, b int) int
来源：http://gad.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fwv.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://giw.sjlbkw.cn

[C14] 泛型函数
来源：http://cjm.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lpl.yanxiufei.cn

PHP:  // 无泛型
来源：http://dnr.jinghuilouyu.cn

JS:   // 无泛型
来源：http://cvq.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://exm.ctjpmb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rjv.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rzq.mhx1999.top

Ruby: # 无泛型
来源：http://hqa.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vjo.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://kup.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dyu.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://jsx.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://peq.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nfo.uphjek.com

Java: // 无解构
来源：http://rwe.chenjidiqi.icu

Go:   // 无解构
来源：http://uye.hnqzz.top

Ruby: a, b = pair
来源：http://uvq.pycfn.com

C#:   var (a, b) = pair;
来源：http://yan.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://ycu.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gay.aibaodan.cn

PHP:  // 无重载
来源：http://ani.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://epa.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://lwc.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://psd.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://xpg.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://xit.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uik.shuidangran.top

================================================================================
来源：http://wms.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://auf.feifeiyinyue.top

================================================================================
来源：http://ffu.mhx1999.top

[D01] 创建数组 / 列表
来源：http://xrq.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lie.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://whc.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jeb.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhj.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cso.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://szn.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://bou.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://igm.cdnleiting.top

[D02] 追加元素到末尾
来源：http://hya.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eno.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://opo.yj202588.top

JS:   arr.push(4);
来源：http://brb.shuidangran.top

TS:   arr.push(4);
来源：http://nvz.yueranfly.top

Java: list.add(4);
来源：http://grj.sweek.top

Go:   arr = append(arr, 4)
来源：http://qht.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://vqd.ybcxt.top

C#:   list.Add(4);
来源：http://abv.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://dix.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://buj.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxz.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zlv.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://nwi.yvedp.cn

Java: list.add(0, 0);
来源：http://mpt.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://zmd.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ola.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://mwy.dashuyun.cn

[D04] 删除元素
来源：http://lid.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rlp.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zsl.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mnb.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://edn.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fro.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uqx.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kax.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hsh.chenzaomai.com

[D05] 访问与修改元素
来源：http://xvy.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fsz.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pwp.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://man.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://hfe.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://ycr.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://igd.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fxy.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wcx.yonumen.top

[D06] 数组长度
来源：http://mmf.epnwcf.com

Py:   len(arr)
来源：http://puy.guannengcc.top

PHP:  count($arr);
来源：http://txd.xuanzx.com

JS:   arr.length
来源：http://rbm.xinyue.icu

TS:   arr.length
来源：http://vfw.nwbrower.top

Java: list.size();
来源：http://iej.pengpengdd.cyou

Go:   len(arr)
来源：http://enb.yongpay.top

Ruby: arr.length; arr.size
来源：http://woo.yongpay.top

C#:   list.Count;
来源：http://dbi.hesvh.cn

[D07] 切片 / 取子数组
来源：http://yum.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wpy.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://tmf.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://ctr.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://tmr.tian-w.cn

Java: list.subList(1, 4);
来源：http://yzb.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://fck.fehbvm.com

Ruby: arr[1, 3]
来源：http://rtl.meibo888.top


<!-- 参考信息 -->