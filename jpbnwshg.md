代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://pla.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qta.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kdp.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://ctj.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uzb.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://sxb.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://upe.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://odk.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vsz.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjr.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ebh.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fsv.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rnh.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://foa.zhoulong.xyz

[B07] while 循环
来源：http://yoc.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://its.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://krq.sweek.top

JS:   while (i < 10) { i++; }
来源：http://lky.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://mbh.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://ypb.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xbk.yvedp.cn

Ruby: while i < 10; i += 1; end
来源：http://uvm.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://gbj.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://nfi.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://wqk.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://iqy.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://bpy.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://qyy.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://huh.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ejp.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nsy.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://bqb.ctjpmb.com

[B09] break 与 continue
来源：http://nbi.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://neh.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xgq.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftd.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oxi.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyt.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uzo.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pmk.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzv.birdmap.top

[B10] 遍历同时拿索引
来源：http://ogb.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nhs.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pjq.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tmk.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yuh.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pwk.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wii.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ssk.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qsi.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://gxi.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://iot.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://dsh.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mky.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgz.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vka.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ccs.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://pcs.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wpv.jlsjyb.cn

[B12] 跳出多层循环
来源：http://kbr.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ajm.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://brv.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xee.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zea.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efn.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bfq.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qic.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mbm.jinqigufen.top

[B13] 判断是否为数字
来源：http://tey.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://ceu.redwolf501.top

PHP:  is_numeric($x)
来源：http://rci.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aiq.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zeb.gogol.net.cn

Java: x instanceof Number
来源：http://qnt.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yoz.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://ouw.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://jes.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://gtm.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yry.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wpk.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://sjb.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://jvc.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wfb.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qes.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tcc.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xtc.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://wor.shuidangran.top

Py:   a and b or not c
来源：http://gow.gzhubu.top

PHP:  $a && $b || !$c
来源：http://sqj.kuanghao11.cn

JS:   a && b || !c
来源：http://xxj.tianlin.xyz

TS:   a && b || !c
来源：http://qhs.fehbvm.com

Java: a && b || !c
来源：http://qbm.mhx1999.top

Go:   a && b || !c
来源：http://ysy.sxryk.cn

Ruby: a && b || !c
来源：http://rkm.hesvh.cn

C#:   a && b || !c
来源：http://nzp.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qug.yj20258.top

Py:   if not data: return
来源：http://nii.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://xow.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://sjx.dianchejie.cn

TS:   if (!data) return;
来源：http://spo.52xcode.cn

Java: if (data == null) return;
来源：http://dmq.aizwys.cn

Go:   if data == nil { return }
来源：http://iei.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://dgx.havefunace.top

C#:   if (data == null) return;
来源：http://lkr.cqqwz.cn

================================================================================
来源：http://wkv.iojbl.cn

C. 函数与作用域
来源：http://pys.pengpengdd.cyou

================================================================================
来源：http://kza.yj20258888.top

[C01] 定义函数
来源：http://ijt.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://owp.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ros.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://eex.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccz.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xgr.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://bsx.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://mbf.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lmc.ydzc1.top

[C02] 默认参数
来源：http://dea.sweek.top

Py:   def greet(name="World"): return name
来源：http://woy.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xwp.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://wpk.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nna.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sru.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mnm.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://rcf.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://hbq.xinyue.icu

[C03] 可变参数
来源：http://enp.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://hyg.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://smt.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pih.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nhx.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dwp.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kdi.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://bdj.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pds.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://gjs.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ngz.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bdg.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wom.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sea.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://ihq.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://wey.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://hgs.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://jjw.chenlongwang.top

[C05] 返回多个值
来源：http://rjf.jinqigufen.top

Py:   return a, b
来源：http://lte.c1oappe.top

PHP:  return [$a, $b];
来源：http://fxp.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://atp.hcnkem.com

TS:   return { a, b };
来源：http://yap.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fuz.gotoacloud.top

Go:   return a, b
来源：http://icj.jinqigfzy.top

