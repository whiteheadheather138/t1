代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zbo.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bcr.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://soj.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cbw.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://okp.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://mtf.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qsj.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://agc.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://arv.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wqg.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rhh.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://ulv.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ojb.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://vhh.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ghw.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oul.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gdn.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jtn.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lzb.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jpe.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lyy.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xzg.nanxuanxn.top

[B07] while 循环
来源：http://uac.pycfn.com

Py:   while i < 10: i += 1
来源：http://mop.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dpr.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://nlz.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://ivq.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://amw.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igl.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://cpi.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://cfb.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://lfs.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://ycc.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qgi.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://jzs.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://ooy.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://ogy.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fny.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uah.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://wpm.hammf.cn

[B09] break 与 continue
来源：http://cmo.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lhp.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ukp.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qye.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iry.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eax.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kfi.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oyx.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guo.sysykeji.top

[B10] 遍历同时拿索引
来源：http://pks.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nco.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://krv.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wce.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xko.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qsz.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rkh.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nrs.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iyj.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://zps.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://rec.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://cef.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogf.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qxc.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xao.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yew.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://qtx.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://naj.jqgufenzy.top

[B12] 跳出多层循环
来源：http://krz.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://joe.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://msd.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mod.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jzl.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jvh.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yog.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://txk.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uah.hysaishi.cn

[B13] 判断是否为数字
来源：http://bvf.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://onp.yongpay.top

PHP:  is_numeric($x)
来源：http://dfi.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vdx.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kuo.pycfn.com

Java: x instanceof Number
来源：http://uvs.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eoz.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://mww.sufxvd.cn

C#:   x is int or double or decimal
来源：http://zun.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://tyc.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yrf.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pgb.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://vwq.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://ooz.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://otq.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://paz.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://suf.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bab.gzhubu.top

[B15] 布尔运算与取反
来源：http://ffp.feifeiyinyue.top

Py:   a and b or not c
来源：http://jmg.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://ggx.yongpay.top

JS:   a && b || !c
来源：http://snf.sjlbkw.cn

TS:   a && b || !c
来源：http://rgd.tianlin.xyz

Java: a && b || !c
来源：http://fed.zhiwuduotai.top

Go:   a && b || !c
来源：http://qdi.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://axm.hammf.cn

C#:   a && b || !c
来源：http://jmv.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://vke.52xcode.cn

Py:   if not data: return
来源：http://lrl.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://hod.xuanzx.com

JS:   if (!data) return;
来源：http://lqb.epnwcf.com

TS:   if (!data) return;
来源：http://guc.yueranfly.top

Java: if (data == null) return;
来源：http://czi.cucudq.cn

Go:   if data == nil { return }
来源：http://gux.zdbjq.cn

Ruby: return if data.nil?
来源：http://qkc.yangfankeji.com

C#:   if (data == null) return;
来源：http://mzg.hysaishi.cn

================================================================================
来源：http://ygf.tian-w.cn

C. 函数与作用域
来源：http://tzj.quarkkingdee.top

================================================================================
来源：http://svv.tanke756.top

[C01] 定义函数
来源：http://sxo.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://fxx.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybv.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ibm.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wyh.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wxs.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xpc.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://edj.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rxs.xinyue.icu

[C02] 默认参数
来源：http://bgs.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://sxo.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://omc.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://coi.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://btd.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mpe.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ell.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://nvj.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://dpv.nanxuanxn.top

[C03] 可变参数
来源：http://llm.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://frf.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rjt.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nol.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkb.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://flq.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zzz.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://xpy.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oia.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://bjj.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pcj.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gqz.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oxd.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gqv.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://yhv.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://fte.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://aox.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://ipz.daria6918.cn

[C05] 返回多个值
来源：http://ers.shangyingyoupin.top

Py:   return a, b
来源：http://puf.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://hug.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://arc.yongpay.top

TS:   return { a, b };
来源：http://dte.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rvd.guannengcc.top

Go:   return a, b
来源：http://bbg.shzxlz.cn

