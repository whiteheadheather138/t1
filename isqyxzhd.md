代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://awo.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sdm.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gkd.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://lfz.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kvv.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://yig.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qil.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://umq.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pka.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vpp.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pug.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vcj.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cwv.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bmr.c1oappe.top

[B07] while 循环
来源：http://add.yj20258888.top

Py:   while i < 10: i += 1
来源：http://azp.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://dns.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://mec.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://igo.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://wey.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pxl.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://bco.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://gfq.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://spw.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://snm.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gwe.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://jmm.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://qpe.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://bok.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rpv.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://lrj.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://drx.yvedp.cn

[B09] break 与 continue
来源：http://zeo.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tgy.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfj.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjv.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://frn.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzc.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://son.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rpn.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dch.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://lcj.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iuu.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pej.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szd.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://djj.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ivv.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wwo.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://otu.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lhw.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://ixu.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://vav.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://vza.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdp.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uov.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pjp.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://snr.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://mmf.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://was.jinqigfzy.top

[B12] 跳出多层循环
来源：http://bha.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://moa.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ria.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vly.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ynj.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lts.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dnm.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kjo.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hec.jinqigufen.top

[B13] 判断是否为数字
来源：http://vgg.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://tkq.ivvv.top

PHP:  is_numeric($x)
来源：http://tvb.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pad.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://enj.gaohongyu789.top

Java: x instanceof Number
来源：http://hsi.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zyk.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://mhr.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://ndx.bbcook.cn

[B14] 判断值是否在集合内
来源：http://gkx.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fwa.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tsq.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://ctg.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://rgj.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wdt.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sul.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mwt.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nit.chenlongwang.top

[B15] 布尔运算与取反
来源：http://znz.cashguo.top

Py:   a and b or not c
来源：http://uve.yj20258888.top

PHP:  $a && $b || !$c
来源：http://pur.gzhubu.top

JS:   a && b || !c
来源：http://qxi.jqgfzy.top

TS:   a && b || !c
来源：http://fvl.wangdashe.top

Java: a && b || !c
来源：http://vzd.guowangkeji.top

Go:   a && b || !c
来源：http://nyf.cashguo.top

Ruby: a && b || !c
来源：http://rum.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://bep.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://bwx.haohaochexian.top

Py:   if not data: return
来源：http://dhb.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://sxv.cheryme.top

JS:   if (!data) return;
来源：http://blq.nanxinkj.top

TS:   if (!data) return;
来源：http://fjp.gzhubu.top

Java: if (data == null) return;
来源：http://ugc.birdmap.top

Go:   if data == nil { return }
来源：http://mxz.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://mse.hnqzz.top

C#:   if (data == null) return;
来源：http://ffv.zycfv.cn

================================================================================
来源：http://uri.xylfe.cn

C. 函数与作用域
来源：http://uyi.jinghuilouyu.cn

================================================================================
来源：http://rbu.shanyushiyangtech.top

[C01] 定义函数
来源：http://uqc.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://ajf.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ecr.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://fxi.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wom.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jfh.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fey.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://lpa.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qyy.svipenyu.cn

[C02] 默认参数
来源：http://xkf.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://hol.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://daa.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://foi.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vvg.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qda.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aqp.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://pfk.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://kek.hnqzz.top

[C03] 可变参数
来源：http://uwv.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://cbz.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uvr.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nls.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://woc.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gdt.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bbe.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://koz.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rkm.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://fla.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ccc.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pgx.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bwn.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dvk.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://cfq.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://ezk.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://ete.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://xjc.hysaishi.cn

[C05] 返回多个值
来源：http://xse.tian-w.cn

Py:   return a, b
来源：http://cxp.bbcook.cn

PHP:  return [$a, $b];
来源：http://oxs.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eeg.hywenlv.cn

TS:   return { a, b };
来源：http://xkn.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wkm.ywan-chungtsiang.top

Go:   return a, b
来源：http://usm.xziqi.cn

