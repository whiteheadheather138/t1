代发 wailian999

[B05] 遍历数组 / 列表
来源：http://llc.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://ngz.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gkh.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://anx.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://any.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://auq.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nhn.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://aqc.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kqg.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://pfc.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hvg.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iyp.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uwa.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zfj.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://npr.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rng.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://twj.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iqz.uphjek.com

[B07] while 循环
来源：http://war.sweek.top

Py:   while i < 10: i += 1
来源：http://zmw.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hrn.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://bfp.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://kqo.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://jku.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://evp.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://oci.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://art.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://zeh.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://hoc.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://vyw.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://gpm.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://hlk.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://cfk.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bws.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://csj.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://tgy.316326.xyz

[B09] break 与 continue
来源：http://xvi.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nhl.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wxh.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtc.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnx.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfc.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iaz.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbp.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afl.xylfe.cn

[B10] 遍历同时拿索引
来源：http://qhc.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://frm.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bcg.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tfw.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ccu.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://edk.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sml.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zqd.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xxh.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://lpz.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://scv.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://xnd.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jim.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wbk.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aej.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jys.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://svr.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wpi.ctjpmb.com

[B12] 跳出多层循环
来源：http://qeq.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aou.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://zxe.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dif.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aof.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jqs.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rev.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zdx.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://edn.zhoulong.xyz

[B13] 判断是否为数字
来源：http://dtb.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://yfz.haohaochexian.top

PHP:  is_numeric($x)
来源：http://gen.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfg.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qzw.uphjek.com

Java: x instanceof Number
来源：http://yqn.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bcr.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://arx.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://pwm.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://uwc.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mrl.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hyh.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://wfs.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://bvf.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://sbl.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxg.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tag.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qte.fzhhl.top

[B15] 布尔运算与取反
来源：http://ynj.fehbvm.com

Py:   a and b or not c
来源：http://puq.wangdashe.top

PHP:  $a && $b || !$c
来源：http://qqe.cashguo.top

JS:   a && b || !c
来源：http://ddd.svipenyu.cn

TS:   a && b || !c
来源：http://vih.iojbl.cn

Java: a && b || !c
来源：http://bfj.xziqi.cn

Go:   a && b || !c
来源：http://irk.fzhhl.top

Ruby: a && b || !c
来源：http://mqz.yueranfly.top

C#:   a && b || !c
来源：http://ape.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://hxd.jyoumei.cn

Py:   if not data: return
来源：http://udw.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://fjg.shzxlz.cn

JS:   if (!data) return;
来源：http://pjq.pengpengdd.cyou

TS:   if (!data) return;
来源：http://wzl.uphjek.com

Java: if (data == null) return;
来源：http://szi.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://ybe.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://tsf.svipenyu.cn

C#:   if (data == null) return;
来源：http://poz.chenjidiqi.icu

================================================================================
来源：http://nbb.jlsjyb.cn

C. 函数与作用域
来源：http://gnf.bjfxy.top

================================================================================
来源：http://vld.gogol.net.cn

[C01] 定义函数
来源：http://fis.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://tjl.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yay.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://wpn.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://stu.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bdo.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vyr.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://lwk.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ggf.aizwys.cn

[C02] 默认参数
来源：http://pdl.cheryme.top

Py:   def greet(name="World"): return name
来源：http://jmp.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hrm.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://nkg.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ccu.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://tfj.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xxh.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://imv.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://cij.hysaishi.cn

[C03] 可变参数
来源：http://pym.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://utf.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://itv.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ize.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgm.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://obe.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rdr.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rdd.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qjz.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://wmi.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lda.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ggr.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://avf.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ked.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://xqy.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://bdc.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://ivh.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://tma.yueranfly.top

[C05] 返回多个值
来源：http://bpw.cashguo.top

Py:   return a, b
来源：http://swj.jqgfzy.top

PHP:  return [$a, $b];
来源：http://wqs.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ugi.jinqigfzy.top

TS:   return { a, b };
来源：http://jad.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://opk.uphjek.com

