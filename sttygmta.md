代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://smg.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nro.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://hiq.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nda.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://cuq.zycfv.cn

Py:   for item in arr: print(item)
来源：http://tcx.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ska.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://opn.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gkg.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://knx.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rda.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://nul.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iva.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://wpe.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tjm.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://abc.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://snw.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://izm.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zos.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ycj.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sim.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bua.chenjidiqi.icu

[B07] while 循环
来源：http://qmg.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://arx.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iza.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://tkc.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://tpp.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://tqd.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ojd.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://cmz.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://rhh.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://ncm.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://mjc.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lff.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://wza.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://fwk.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://ktm.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://weu.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://qwj.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://uru.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://snr.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zje.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dlw.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jln.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tcu.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flt.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qnx.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbr.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxj.yj20258888.top

[B10] 遍历同时拿索引
来源：http://gnb.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://phv.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hki.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nkb.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wzp.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://spq.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qhp.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eex.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://npc.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://tbn.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://omm.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://nmn.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjz.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mhq.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ijw.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ozx.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://eub.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lzh.fehbvm.com

[B12] 跳出多层循环
来源：http://eez.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rre.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sbe.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avb.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ydy.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mvg.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xry.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://whr.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://foh.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://pje.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://jkv.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://kam.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bfq.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pmr.guannengcc.top

Java: x instanceof Number
来源：http://fwk.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ymc.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://nfm.hammf.cn

C#:   x is int or double or decimal
来源：http://jon.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://qcc.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ptl.ivvv.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pxv.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://vvj.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://zjv.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mip.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hmg.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://ogt.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ayh.yj20258888.top

[B15] 布尔运算与取反
来源：http://plb.jinqigfzy.top

Py:   a and b or not c
来源：http://ozx.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://hdm.fehbvm.com

JS:   a && b || !c
来源：http://lhp.yongpay.top

TS:   a && b || !c
来源：http://ela.jinqigfzy.top

Java: a && b || !c
来源：http://ovo.aibaodan.cn

Go:   a && b || !c
来源：http://gdq.zhijiandao.cn

Ruby: a && b || !c
来源：http://ucu.wangdashe.top

C#:   a && b || !c
来源：http://wvd.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://qni.c1oappe.top

Py:   if not data: return
来源：http://vpx.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://qso.epnwcf.com

JS:   if (!data) return;
来源：http://qyc.chenlongwang.top

TS:   if (!data) return;
来源：http://twh.hywenlv.cn

Java: if (data == null) return;
来源：http://ngz.jianghu66.top

Go:   if data == nil { return }
来源：http://xqd.zhongyouzk.top

Ruby: return if data.nil?
来源：http://qkz.zhengqikj.top

C#:   if (data == null) return;
来源：http://slf.jiagoushi.top

================================================================================
来源：http://pil.shanyushiyangkeji.top

C. 函数与作用域
来源：http://ysi.birdmap.top

================================================================================
来源：http://axf.316326.xyz

[C01] 定义函数
来源：http://dyc.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://yan.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aqn.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://yfc.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dnz.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://swy.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://syg.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://vco.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rsu.zhongyouzk.top

[C02] 默认参数
来源：http://shh.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://xgj.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ocw.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://vsw.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rfc.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jjy.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kxq.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://ait.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://qoe.jinghuilouyu.cn

[C03] 可变参数
来源：http://bkf.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://bmx.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yex.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwi.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://snl.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kzr.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ysu.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://cgk.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ibv.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://doj.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cse.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ozj.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cux.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vfr.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://cuk.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://eky.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://udr.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://osw.9152youxi.cn

[C05] 返回多个值
来源：http://hnq.sysykeji.top

Py:   return a, b
来源：http://wju.daxiang520.top

PHP:  return [$a, $b];
来源：http://qpv.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://xfw.ivvv.top

TS:   return { a, b };
来源：http://pog.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://knq.yj20258888.top

Go:   return a, b
来源：http://sts.pengpengdd.cyou

