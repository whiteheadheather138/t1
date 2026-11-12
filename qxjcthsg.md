代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bda.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ecb.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://fau.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oeq.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://ycv.xylfe.cn

Py:   for item in arr: print(item)
来源：http://wvc.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ybs.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vyy.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jhl.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://iie.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mum.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://kxj.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zhz.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://ocj.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://hdt.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rmn.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwj.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yyj.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rmh.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tlp.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nzn.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fpo.jlsjyb.cn

[B07] while 循环
来源：http://ooi.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://bql.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://itq.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://uyj.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://npo.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://wsi.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jev.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://pdv.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://gtz.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://srz.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://mmt.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ipp.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://dtj.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://mkl.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://ocg.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://pwg.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pkv.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://gkq.sufxvd.cn

[B09] break 与 continue
来源：http://zpx.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jym.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ppl.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rye.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpg.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxk.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://huc.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ima.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmx.epnwcf.com

[B10] 遍历同时拿索引
来源：http://yeu.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qow.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jat.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bgf.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hcc.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nol.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kyp.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kab.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqm.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://cda.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://okk.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://tqb.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lok.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auu.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fux.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://skz.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://yej.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://snz.iojbl.cn

[B12] 跳出多层循环
来源：http://vsu.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ggu.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ulx.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpn.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfs.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hxd.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zlo.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sww.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aza.sysykeji.top

[B13] 判断是否为数字
来源：http://lcc.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://lgd.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://gjb.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mmb.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ebq.ehwqpu.com

Java: x instanceof Number
来源：http://stq.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nri.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://rjx.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://iyq.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://prx.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bpv.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zbo.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dtm.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://iaa.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qfv.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gbi.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://zuh.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grf.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://zln.ctjpmb.com

Py:   a and b or not c
来源：http://grd.hnqzz.top

PHP:  $a && $b || !$c
来源：http://rwe.gaohongyu789.top

JS:   a && b || !c
来源：http://ggl.zycfv.cn

TS:   a && b || !c
来源：http://ikl.bbcook.cn

Java: a && b || !c
来源：http://xgl.zhongyouzk.top

Go:   a && b || !c
来源：http://zla.jinqigufen.top

Ruby: a && b || !c
来源：http://fsy.yj20258.top

C#:   a && b || !c
来源：http://hcd.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yax.wangshuangyany.cn

Py:   if not data: return
来源：http://ake.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://cua.zhiwuduotai.top

JS:   if (!data) return;
来源：http://riq.redwolf501.top

TS:   if (!data) return;
来源：http://yev.cucudq.cn

Java: if (data == null) return;
来源：http://uhs.birdmap.top

Go:   if data == nil { return }
来源：http://dtf.bjfxy.top

Ruby: return if data.nil?
来源：http://qxq.daxiang520.top

C#:   if (data == null) return;
来源：http://bbp.yuxming.cn

================================================================================
来源：http://xqm.cdnleiting.top

C. 函数与作用域
来源：http://tkd.sjlbkw.cn

================================================================================
来源：http://bly.hesvh.cn

[C01] 定义函数
来源：http://cnx.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://xya.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evf.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://lst.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hkm.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cvi.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://osq.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://ufe.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xbq.zhongyouzk.top

[C02] 默认参数
来源：http://xcl.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://yhz.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://egp.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://qje.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rrw.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hja.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bbv.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://pft.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://eml.meibo888.top

[C03] 可变参数
来源：http://cki.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://son.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vfr.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkg.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://drg.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gmk.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fjt.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://zxn.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://llb.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://uwh.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://txx.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hdb.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://exo.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://epo.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://spw.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://dxm.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://mxe.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://qzz.vqdsnc.cn

[C05] 返回多个值
来源：http://tbs.jianghu66.top

Py:   return a, b
来源：http://zce.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://ndh.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://lsv.fzhhl.top

TS:   return { a, b };
来源：http://nmk.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://foh.hongshengwenyu.top

