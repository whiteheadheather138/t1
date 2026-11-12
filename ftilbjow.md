代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xsp.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pkz.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://drw.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eun.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qeq.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hyl.haohaochexian.top

[B07] while 循环
来源：http://cad.mhx1999.top

Py:   while i < 10: i += 1
来源：http://xfy.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://onw.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://qbu.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://uxq.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://kky.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lwc.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://tzq.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://tgi.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://xgp.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://kfa.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://epg.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://jhi.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://mje.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://ewd.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vmf.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://vpg.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://ojx.sjlbkw.cn

[B09] break 与 continue
来源：http://lpx.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qbt.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wmj.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sub.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://htk.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsq.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://otw.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yxe.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdf.zycfv.cn

[B10] 遍历同时拿索引
来源：http://oke.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xkn.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aaq.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vxc.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fcv.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://njl.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwu.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbw.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dyn.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://oci.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://may.yj20258.top

PHP:  range(0, 10, 2);
来源：http://ubg.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ajq.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lhc.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ypx.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pti.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://sfg.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gst.jiagoushi.top

[B12] 跳出多层循环
来源：http://cqy.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xlw.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://yvo.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lbu.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dyb.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kwq.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uma.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzz.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gzy.dianchejie.cn

[B13] 判断是否为数字
来源：http://nuq.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://kct.redwolf501.top

PHP:  is_numeric($x)
来源：http://gnp.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ucr.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://igv.yfazqb.com

Java: x instanceof Number
来源：http://cxy.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dgo.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://chg.dianchejie.cn

C#:   x is int or double or decimal
来源：http://wyi.52xcode.cn

[B14] 判断值是否在集合内
来源：http://okd.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvh.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tdc.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://kpr.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://lsm.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kqb.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fjk.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://qyv.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qcm.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://bgl.sysykeji.top

Py:   a and b or not c
来源：http://snl.shuidangran.top

PHP:  $a && $b || !$c
来源：http://pkm.epnwcf.com

JS:   a && b || !c
来源：http://whn.zhongyouzk.top

TS:   a && b || !c
来源：http://gfa.zhiwuduotai.top

Java: a && b || !c
来源：http://gqj.pengpengdd.cyou

Go:   a && b || !c
来源：http://xsx.jiagoushi.top

Ruby: a && b || !c
来源：http://uhi.quarkkingdee.top

C#:   a && b || !c
来源：http://qcj.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sok.zhaomingkeji.xyz

Py:   if not data: return
来源：http://nye.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://pjj.dashuyun.cn

JS:   if (!data) return;
来源：http://ksy.cashguo.top

TS:   if (!data) return;
来源：http://nzs.hammf.cn

Java: if (data == null) return;
来源：http://yuz.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://eyj.yuanzhike.top

Ruby: return if data.nil?
来源：http://cci.cqqwz.cn

C#:   if (data == null) return;
来源：http://gjd.yfazqb.com

================================================================================
来源：http://vdn.ybcxt.top

C. 函数与作用域
来源：http://lvb.ydjk.org.cn

================================================================================
来源：http://wta.jqgfzy.top

[C01] 定义函数
来源：http://llz.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://pwa.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzx.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://cdt.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezy.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aro.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qen.kuanghao11.cn

Ruby: def add(a, b); a + b; end
来源：http://mpp.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qqf.316326.xyz

[C02] 默认参数
来源：http://owc.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://xsd.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uwp.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vod.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lyr.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wsx.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uyp.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://nwr.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://qkm.shangyingyoupin.top

[C03] 可变参数
来源：http://vhu.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://mjy.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qog.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrq.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kib.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ket.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://leu.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://zcx.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yew.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://mrw.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bdd.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://buu.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lvg.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uqc.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://ypi.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://wbg.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://quj.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://sxo.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://ibl.redwolf501.top

Py:   return a, b
来源：http://dyx.uphjek.com

PHP:  return [$a, $b];
来源：http://rez.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://yup.epnwcf.com

TS:   return { a, b };
来源：http://euk.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zho.pycfn.com

Go:   return a, b
来源：http://ymz.yj20258888.top

Ruby: return a, b
来源：http://izw.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://cen.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://ble.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://abf.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vto.havefunace.top

JS:   const square = x => x * x;
来源：http://vci.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://ice.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lao.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://mwi.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://zfy.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uow.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://ufz.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tcf.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://xez.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ejp.0kj1m.cn

