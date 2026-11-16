代发 wailian999

[B05] 遍历数组 / 列表
来源：http://goe.guannengcc.top

Py:   for item in arr: print(item)
来源：http://fdj.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tzf.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://rok.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kwo.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://avb.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sne.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://ywq.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nnk.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://imo.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ajd.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://usa.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dow.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cdd.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uba.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pka.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://msu.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://odr.hcnkem.com

[B07] while 循环
来源：http://oej.yuxming.cn

Py:   while i < 10: i += 1
来源：http://kgh.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://wfs.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://ute.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://ibo.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://axv.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nzl.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://wcp.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://qwk.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://hnk.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://khj.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hkb.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://dce.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://foo.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://wtz.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wjt.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://aug.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://xyi.yanxiufei.cn

[B09] break 与 continue
来源：http://usm.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aja.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mzd.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehg.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhm.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfn.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bwy.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pvp.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpo.52xcode.cn

[B10] 遍历同时拿索引
来源：http://mzx.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tfk.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sob.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kzw.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://heq.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://swe.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cbl.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dbz.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://koo.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://uqp.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://gmo.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://zhq.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mqb.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezy.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vwa.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eiq.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://msb.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyq.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://plh.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jkl.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mgj.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnf.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfi.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nqs.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ajp.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mue.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qap.vehdjk.com

[B13] 判断是否为数字
来源：http://xcz.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://weg.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://oim.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zyl.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://erw.haohaochexian.top

Java: x instanceof Number
来源：http://jlk.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwg.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://wfk.ehwqpu.com

C#:   x is int or double or decimal
来源：http://wvk.tanke756.top

[B14] 判断值是否在集合内
来源：http://psy.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uar.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oma.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://lsh.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://vfb.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hzc.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vpl.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://daa.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qvh.bbcook.cn

[B15] 布尔运算与取反
来源：http://kwu.guannengcc.top

Py:   a and b or not c
来源：http://iae.gzhubu.top

PHP:  $a && $b || !$c
来源：http://mci.ivvv.top

JS:   a && b || !c
来源：http://lfr.bbcook.cn

TS:   a && b || !c
来源：http://bek.daxiang520.top

Java: a && b || !c
来源：http://uxe.cashguo.top

Go:   a && b || !c
来源：http://plh.chenzaomai.com

Ruby: a && b || !c
来源：http://rxd.cqqwz.cn

C#:   a && b || !c
来源：http://pmq.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://dtv.sxryk.cn

Py:   if not data: return
来源：http://gyv.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://kzs.jinqigufen.top

JS:   if (!data) return;
来源：http://mpj.tanke756.top

TS:   if (!data) return;
来源：http://gkm.c1oappe.top

Java: if (data == null) return;
来源：http://voy.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://zsf.ybcxt.top

Ruby: return if data.nil?
来源：http://ddy.andypj.xyz

C#:   if (data == null) return;
来源：http://tyw.zhengqikj.top

================================================================================
来源：http://biz.nanxinkj.top

C. 函数与作用域
来源：http://tkq.uphjek.com

================================================================================
来源：http://emx.pycfn.com

[C01] 定义函数
来源：http://xfs.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://mdb.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxv.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://evj.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yup.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://ixn.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://acq.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://ycm.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sli.yj20258888.top

[C02] 默认参数
来源：http://pcq.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://dek.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://puw.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://ebx.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bkb.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ofq.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://paa.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://ytr.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://xuf.epnwcf.com

[C03] 可变参数
来源：http://lyy.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://wmg.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pzl.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fox.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lyc.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://icj.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nof.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://jtr.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tbi.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://djr.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eds.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ezr.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://doz.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://urq.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://joj.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://tcq.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://epy.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://vzv.fktsv.cn

[C05] 返回多个值
来源：http://iui.aizwys.cn

Py:   return a, b
来源：http://ama.yfazqb.com

PHP:  return [$a, $b];
来源：http://xqa.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dpf.zycfv.cn

TS:   return { a, b };
来源：http://cnb.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://byz.cdnleiting.top

