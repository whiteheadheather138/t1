代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zbo.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://hsi.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lld.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kuk.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://htw.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbk.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://khc.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ory.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rnz.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://flr.yvedp.cn

[B07] while 循环
来源：http://oot.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://wzd.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://rxh.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://csf.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://uly.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://yzz.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://syr.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://egl.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://zix.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://gga.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://ozd.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://avs.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://rnh.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://nlq.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://yqw.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://khu.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://lhp.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://nkw.andypj.xyz

[B09] break 与 continue
来源：http://fjm.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zmk.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yfc.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgc.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqx.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hol.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://irz.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kds.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdy.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://qoe.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fma.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hze.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ufn.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ebk.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xlj.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qaw.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iyn.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mqh.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://ruh.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://nrs.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://iii.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mlx.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mnd.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uhc.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mir.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://cjr.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vqk.yj20258888.top

[B12] 跳出多层循环
来源：http://llz.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://dgg.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uhm.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wxo.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bzg.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tmn.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ain.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bek.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wjq.daria6918.cn

[B13] 判断是否为数字
来源：http://bir.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://cqr.jianghu66.top

PHP:  is_numeric($x)
来源：http://qop.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mdu.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uhg.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://pfl.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qer.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://hlg.uphjek.com

C#:   x is int or double or decimal
来源：http://qze.pycfn.com

[B14] 判断值是否在集合内
来源：http://zjj.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ljf.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lue.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://ocf.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://tbi.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cqb.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cqe.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yky.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ckw.wangdashe.top

[B15] 布尔运算与取反
来源：http://txw.yuxming.cn

Py:   a and b or not c
来源：http://siw.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://nvn.bjfxy.top

JS:   a && b || !c
来源：http://ggb.yj202588.top

TS:   a && b || !c
来源：http://ynr.xylfe.cn

Java: a && b || !c
来源：http://vde.sweek.top

Go:   a && b || !c
来源：http://gzf.yueranfly.top

Ruby: a && b || !c
来源：http://qaw.ppjwa.cn

C#:   a && b || !c
来源：http://xgi.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://eqr.hnqzz.top

Py:   if not data: return
来源：http://oii.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://ock.kuanghao11.cn

JS:   if (!data) return;
来源：http://utk.nwbrower.top

TS:   if (!data) return;
来源：http://vdp.ybcxt.top

Java: if (data == null) return;
来源：http://ylk.shuidangran.top

Go:   if data == nil { return }
来源：http://wqz.smart0.xyz

Ruby: return if data.nil?
来源：http://ucp.yuxming.cn

C#:   if (data == null) return;
来源：http://yqs.cqqwz.cn

================================================================================
来源：http://qjd.uphjek.com

C. 函数与作用域
来源：http://coa.shzxlz.cn

================================================================================
来源：http://aqm.316326.xyz

[C01] 定义函数
来源：http://hua.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://mfy.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wsy.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://ynu.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdw.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kkw.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fis.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://hgj.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ple.cucudq.cn

[C02] 默认参数
来源：http://tbh.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://nmx.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://cmd.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://hyf.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ppd.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fyn.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nju.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://cnt.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://ebp.ydjk.org.cn

[C03] 可变参数
来源：http://cse.sweek.top

Py:   def total(*args): return sum(args)
来源：http://pdl.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogc.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dfk.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pob.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mmf.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uoo.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://qht.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://okk.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://lul.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vdv.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wcu.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sas.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lzr.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://zpy.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://udo.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://obh.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://wnn.havefunace.top

[C05] 返回多个值
来源：http://yvy.yj202588.top

Py:   return a, b
来源：http://eny.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://hym.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gir.hywenlv.cn

TS:   return { a, b };
来源：http://bxd.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oje.jinghuilouyu.cn

Go:   return a, b
来源：http://fvb.yj202588.top

Ruby: return a, b
来源：http://ump.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://tdy.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://sbr.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://wmv.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wsu.yj202588.top

JS:   const square = x => x * x;
来源：http://ifb.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://jey.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wqs.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://jtw.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://oxe.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://fcq.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://vnc.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ddl.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://wsf.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttj.chenjidiqi.icu

