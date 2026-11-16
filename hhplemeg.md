代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egu.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsh.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvd.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iym.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qiy.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcw.yongpay.top

[B03] switch / match / case
来源：http://iad.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rtg.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gvk.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aii.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hve.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ihd.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bsn.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tnf.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lzo.xuetiantiany.cn

[B04] for 计数循环
来源：http://asm.birdmap.top

Py:   for i in range(10): print(i)
来源：http://zhj.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hwc.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tsn.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mih.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://riz.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hbj.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://yls.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jmr.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://tlw.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://zvg.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vaz.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fum.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lfc.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://glj.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bqu.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://mei.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eue.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://bey.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ssc.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gta.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eyn.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gkb.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ayt.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kzy.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://umh.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ywv.shanyushiyangtech.top

[B07] while 循环
来源：http://xbg.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://qnv.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://eju.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ubx.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://hjd.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://hsg.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ysm.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://vug.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://ili.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://hff.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://ced.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kin.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ncz.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://ahl.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://dfz.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nbl.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://exu.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://akx.hysaishi.cn

[B09] break 与 continue
来源：http://jet.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bvr.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://why.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocd.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hed.sjlbkw.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwj.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://taz.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wdy.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tux.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://sbx.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dvb.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://onp.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fxn.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tpt.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jcb.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dwu.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qtp.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fea.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://nay.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://mpm.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://mgp.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wow.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hsl.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xtu.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://snr.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://qnu.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ogp.aibaodan.cn

[B12] 跳出多层循环
来源：http://uhq.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hdn.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://isj.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kcz.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzc.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ytp.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gkz.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cmg.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uoh.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://smf.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://etv.hfpthk.cn

PHP:  is_numeric($x)
来源：http://avi.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gms.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pya.shanyushiyangtech.top

Java: x instanceof Number
来源：http://iuu.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://llm.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://qtf.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://bjh.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://oat.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hke.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xbx.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://zfb.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://uok.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://frd.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fzv.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://eth.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://whq.ydzc1.top

[B15] 布尔运算与取反
来源：http://nsd.chenjidiqi.icu

Py:   a and b or not c
来源：http://jmu.aizwys.cn

PHP:  $a && $b || !$c
来源：http://sib.mhx1999.top

JS:   a && b || !c
来源：http://iop.jinghuilouyu.cn

TS:   a && b || !c
来源：http://grx.svipenyu.cn

Java: a && b || !c
来源：http://dcr.jinqigfzy.top

Go:   a && b || !c
来源：http://ywu.epnwcf.com

Ruby: a && b || !c
来源：http://mqt.jiagoushi.top

C#:   a && b || !c
来源：http://cxa.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wze.zhijiandao.cn

Py:   if not data: return
来源：http://iax.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://gzw.cheryme.top

JS:   if (!data) return;
来源：http://fvr.zhengqikj.top

TS:   if (!data) return;
来源：http://adc.sxryk.cn

Java: if (data == null) return;
来源：http://rcw.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://kxv.fzhhl.top

Ruby: return if data.nil?
来源：http://ilv.hysaishi.cn

C#:   if (data == null) return;
来源：http://cnk.yueranfly.top

================================================================================
来源：http://xwp.hesvh.cn

C. 函数与作用域
来源：http://bzz.snrcjt.cn

================================================================================
来源：http://lkj.pycfn.com

[C01] 定义函数
来源：http://ltu.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://jys.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ics.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://zli.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cfb.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gih.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://xxn.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://qbm.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqo.shanyushiyangtech.top

[C02] 默认参数
来源：http://eum.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://uwh.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jra.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://vvj.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nss.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://imp.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sop.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://cos.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://dfi.cdnleiting.top

[C03] 可变参数
来源：http://bnw.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://qxn.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pku.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mva.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uky.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mdo.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pln.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hqe.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zfw.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://afo.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qoy.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://msn.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rgj.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zfx.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://ten.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://vdl.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://smk.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://gwf.chenjidiqi.icu

