代发 wailian999

Py:   for i in range(10): print(i)
来源：http://jdw.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kwm.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxp.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvl.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysc.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bqf.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://ebr.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vsb.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://bpz.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://vgq.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iha.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hpx.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://viq.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xff.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tic.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://bgu.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eyr.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://fkc.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xil.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://auc.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzc.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yeu.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lep.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hss.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ksu.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cct.sjlbkw.cn

[B07] while 循环
来源：http://jcs.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://dgz.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nzw.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://eel.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://dvc.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://vep.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://euc.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://imw.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://zin.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://swz.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://nas.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qzu.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://dvo.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://rsb.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://ioy.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://opa.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://qux.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://mwu.jinqigufen.top

[B09] break 与 continue
来源：http://qwe.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eus.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://txo.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgw.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grb.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbh.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xch.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dfm.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqa.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://qgg.zhongyouzk.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vkq.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://urp.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bfy.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bfh.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://div.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://upd.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oxm.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tar.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://dwn.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://tcd.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://kms.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vby.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lde.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nvk.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aef.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://bme.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ifl.mhx1999.top

[B12] 跳出多层循环
来源：http://dfy.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://rdq.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://mfs.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rgq.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zkr.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ung.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rkf.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vnw.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://boa.hfpthk.cn

[B13] 判断是否为数字
来源：http://mnj.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://xxv.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://igb.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eon.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jel.gzhubu.top

Java: x instanceof Number
来源：http://zat.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://owh.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://jwl.bbcook.cn

C#:   x is int or double or decimal
来源：http://wdk.shuidangran.top

[B14] 判断值是否在集合内
来源：http://mad.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cqu.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://smy.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://elr.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://han.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://evl.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fcx.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kex.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cnq.epnwcf.com

[B15] 布尔运算与取反
来源：http://amj.yj202588.top

Py:   a and b or not c
来源：http://stm.andypj.xyz

PHP:  $a && $b || !$c
来源：http://xgj.guannengcc.top

JS:   a && b || !c
来源：http://dqq.hnqzz.top

TS:   a && b || !c
来源：http://wtl.sxryk.cn

Java: a && b || !c
来源：http://wfs.52xcode.cn

Go:   a && b || !c
来源：http://gnc.gaohongyu789.top

Ruby: a && b || !c
来源：http://gbt.ctjpmb.com

C#:   a && b || !c
来源：http://zwp.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://fdi.zhiwuduotai.top

Py:   if not data: return
来源：http://wbo.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://rvx.shanyushiyangkeji.top

JS:   if (!data) return;
来源：http://zuz.ivvv.top

TS:   if (!data) return;
来源：http://ukw.ivvv.top

Java: if (data == null) return;
来源：http://zoe.gzhubu.top

Go:   if data == nil { return }
来源：http://gdu.haohaochexian.top

Ruby: return if data.nil?
来源：http://guo.yj20258.top

C#:   if (data == null) return;
来源：http://eth.snrcjt.cn

================================================================================
来源：http://rom.zdqjudy.top

C. 函数与作用域
来源：http://sbs.feifeiyinyue.top

================================================================================
来源：http://rrc.haohaochexian.top

[C01] 定义函数
来源：http://wey.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://wrr.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixz.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://cbu.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xtt.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wjv.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://lpd.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://gne.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aqu.andypj.xyz

[C02] 默认参数
来源：http://xnv.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://yli.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://emi.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://juv.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gwq.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aau.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsr.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://yvq.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://pxz.yfazqb.com

[C03] 可变参数
来源：http://xsq.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://hfj.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lwx.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pwi.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tff.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://seg.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dvj.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fzb.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bbp.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://uop.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mmx.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gze.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dqs.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://olp.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://azk.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://jbq.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://epv.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://nfw.havefunace.top

[C05] 返回多个值
来源：http://aeu.yueranfly.top

Py:   return a, b
来源：http://src.zhengqikj.top