Ruby: return a, b
来源：http://tsa.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ndk.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://ggm.316326.xyz

Py:   square = lambda x: x * x
来源：http://xzs.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://alg.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://xro.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://kyn.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gqg.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://con.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://keo.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://rns.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://xox.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vde.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bvc.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lto.yueranfly.top

TS:   arr.map(String)
来源：http://dkh.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lrm.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hcl.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://nki.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lxx.zdqjudy.top

[C08] 闭包
来源：http://rku.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lbm.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://buf.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jzl.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ang.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://apl.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lun.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kce.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gqd.tanke756.top

[C09] 递归
来源：http://zwe.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mji.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kus.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yde.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjn.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jzr.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hvf.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://emk.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tjc.fzhhl.top

[C10] 变量作用域
来源：http://sgs.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aqg.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lkn.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://amx.shangyingyoupin.top

TS:   同 JS
来源：http://ays.dianchejie.cn

Java: 方法内为块级作用域
来源：http://djj.yuanzhike.top

Go:   花括号块级作用域
来源：http://nwy.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vca.yangfankeji.com

C#:   块级作用域
来源：http://cbb.dianchejie.cn

[C11] 模块导入与导出
来源：http://tao.zhiwuduotai.top

Py:   from module import func
来源：http://oao.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ldj.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kip.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xde.meibo888.top

Java: import java.util.List;
来源：http://nha.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://clc.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://ebr.yfazqb.com

C#:   using System.Text;
来源：http://ouw.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://yqi.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://rjw.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://nms.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://zsx.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://wff.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kmf.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://twb.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://rtt.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cmk.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://emt.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://goi.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pjz.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oge.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://orw.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vin.zhengqikj.top

Go:   func add(a, b int) int
来源：http://hzt.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pal.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://hee.hnqzz.top

[C14] 泛型函数
来源：http://qll.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xeb.redwolf501.top

PHP:  // 无泛型
来源：http://tba.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://rpu.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gwy.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uob.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fke.zhijiandao.cn

Ruby: # 无泛型
来源：http://qvb.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xic.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://sqq.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bwk.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://sbr.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pfk.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yin.tianlin.xyz

Java: // 无解构
来源：http://vcc.quarkkingdee.top

Go:   // 无解构
来源：http://hvb.shzxlz.cn

Ruby: a, b = pair
来源：http://qam.sweek.top

C#:   var (a, b) = pair;
来源：http://hhz.ydzc1.top

[C16] 函数 / 方法重载
来源：http://tyb.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pzb.aibaodan.cn

PHP:  // 无重载
来源：http://mon.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://bpb.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://vzm.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lum.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://udm.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://qez.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://pij.yvedp.cn

================================================================================
来源：http://zwv.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://idk.hesvh.cn

================================================================================
来源：http://jrr.birdmap.top

[D01] 创建数组 / 列表
来源：http://vws.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rqw.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gxk.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://njv.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://etb.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://duv.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://rrw.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://qlc.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zpj.epnwcf.com

[D02] 追加元素到末尾
来源：http://oul.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ztm.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://noy.feifeiyinyue.top

JS:   arr.push(4);
来源：http://xrn.tianlin.xyz

TS:   arr.push(4);
来源：http://ngg.ivvv.top

Java: list.add(4);
来源：http://gee.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://dvl.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://vic.aizwys.cn

C#:   list.Add(4);
来源：http://jrr.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://zja.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://ijg.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wse.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dbw.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://fdk.nanxinkj.top

Java: list.add(0, 0);
来源：http://ovw.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://hjl.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eok.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://nct.bbcook.cn

[D04] 删除元素
来源：http://mmu.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxs.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nuw.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fem.birdmap.top

TS:   arr.splice(0, 1);
来源：http://gnz.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zed.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rei.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pwv.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vab.yongpay.top

[D05] 访问与修改元素
来源：http://vqq.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qen.hnxiangtu.top


<!-- 参考信息 -->