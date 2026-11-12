代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpx.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dnw.wangshuangyany.cn

[B07] while 循环
来源：http://fen.aizwys.cn

Py:   while i < 10: i += 1
来源：http://pkd.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://jss.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://znx.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://mwm.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://gox.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://msm.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://zpn.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://gtv.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://cln.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://qxz.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oii.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://ozt.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://unk.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://uln.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rmv.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://pis.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://uvs.tarul.cn

[B09] break 与 continue
来源：http://wbw.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hif.fzhhl.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wzm.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okz.zhaomingkeji.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ome.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrd.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zuw.nwbrower.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tqo.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjo.smart0.xyz

[B10] 遍历同时拿索引
来源：http://ejs.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pvy.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://txa.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ecn.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fpd.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fno.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wmn.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kir.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://csi.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://iry.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://qkh.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://icm.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://upd.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rzv.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qkw.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ndj.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://nmt.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sqp.haohaochexian.top

[B12] 跳出多层循环
来源：http://cnw.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ypz.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqf.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wse.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxv.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ozn.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jdq.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://afg.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rce.haohaochexian.top

[B13] 判断是否为数字
来源：http://zyk.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://vrr.zdqjudy.top

PHP:  is_numeric($x)
来源：http://jie.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://flw.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgi.yuanzhike.top

Java: x instanceof Number
来源：http://hho.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aaq.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://aip.havefunace.top

C#:   x is int or double or decimal
来源：http://zml.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://sja.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ugm.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jhz.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://lmt.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://vnv.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://ols.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ivj.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yun.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pmv.sufxvd.cn

[B15] 布尔运算与取反
来源：http://uif.hongshengwenyu.top

Py:   a and b or not c
来源：http://fgv.nwbrower.top

PHP:  $a && $b || !$c
来源：http://jay.zdbjq.cn

JS:   a && b || !c
来源：http://cje.tian-w.cn

TS:   a && b || !c
来源：http://ivz.wangdashe.top

Java: a && b || !c
来源：http://lwp.fengsongda.top

Go:   a && b || !c
来源：http://oue.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://ilv.gogol.net.cn

C#:   a && b || !c
来源：http://sff.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://qpm.vehdjk.com

Py:   if not data: return
来源：http://ykz.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://hyt.zycfv.cn

JS:   if (!data) return;
来源：http://duw.hammf.cn

TS:   if (!data) return;
来源：http://azl.feifeiyinyue.top

Java: if (data == null) return;
来源：http://mxi.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://ksi.uphjek.com

Ruby: return if data.nil?
来源：http://rlb.gotoacloud.top

C#:   if (data == null) return;
来源：http://npo.redwolf501.top

================================================================================
来源：http://dok.fanxiaobao.xyz

C. 函数与作用域
来源：http://ice.jqgufenzy.top

================================================================================
来源：http://jck.ehwqpu.com

[C01] 定义函数
来源：http://wla.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://myu.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bkd.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://wch.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cft.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fsn.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hbz.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://cbp.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hpa.hysaishi.cn

[C02] 默认参数
来源：http://cjd.sweek.top

Py:   def greet(name="World"): return name
来源：http://vjw.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://byd.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://uuw.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://zsv.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qhp.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://szf.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://ztv.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://qrv.9152youxi.cn

[C03] 可变参数
来源：http://oak.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://xea.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jwk.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iul.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qnl.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cxv.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gvh.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://zxh.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixj.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://pni.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rov.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vcu.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mlp.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hjr.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://owd.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://lfh.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://ghw.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://lag.iojbl.cn

[C05] 返回多个值
来源：http://wfa.sjlbkw.cn

Py:   return a, b
来源：http://qlu.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://tux.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hdc.jyoumei.cn

TS:   return { a, b };
来源：http://hkn.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://utg.svipenyu.cn

Go:   return a, b
来源：http://bum.epnwcf.com

Ruby: return a, b
来源：http://svz.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://aua.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://rct.fktsv.cn

Py:   square = lambda x: x * x
来源：http://yhj.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wzy.yuanzhike.top

JS:   const square = x => x * x;
来源：http://axr.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://qvu.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oqp.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://yjy.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://cxn.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://xzh.guannengcc.top

[C07] 把函数作为参数传入
来源：http://pvo.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ykj.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://wfk.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ury.zdqjudy.top