Ruby: return a, b
来源：http://rwd.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://mpz.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://ryh.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://jjg.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cjc.jyoumei.cn

JS:   const square = x => x * x;
来源：http://igl.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://gyf.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://phd.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://hps.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://fxu.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://osl.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://cck.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yzl.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hqj.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rpr.fengsongda.top

TS:   arr.map(String)
来源：http://ozx.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://udp.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rzo.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://cag.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hwe.jlsjyb.cn

[C08] 闭包
来源：http://xbn.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://agb.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rmf.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cet.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gur.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://obm.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wwo.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uan.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ywu.ybcxt.top

[C09] 递归
来源：http://rij.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nqj.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zui.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://guv.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ywx.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tgh.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rgo.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dhe.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cgf.yonumen.top

[C10] 变量作用域
来源：http://uml.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tgl.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://doc.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cqt.yvedp.cn

TS:   同 JS
来源：http://fic.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://qgr.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://wrq.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://esj.pycfn.com

C#:   块级作用域
来源：http://ggr.yangfankeji.com

[C11] 模块导入与导出
来源：http://xuy.birdmap.top

Py:   from module import func
来源：http://ugj.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kbc.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hvh.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pue.redwolf501.top

Java: import java.util.List;
来源：http://qcp.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zun.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://ifo.meibo888.top

C#:   using System.Text;
来源：http://kbc.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://xpl.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://kov.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://umr.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://odb.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://jcw.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mke.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://qdq.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://mku.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hek.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://ffi.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bhn.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgs.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zmo.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nus.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://hjr.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://gve.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kke.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://jwe.zdqjudy.top

[C14] 泛型函数
来源：http://lio.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkv.shangyingyoupin.top

PHP:  // 无泛型
来源：http://ngv.tarul.cn

JS:   // 无泛型
来源：http://nmy.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mex.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tgh.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pwf.birdmap.top

Ruby: # 无泛型
来源：http://nmw.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cxm.pycfn.com

[C15] 解构 / 展开参数
来源：http://adv.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yct.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://uoq.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fkv.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ufb.yj202588.top

Java: // 无解构
来源：http://wfw.9152youxi.cn

Go:   // 无解构
来源：http://jgp.tanke756.top

Ruby: a, b = pair
来源：http://cps.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://bky.fehbvm.com

[C16] 函数 / 方法重载
来源：http://xut.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mmu.ydzc1.top

PHP:  // 无重载
来源：http://bya.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nmz.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://rhx.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ove.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://saz.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://fvf.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qtw.aizwys.cn

================================================================================
来源：http://rpq.316326.xyz

D. 数组 / 列表 / 集合
来源：http://qst.wangdashe.top

================================================================================
来源：http://yvl.hnqzz.top

[D01] 创建数组 / 列表
来源：http://bam.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fpz.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://unq.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://utv.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://feu.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fzj.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://mqc.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://wah.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nlc.zdbjq.cn

[D02] 追加元素到末尾
来源：http://cvy.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xft.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jde.ivvv.top

JS:   arr.push(4);
来源：http://yxz.fehbvm.com

TS:   arr.push(4);
来源：http://qmf.sysykeji.top

Java: list.add(4);
来源：http://tzv.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://mrw.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://evo.cqqwz.cn

C#:   list.Add(4);
来源：http://jsm.andypj.xyz

[D03] 在指定位置插入元素
来源：http://smr.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://rcd.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wjo.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://der.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://eeg.shuidangran.top

Java: list.add(0, 0);
来源：http://tsf.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ubf.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rhk.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://nmk.wangshuangyany.cn

[D04] 删除元素
来源：http://doo.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kjt.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tef.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rtw.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://vdz.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://njr.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hib.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrw.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zof.jinqigfzy.top

[D05] 访问与修改元素
来源：http://ueh.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sgv.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kcn.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://anq.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://vuo.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://ctc.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://rdq.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rnz.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yhe.ybcxt.top

[D06] 数组长度
来源：http://zgc.xuetiantiany.cn


<!-- 参考信息 -->