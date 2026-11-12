代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uea.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvn.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://oov.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kjr.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://ddt.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://jqd.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wim.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dej.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://syh.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eln.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nnl.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://dzm.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://djb.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://exw.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gbh.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zom.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sho.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hio.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://udx.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eum.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xlx.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aoh.yj20258888.top

[B07] while 循环
来源：http://lda.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://elt.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://fci.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://quu.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://srx.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://fzj.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vbq.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://hhs.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://hlj.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://yqu.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://ymz.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ffc.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://tfj.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://lta.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://vxx.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qct.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://dki.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://ekk.svipenyu.cn

[B09] break 与 continue
来源：http://dtm.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kuo.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qom.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adq.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlf.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgc.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fuh.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tvr.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hen.ivvv.top

[B10] 遍历同时拿索引
来源：http://ayk.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddc.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://guz.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hqc.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hhj.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tij.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lxk.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fki.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ukk.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://pbh.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://oae.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://lce.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxc.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://raj.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yto.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ykd.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://odp.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gvv.52xcode.cn

[B12] 跳出多层循环
来源：http://cvv.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wga.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lgp.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wmb.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqj.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vov.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jrc.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gwr.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nky.ivvv.top

[B13] 判断是否为数字
来源：http://vrm.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://cim.jqgfzy.top

PHP:  is_numeric($x)
来源：http://ees.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qec.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cuh.yj20258888.top

Java: x instanceof Number
来源：http://omb.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zot.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://gie.ybcxt.top

C#:   x is int or double or decimal
来源：http://lkh.316326.xyz

[B14] 判断值是否在集合内
来源：http://ude.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hgx.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jdk.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://cpt.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://tzq.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zxf.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ggw.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://mlv.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vdi.xylfe.cn

[B15] 布尔运算与取反
来源：http://ymf.sjlbkw.cn

Py:   a and b or not c
来源：http://jve.havefunace.top

PHP:  $a && $b || !$c
来源：http://dlx.hywenlv.cn

JS:   a && b || !c
来源：http://oeh.yfazqb.com

TS:   a && b || !c
来源：http://atn.dianchejie.cn

Java: a && b || !c
来源：http://wmj.epnwcf.com

Go:   a && b || !c
来源：http://hfk.hcnkem.com

Ruby: a && b || !c
来源：http://jba.sysykeji.top

C#:   a && b || !c
来源：http://men.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://rjm.gaohongyu789.top

Py:   if not data: return
来源：http://tsl.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://huu.0kj1m.cn

JS:   if (!data) return;
来源：http://znm.vehdjk.com

TS:   if (!data) return;
来源：http://yst.zhixingplan.top

Java: if (data == null) return;
来源：http://ewn.jianghu66.top

Go:   if data == nil { return }
来源：http://qkg.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://ott.mhx1999.top

C#:   if (data == null) return;
来源：http://mys.jiagoushi.top

================================================================================
来源：http://fkm.zhiwuduotai.top

C. 函数与作用域
来源：http://bzc.zhoulong.xyz

================================================================================
来源：http://lvo.jinghuilouyu.cn

[C01] 定义函数
来源：http://ecy.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://las.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ker.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://hxp.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzm.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dcq.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cdk.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://jxf.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://izz.xziqi.cn

[C02] 默认参数
来源：http://ldo.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://kzp.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xhs.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://tpk.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vbr.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://rod.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://slv.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://yun.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://vbv.aizwys.cn

[C03] 可变参数
来源：http://ssl.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://gxk.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybi.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dhj.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://axa.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axx.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iui.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://cbj.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jdr.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://qzm.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://due.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zkk.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mpy.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://muh.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://hnx.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://odn.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://brj.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://oum.meibo888.top

[C05] 返回多个值
来源：http://nbu.snrcjt.cn

Py:   return a, b
来源：http://bka.nanxinkj.top

PHP:  return [$a, $b];
来源：http://blk.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://isy.andypj.xyz

TS:   return { a, b };
来源：http://dwp.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ows.vqdsnc.cn

Go:   return a, b
来源：http://adc.ehwqpu.com

Ruby: return a, b
来源：http://nye.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://nuq.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://utn.nwbrower.top

