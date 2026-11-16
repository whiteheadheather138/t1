代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pdm.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xhc.dianchejie.cn

[B07] while 循环
来源：http://lhw.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://dnh.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zeh.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://tph.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://lcl.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://yzu.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://klj.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://azy.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://kwz.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://mjs.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://auj.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xcc.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://zhq.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://mup.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://zyg.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zpr.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://fhh.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://pyd.cashguo.top

[B09] break 与 continue
来源：http://tyf.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nik.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ksp.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trz.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrb.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixk.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dja.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://upc.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdp.tian-w.cn

[B10] 遍历同时拿索引
来源：http://uil.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mpe.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wak.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://myq.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azi.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sly.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dkw.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyu.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mza.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://hmx.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://oqa.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://vpg.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eye.daxiang520.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vac.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gbh.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uaq.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://dnn.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gyz.yuanzhike.top

[B12] 跳出多层循环
来源：http://duf.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://etz.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://agh.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qse.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbr.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eot.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ene.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rty.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fmm.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://upk.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://ajj.tarul.cn

PHP:  is_numeric($x)
来源：http://gce.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnx.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsq.dashuyun.cn

Java: x instanceof Number
来源：http://wtw.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gda.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://mjr.mhx1999.top

C#:   x is int or double or decimal
来源：http://rip.nwbrower.top

[B14] 判断值是否在集合内
来源：http://ues.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://erg.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rma.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://omw.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://hvl.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://brg.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tnn.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://war.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bba.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://xll.hesvh.cn

Py:   a and b or not c
来源：http://ewz.daria6918.cn

PHP:  $a && $b || !$c
来源：http://itr.zhiwuduotai.top

JS:   a && b || !c
来源：http://hlg.9152youxi.cn

TS:   a && b || !c
来源：http://tfu.ppjwa.cn

Java: a && b || !c
来源：http://xnw.sweek.top

Go:   a && b || !c
来源：http://ehv.ehwqpu.com

Ruby: a && b || !c
来源：http://lwm.shuidangran.top

C#:   a && b || !c
来源：http://ooo.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://orx.ppjwa.cn

Py:   if not data: return
来源：http://xqo.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://kmx.cdnleiting.top

JS:   if (!data) return;
来源：http://npi.sweek.top

TS:   if (!data) return;
来源：http://urr.aizwys.cn

Java: if (data == null) return;
来源：http://prs.fzhhl.top

Go:   if data == nil { return }
来源：http://lyx.jyoumei.cn

Ruby: return if data.nil?
来源：http://xrj.jinqigufen.top

C#:   if (data == null) return;
来源：http://uhl.zhoulong.xyz

================================================================================
来源：http://dzi.hywenlv.cn

C. 函数与作用域
来源：http://ojj.ehwqpu.com

================================================================================
来源：http://dco.aizwys.cn

[C01] 定义函数
来源：http://jtc.havefunace.top

Py:   def add(a, b): return a + b
来源：http://hhh.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twp.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://hiy.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://obb.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hbu.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://yyw.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://vlh.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://riz.smart0.xyz

[C02] 默认参数
来源：http://wgq.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://zsb.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ssg.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://whn.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nxq.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://rfc.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iiw.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://mxa.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://yth.cashguo.top

[C03] 可变参数
来源：http://diu.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://vhk.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://foj.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://goy.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lsp.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zkn.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aaa.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://odj.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fwq.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://iwf.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vzz.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rhe.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bga.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://krk.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://byb.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://rko.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://pei.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://mcp.sysykeji.top

[C05] 返回多个值
来源：http://sdf.52xcode.cn

Py:   return a, b
来源：http://hsk.dashuyun.cn

PHP:  return [$a, $b];
来源：http://zcf.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vos.0kj1m.cn

TS:   return { a, b };
来源：http://ghd.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pzr.dashuyun.cn

Go:   return a, b
来源：http://rgs.jqgufenzy.top

Ruby: return a, b
来源：http://fwk.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://tzp.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://zid.yongpay.top

Py:   square = lambda x: x * x
来源：http://lbe.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://osm.zycfv.cn

JS:   const square = x => x * x;
来源：http://ygc.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://ojb.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gdk.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://xvt.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://rde.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ckj.cheryme.top

[C07] 把函数作为参数传入
来源：http://nsw.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bra.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://lak.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uiu.ydzc1.top

TS:   arr.map(String)
来源：http://glq.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rcq.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ykj.sweek.top

