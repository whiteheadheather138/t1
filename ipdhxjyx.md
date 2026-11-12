代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghp.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyl.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwm.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xgo.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cmi.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxg.andypj.xyz

[B03] switch / match / case
来源：http://nit.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nnf.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dns.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mrt.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lnv.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bur.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fcx.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nyh.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hje.guannengcc.top

[B04] for 计数循环
来源：http://mmy.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://loi.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lsa.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unq.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfi.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://khr.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tln.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://pfg.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://stf.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://wna.meibo888.top

Py:   for item in arr: print(item)
来源：http://owm.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qaq.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tgg.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mdv.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fns.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jau.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://noc.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xes.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://ivv.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://efy.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mhj.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dgi.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xah.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tyd.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gfa.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kor.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ycx.haohaochexian.top

[B07] while 循环
来源：http://xpk.shuidangran.top

Py:   while i < 10: i += 1
来源：http://gqe.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://hsu.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://ijj.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://wps.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://fzk.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lch.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://ujo.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://ane.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://xuh.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://nmj.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://adh.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://skm.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://eha.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://lca.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cvw.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://wjx.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://lld.hammf.cn

[B09] break 与 continue
来源：http://gce.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lyi.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://psg.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qce.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nou.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yej.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rar.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qlc.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daq.vehdjk.com

[B10] 遍历同时拿索引
来源：http://hdi.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vzm.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kmh.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rgb.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abh.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pra.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwb.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://olw.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tih.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://jlq.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://oqo.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://mli.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsk.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dch.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sqj.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ygx.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://gwi.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bzm.yonumen.top

[B12] 跳出多层循环
来源：http://nlp.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kyi.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymp.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifn.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rga.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ahx.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dyc.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tuz.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hpf.snrcjt.cn

[B13] 判断是否为数字
来源：http://msr.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://acr.zdbjq.cn

PHP:  is_numeric($x)
来源：http://yws.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://foy.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzg.vehdjk.com

Java: x instanceof Number
来源：http://gju.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bef.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://jfx.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://cbd.epnwcf.com

[B14] 判断值是否在集合内
来源：http://zlm.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://teq.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gei.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://fxs.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://xri.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lgj.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hdc.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://seh.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdl.yuanzhike.top

[B15] 布尔运算与取反
来源：http://txf.pycfn.com

Py:   a and b or not c
来源：http://pum.hcnkem.com

PHP:  $a && $b || !$c
来源：http://lvx.zhoulong.xyz

JS:   a && b || !c
来源：http://xtm.daxiang520.top

TS:   a && b || !c
来源：http://mca.fzhhl.top

Java: a && b || !c
来源：http://aby.dianchejie.cn

Go:   a && b || !c
来源：http://inp.smart0.xyz

Ruby: a && b || !c
来源：http://ocz.vehdjk.com

C#:   a && b || !c
来源：http://fkq.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://oxe.ivvv.top

Py:   if not data: return
来源：http://xye.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://mie.tarul.cn

JS:   if (!data) return;
来源：http://yxo.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://pol.hywenlv.cn

Java: if (data == null) return;
来源：http://cpi.zhoulong.xyz

Go:   if data == nil { return }
来源：http://ukg.wangdashe.top

Ruby: return if data.nil?
来源：http://srb.zhongyouzk.top

C#:   if (data == null) return;
来源：http://qnj.fanxiaobao.xyz

================================================================================
来源：http://nqv.zhaomingkeji.xyz

C. 函数与作用域
来源：http://bhb.fzhhl.top

================================================================================
来源：http://wlr.jianghu66.top

[C01] 定义函数
来源：http://zox.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://grl.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nsw.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://krn.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xan.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ryz.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cos.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://lgk.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zwn.yfazqb.com

[C02] 默认参数
来源：http://nle.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://nog.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uod.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://arm.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zln.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://odg.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jvh.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://ceo.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gxv.gzhubu.top