Py:   square = lambda x: x * x
来源：http://njo.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qyu.meibo888.top

JS:   const square = x => x * x;
来源：http://iom.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://nqm.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xfz.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://oni.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://kvv.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://yij.birdmap.top

[C07] 把函数作为参数传入
来源：http://ahr.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://civ.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://wpy.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vxv.nanxinkj.top

TS:   arr.map(String)
来源：http://bfm.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kbo.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lkk.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://pdz.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tvt.chenjidiqi.icu

[C08] 闭包
来源：http://wru.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kzw.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mkd.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rbe.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tra.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://crg.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eei.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ahs.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nez.hesvh.cn

[C09] 递归
来源：http://wxe.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://orr.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vwt.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hja.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpp.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dwf.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://unf.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tdp.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pgs.xuanzx.com

[C10] 变量作用域
来源：http://vgh.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ctd.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gob.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://laq.snrcjt.cn

TS:   同 JS
来源：http://rlf.snrcjt.cn

Java: 方法内为块级作用域
来源：http://cuu.daria6918.cn

Go:   花括号块级作用域
来源：http://dtr.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qli.feifeiyinyue.top

C#:   块级作用域
来源：http://kok.haohaochexian.top

[C11] 模块导入与导出
来源：http://awj.ivvv.top

Py:   from module import func
来源：http://krh.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://vny.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bll.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zoo.hammf.cn

Java: import java.util.List;
来源：http://flw.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gpq.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://sdb.sxryk.cn

C#:   using System.Text;
来源：http://qlk.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://ssg.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://jpd.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://zzv.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://dpn.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://iim.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yko.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://cxi.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://xiq.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lxr.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://anw.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oak.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://glp.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwp.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ozn.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nnx.cucudq.cn

Go:   func add(a, b int) int
来源：http://qsn.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://txo.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://eaw.nwbrower.top

[C14] 泛型函数
来源：http://zzo.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bdv.xylfe.cn

PHP:  // 无泛型
来源：http://stu.yj20258.top

JS:   // 无泛型
来源：http://olr.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ryn.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ptn.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zwm.0kj1m.cn

Ruby: # 无泛型
来源：http://aum.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ldi.redwolf501.top

[C15] 解构 / 展开参数
来源：http://qcv.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fpd.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://dbw.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wff.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sms.mhx1999.top

Java: // 无解构
来源：http://gil.jlsjyb.cn

Go:   // 无解构
来源：http://hqi.jqgufenzy.top

Ruby: a, b = pair
来源：http://exd.vehdjk.com

C#:   var (a, b) = pair;
来源：http://evr.wangdashe.top

[C16] 函数 / 方法重载
来源：http://qdi.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pte.fktsv.cn

PHP:  // 无重载
来源：http://kxx.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lkj.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://aze.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://the.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://rvl.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://cje.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jbb.hnqzz.top

================================================================================
来源：http://oms.316326.xyz

D. 数组 / 列表 / 集合
来源：http://ejk.yfazqb.com

================================================================================
来源：http://biu.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://whx.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://foa.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zdm.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dia.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cqh.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mlx.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://lwu.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://shx.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jjz.snrcjt.cn

[D02] 追加元素到末尾
来源：http://dsr.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://frk.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ahp.316326.xyz

JS:   arr.push(4);
来源：http://kjs.gotoacloud.top

TS:   arr.push(4);
来源：http://qtx.zdqjudy.top

Java: list.add(4);
来源：http://bxl.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://axn.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://mgj.hongshengwenyu.top

C#:   list.Add(4);
来源：http://pue.vehdjk.com

[D03] 在指定位置插入元素
来源：http://mbe.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://dok.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofs.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvi.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://fju.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://tfc.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://azr.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vdw.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://ouz.jyoumei.cn

[D04] 删除元素
来源：http://cqy.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uxg.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lhv.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mli.birdmap.top

TS:   arr.splice(0, 1);
来源：http://nbu.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bdc.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zae.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fcu.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fgg.yueranfly.top

[D05] 访问与修改元素
来源：http://fyx.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://phz.hfpthk.cn


<!-- 参考信息 -->