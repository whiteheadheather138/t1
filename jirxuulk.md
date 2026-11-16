代发 wailian999

[B05] 遍历数组 / 列表
来源：http://brp.birdmap.top

Py:   for item in arr: print(item)
来源：http://kwb.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mho.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dds.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://orh.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wzq.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://srz.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://mby.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ddz.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://qbr.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bww.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jzy.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bxc.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uuf.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vsf.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jcs.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iiy.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oze.sufxvd.cn

[B07] while 循环
来源：http://thg.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://hgs.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ulr.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://gqp.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://qya.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://jtx.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dbi.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://otq.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://yxg.sweek.top

[B08] do-while（至少执行一次）
来源：http://gop.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://lct.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bzz.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://hom.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://ank.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://hem.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://keo.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://scp.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://muq.jianghu66.top

[B09] break 与 continue
来源：http://jny.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://otx.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pci.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mhk.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrm.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbz.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pjt.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dok.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybf.yueranfly.top

[B10] 遍历同时拿索引
来源：http://rmj.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pef.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nve.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmu.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://smi.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qey.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhj.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kci.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jzm.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://pko.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://zxf.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://xlz.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://imk.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://alt.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://khz.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://quv.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://rxb.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kae.tian-w.cn

[B12] 跳出多层循环
来源：http://fis.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kng.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sxg.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oib.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yeh.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aiv.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oox.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://awp.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://asa.yonumen.top

[B13] 判断是否为数字
来源：http://zep.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://wjj.vehdjk.com

PHP:  is_numeric($x)
来源：http://xoc.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxr.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eqp.tianlin.xyz

Java: x instanceof Number
来源：http://cli.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zpg.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://gid.cdnleiting.top

C#:   x is int or double or decimal
来源：http://bap.gzhubu.top

[B14] 判断值是否在集合内
来源：http://dwq.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kvz.chenzaomai.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gqz.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://akx.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://bmg.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yep.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xqg.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://sxz.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uvv.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://rvs.tarul.cn

Py:   a and b or not c
来源：http://jzb.316326.xyz

PHP:  $a && $b || !$c
来源：http://icj.zycfv.cn

JS:   a && b || !c
来源：http://uis.yongpay.top

TS:   a && b || !c
来源：http://nyh.fehbvm.com

Java: a && b || !c
来源：http://dti.vehdjk.com

Go:   a && b || !c
来源：http://tjh.haohaochexian.top

Ruby: a && b || !c
来源：http://kyg.redwolf501.top

C#:   a && b || !c
来源：http://epy.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qqv.jqgufenzy.top

Py:   if not data: return
来源：http://kmh.hammf.cn

PHP:  if (!$data) { return; }
来源：http://com.zhoulong.xyz

JS:   if (!data) return;
来源：http://lwm.havefunace.top

TS:   if (!data) return;
来源：http://hcw.kuanghao11.cn

Java: if (data == null) return;
来源：http://nsv.daxiang520.top

Go:   if data == nil { return }
来源：http://mff.jqgfzy.top

Ruby: return if data.nil?
来源：http://wut.sjlbkw.cn

C#:   if (data == null) return;
来源：http://jds.yvedp.cn

================================================================================
来源：http://ulq.jinqigfzy.top

C. 函数与作用域
来源：http://kqs.dianchejie.cn

================================================================================
来源：http://elx.mhx1999.top

[C01] 定义函数
来源：http://loh.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://tqi.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pjl.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://veg.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uaq.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hio.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wqi.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://esj.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wtv.52xcode.cn

[C02] 默认参数
来源：http://kav.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://yul.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yah.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://bhr.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fma.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nvo.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hsn.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://cyc.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://jel.cheryme.top

[C03] 可变参数
来源：http://aep.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://sgt.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cyw.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vwy.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcb.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uan.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ibh.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://npa.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zqu.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://tbp.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://okx.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nfr.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vjr.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://duj.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://byz.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://inf.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://phr.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://ull.jqgfzy.top

[C05] 返回多个值
来源：http://mto.ivvv.top

Py:   return a, b
来源：http://sah.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://nri.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vdc.sweek.top