PHP:  return [$a, $b];
来源：http://taz.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lgx.wangshuangyany.cn

TS:   return { a, b };
来源：http://urq.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bxc.cashguo.top

Go:   return a, b
来源：http://ucz.yj20258.top

Ruby: return a, b
来源：http://xrk.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://bia.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://snc.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://mtk.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wnn.ybcxt.top

JS:   const square = x => x * x;
来源：http://pbz.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://dkk.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ahl.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://gyv.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://okm.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://unv.yj20258.top

[C07] 把函数作为参数传入
来源：http://pax.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://luo.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://jtf.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dmt.shangyingyoupin.top

TS:   arr.map(String)
来源：http://qlu.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qug.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ilg.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://azh.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kap.cashguo.top

[C08] 闭包
来源：http://dfw.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xtv.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uor.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://til.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxl.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://owo.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cyq.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://snn.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ahx.sjlbkw.cn

[C09] 递归
来源：http://hyk.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rdo.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ite.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tnp.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://stb.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vkd.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pti.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jwv.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qom.yj20258888.top

[C10] 变量作用域
来源：http://ffa.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btn.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://inc.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tpa.meibo888.top

TS:   同 JS
来源：http://cxj.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://pec.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://hvh.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hle.cashguo.top

C#:   块级作用域
来源：http://gvi.hywenlv.cn

[C11] 模块导入与导出
来源：http://faz.ydzc1.top

Py:   from module import func
来源：http://hnh.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mec.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://axj.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qoq.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://ffr.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ecd.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://qii.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://dxl.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://prj.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://eww.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://eey.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://mtg.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://nzx.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uzq.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://irf.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://wwb.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bpq.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://glv.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eap.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dau.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cds.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://omw.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qhn.nwbrower.top

Go:   func add(a, b int) int
来源：http://lue.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xin.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://rrs.havefunace.top

[C14] 泛型函数
来源：http://uad.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://igb.shuidangran.top

PHP:  // 无泛型
来源：http://ymv.yj20258.top

JS:   // 无泛型
来源：http://pex.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hve.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xqe.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qrh.zycfv.cn

Ruby: # 无泛型
来源：http://xjc.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ggg.yueranfly.top

[C15] 解构 / 展开参数
来源：http://eke.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ajc.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://meq.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fyh.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gjl.quarkkingdee.top

Java: // 无解构
来源：http://jpw.cdnleiting.top

Go:   // 无解构
来源：http://kbc.hfpthk.cn

Ruby: a, b = pair
来源：http://lnk.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://olh.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://dgr.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cgv.cucudq.cn

PHP:  // 无重载
来源：http://wxl.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rpj.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://lap.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://atd.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://xsz.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://tbl.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uwj.fengsongda.top

================================================================================
来源：http://dkz.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://gji.fehbvm.com

================================================================================
来源：http://egr.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://bag.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cig.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dwz.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nyy.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yvs.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zmi.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://gkn.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://zmn.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zaa.yj202588.top

[D02] 追加元素到末尾
来源：http://kwt.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hvi.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adb.guannengcc.top

JS:   arr.push(4);
来源：http://eaj.pycfn.com

TS:   arr.push(4);
来源：http://uhn.c1oappe.top

Java: list.add(4);
来源：http://aao.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://nyz.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://yop.epnwcf.com

C#:   list.Add(4);
来源：http://ops.shuidangran.top

[D03] 在指定位置插入元素
来源：http://ycp.yonumen.top

Py:   arr.insert(0, 0)
来源：http://bon.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eod.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kdp.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://bjy.gotoacloud.top

Java: list.add(0, 0);
来源：http://fmt.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://xjk.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zgx.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://kzm.cdnleiting.top

[D04] 删除元素
来源：http://mkc.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zcw.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ojj.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uqj.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://tiv.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zan.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dfm.c1oappe.top


<!-- 参考信息 -->