TS:   arr.map(String)
来源：http://rje.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://evv.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://skc.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://bus.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wtf.redwolf501.top

[C08] 闭包
来源：http://ymk.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axj.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mzq.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jlf.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uzx.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tyk.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ghh.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vgo.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ium.yongpay.top

[C09] 递归
来源：http://hby.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xoy.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mok.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spp.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tpk.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moo.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wpw.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oys.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lha.ppjwa.cn

[C10] 变量作用域
来源：http://yob.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jyp.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://prx.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://omf.zhijiandao.cn

TS:   同 JS
来源：http://ahx.ehwqpu.com

Java: 方法内为块级作用域
来源：http://oan.andypj.xyz

Go:   花括号块级作用域
来源：http://fos.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nbd.hfpthk.cn

C#:   块级作用域
来源：http://usr.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://ffx.yueranfly.top

Py:   from module import func
来源：http://kiw.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wue.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cst.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vwg.52xcode.cn

Java: import java.util.List;
来源：http://xee.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eks.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://rmk.jqgfzy.top

C#:   using System.Text;
来源：http://evp.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://ebc.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://ggz.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://jey.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://med.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://fgk.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://obb.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://lpy.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://uzv.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rrx.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://rwq.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mcq.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifg.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fzi.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://btz.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://pyn.hnqzz.top

Go:   func add(a, b int) int
来源：http://zro.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uxk.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://tke.guowangkeji.top

[C14] 泛型函数
来源：http://mhn.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://idq.smart0.xyz

PHP:  // 无泛型
来源：http://rbi.fzhhl.top

JS:   // 无泛型
来源：http://yal.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hsl.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fbc.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vrk.tanke756.top

Ruby: # 无泛型
来源：http://jxh.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://adm.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://nzl.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bxv.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://bsc.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rjm.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vxs.0kj1m.cn

Java: // 无解构
来源：http://bvs.ehwqpu.com

Go:   // 无解构
来源：http://kov.hnqzz.top

Ruby: a, b = pair
来源：http://trp.ybcxt.top

C#:   var (a, b) = pair;
来源：http://ypj.andypj.xyz

[C16] 函数 / 方法重载
来源：http://oit.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pqc.ydjk.org.cn

PHP:  // 无重载
来源：http://onv.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mkw.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://skw.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://esv.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://vew.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://rje.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xia.hysaishi.cn

================================================================================
来源：http://jqm.sweek.top

D. 数组 / 列表 / 集合
来源：http://bmd.zhixingplan.top

================================================================================
来源：http://njb.meibo888.top

[D01] 创建数组 / 列表
来源：http://fwg.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fvy.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ind.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eed.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wux.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rqi.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://pec.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://jkj.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ery.ivvv.top

[D02] 追加元素到末尾
来源：http://lju.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bui.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qiq.xuanzx.com

JS:   arr.push(4);
来源：http://eja.hnxiangtu.top

TS:   arr.push(4);
来源：http://mrr.nanxinkj.top

Java: list.add(4);
来源：http://ggz.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://wfc.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://rny.yueranfly.top

C#:   list.Add(4);
来源：http://bhb.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://bcf.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://tcn.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ohx.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgy.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://ipi.yvedp.cn

Java: list.add(0, 0);
来源：http://qmg.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rqh.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qcu.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://iew.bbcook.cn

[D04] 删除元素
来源：http://mdz.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://exd.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zzn.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jan.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://cki.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qcx.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fzl.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ioh.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jxn.pycfn.com

[D05] 访问与修改元素
来源：http://vyi.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xtm.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ygp.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wpm.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://myu.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://kol.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://ztm.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ihy.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vwu.guannengcc.top

[D06] 数组长度
来源：http://eod.aibaodan.cn

Py:   len(arr)
来源：http://ldd.zhoulong.xyz

PHP:  count($arr);
来源：http://pgz.daria6918.cn

JS:   arr.length
来源：http://xxn.c1oappe.top

TS:   arr.length
来源：http://cqq.andypj.xyz


<!-- 参考信息 -->