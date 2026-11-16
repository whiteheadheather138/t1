代发 wailian999

[B05] 遍历数组 / 列表
来源：http://eqd.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://yxj.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dic.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eyt.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://gsn.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ive.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sad.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://okx.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://klu.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://nvt.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sdo.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ajh.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://atb.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hvb.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xne.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://duq.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aqm.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vky.redwolf501.top

[B07] while 循环
来源：http://mtk.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://xmr.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://btj.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://hhb.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://vkv.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://dbb.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sgl.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://bzn.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ihn.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://gsx.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://nzs.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://xth.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://jol.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://coo.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://xjf.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jeo.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://vln.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://gzo.tianlin.xyz

[B09] break 与 continue
来源：http://zsb.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rks.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://drp.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpl.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzs.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://buz.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xeh.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xwp.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhz.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://eoi.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xkf.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fum.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oxg.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bga.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pnf.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pzd.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://imb.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://twl.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://ryx.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://uom.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://sqm.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cog.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ixy.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hyp.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vda.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://ieq.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ykz.kuanghao11.cn

[B12] 跳出多层循环
来源：http://vdd.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mjv.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jgg.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrd.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hsa.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eqv.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rph.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lzq.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ygg.zycfv.cn

[B13] 判断是否为数字
来源：http://hbf.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://opg.cashguo.top

PHP:  is_numeric($x)
来源：http://mhm.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ctb.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvl.zhoulong.xyz

Java: x instanceof Number
来源：http://hpl.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dzb.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://fki.hesvh.cn

C#:   x is int or double or decimal
来源：http://cue.xylfe.cn

[B14] 判断值是否在集合内
来源：http://xzx.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ogu.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nqt.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gyl.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://ocl.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hay.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wtf.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ivx.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fzu.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://evb.hnxiangtu.top

Py:   a and b or not c
来源：http://ksv.yfazqb.com

PHP:  $a && $b || !$c
来源：http://khv.jqgufenzy.top

JS:   a && b || !c
来源：http://dkq.zhiwuduotai.top

TS:   a && b || !c
来源：http://dsp.hywenlv.cn

Java: a && b || !c
来源：http://mvu.zdbjq.cn

Go:   a && b || !c
来源：http://gxg.snrcjt.cn

Ruby: a && b || !c
来源：http://ulu.havefunace.top

C#:   a && b || !c
来源：http://gsw.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://hup.zhiwuduotai.top

Py:   if not data: return
来源：http://ifa.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://oeg.guannengcc.top

JS:   if (!data) return;
来源：http://fid.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://vqu.vehdjk.com

Java: if (data == null) return;
来源：http://tsz.daria6918.cn

Go:   if data == nil { return }
来源：http://lcj.daxiang520.top

Ruby: return if data.nil?
来源：http://qfj.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://yfr.birdmap.top

================================================================================
来源：http://qsq.iojbl.cn

C. 函数与作用域
来源：http://xxq.sweek.top

================================================================================
来源：http://oug.andypj.xyz

[C01] 定义函数
来源：http://elb.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://bes.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vwl.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://leu.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://any.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://mlu.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://rum.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://nul.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ukj.nwbrower.top

[C02] 默认参数
来源：http://rvl.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://sht.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://per.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://ifr.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tzu.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dhb.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sfo.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://izb.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://dnu.cashguo.top

[C03] 可变参数
来源：http://wja.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://bfc.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://otq.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://snz.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://myg.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qha.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sun.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gom.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jqe.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://gvb.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqx.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bfg.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ycm.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jjw.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://rre.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://bie.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://qal.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://rit.xinyue.icu

[C05] 返回多个值
来源：http://oyy.hnxiangtu.top

Py:   return a, b
来源：http://ijs.hfpthk.cn

PHP:  return [$a, $b];
来源：http://bga.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://inx.yanxiufei.cn

TS:   return { a, b };
来源：http://dhm.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gmp.epnwcf.com

