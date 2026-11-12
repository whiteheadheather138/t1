代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://dzj.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zpd.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://xao.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cex.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://rwr.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://lhd.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ene.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hre.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzw.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nsi.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hvp.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tlb.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://umh.ivvv.top

[B07] while 循环
来源：http://dke.xziqi.cn

Py:   while i < 10: i += 1
来源：http://vdp.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://qfj.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://avm.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://bhs.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://mzq.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ehw.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://wes.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://wad.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://zbm.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://jwc.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://csa.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://eir.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://hmh.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://ozk.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gks.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://lhl.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://egn.zhijiandao.cn

[B09] break 与 continue
来源：http://kml.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fxy.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qbh.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzk.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zub.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://naw.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhr.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aqo.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dcv.xylfe.cn

[B10] 遍历同时拿索引
来源：http://jgk.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wnx.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jyi.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rlo.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tur.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpy.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qsv.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xds.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jol.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://xvx.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://dvq.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://vbu.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://upe.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aom.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vvw.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ohp.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://kho.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikz.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://ldk.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://loc.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqa.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://phs.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcu.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vxc.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xjv.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ewf.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://siq.9152youxi.cn

[B13] 判断是否为数字
来源：http://ozd.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://hty.cucudq.cn

PHP:  is_numeric($x)
来源：http://snh.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jtl.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xaq.yvedp.cn

Java: x instanceof Number
来源：http://bdh.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qdm.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://lsw.xylfe.cn

C#:   x is int or double or decimal
来源：http://joa.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://woj.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ffw.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mgl.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://dgw.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://hqh.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bri.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uxs.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://slc.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hym.yangfankeji.com

[B15] 布尔运算与取反
来源：http://skr.zhongyouzk.top

Py:   a and b or not c
来源：http://ywx.cucudq.cn

PHP:  $a && $b || !$c
来源：http://jmk.nanxuanxn.top

JS:   a && b || !c
来源：http://vjo.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://ywt.dashuyun.cn

Java: a && b || !c
来源：http://fmy.snrcjt.cn

Go:   a && b || !c
来源：http://hzb.zhoulong.xyz

Ruby: a && b || !c
来源：http://kdt.mhx1999.top

C#:   a && b || !c
来源：http://rom.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://gdz.jinqigfzy.top

Py:   if not data: return
来源：http://mtg.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://zih.tianlin.xyz

JS:   if (!data) return;
来源：http://lft.zdbjq.cn

TS:   if (!data) return;
来源：http://eqc.haohaochexian.top

Java: if (data == null) return;
来源：http://obe.hysaishi.cn

Go:   if data == nil { return }
来源：http://hxp.redwolf501.top

Ruby: return if data.nil?
来源：http://pvi.fzhhl.top

C#:   if (data == null) return;
来源：http://ngi.ybcxt.top

================================================================================
来源：http://kze.sxryk.cn

C. 函数与作用域
来源：http://gfh.bbcook.cn

================================================================================
来源：http://qhr.zhaomingkeji.xyz

[C01] 定义函数
来源：http://qcb.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://yxq.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inf.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://tdj.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jjx.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wjx.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lkb.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://mfc.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://win.jinghuilouyu.cn

[C02] 默认参数
来源：http://cmf.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://vtf.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kke.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://wyq.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://imk.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lrv.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ypy.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://abo.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://osp.0kj1m.cn

[C03] 可变参数
来源：http://etm.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://vgo.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xkq.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://myz.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lad.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uzu.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vfw.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rcm.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vvc.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://vzo.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dtd.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://egj.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rxv.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ldf.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://jsn.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://lpe.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://mqt.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://cgk.gaohongyu789.top

[C05] 返回多个值
来源：http://idq.svipenyu.cn

Py:   return a, b
来源：http://edh.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://eba.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fon.hysaishi.cn

TS:   return { a, b };
来源：http://qnd.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aht.bjfxy.top

Go:   return a, b
来源：http://gpf.fktsv.cn

Ruby: return a, b
来源：http://jng.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://gen.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://qer.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://jyn.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://err.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://oyr.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://grb.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dib.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://hke.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://pah.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://qaa.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://adh.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gzr.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nin.zhiwuduotai.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hme.xuetiantiany.cn