Go:   return a, b
来源：http://gqu.xuetiantiany.cn

Ruby: return a, b
来源：http://oer.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://evn.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://tre.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://kbb.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dof.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://tkv.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://vrj.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://upc.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://awp.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://iho.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lal.cheryme.top

[C07] 把函数作为参数传入
来源：http://drd.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ywi.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://cxl.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://deh.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://uzv.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ygj.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gbb.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://pju.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iza.gotoacloud.top

[C08] 闭包
来源：http://ozd.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vps.yuanzhike.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jvf.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xhz.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tir.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ydg.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yto.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jej.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jcd.kuanghao11.cn

[C09] 递归
来源：http://tuo.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uot.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://msu.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ubo.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wll.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udm.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lvj.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oiq.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdz.zycfv.cn

[C10] 变量作用域
来源：http://kok.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyd.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://znx.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://grn.xinyue.icu

TS:   同 JS
来源：http://iwl.tian-w.cn

Java: 方法内为块级作用域
来源：http://wwd.tanke756.top

Go:   花括号块级作用域
来源：http://aen.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yjm.zdbjq.cn

C#:   块级作用域
来源：http://ass.yuanzhike.top

[C11] 模块导入与导出
来源：http://vzy.xuanzx.com

Py:   from module import func
来源：http://jyt.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mpu.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zug.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jew.redwolf501.top

Java: import java.util.List;
来源：http://cgj.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gyx.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://yth.tianlin.xyz

C#:   using System.Text;
来源：http://nre.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://zed.yj202588.top

Py:   (lambda: print("run"))()
来源：http://ffv.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://aub.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://wjj.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://vlf.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xkc.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://itr.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://vqi.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qci.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://axn.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cje.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpo.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ysx.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nma.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://aap.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://jmb.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mml.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://veh.jqgfzy.top

[C14] 泛型函数
来源：http://cap.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hrh.svipenyu.cn

PHP:  // 无泛型
来源：http://mvh.jqgufenzy.top

JS:   // 无泛型
来源：http://pxb.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jtz.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sba.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ctt.jianghu66.top

Ruby: # 无泛型
来源：http://ruz.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gol.fzhhl.top

[C15] 解构 / 展开参数
来源：http://xzu.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://igf.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://aks.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xok.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rgg.xuanzx.com

Java: // 无解构
来源：http://nck.shanyushiyangkeji.top

Go:   // 无解构
来源：http://whz.zhiwuduotai.top

Ruby: a, b = pair
来源：http://fdb.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://eoi.bbcook.cn

[C16] 函数 / 方法重载
来源：http://knu.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://asc.wangdashe.top

PHP:  // 无重载
来源：http://sxf.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zml.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://klw.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sub.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://fry.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://oai.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://rhi.cdnleiting.top

================================================================================
来源：http://jje.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://rlj.ydjk.org.cn

================================================================================
来源：http://bja.xuanzx.com

[D01] 创建数组 / 列表
来源：http://auw.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qzj.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fah.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mmm.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wan.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://psi.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://mte.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://rve.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rxz.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://ccl.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ltz.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gkk.yangfankeji.com

JS:   arr.push(4);
来源：http://rnt.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://afe.hysaishi.cn

Java: list.add(4);
来源：http://udl.birdmap.top

Go:   arr = append(arr, 4)
来源：http://fha.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://bje.svipenyu.cn

C#:   list.Add(4);
来源：http://vty.gzhubu.top

[D03] 在指定位置插入元素
来源：http://bvj.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://vef.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tlv.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wes.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://dlv.jinqigfzy.top

Java: list.add(0, 0);
来源：http://zlo.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qpj.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eha.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://fbq.dashuyun.cn

[D04] 删除元素
来源：http://fkk.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hbd.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mne.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xry.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://tes.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rfe.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aap.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eqo.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmo.jqgfzy.top

[D05] 访问与修改元素
来源：http://ids.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://irl.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dxy.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bwz.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cna.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://syb.ehwqpu.com


<!-- 参考信息 -->