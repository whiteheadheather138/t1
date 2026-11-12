代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yca.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jdq.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lgh.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://shl.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://whf.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kyg.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qjq.fanxiaobao.xyz

[B04] for 计数循环
来源：http://oyz.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://smi.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://omy.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ygf.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tcs.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tys.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mpe.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://nvj.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pss.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://nlv.fktsv.cn

Py:   for item in arr: print(item)
来源：http://uds.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hzd.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ggp.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ing.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oon.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vam.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://nlo.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nuw.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://ujw.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nws.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eph.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://haf.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zfa.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dvq.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zjm.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://djy.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jnw.snrcjt.cn

[B07] while 循环
来源：http://qcd.vehdjk.com

Py:   while i < 10: i += 1
来源：http://oim.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://kiy.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://vbo.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://cku.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://vzv.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kqu.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://rng.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://mvr.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://prn.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://tub.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zkm.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://tpi.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://irw.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://qif.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lwd.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://hfe.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://jsk.tianlin.xyz

[B09] break 与 continue
来源：http://xiu.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ewq.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zvc.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksi.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjv.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mod.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wry.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ubx.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://maa.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://rnv.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gzo.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qyy.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://izr.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bmx.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ner.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fyr.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nki.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://map.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://ikx.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://juf.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://bmv.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dbi.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyc.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dcj.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://msj.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://vhg.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uih.ctjpmb.com

[B12] 跳出多层循环
来源：http://ose.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kxw.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mcv.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nca.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijy.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nfo.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://drx.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sjr.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bib.hysaishi.cn

[B13] 判断是否为数字
来源：http://iuf.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://glx.sxryk.cn

PHP:  is_numeric($x)
来源：http://enm.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocv.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbh.hnqzz.top

Java: x instanceof Number
来源：http://ntc.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tkn.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://zlo.xinyue.icu

C#:   x is int or double or decimal
来源：http://djz.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://ivu.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wuf.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mst.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://mrq.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://gya.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ztg.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aby.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://kup.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vhw.tian-w.cn

[B15] 布尔运算与取反
来源：http://gym.cdnleiting.top

Py:   a and b or not c
来源：http://spr.andypj.xyz

PHP:  $a && $b || !$c
来源：http://rsx.fanxiaobao.xyz

JS:   a && b || !c
来源：http://dwn.cqqwz.cn

TS:   a && b || !c
来源：http://qvr.jlsjyb.cn

Java: a && b || !c
来源：http://tos.9152youxi.cn

Go:   a && b || !c
来源：http://yjl.zhixingplan.top

Ruby: a && b || !c
来源：http://gou.zhengqikj.top

C#:   a && b || !c
来源：http://fjb.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://drs.jlsjyb.cn

Py:   if not data: return
来源：http://wil.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://miv.jinqigfzy.top

JS:   if (!data) return;
来源：http://gig.wangdashe.top

TS:   if (!data) return;
来源：http://has.ydjk.org.cn

Java: if (data == null) return;
来源：http://bni.fktsv.cn

Go:   if data == nil { return }
来源：http://lfi.jiagoushi.top

Ruby: return if data.nil?
来源：http://nli.hywenlv.cn

C#:   if (data == null) return;
来源：http://esh.tanke756.top

================================================================================
来源：http://tie.hnqzz.top

C. 函数与作用域
来源：http://vka.xingfuxueyuan.xyz

================================================================================
来源：http://blv.zycfv.cn

[C01] 定义函数
来源：http://xym.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://xwz.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rks.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://iie.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgh.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://dfk.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://vtm.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://wks.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sga.gotoacloud.top

[C02] 默认参数
来源：http://zqn.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://qmy.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lcw.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://elb.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rcu.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://url.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bvf.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://awu.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://eif.sweek.top

[C03] 可变参数
来源：http://afa.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://qpw.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dfo.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vze.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://guf.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gym.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xmu.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://pkn.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzr.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://umr.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uwz.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pve.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://etn.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zzf.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://sjh.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://tyo.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://nth.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://kwm.yfazqb.com

[C05] 返回多个值
来源：http://sho.ctjpmb.com

Py:   return a, b
来源：http://gbx.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://gmi.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bzi.zhixingplan.top

TS:   return { a, b };
来源：http://tyr.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gph.cashguo.top

Go:   return a, b
来源：http://klm.kuanghao11.cn

Ruby: return a, b
来源：http://hqi.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://wxj.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://kma.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://bdm.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://etk.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://epe.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://pkd.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ulr.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ysu.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://mcv.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://wbw.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://pug.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fje.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xmq.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iig.zhoulong.xyz

TS:   arr.map(String)
来源：http://gul.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wsv.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cup.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://gis.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pss.redwolf501.top

[C08] 闭包
来源：http://omk.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zgd.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ulo.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nom.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pkk.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lcr.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rmx.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qme.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpx.hywenlv.cn

[C09] 递归
来源：http://fra.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lfz.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aov.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vxx.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lol.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yie.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fwa.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://htr.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rjv.shzxlz.cn

[C10] 变量作用域
来源：http://vpg.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eni.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mhx.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lss.shanyushiyangtech.top

TS:   同 JS
来源：http://brx.bjfxy.top

Java: 方法内为块级作用域
来源：http://dkg.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://sga.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ixw.yj20258.top

C#:   块级作用域
来源：http://qbd.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://suz.9152youxi.cn

Py:   from module import func
来源：http://fdv.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qsd.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tks.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqj.zdbjq.cn

Java: import java.util.List;
来源：http://zty.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fsk.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://wkw.pengpengdd.cyou

C#:   using System.Text;
来源：http://bpd.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://djj.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://aao.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://viy.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://abo.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://chk.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjo.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://csx.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://imc.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qyr.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://mkf.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hav.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypz.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlm.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bep.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://eoj.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://crz.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yqa.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://zki.yj20258.top

[C14] 泛型函数
来源：http://kfi.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zvx.fehbvm.com

PHP:  // 无泛型
来源：http://rjs.fktsv.cn

JS:   // 无泛型
来源：http://aop.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zne.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uhm.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dsk.yanxiufei.cn

Ruby: # 无泛型
来源：http://wjz.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ojz.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://kuj.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tyn.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://yuq.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nui.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://noi.birdmap.top

Java: // 无解构
来源：http://qrq.sufxvd.cn

Go:   // 无解构
来源：http://euk.xinyue.icu

Ruby: a, b = pair
来源：http://kmp.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://hvk.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://nvi.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fbq.meibo888.top

PHP:  // 无重载
来源：http://fns.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bap.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://wkm.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lig.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://jvc.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://qba.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://agd.cashguo.top

================================================================================
来源：http://lpe.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://dhs.redwolf501.top

================================================================================
来源：http://xxg.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://uzo.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://joi.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jrm.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xof.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ihj.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hra.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://uhi.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://ndj.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://usb.sufxvd.cn

[D02] 追加元素到末尾
来源：http://brx.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kpc.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gkn.bbcook.cn

JS:   arr.push(4);
来源：http://uqz.daria6918.cn

TS:   arr.push(4);
来源：http://hsj.ywan-chungtsiang.top

Java: list.add(4);
来源：http://fed.yj202588.top

Go:   arr = append(arr, 4)
来源：http://rkz.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://riu.feifeiyinyue.top

C#:   list.Add(4);
来源：http://fjq.cashguo.top

[D03] 在指定位置插入元素
来源：http://dsz.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://frp.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nob.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rct.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://wfe.hywenlv.cn

Java: list.add(0, 0);
来源：http://wxr.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://sit.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zak.zhiwuduotai.top


<!-- 参考信息 -->