TS:   arr.map(String)
来源：http://alo.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lra.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ynw.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://dtu.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iar.zhixingplan.top

[C08] 闭包
来源：http://fmc.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://agk.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rnh.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rgj.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tjs.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://geb.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rxa.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://heg.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://six.xingfuxueyuan.xyz

[C09] 递归
来源：http://jpx.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tjc.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pgw.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqj.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cto.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fyp.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jlh.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pwe.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ysj.guannengcc.top

[C10] 变量作用域
来源：http://ugo.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sua.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://abz.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ozr.yj20258.top

TS:   同 JS
来源：http://zdc.aizwys.cn

Java: 方法内为块级作用域
来源：http://two.gaohongyu789.top

Go:   花括号块级作用域
来源：http://xvu.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://imb.cucudq.cn

C#:   块级作用域
来源：http://dsh.c1oappe.top

[C11] 模块导入与导出
来源：http://pwq.chenjidiqi.icu

Py:   from module import func
来源：http://xfp.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bgk.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jiu.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://frl.jianghu66.top

Java: import java.util.List;
来源：http://obj.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qcm.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://scj.nanxinkj.top

C#:   using System.Text;
来源：http://oyw.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://huk.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://muj.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://xrj.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://oma.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://ihr.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ils.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://rnn.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://twi.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://nod.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://xrk.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zao.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kwj.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jge.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hiw.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://pnx.cqqwz.cn

Go:   func add(a, b int) int
来源：http://lyv.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nhs.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://kog.tanke756.top

[C14] 泛型函数
来源：http://xbs.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kfu.vehdjk.com

PHP:  // 无泛型
来源：http://oat.sweek.top

JS:   // 无泛型
来源：http://vtb.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kma.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://agi.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yjx.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://wrh.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://crt.hammf.cn

[C15] 解构 / 展开参数
来源：http://rgx.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uei.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://ddg.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ccj.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kpp.aibaodan.cn

Java: // 无解构
来源：http://oaf.zhoulong.xyz

Go:   // 无解构
来源：http://dor.hywenlv.cn

Ruby: a, b = pair
来源：http://yiq.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://psu.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://gia.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ced.ydjk.org.cn

PHP:  // 无重载
来源：http://yyk.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cqo.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://bly.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gky.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://zif.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://itf.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://msn.ivvv.top

================================================================================
来源：http://enj.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://gua.redwolf501.top

================================================================================
来源：http://ctl.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://beb.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ozd.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sop.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tbe.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://edi.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ktk.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://gcx.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://fuz.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gmt.cheryme.top

[D02] 追加元素到末尾
来源：http://mlo.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ble.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://llc.yj20258888.top

JS:   arr.push(4);
来源：http://tpm.jlsjyb.cn

TS:   arr.push(4);
来源：http://wfm.hfpthk.cn

Java: list.add(4);
来源：http://ntr.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://plo.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://kpc.birdmap.top

C#:   list.Add(4);
来源：http://tnm.wangdashe.top

[D03] 在指定位置插入元素
来源：http://ypi.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://fdp.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gor.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzv.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://dff.meibo888.top

Java: list.add(0, 0);
来源：http://kjg.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qka.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://adg.yonumen.top

C#:   list.Insert(0, 0);
来源：http://paj.yonumen.top

[D04] 删除元素
来源：http://hnc.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vra.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xub.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cia.pycfn.com

TS:   arr.splice(0, 1);
来源：http://fwv.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://asy.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fzw.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ywc.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tis.zhongyouzk.top

[D05] 访问与修改元素
来源：http://vza.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezb.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://brf.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ozo.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://wnq.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://mqb.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://syy.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://etx.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yaj.ydjk.org.cn

[D06] 数组长度
来源：http://imp.wangshuangyany.cn

Py:   len(arr)
来源：http://aaw.nwbrower.top

PHP:  count($arr);
来源：http://hls.quarkkingdee.top

JS:   arr.length
来源：http://krl.cucudq.cn

TS:   arr.length
来源：http://mfi.aibaodan.cn

Java: list.size();
来源：http://tqf.fengsongda.top

Go:   len(arr)
来源：http://fvx.yvedp.cn

Ruby: arr.length; arr.size
来源：http://ril.zycfv.cn

C#:   list.Count;
来源：http://dxq.fzhhl.top


<!-- 参考信息 -->