Ruby: return a, b
来源：http://utn.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://nxe.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://sxu.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://jiw.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rnz.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://emv.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://pea.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yeq.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zri.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://fjz.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://aml.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://jkg.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gzo.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://vpd.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bhm.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://hdv.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xmy.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yry.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://lgm.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://htd.zhixingplan.top

[C08] 闭包
来源：http://cso.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kau.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hgu.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xfy.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sat.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zhb.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bix.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oob.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aqf.ydzc1.top

[C09] 递归
来源：http://wzb.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://inf.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qgd.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cvr.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xan.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yjn.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tpa.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qsq.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uvg.meibo888.top

[C10] 变量作用域
来源：http://xab.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rps.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gmz.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://slt.ctjpmb.com

TS:   同 JS
来源：http://waj.guowangkeji.top

Java: 方法内为块级作用域
来源：http://mus.dianchejie.cn

Go:   花括号块级作用域
来源：http://lzg.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ihy.fktsv.cn

C#:   块级作用域
来源：http://pei.birdmap.top

[C11] 模块导入与导出
来源：http://byv.xinyue.icu

Py:   from module import func
来源：http://ljc.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ukv.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://gwe.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tyf.fanxiaobao.xyz

Java: import java.util.List;
来源：http://xwq.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pae.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://ntn.zhengqikj.top

C#:   using System.Text;
来源：http://xox.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://hvi.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://drh.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://xsu.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://zyq.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://pwi.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvu.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://xci.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://gnl.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jkz.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://nzi.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bnn.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rim.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://poo.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ino.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://drz.ppjwa.cn

Go:   func add(a, b int) int
来源：http://pwl.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pqc.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://bwd.gogol.net.cn

[C14] 泛型函数
来源：http://uiw.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://alu.cqqwz.cn

PHP:  // 无泛型
来源：http://ept.jianghu66.top

JS:   // 无泛型
来源：http://cbf.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fzr.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uyq.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lde.xylfe.cn

Ruby: # 无泛型
来源：http://jzf.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://apn.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://vbv.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ziw.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://bkj.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tfr.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gdl.sxryk.cn

Java: // 无解构
来源：http://cii.chenzaomai.com

Go:   // 无解构
来源：http://pof.fktsv.cn

Ruby: a, b = pair
来源：http://rij.yongpay.top

C#:   var (a, b) = pair;
来源：http://axn.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://blz.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xoc.9152youxi.cn

PHP:  // 无重载
来源：http://bbg.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xpg.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://kly.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fef.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://oce.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://uzb.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sby.zhixingplan.top

================================================================================
来源：http://eax.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://vpa.zdqjudy.top

================================================================================
来源：http://wcx.sxryk.cn

[D01] 创建数组 / 列表
来源：http://jte.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ybn.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xvs.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lmh.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://biz.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kgb.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://kau.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://mpc.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rkn.cheryme.top

[D02] 追加元素到末尾
来源：http://uhb.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpc.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qbx.gotoacloud.top

JS:   arr.push(4);
来源：http://shz.hammf.cn

TS:   arr.push(4);
来源：http://gqa.svipenyu.cn

Java: list.add(4);
来源：http://lwq.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://sis.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://jdh.hysaishi.cn

C#:   list.Add(4);
来源：http://rhn.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://mrh.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://pgw.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ijm.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ltm.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://aot.havefunace.top

Java: list.add(0, 0);
来源：http://kmh.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://tyh.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qge.cheryme.top

C#:   list.Insert(0, 0);
来源：http://kgl.hysaishi.cn

[D04] 删除元素
来源：http://ouq.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rpj.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wno.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gsl.yj20258.top

TS:   arr.splice(0, 1);
来源：http://siy.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://djg.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wbd.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yjy.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rpv.ivvv.top

[D05] 访问与修改元素
来源：http://ave.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pqp.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iwm.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pef.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://wkr.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://zrb.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://koh.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rqx.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rkq.havefunace.top

[D06] 数组长度
来源：http://osa.cqqwz.cn


<!-- 参考信息 -->