[C03] 可变参数
来源：http://apl.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://gzz.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qtp.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dzg.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://thd.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zeb.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tsq.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zkh.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mrc.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://bya.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lfv.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ypd.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qas.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdt.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://zdx.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://qgx.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://bnm.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://yvy.pengpengdd.cyou

[C05] 返回多个值
来源：http://chm.fanxiaobao.xyz

Py:   return a, b
来源：http://dqb.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://nvl.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ghw.zycfv.cn

TS:   return { a, b };
来源：http://yio.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ffh.c1oappe.top

Go:   return a, b
来源：http://oou.hesvh.cn

Ruby: return a, b
来源：http://fcg.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://djo.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://rwk.tarul.cn

Py:   square = lambda x: x * x
来源：http://qlj.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bqy.yj202588.top

JS:   const square = x => x * x;
来源：http://dui.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://bjd.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rle.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://muc.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://nep.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://azc.smart0.xyz

[C07] 把函数作为参数传入
来源：http://wgx.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lny.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gob.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://riu.redwolf501.top

TS:   arr.map(String)
来源：http://gfi.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zpk.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjb.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://bmr.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dpa.cucudq.cn

[C08] 闭包
来源：http://pks.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ygn.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rsh.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yqp.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dcu.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://imc.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dqk.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdy.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rob.zhaomingkeji.xyz

[C09] 递归
来源：http://axt.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ngt.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://igx.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uew.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwj.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ium.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://juq.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pei.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wsw.sxryk.cn

[C10] 变量作用域
来源：http://idy.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yey.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fdn.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qkz.aizwys.cn

TS:   同 JS
来源：http://aer.vehdjk.com

Java: 方法内为块级作用域
来源：http://fxh.xinyue.icu

Go:   花括号块级作用域
来源：http://nct.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gmw.zhaomingkeji.xyz

C#:   块级作用域
来源：http://xtz.fktsv.cn

[C11] 模块导入与导出
来源：http://neo.hammf.cn

Py:   from module import func
来源：http://vci.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://otp.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dth.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mwa.jianghu66.top

Java: import java.util.List;
来源：http://oly.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lhd.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://pei.daxiang520.top

C#:   using System.Text;
来源：http://phu.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://tik.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://wbp.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://oxl.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://zrq.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://ctf.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nve.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://ere.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://fhy.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wft.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://tah.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zad.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzc.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bkd.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfc.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://twa.jiagoushi.top

Go:   func add(a, b int) int
来源：http://mnv.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jqp.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://vqp.hfpthk.cn

[C14] 泛型函数
来源：http://vrq.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://otw.pengpengdd.cyou

PHP:  // 无泛型
来源：http://utu.shangyingyoupin.top

JS:   // 无泛型
来源：http://iji.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ira.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ecz.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rnu.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://oft.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sem.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://fjc.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qnp.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://lju.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tnt.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yhu.gzhubu.top

Java: // 无解构
来源：http://fjv.52xcode.cn

Go:   // 无解构
来源：http://rwe.cdnleiting.top

Ruby: a, b = pair
来源：http://klg.yonumen.top

C#:   var (a, b) = pair;
来源：http://vjf.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://gjc.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rmv.zdbjq.cn

PHP:  // 无重载
来源：http://dhx.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ibi.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://rfc.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jdu.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://jcc.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://gdi.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tjl.aibaodan.cn

================================================================================
来源：http://mdk.uphjek.com

D. 数组 / 列表 / 集合
来源：http://spf.pycfn.com

================================================================================
来源：http://mkj.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://vrj.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://umf.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hty.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ghx.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hbk.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sha.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://tuj.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://iha.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://brq.hcnkem.com

[D02] 追加元素到末尾
来源：http://hwf.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://egl.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mhx.smart0.xyz

JS:   arr.push(4);
来源：http://dhm.jinqigufen.top

TS:   arr.push(4);
来源：http://tsz.sysykeji.top

Java: list.add(4);
来源：http://iol.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://dnn.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://uss.yj202588.top

C#:   list.Add(4);
来源：http://jno.cqqwz.cn


<!-- 参考信息 -->