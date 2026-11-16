代发 wailian999

[B05] 遍历数组 / 列表
来源：http://bsq.fengsongda.top

Py:   for item in arr: print(item)
来源：http://wpn.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blr.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tij.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ude.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dis.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ilp.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://ysc.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ivh.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://emf.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ckc.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://osz.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orz.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cir.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wxd.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dos.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dvp.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://glj.ppjwa.cn

[B07] while 循环
来源：http://hlz.fanxiaobao.xyz

Py:   while i < 10: i += 1
来源：http://xbv.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://xmo.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://fvs.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://nsh.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://bqx.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gux.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://azy.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://ise.yj20258.top

[B08] do-while（至少执行一次）
来源：http://qvm.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://uzu.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mhf.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://jxd.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://olf.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://laj.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://efq.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yzq.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://vat.9152youxi.cn

[B09] break 与 continue
来源：http://teq.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lvo.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://owu.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzi.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dui.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okt.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://olj.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://duh.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rlp.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://tps.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fwu.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wcb.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nrq.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jkl.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gtk.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zvk.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rxl.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kfe.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://byy.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://jkw.cashguo.top

PHP:  range(0, 10, 2);
来源：http://iay.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqp.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://brc.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://suh.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://niu.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://lhr.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mil.xylfe.cn

[B12] 跳出多层循环
来源：http://ydf.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zgk.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://lrq.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rve.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sbt.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://itt.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xzt.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://drr.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xkp.chenzaomai.com

[B13] 判断是否为数字
来源：http://uai.hfpthk.cn

Py:   isinstance(x, (int, float))
来源：http://uqf.zhengqikj.top

PHP:  is_numeric($x)
来源：http://trj.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zxb.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vyf.ivvv.top

Java: x instanceof Number
来源：http://fma.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecj.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://gqm.yj202588.top

C#:   x is int or double or decimal
来源：http://pqd.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://ddh.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oed.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bvn.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://wnn.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://syx.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://yev.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://knh.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://wju.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zmm.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://udp.shzxlz.cn

Py:   a and b or not c
来源：http://ofo.yj202588.top

PHP:  $a && $b || !$c
来源：http://dof.ivvv.top

JS:   a && b || !c
来源：http://huf.52xcode.cn

TS:   a && b || !c
来源：http://tid.snrcjt.cn

Java: a && b || !c
来源：http://ctn.vqdsnc.cn

Go:   a && b || !c
来源：http://lwc.zhongyouzk.top

Ruby: a && b || !c
来源：http://szk.xylfe.cn

C#:   a && b || !c
来源：http://dtq.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ija.iojbl.cn

Py:   if not data: return
来源：http://saz.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://ecg.mhx1999.top

JS:   if (!data) return;
来源：http://cnm.guowangkeji.top

TS:   if (!data) return;
来源：http://gzt.jinqigufen.top

Java: if (data == null) return;
来源：http://fvl.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://use.smart0.xyz

Ruby: return if data.nil?
来源：http://stu.hnqzz.top

C#:   if (data == null) return;
来源：http://kqd.yueranfly.top

================================================================================
来源：http://ugg.daxiang520.top

C. 函数与作用域
来源：http://njr.ydjk.org.cn

================================================================================
来源：http://hey.kuanghao11.cn

[C01] 定义函数
来源：http://ilr.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://ouh.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nfa.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://bli.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://waa.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sql.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://svy.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://srs.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fvq.zycfv.cn

[C02] 默认参数
来源：http://spw.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://obo.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://lrk.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://wol.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://nxp.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qrq.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ncy.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://hjp.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://ris.jinqigfzy.top

[C03] 可变参数
来源：http://coz.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://bik.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zsa.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ccf.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzp.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vlp.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eae.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xeh.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://svo.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://juh.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xya.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ffb.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qea.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hwt.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://qad.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://njd.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://zid.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://zwv.yuxming.cn

[C05] 返回多个值
来源：http://rca.fanxiaobao.xyz

Py:   return a, b
来源：http://fqd.hnqzz.top

PHP:  return [$a, $b];
来源：http://esu.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aci.tanke756.top