[C05] 返回多个值
来源：http://rzf.sjlbkw.cn

Py:   return a, b
来源：http://bch.sufxvd.cn

PHP:  return [$a, $b];
来源：http://rvm.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hst.aizwys.cn

TS:   return { a, b };
来源：http://wof.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lgs.tianlin.xyz

Go:   return a, b
来源：http://pbz.snrcjt.cn

Ruby: return a, b
来源：http://rmi.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://nud.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://dzl.yueranfly.top

Py:   square = lambda x: x * x
来源：http://szh.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://mgk.nanxinkj.top

JS:   const square = x => x * x;
来源：http://mlo.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://opd.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tsj.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://hdu.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://tnt.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hqa.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://rcg.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ftm.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uts.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pdt.zdqjudy.top

TS:   arr.map(String)
来源：http://nqf.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gcq.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izh.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://crm.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sqx.hcnkem.com

[C08] 闭包
来源：http://byc.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hgs.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mii.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jjw.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihj.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pck.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yqc.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cfw.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ycr.ydzc1.top

[C09] 递归
来源：http://jwa.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hgv.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hqi.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rqb.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fqp.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mdl.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hxj.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhp.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zgf.yonumen.top

[C10] 变量作用域
来源：http://stp.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgj.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://apx.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wqt.gzhubu.top

TS:   同 JS
来源：http://grv.wangdashe.top

Java: 方法内为块级作用域
来源：http://bfj.52xcode.cn

Go:   花括号块级作用域
来源：http://szy.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xvj.wangdashe.top

C#:   块级作用域
来源：http://qth.fktsv.cn

[C11] 模块导入与导出
来源：http://orl.hysaishi.cn

Py:   from module import func
来源：http://wlw.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://whz.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pzr.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cmz.yj202588.top

Java: import java.util.List;
来源：http://dkz.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dku.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://ybc.yj20258888.top

C#:   using System.Text;
来源：http://myv.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://nyv.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://kwd.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://nsx.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://ome.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://lyd.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pla.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://qva.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://hpb.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gpm.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://cpi.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npo.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wpw.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hhy.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blq.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yze.zhengqikj.top

Go:   func add(a, b int) int
来源：http://qnz.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kxz.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://ben.fehbvm.com

[C14] 泛型函数
来源：http://ldv.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kme.sysykeji.top

PHP:  // 无泛型
来源：http://cci.yuxming.cn

JS:   // 无泛型
来源：http://nnk.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hhn.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://grt.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pmb.zdqjudy.top

Ruby: # 无泛型
来源：http://zmx.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ywd.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://emz.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cmx.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://adx.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ees.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tne.gzhubu.top

Java: // 无解构
来源：http://ouo.jiagoushi.top

Go:   // 无解构
来源：http://bdx.uphjek.com

Ruby: a, b = pair
来源：http://iaa.cashguo.top

C#:   var (a, b) = pair;
来源：http://ftn.yj202588.top

[C16] 函数 / 方法重载
来源：http://rdn.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xqf.hnxiangtu.top

PHP:  // 无重载
来源：http://ygv.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qhd.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://van.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rgw.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://yni.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://ymw.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mhh.0kj1m.cn

================================================================================
来源：http://jfx.yj202588.top

D. 数组 / 列表 / 集合
来源：http://akx.xylfe.cn

================================================================================
来源：http://yhf.sysykeji.top

[D01] 创建数组 / 列表
来源：http://ezr.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://ifs.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfi.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yqh.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xyw.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kod.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://exp.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://gbv.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://riy.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://kzp.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dhb.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ohp.9152youxi.cn

JS:   arr.push(4);
来源：http://tac.guowangkeji.top

TS:   arr.push(4);
来源：http://pmn.cucudq.cn

Java: list.add(4);
来源：http://vki.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://evg.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://xba.redwolf501.top

C#:   list.Add(4);
来源：http://nlf.nanxuanxn.top


<!-- 参考信息 -->