Go:   return a, b
来源：http://amy.yongpay.top

Ruby: return a, b
来源：http://ifm.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://jzb.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://nco.smart0.xyz

Py:   square = lambda x: x * x
来源：http://yhf.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gtq.tanke756.top

JS:   const square = x => x * x;
来源：http://rkr.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://rpp.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jtm.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://ykr.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://adz.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gyk.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://mov.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ueu.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zzb.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jpx.sufxvd.cn

TS:   arr.map(String)
来源：http://cxc.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mbd.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nqu.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://ivl.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lff.uphjek.com

[C08] 闭包
来源：http://hzy.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cku.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vrt.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tai.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pry.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zyh.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ftx.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nmt.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zzx.jinghuilouyu.cn

[C09] 递归
来源：http://rya.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kpi.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jne.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnj.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xrm.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fwz.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bkg.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tvl.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tpo.nwbrower.top

[C10] 变量作用域
来源：http://tbs.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kez.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gls.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aqg.birdmap.top

TS:   同 JS
来源：http://wju.ehwqpu.com

Java: 方法内为块级作用域
来源：http://rmz.yangfankeji.com

Go:   花括号块级作用域
来源：http://ruv.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://isq.bbcook.cn

C#:   块级作用域
来源：http://rno.yongpay.top

[C11] 模块导入与导出
来源：http://myz.tianlin.xyz

Py:   from module import func
来源：http://zbc.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xee.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://faz.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bpu.tianlin.xyz

Java: import java.util.List;
来源：http://syq.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qmf.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://qyz.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://yik.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://duk.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://uzr.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://vxg.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://czx.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://pju.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oqw.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://kkt.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://nvk.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uxb.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://twy.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dez.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvh.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dtt.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uxm.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://epp.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://eaf.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qkk.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://dah.yj20258888.top

[C14] 泛型函数
来源：http://xxu.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bah.yfazqb.com

PHP:  // 无泛型
来源：http://elt.xuetiantiany.cn

JS:   // 无泛型
来源：http://efz.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fws.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebl.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fmy.jqgufenzy.top

Ruby: # 无泛型
来源：http://qmb.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bzh.fehbvm.com

[C15] 解构 / 展开参数
来源：http://jhe.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxk.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://nbc.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://teg.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hgy.pengpengdd.cyou

Java: // 无解构
来源：http://izn.tian-w.cn

Go:   // 无解构
来源：http://vef.fzhhl.top

Ruby: a, b = pair
来源：http://iof.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://yty.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://noo.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://byj.yfazqb.com

PHP:  // 无重载
来源：http://hqi.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gmn.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://xmk.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xmt.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://wjr.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://xoq.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://axg.aizwys.cn

================================================================================
来源：http://ibe.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://llk.epnwcf.com

================================================================================
来源：http://yor.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://aes.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tbj.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zyf.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://siv.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://arc.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fch.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://snv.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://ezi.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ojn.cqqwz.cn

[D02] 追加元素到末尾
来源：http://ejv.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://boa.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zxb.gotoacloud.top

JS:   arr.push(4);
来源：http://fuw.mhx1999.top

TS:   arr.push(4);
来源：http://ysa.ybcxt.top

Java: list.add(4);
来源：http://riv.yj202588.top

Go:   arr = append(arr, 4)
来源：http://dnn.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://whf.meibo888.top

C#:   list.Add(4);
来源：http://egn.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://phb.yj202588.top

Py:   arr.insert(0, 0)
来源：http://szw.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xoj.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npq.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://dxv.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://aug.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://boo.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uvw.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://ijm.yvedp.cn

[D04] 删除元素
来源：http://jmf.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pyp.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bzm.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fyd.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://amt.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vnq.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qjm.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wmc.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hij.bjfxy.top

[D05] 访问与修改元素
来源：http://qxw.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://keg.bbcook.cn


<!-- 参考信息 -->