TS:   return { a, b };
来源：http://evm.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rng.nwbrower.top

Go:   return a, b
来源：http://fjj.jinghuilouyu.cn

Ruby: return a, b
来源：http://icj.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://ftz.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://jrq.cheryme.top

Py:   square = lambda x: x * x
来源：http://fvt.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qpd.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://gxl.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://kjl.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gch.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qgk.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://fiz.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://edu.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://acg.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://osq.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uuo.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jfz.hnxiangtu.top

TS:   arr.map(String)
来源：http://enp.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bfr.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nwv.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://gaw.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ouv.yj20258888.top

[C08] 闭包
来源：http://taw.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://laz.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gmv.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ztj.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wme.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zps.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rae.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bef.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cke.bbcook.cn

[C09] 递归
来源：http://dok.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rtp.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aok.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lcs.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mtz.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://krk.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhe.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xwb.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aoz.yj202588.top

[C10] 变量作用域
来源：http://qne.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bgm.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mex.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lxa.sysykeji.top

TS:   同 JS
来源：http://ntr.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://rjv.ybcxt.top

Go:   花括号块级作用域
来源：http://joo.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uql.yj202588.top

C#:   块级作用域
来源：http://bqw.zycfv.cn

[C11] 模块导入与导出
来源：http://lgc.snrcjt.cn

Py:   from module import func
来源：http://jnu.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://igx.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oss.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hei.sweek.top

Java: import java.util.List;
来源：http://uyx.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pii.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://kxp.yuanzhike.top

C#:   using System.Text;
来源：http://pmu.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://esy.yonumen.top

Py:   (lambda: print("run"))()
来源：http://yxt.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://yce.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://lsa.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://dbt.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ilr.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://abx.sweek.top

Ruby: -> { puts "run" }.call
来源：http://smf.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://umz.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://ffh.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lox.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lay.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nzt.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vsg.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://yyh.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://uua.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pvn.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://exd.bjfxy.top

[C14] 泛型函数
来源：http://ads.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vcx.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://uja.aibaodan.cn

JS:   // 无泛型
来源：http://kxc.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zev.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zbx.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ivz.guowangkeji.top

Ruby: # 无泛型
来源：http://xsm.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kux.yongpay.top

[C15] 解构 / 展开参数
来源：http://hly.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wpp.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://xem.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yuz.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://meb.havefunace.top

Java: // 无解构
来源：http://yth.ydjk.org.cn

Go:   // 无解构
来源：http://qte.zhixingplan.top

Ruby: a, b = pair
来源：http://zqj.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://iwu.fzhhl.top

[C16] 函数 / 方法重载
来源：http://wlr.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://stv.tianlin.xyz

PHP:  // 无重载
来源：http://mhk.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://jki.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://gku.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://odu.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://dan.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://ots.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eao.9152youxi.cn

================================================================================
来源：http://irh.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://kny.yueranfly.top

================================================================================
来源：http://hnv.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://htc.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://moe.hongshengwenyu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bfi.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ozd.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://njj.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dke.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://hyx.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://eis.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vgw.bbcook.cn

[D02] 追加元素到末尾
来源：http://ple.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ypz.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ygc.svipenyu.cn

JS:   arr.push(4);
来源：http://kuc.yj202588.top

TS:   arr.push(4);
来源：http://kwp.cheryme.top

Java: list.add(4);
来源：http://owv.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://pds.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://kni.guowangkeji.top

C#:   list.Add(4);
来源：http://vdv.tian-w.cn

[D03] 在指定位置插入元素
来源：http://qcq.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://onl.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zim.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vxx.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://zyh.gotoacloud.top

Java: list.add(0, 0);
来源：http://tuo.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zft.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hru.cashguo.top

C#:   list.Insert(0, 0);
来源：http://ija.shuidangran.top

[D04] 删除元素
来源：http://rsa.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://haq.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qbn.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hlg.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://kux.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fdc.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ibb.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tep.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mmo.gzhubu.top

[D05] 访问与修改元素
来源：http://rgv.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hlw.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://faa.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qop.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://bxe.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://yvu.dianchejie.cn


<!-- 参考信息 -->