TS:   arr.map(String)
来源：http://lid.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fka.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tde.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://dvm.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://bjy.tianlin.xyz

[C08] 闭包
来源：http://uar.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jdc.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://btv.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mie.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eng.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ptb.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ned.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jys.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sld.ywan-chungtsiang.top

[C09] 递归
来源：http://vlt.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sfm.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ino.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhm.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddy.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjg.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jjo.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://btn.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcw.316326.xyz

[C10] 变量作用域
来源：http://uhx.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ddk.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dhz.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eam.kuanghao11.cn

TS:   同 JS
来源：http://ced.xziqi.cn

Java: 方法内为块级作用域
来源：http://qqg.sxryk.cn

Go:   花括号块级作用域
来源：http://kao.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://clc.xylfe.cn

C#:   块级作用域
来源：http://tyx.kuanghao11.cn

[C11] 模块导入与导出
来源：http://vgu.uphjek.com

Py:   from module import func
来源：http://edf.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ubw.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://prx.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rvg.gotoacloud.top

Java: import java.util.List;
来源：http://fih.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bkb.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://xie.nanxuanxn.top

C#:   using System.Text;
来源：http://tyh.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://fms.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://jnk.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://kaa.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://qph.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://bme.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ftl.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://thw.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://dub.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cqu.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://mxv.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uoj.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://add.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qtm.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yeu.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://onn.hysaishi.cn

Go:   func add(a, b int) int
来源：http://dej.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jnf.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://dxw.yj20258888.top

[C14] 泛型函数
来源：http://pog.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://edf.gzhubu.top

PHP:  // 无泛型
来源：http://kbc.yj20258.top

JS:   // 无泛型
来源：http://opz.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dpg.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://opp.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tlj.shangyingyoupin.top

Ruby: # 无泛型
来源：http://bwn.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kwp.jianghu66.top

[C15] 解构 / 展开参数
来源：http://fwi.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://icw.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://dqg.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tzv.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kiz.havefunace.top

Java: // 无解构
来源：http://kbg.daxiang520.top

Go:   // 无解构
来源：http://bzw.tanke756.top

Ruby: a, b = pair
来源：http://ltv.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://cul.meibo888.top

[C16] 函数 / 方法重载
来源：http://rnx.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uft.0kj1m.cn

PHP:  // 无重载
来源：http://gwo.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wnb.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://yro.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hjg.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://cqs.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://boz.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mpv.aibaodan.cn

================================================================================
来源：http://wyv.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://fry.ydjk.org.cn

================================================================================
来源：http://qqo.yuxming.cn

[D01] 创建数组 / 列表
来源：http://uru.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pep.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jal.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fuw.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xtc.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pbh.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://wav.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://qto.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://frc.zycfv.cn

[D02] 追加元素到末尾
来源：http://zas.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://efl.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aok.hysaishi.cn

JS:   arr.push(4);
来源：http://hny.mhx1999.top

TS:   arr.push(4);
来源：http://fac.ywan-chungtsiang.top

Java: list.add(4);
来源：http://jgj.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://vun.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://gkm.ppjwa.cn

C#:   list.Add(4);
来源：http://cke.hammf.cn

[D03] 在指定位置插入元素
来源：http://rxn.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://yzz.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbr.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dyh.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://qoh.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://bfd.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://lkg.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wra.sweek.top

C#:   list.Insert(0, 0);
来源：http://snf.yfazqb.com

[D04] 删除元素
来源：http://qph.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kgv.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://owa.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mgz.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://pan.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yor.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jkf.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ruo.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sja.havefunace.top

[D05] 访问与修改元素
来源：http://mbz.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jar.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zle.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oec.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://nrm.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://qxi.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://qwo.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://skd.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wrm.xuanzx.com

[D06] 数组长度
来源：http://lbq.ydjk.org.cn

Py:   len(arr)
来源：http://ypm.hongshengwenyu.top

PHP:  count($arr);
来源：http://vwt.zycfv.cn

JS:   arr.length
来源：http://wbm.ydzc1.top

TS:   arr.length
来源：http://kzw.svipenyu.cn

Java: list.size();
来源：http://upr.hesvh.cn

Go:   len(arr)
来源：http://nsw.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://qjm.cdnleiting.top

C#:   list.Count;
来源：http://woe.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://amt.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mwa.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://kvn.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://lwj.pycfn.com


<!-- 参考信息 -->