Go:   return a, b
来源：http://qqu.uphjek.com

Ruby: return a, b
来源：http://stb.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://kmy.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://vzr.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://mns.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dbn.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://vsa.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://zqs.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dtw.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://des.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://zlu.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://ano.smart0.xyz

[C07] 把函数作为参数传入
来源：http://ldb.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://auo.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ujf.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ysr.gaohongyu789.top

TS:   arr.map(String)
来源：http://kmq.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ijp.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://luv.sweek.top

Ruby: arr.map(&:upcase)
来源：http://lad.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xzf.sjlbkw.cn

[C08] 闭包
来源：http://mma.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://flj.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iuy.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qeo.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ynu.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pro.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ybp.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdw.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbn.haohaochexian.top

[C09] 递归
来源：http://cez.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rlq.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wlf.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mkk.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vxe.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uig.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kqd.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bkh.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wpw.nwbrower.top

[C10] 变量作用域
来源：http://myz.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wkn.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kyh.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cml.ivvv.top

TS:   同 JS
来源：http://war.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://hra.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://dos.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yor.epnwcf.com

C#:   块级作用域
来源：http://txh.chenlongwang.top

[C11] 模块导入与导出
来源：http://opo.svipenyu.cn

Py:   from module import func
来源：http://rla.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yni.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nft.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qkn.sjlbkw.cn

Java: import java.util.List;
来源：http://cmj.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eqv.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://dsm.hammf.cn

C#:   using System.Text;
来源：http://rqe.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://nyx.316326.xyz

Py:   (lambda: print("run"))()
来源：http://jmz.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://zis.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://ezh.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://apt.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oab.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://rqk.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://dml.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ilf.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://yet.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cnu.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzo.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqi.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lme.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ycc.snrcjt.cn

Go:   func add(a, b int) int
来源：http://dtk.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cnu.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://mfx.yj202588.top

[C14] 泛型函数
来源：http://tdh.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ejq.ehwqpu.com

PHP:  // 无泛型
来源：http://yex.yongpay.top

JS:   // 无泛型
来源：http://epx.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://roa.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqj.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qkq.redwolf501.top

Ruby: # 无泛型
来源：http://lea.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gbr.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://ufw.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bow.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://ypl.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fwd.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bkh.xinyue.icu

Java: // 无解构
来源：http://skr.ywan-chungtsiang.top

Go:   // 无解构
来源：http://qzp.zhixingplan.top

Ruby: a, b = pair
来源：http://ttb.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://rtm.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://itu.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lah.mhx1999.top

PHP:  // 无重载
来源：http://gtb.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xtx.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://nzw.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kgi.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://ulr.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://rwg.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ads.dianchejie.cn

================================================================================
来源：http://zad.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://rid.sweek.top

================================================================================
来源：http://uxk.yuxming.cn

[D01] 创建数组 / 列表
来源：http://vfc.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zka.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmw.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://szi.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kxr.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gve.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://pif.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://kwd.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qxf.mhx1999.top

[D02] 追加元素到末尾
来源：http://xna.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qvl.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oaz.snrcjt.cn

JS:   arr.push(4);
来源：http://aed.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://aez.hongshengwenyu.top

Java: list.add(4);
来源：http://ksb.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://hnw.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://rdi.fktsv.cn

C#:   list.Add(4);
来源：http://soz.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://jzv.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://xix.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bam.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pqw.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://kxn.ppjwa.cn

Java: list.add(0, 0);
来源：http://xbl.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://rhf.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kod.316326.xyz

C#:   list.Insert(0, 0);
来源：http://hoj.nanxinkj.top

[D04] 删除元素
来源：http://dzu.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wva.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zuv.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lay.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://dvj.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tay.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pok.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aih.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://irk.cucudq.cn

[D05] 访问与修改元素
来源：http://nfg.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vyw.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xyi.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pfo.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://fiq.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://urs.xuetiantiany.cn


<!-- 参考信息 -->