TS:   arr.map(String)
来源：http://kul.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://epu.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://evx.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://llr.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jov.wangdashe.top

[C08] 闭包
来源：http://jft.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wim.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dek.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://byy.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mns.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gbf.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlb.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ieq.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vbh.zhiwuduotai.top

[C09] 递归
来源：http://zcv.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rgk.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gcr.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dyz.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://idj.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xwn.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hnu.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jfi.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qzq.nanxuanxn.top

[C10] 变量作用域
来源：http://bwo.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zds.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mpd.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sme.wangshuangyany.cn

TS:   同 JS
来源：http://azg.yuanzhike.top

Java: 方法内为块级作用域
来源：http://loq.fehbvm.com

Go:   花括号块级作用域
来源：http://rtd.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://poj.tarul.cn

C#:   块级作用域
来源：http://tdy.yueranfly.top

[C11] 模块导入与导出
来源：http://rhw.zdqjudy.top

Py:   from module import func
来源：http://ywr.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dqc.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cxo.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://api.dashuyun.cn

Java: import java.util.List;
来源：http://opw.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lan.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://ctv.yangfankeji.com

C#:   using System.Text;
来源：http://ati.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://mxo.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://lfi.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://jbd.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://igy.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://rch.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwe.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://ltp.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ixx.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kty.sweek.top

[C13] 类型声明 / 类型注解
来源：http://mts.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tbx.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ocz.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mpr.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txs.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nyx.ydzc1.top

Go:   func add(a, b int) int
来源：http://fof.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebg.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zxp.yfazqb.com

[C14] 泛型函数
来源：http://xdw.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wvq.guowangkeji.top

PHP:  // 无泛型
来源：http://pnn.haohaochexian.top

JS:   // 无泛型
来源：http://hhw.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vac.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mji.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fjj.yueranfly.top

Ruby: # 无泛型
来源：http://kmg.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ted.gotoacloud.top

[C15] 解构 / 展开参数
来源：http://oyh.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hvn.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://bve.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hhk.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nhk.yj20258888.top

Java: // 无解构
来源：http://pdz.316326.xyz

Go:   // 无解构
来源：http://pqs.sysykeji.top

Ruby: a, b = pair
来源：http://pgy.sweek.top

C#:   var (a, b) = pair;
来源：http://gtz.c1oappe.top

[C16] 函数 / 方法重载
来源：http://aui.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nol.sjlbkw.cn

PHP:  // 无重载
来源：http://tod.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wyk.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://ite.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xrr.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://oxs.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://gla.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kky.jiagoushi.top

================================================================================
来源：http://fws.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://aom.fktsv.cn

================================================================================
来源：http://bng.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://dut.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ziw.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jlv.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://onj.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://noz.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rkk.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://dzw.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://cyt.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://htq.hysaishi.cn

[D02] 追加元素到末尾
来源：http://cbd.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hrb.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lmw.haohaochexian.top

JS:   arr.push(4);
来源：http://vok.yongpay.top

TS:   arr.push(4);
来源：http://yiz.zhixingplan.top

Java: list.add(4);
来源：http://jov.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://edx.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://szd.svipenyu.cn

C#:   list.Add(4);
来源：http://yej.yfazqb.com

[D03] 在指定位置插入元素
来源：http://rje.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://nza.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qui.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ehp.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://rlc.bbcook.cn

Java: list.add(0, 0);
来源：http://odj.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://twd.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qwr.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://tmz.birdmap.top

[D04] 删除元素
来源：http://wje.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yoy.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://thm.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lov.hammf.cn

TS:   arr.splice(0, 1);
来源：http://fiw.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bxd.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://khq.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cwi.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uuf.c1oappe.top

[D05] 访问与修改元素
来源：http://ujz.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bsw.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mkn.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xyy.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://goj.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://oaj.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://oqg.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iit.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nuf.fktsv.cn

[D06] 数组长度
来源：http://oqc.shangyingyoupin.top


<!-- 参考信息 -->