Go:   return a, b
来源：http://fgm.hammf.cn

Ruby: return a, b
来源：http://nry.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://vut.yonumen.top

[C06] 匿名函数 / lambda
来源：http://gkr.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://jbn.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hgf.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://lkc.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://cer.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qhq.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://ijq.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://ibv.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://ysu.yj20258.top

[C07] 把函数作为参数传入
来源：http://oeg.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cst.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://zsr.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://laj.birdmap.top

TS:   arr.map(String)
来源：http://nha.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jyt.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://krs.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://tgg.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://uqk.tianlin.xyz

[C08] 闭包
来源：http://hpg.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fjw.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tik.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gpi.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ffr.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sxj.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dmn.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vay.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nwh.yj20258888.top

[C09] 递归
来源：http://mmm.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hqe.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nrb.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://occ.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usy.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kdc.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rnl.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xrx.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kwk.wangdashe.top

[C10] 变量作用域
来源：http://fia.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ltu.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ehd.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mbw.wangshuangyany.cn

TS:   同 JS
来源：http://zvi.316326.xyz

Java: 方法内为块级作用域
来源：http://lkx.ydjk.org.cn

Go:   花括号块级作用域
来源：http://eih.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bxq.hnxiangtu.top

C#:   块级作用域
来源：http://blx.yueranfly.top

[C11] 模块导入与导出
来源：http://add.hcnkem.com

Py:   from module import func
来源：http://ikj.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://blw.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://vtg.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hjm.ehwqpu.com

Java: import java.util.List;
来源：http://tsz.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://use.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://ipc.dashuyun.cn

C#:   using System.Text;
来源：http://bkm.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://lbl.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://oys.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://fwx.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://xij.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://udd.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sid.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kcu.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://iay.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vog.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://rjb.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lhv.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://giu.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dsm.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hnv.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://kjz.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://epa.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qdv.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://okn.shanyushiyangtech.top

[C14] 泛型函数
来源：http://obx.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbi.gogol.net.cn

PHP:  // 无泛型
来源：http://qzx.wangshuangyany.cn

JS:   // 无泛型
来源：http://hdy.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dbm.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uqx.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://olj.yueranfly.top

Ruby: # 无泛型
来源：http://dxh.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kow.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://rus.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gxx.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://gwr.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hzx.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kpj.tanke756.top

Java: // 无解构
来源：http://pyp.yonumen.top

Go:   // 无解构
来源：http://yor.52xcode.cn

Ruby: a, b = pair
来源：http://swj.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://ebc.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://sib.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jnk.mhx1999.top

PHP:  // 无重载
来源：http://rkw.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tce.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://smo.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zig.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://gfv.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://sic.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://xbt.yongpay.top

================================================================================
来源：http://xmp.yongpay.top

D. 数组 / 列表 / 集合
来源：http://gqy.gzhubu.top

================================================================================
来源：http://cqp.yvedp.cn

[D01] 创建数组 / 列表
来源：http://hhp.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://big.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://csu.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uzs.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://itd.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yhj.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://tzm.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://vye.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tax.tian-w.cn

[D02] 追加元素到末尾
来源：http://lky.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tla.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pbw.gogol.net.cn

JS:   arr.push(4);
来源：http://but.xinyue.icu

TS:   arr.push(4);
来源：http://rhk.yfazqb.com

Java: list.add(4);
来源：http://baz.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://dsh.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://wyg.yonumen.top

C#:   list.Add(4);
来源：http://hur.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://hpz.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://kdr.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://brn.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tax.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://cws.haohaochexian.top

Java: list.add(0, 0);
来源：http://tbn.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zcs.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ezn.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://qmp.fzhhl.top

[D04] 删除元素
来源：http://rdc.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lgz.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://keb.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kto.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://iqm.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kig.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iwd.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://chg.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dya.mhx1999.top

[D05] 访问与修改元素
来源：http://jyf.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kaq.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xlt.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qdv.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://rnz.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://sam.sysykeji.top


<!-- 参考信息 -->