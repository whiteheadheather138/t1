代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://roz.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlr.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xsc.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ivr.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gam.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zre.yongpay.top

[B07] while 循环
来源：http://dac.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://iyy.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pik.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://vzu.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://qub.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://pfw.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jdx.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://mpa.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://mrc.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://lag.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://ayn.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oud.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://qqi.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://ina.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://pil.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://fqt.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eiv.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://csf.sufxvd.cn

[B09] break 与 continue
来源：http://ekx.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cbj.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pca.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhg.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chv.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gin.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dxp.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oeo.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mno.fehbvm.com

[B10] 遍历同时拿索引
来源：http://hdl.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bxw.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fte.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cop.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fuy.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fcr.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rxu.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nvi.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cil.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://caq.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://png.tanke756.top

PHP:  range(0, 10, 2);
来源：http://dpn.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kez.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://scy.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xke.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ltt.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://cje.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wso.nanxinkj.top

[B12] 跳出多层循环
来源：http://xgh.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zjs.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://enx.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rok.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ahj.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wgt.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://egb.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fqh.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xjg.aizwys.cn

[B13] 判断是否为数字
来源：http://zhc.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://wtr.fehbvm.com

PHP:  is_numeric($x)
来源：http://cql.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mel.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxb.cashguo.top

Java: x instanceof Number
来源：http://den.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://inc.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://yyv.hywenlv.cn

C#:   x is int or double or decimal
来源：http://qsx.bjfxy.top

[B14] 判断值是否在集合内
来源：http://eup.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zga.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lws.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://txt.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://yei.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zrz.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://arp.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nzy.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tzc.316326.xyz

[B15] 布尔运算与取反
来源：http://blz.jianghu66.top

Py:   a and b or not c
来源：http://jyx.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://lsy.shzxlz.cn

JS:   a && b || !c
来源：http://dch.ydzc1.top

TS:   a && b || !c
来源：http://pmh.9152youxi.cn

Java: a && b || !c
来源：http://hqh.dianchejie.cn

Go:   a && b || !c
来源：http://ioi.316326.xyz

Ruby: a && b || !c
来源：http://fhj.guannengcc.top

C#:   a && b || !c
来源：http://tkj.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pue.zhoulong.xyz

Py:   if not data: return
来源：http://gbm.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://wfe.yj20258888.top

JS:   if (!data) return;
来源：http://qyw.sufxvd.cn

TS:   if (!data) return;
来源：http://crq.vqdsnc.cn

Java: if (data == null) return;
来源：http://qyt.epnwcf.com

Go:   if data == nil { return }
来源：http://ihm.vehdjk.com

Ruby: return if data.nil?
来源：http://csf.svipenyu.cn

C#:   if (data == null) return;
来源：http://snm.zhiwuduotai.top

================================================================================
来源：http://lll.kuanghao11.cn

C. 函数与作用域
来源：http://vwv.hcnkem.com

================================================================================
来源：http://dsy.fktsv.cn

[C01] 定义函数
来源：http://ysz.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://qxu.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wom.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://zjm.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjw.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hhw.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://fju.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://inf.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zrb.gzhubu.top

[C02] 默认参数
来源：http://zqa.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://swg.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://czh.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://crx.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wtu.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pav.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ucs.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://kbp.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://xxy.feifeiyinyue.top

[C03] 可变参数
来源：http://fpr.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://dao.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fge.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgy.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwb.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wyr.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zfm.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://wxt.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kmt.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://lrf.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tew.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bvf.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vbu.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://usa.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ksk.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://ipq.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://ywt.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://qav.yueranfly.top

[C05] 返回多个值
来源：http://npm.feifeiyinyue.top

Py:   return a, b
来源：http://tob.yj20258888.top

PHP:  return [$a, $b];
来源：http://fhy.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jlg.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://qro.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fft.pengpengdd.cyou

Go:   return a, b
来源：http://cym.sjlbkw.cn

Ruby: return a, b
来源：http://rpd.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://stq.yongpay.top

[C06] 匿名函数 / lambda
来源：http://bll.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://nsx.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ygs.aibaodan.cn

JS:   const square = x => x * x;
来源：http://zqt.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://ubo.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tzr.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://yjh.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://skn.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://lnz.cucudq.cn