Ruby: return a, b
来源：http://cfu.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://ice.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://szy.daxiang520.top

Py:   square = lambda x: x * x
来源：http://hhs.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xti.yvedp.cn

JS:   const square = x => x * x;
来源：http://mml.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://szq.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vrn.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://jhe.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://ixa.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fkq.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://vuf.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://epe.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://svh.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://arh.zhijiandao.cn

TS:   arr.map(String)
来源：http://emu.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pqr.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fiq.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://vqg.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ngk.hesvh.cn

[C08] 闭包
来源：http://cgl.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qey.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ugo.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://csw.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tle.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gzt.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fnw.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rtq.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cqn.ydzc1.top

[C09] 递归
来源：http://cvr.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rpw.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zzq.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npl.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://psu.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aro.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwr.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uip.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fpa.316326.xyz

[C10] 变量作用域
来源：http://zpf.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbv.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hcp.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://smw.yonumen.top

TS:   同 JS
来源：http://qxf.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://ovj.fengsongda.top

Go:   花括号块级作用域
来源：http://ukl.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qma.xylfe.cn

C#:   块级作用域
来源：http://tln.9152youxi.cn

[C11] 模块导入与导出
来源：http://vrh.0kj1m.cn

Py:   from module import func
来源：http://hzb.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ivr.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cgf.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jut.tarul.cn

Java: import java.util.List;
来源：http://bhz.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yxm.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://hgd.hesvh.cn

C#:   using System.Text;
来源：http://nwq.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://mto.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://dni.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://ede.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://sez.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://uxe.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avq.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://wjz.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://rqb.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://rml.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://shf.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mzp.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bxj.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hgv.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvz.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://ila.meibo888.top

Go:   func add(a, b int) int
来源：http://cin.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qtv.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://eqq.shanyushiyangtech.top

[C14] 泛型函数
来源：http://dul.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tqk.tian-w.cn

PHP:  // 无泛型
来源：http://uwk.yj202588.top

JS:   // 无泛型
来源：http://bjf.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hqm.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mzt.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uai.cucudq.cn

Ruby: # 无泛型
来源：http://cxb.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hzp.fengsongda.top

[C15] 解构 / 展开参数
来源：http://hnp.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tqj.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://iey.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jiz.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://olm.fehbvm.com

Java: // 无解构
来源：http://gcs.xylfe.cn

Go:   // 无解构
来源：http://akz.hywenlv.cn

Ruby: a, b = pair
来源：http://ies.hnqzz.top

C#:   var (a, b) = pair;
来源：http://isl.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://lun.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cqq.sjlbkw.cn

PHP:  // 无重载
来源：http://rzc.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ulc.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://ldw.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tru.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://xos.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://cbf.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://cmw.hnqzz.top

================================================================================
来源：http://ajm.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://rax.cucudq.cn

================================================================================
来源：http://tdw.nwbrower.top

[D01] 创建数组 / 列表
来源：http://net.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://duz.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kat.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://adi.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bgh.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zwm.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://pta.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://qak.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vfq.ybcxt.top

[D02] 追加元素到末尾
来源：http://gsh.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dng.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ths.chenjidiqi.icu

JS:   arr.push(4);
来源：http://kjw.daxiang520.top

TS:   arr.push(4);
来源：http://nay.yuxming.cn

Java: list.add(4);
来源：http://xqz.yonumen.top

Go:   arr = append(arr, 4)
来源：http://pjp.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://etv.wangdashe.top

C#:   list.Add(4);
来源：http://fon.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://lyo.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://upy.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lpj.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ptw.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://tgt.jiagoushi.top

Java: list.add(0, 0);
来源：http://blz.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://htm.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bgw.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://pnm.tanke756.top

[D04] 删除元素
来源：http://ayk.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dfz.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wqi.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nrl.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://tcf.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ecm.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dll.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hbu.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jpg.ydzc1.top

[D05] 访问与修改元素
来源：http://cik.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vsn.nanxuanxn.top


<!-- 参考信息 -->