TS:   return { a, b };
来源：http://bmd.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zmh.zhijiandao.cn

Go:   return a, b
来源：http://bxg.sjlbkw.cn

Ruby: return a, b
来源：http://wrm.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://hqr.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://evz.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://zni.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yyf.yuanzhike.top

JS:   const square = x => x * x;
来源：http://hts.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://qhv.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vdx.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://foh.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://hgy.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://obg.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://ytq.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kpx.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://geu.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syw.ivvv.top

TS:   arr.map(String)
来源：http://kgb.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://otl.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://anc.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://wdj.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rql.kuanghao11.cn

[C08] 闭包
来源：http://qwm.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jos.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mdy.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mun.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwg.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gpb.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mio.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wkh.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lfs.fzhhl.top

[C09] 递归
来源：http://xsu.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jxu.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nnp.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xqz.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nye.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://paj.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wgm.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fnt.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://phw.ydzc1.top

[C10] 变量作用域
来源：http://nca.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lkw.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djh.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xdk.ppjwa.cn

TS:   同 JS
来源：http://czi.hcnkem.com

Java: 方法内为块级作用域
来源：http://pdj.ydjk.org.cn

Go:   花括号块级作用域
来源：http://apn.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://shd.feifeiyinyue.top

C#:   块级作用域
来源：http://nah.hesvh.cn

[C11] 模块导入与导出
来源：http://psi.hcnkem.com

Py:   from module import func
来源：http://mqe.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kpo.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://idd.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://syr.hysaishi.cn

Java: import java.util.List;
来源：http://quy.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://enr.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://ubq.epnwcf.com

C#:   using System.Text;
来源：http://ucf.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://bbz.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://gbl.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://hvt.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://xnp.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://hbq.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kiu.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://jki.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://uqy.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gth.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://nrn.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://owu.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://biq.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lfu.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jlj.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://xff.andypj.xyz

Go:   func add(a, b int) int
来源：http://dyi.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uvx.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nnv.hfpthk.cn

[C14] 泛型函数
来源：http://jly.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://all.ppjwa.cn

PHP:  // 无泛型
来源：http://kbv.dianchejie.cn

JS:   // 无泛型
来源：http://wum.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vhc.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baj.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ibh.daxiang520.top

Ruby: # 无泛型
来源：http://fvi.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bkm.epnwcf.com

[C15] 解构 / 展开参数
来源：http://eco.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rbl.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://kxk.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://feg.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zyj.tarul.cn

Java: // 无解构
来源：http://zrk.ivvv.top

Go:   // 无解构
来源：http://hbh.hcnkem.com

Ruby: a, b = pair
来源：http://rdz.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://mbn.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://szx.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blk.yonumen.top

PHP:  // 无重载
来源：http://ctu.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uoc.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://ulp.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lns.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://wrm.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://ubs.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xiw.aizwys.cn

================================================================================
来源：http://aap.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://fln.ywan-chungtsiang.top

================================================================================
来源：http://cvf.52xcode.cn

[D01] 创建数组 / 列表
来源：http://xxn.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kbd.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bcz.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hqi.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fsr.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gno.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://aur.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://gma.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vqs.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://hag.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqt.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vuj.xziqi.cn

JS:   arr.push(4);
来源：http://yka.tanke756.top

TS:   arr.push(4);
来源：http://yid.wangdashe.top

Java: list.add(4);
来源：http://buc.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://myl.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://gqw.uphjek.com

C#:   list.Add(4);
来源：http://xpi.epnwcf.com

[D03] 在指定位置插入元素
来源：http://lra.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://sai.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://huk.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jen.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://uui.daxiang520.top

Java: list.add(0, 0);
来源：http://coq.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kol.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dvw.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://efx.xuanzx.com

[D04] 删除元素
来源：http://ugv.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sqk.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zbh.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnf.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://yhi.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fmj.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpo.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gmy.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qbs.nanxinkj.top

[D05] 访问与修改元素
来源：http://mtl.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mfk.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://phr.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wgb.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://ymh.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://ytx.fktsv.cn


<!-- 参考信息 -->