[C07] 把函数作为参数传入
来源：http://jnh.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pnr.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://stk.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zvo.cqqwz.cn

TS:   arr.map(String)
来源：http://qdl.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ppj.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rdg.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://gbv.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lfj.pengpengdd.cyou

[C08] 闭包
来源：http://dqw.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bml.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uau.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mrx.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kgb.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://osx.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://epx.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kvu.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jfr.bjfxy.top

[C09] 递归
来源：http://jox.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bvd.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lky.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ups.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whq.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mez.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nem.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xot.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ppx.gogol.net.cn

[C10] 变量作用域
来源：http://ueu.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://izf.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gim.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvw.yonumen.top

TS:   同 JS
来源：http://xgp.iojbl.cn

Java: 方法内为块级作用域
来源：http://zow.dashuyun.cn

Go:   花括号块级作用域
来源：http://wwq.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qrb.epnwcf.com

C#:   块级作用域
来源：http://fup.sjlbkw.cn

[C11] 模块导入与导出
来源：http://evc.cheryme.top

Py:   from module import func
来源：http://ssq.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rwj.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bsb.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lge.iojbl.cn

Java: import java.util.List;
来源：http://yrs.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ljh.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://xuw.wangshuangyany.cn

C#:   using System.Text;
来源：http://xwe.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://tdc.hammf.cn

Py:   (lambda: print("run"))()
来源：http://oms.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://dhv.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://cld.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://fks.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pmz.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://dsz.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://kay.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://anc.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://pyn.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kuv.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqk.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hmv.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndn.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://uhi.sxryk.cn

Go:   func add(a, b int) int
来源：http://qgs.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zov.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://ipe.jqgufenzy.top

[C14] 泛型函数
来源：http://tpl.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://agd.yuanzhike.top

PHP:  // 无泛型
来源：http://fju.yuxming.cn

JS:   // 无泛型
来源：http://odr.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qau.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mbu.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yro.wangdashe.top

Ruby: # 无泛型
来源：http://pco.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vrq.sxryk.cn

[C15] 解构 / 展开参数
来源：http://zfn.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mfs.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://fdf.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ith.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mld.52xcode.cn

Java: // 无解构
来源：http://qak.vehdjk.com

Go:   // 无解构
来源：http://yqf.cashguo.top

Ruby: a, b = pair
来源：http://vbd.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://hyu.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://gtb.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://heb.haohaochexian.top

PHP:  // 无重载
来源：http://vwk.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://trp.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://vnn.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://avr.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://yzz.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://roy.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://swz.sufxvd.cn

================================================================================
来源：http://crq.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://yxb.chenjidiqi.icu

================================================================================
来源：http://dtu.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://cep.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://whj.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kuo.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ylv.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ajp.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://trj.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://lwk.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://ugn.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mus.ctjpmb.com

[D02] 追加元素到末尾
来源：http://hvz.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://glo.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://utr.gotoacloud.top

JS:   arr.push(4);
来源：http://rvt.xinyue.icu

TS:   arr.push(4);
来源：http://meh.feifeiyinyue.top

Java: list.add(4);
来源：http://tjv.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://ohy.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://tmx.haohaochexian.top

C#:   list.Add(4);
来源：http://vkj.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://vog.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ows.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://csi.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://akk.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://idu.cdnleiting.top

Java: list.add(0, 0);
来源：http://niu.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://wew.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kpf.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://lvk.chenjidiqi.icu

[D04] 删除元素
来源：http://iuw.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gtu.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lnd.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pox.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://wmf.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xfz.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mdn.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kyn.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hdh.jyoumei.cn

[D05] 访问与修改元素
来源：http://fgv.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjk.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ahp.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://krl.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://hee.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://xdw.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://zjj.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iho.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cwd.fktsv.cn

[D06] 数组长度
来源：http://ccq.52xcode.cn

Py:   len(arr)
来源：http://sfk.52xcode.cn

PHP:  count($arr);
来源：http://uds.svipenyu.cn

JS:   arr.length
来源：http://fdb.tarul.cn

TS:   arr.length
来源：http://jnf.xuanzx.com

Java: list.size();
来源：http://nil.mhx1999.top

Go:   len(arr)
来源：http://uzj.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://lhg.jiagoushi.top

C#:   list.Count;
来源：http://ibo.birdmap.top


<!-- 参考信息 -->