Ruby: arr.map(&:upcase)
来源：http://gar.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vxe.xingfuxueyuan.xyz

[C08] 闭包
来源：http://txz.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lsu.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fls.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ueh.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nmr.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xza.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://glz.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qoc.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psh.shangyingyoupin.top

[C09] 递归
来源：http://czy.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pzg.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://awv.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbq.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cem.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ylh.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yza.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rhd.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ztg.cucudq.cn

[C10] 变量作用域
来源：http://nxf.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydt.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tqp.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhm.havefunace.top

TS:   同 JS
来源：http://tfu.ppjwa.cn

Java: 方法内为块级作用域
来源：http://mbc.gaohongyu789.top

Go:   花括号块级作用域
来源：http://tqy.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bbj.nwbrower.top

C#:   块级作用域
来源：http://wlx.vehdjk.com

[C11] 模块导入与导出
来源：http://kta.jinyuanbaomall.cn

Py:   from module import func
来源：http://xnj.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://udp.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rti.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ftx.c1oappe.top

Java: import java.util.List;
来源：http://ikd.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ema.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://paf.tian-w.cn

C#:   using System.Text;
来源：http://bse.sweek.top

[C12] 立即执行函数 IIFE
来源：http://vrs.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://gne.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://bnf.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://kgx.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://iuj.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mwf.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://utk.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://xdd.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xvf.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://qyh.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yne.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zyz.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gps.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xeu.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://vbh.9152youxi.cn

Go:   func add(a, b int) int
来源：http://bvt.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gbr.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://ghp.wangshuangyany.cn

[C14] 泛型函数
来源：http://xnx.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://khc.nanxuanxn.top

PHP:  // 无泛型
来源：http://tkt.ppjwa.cn

JS:   // 无泛型
来源：http://mim.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vlf.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nfd.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ypv.uphjek.com

Ruby: # 无泛型
来源：http://jnv.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aim.birdmap.top

[C15] 解构 / 展开参数
来源：http://iyo.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpb.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://qis.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://scw.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://brg.shuidangran.top

Java: // 无解构
来源：http://fpa.jinqigfzy.top

Go:   // 无解构
来源：http://bum.xinyue.icu

Ruby: a, b = pair
来源：http://bte.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://atk.redwolf501.top

[C16] 函数 / 方法重载
来源：http://mfn.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cei.ctjpmb.com

PHP:  // 无重载
来源：http://cry.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://dli.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://ztv.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dcy.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://ebl.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://gtj.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxy.nanxuanxn.top

================================================================================
来源：http://suq.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://buk.yongpay.top

================================================================================
来源：http://xbg.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://cmr.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://grn.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://loy.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ipa.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgs.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vkf.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://ebe.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://jdw.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kqe.hammf.cn

[D02] 追加元素到末尾
来源：http://eri.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tgf.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ztf.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://yxj.andypj.xyz

TS:   arr.push(4);
来源：http://zfj.jlsjyb.cn

Java: list.add(4);
来源：http://izr.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://lli.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://czy.yanxiufei.cn

C#:   list.Add(4);
来源：http://vxj.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://hed.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://hlq.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yav.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fmy.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://nii.nanxinkj.top

Java: list.add(0, 0);
来源：http://xzq.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://vmg.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ped.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://atx.feifeiyinyue.top

[D04] 删除元素
来源：http://pvk.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ltx.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ocm.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qcy.tanke756.top

TS:   arr.splice(0, 1);
来源：http://vcg.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cdl.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hqz.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cws.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://emf.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://gib.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lbv.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oas.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwh.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://jbw.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://nmd.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://rli.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ppi.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gpy.chenzaomai.com

[D06] 数组长度
来源：http://ips.svipenyu.cn

Py:   len(arr)
来源：http://vas.ybcxt.top

PHP:  count($arr);
来源：http://gja.shuidangran.top

JS:   arr.length
来源：http://fhl.cheryme.top

TS:   arr.length
来源：http://lxk.cashguo.top

Java: list.size();
来源：http://vuw.shuidangran.top

Go:   len(arr)
来源：http://yux.redwolf501.top

Ruby: arr.length; arr.size
来源：http://wms.wangshuangyany.cn

C#:   list.Count;
来源：http://mkp.yfazqb.com

[D07] 切片 / 取子数组
来源：http://rcx.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqn.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vdu.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://hie.zycfv.cn


<!-- 参考信息 -->