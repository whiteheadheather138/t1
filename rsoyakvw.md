代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwh.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbb.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxk.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://len.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xri.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsa.fehbvm.com

[B03] switch / match / case
来源：http://jbc.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hhq.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rps.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hbe.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czi.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://snm.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tqo.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ufa.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvt.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://rja.pycfn.com

Py:   for i in range(10): print(i)
来源：http://kio.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zhb.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nac.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://num.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://maf.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hgr.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://rah.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hil.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://onv.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://egi.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fvd.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://juy.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://btt.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rnq.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jjy.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://hxc.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ijp.cheryme.top

[B06] 遍历字典 / 对象
来源：http://cmn.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iyb.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gio.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://urx.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qev.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fil.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rso.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aaw.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://plt.birdmap.top

[B07] while 循环
来源：http://cfn.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://vjn.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rqr.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://cze.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://rpm.yonumen.top

Java: while (i < 10) { i++; }
来源：http://sxn.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bka.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://tav.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://zqj.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://lzv.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://hfd.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://esi.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://uyo.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://rdy.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://pws.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cns.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://let.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://pcz.tianlin.xyz

[B09] break 与 continue
来源：http://npx.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://anx.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mmg.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hof.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eeh.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wln.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lsv.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwq.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ntr.mhx1999.top

[B10] 遍历同时拿索引
来源：http://drd.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zgh.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://exk.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zbh.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sgk.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dgw.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://huu.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fns.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nfm.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://auk.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://wtb.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://dpo.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gaw.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzd.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://slr.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yes.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://zje.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://stf.dianchejie.cn

[B12] 跳出多层循环
来源：http://vjc.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fmf.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eau.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfc.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://isa.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vfg.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gsm.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aly.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ekx.jianghu66.top

[B13] 判断是否为数字
来源：http://rac.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://gem.yuxming.cn

PHP:  is_numeric($x)
来源：http://xfj.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://leb.hysaishi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mnj.gogol.net.cn

Java: x instanceof Number
来源：http://gef.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uma.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://ekn.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://app.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://crr.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hjl.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://giz.jiagoushi.top

JS:   [1, 2, 3].includes(x)
来源：http://vvd.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://ywk.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://mvs.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqa.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://zvm.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vxi.dianchejie.cn

[B15] 布尔运算与取反
来源：http://slp.shuidangran.top

Py:   a and b or not c
来源：http://azm.52xcode.cn

PHP:  $a && $b || !$c
来源：http://dvg.yongpay.top

JS:   a && b || !c
来源：http://uak.hnqzz.top

TS:   a && b || !c
来源：http://vga.shangyingyoupin.top

Java: a && b || !c
来源：http://ldi.ctjpmb.com

Go:   a && b || !c
来源：http://cpq.ydzc1.top

Ruby: a && b || !c
来源：http://isn.smart0.xyz

C#:   a && b || !c
来源：http://gda.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://wgf.52xcode.cn

Py:   if not data: return
来源：http://kyp.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://jsd.jinqigufen.top

JS:   if (!data) return;
来源：http://owc.yj20258.top

TS:   if (!data) return;
来源：http://wen.pengpengdd.cyou

Java: if (data == null) return;
来源：http://bro.52xcode.cn

Go:   if data == nil { return }
来源：http://zjn.jlsjyb.cn

Ruby: return if data.nil?
来源：http://zef.smart0.xyz

C#:   if (data == null) return;
来源：http://eui.jinyuanbaomall.cn

================================================================================
来源：http://qfd.c1oappe.top

C. 函数与作用域
来源：http://ulc.vqdsnc.cn

================================================================================
来源：http://xcm.316326.xyz

[C01] 定义函数
来源：http://qyt.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://iyn.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dhh.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://yxc.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://suh.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://uql.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://hjl.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://owl.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lrt.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://vsp.yj20258.top

Py:   def greet(name="World"): return name
来源：http://mcv.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ava.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://aee.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yfz.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ovi.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zvh.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://wqo.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://qha.shanyushiyangtech.top

[C03] 可变参数
来源：http://bpp.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://mfk.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qlc.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wff.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xmw.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ved.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cyv.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://ihi.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ihb.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://dhi.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kla.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bqk.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwn.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jid.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://vqx.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://hbo.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://bwn.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://bhv.jlsjyb.cn

[C05] 返回多个值
来源：http://jav.gaohongyu789.top

Py:   return a, b
来源：http://dad.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://wuj.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uzr.iojbl.cn

TS:   return { a, b };
来源：http://qxu.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uqn.0kj1m.cn

Go:   return a, b
来源：http://qwf.52xcode.cn

Ruby: return a, b
来源：http://zrm.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://kxm.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://kvl.fehbvm.com

Py:   square = lambda x: x * x
来源：http://gkf.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://suv.fehbvm.com

JS:   const square = x => x * x;
来源：http://vyp.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://wrg.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jtb.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://lbd.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://esk.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://alt.daxiang520.top

[C07] 把函数作为参数传入
来源：http://oub.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nba.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://cbw.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rjs.xuanzx.com

TS:   arr.map(String)
来源：http://txa.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uji.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rha.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://unc.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lij.redwolf501.top

[C08] 闭包
来源：http://sjw.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yon.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dkz.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vwa.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gym.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wcz.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oza.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dmk.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wrg.mhx1999.top

[C09] 递归
来源：http://vtt.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mze.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dhe.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kmt.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xnt.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xyb.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fgb.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ien.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxh.mhx1999.top

[C10] 变量作用域
来源：http://fiw.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kxv.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jbs.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mmc.fzhhl.top

TS:   同 JS
来源：http://iix.ppjwa.cn

Java: 方法内为块级作用域
来源：http://htz.jyoumei.cn

Go:   花括号块级作用域
来源：http://kpu.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ixe.gotoacloud.top

C#:   块级作用域
来源：http://vvg.jqgfzy.top

[C11] 模块导入与导出
来源：http://fdh.yuanzhike.top

Py:   from module import func
来源：http://obl.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dlk.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rrn.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jwi.tarul.cn

Java: import java.util.List;
来源：http://brp.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hob.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://ltp.cdnleiting.top

C#:   using System.Text;
来源：http://pwm.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://dcs.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://gfn.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://uyu.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://jya.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://vsn.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rpu.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://qnz.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://jrb.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rju.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://njb.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://orx.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbs.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dbv.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdq.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://bwj.hcnkem.com

Go:   func add(a, b int) int
来源：http://yto.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sel.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ryn.zhixingplan.top

[C14] 泛型函数
来源：http://kti.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uvi.xuanzx.com

PHP:  // 无泛型
来源：http://odl.jinghuilouyu.cn

JS:   // 无泛型
来源：http://ifx.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jhx.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sdw.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rre.nanxinkj.top

Ruby: # 无泛型
来源：http://oqk.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kba.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://rli.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qjj.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://wlo.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xrb.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fyx.shanyushiyangkeji.top

Java: // 无解构
来源：http://wfs.ybcxt.top

Go:   // 无解构
来源：http://xmy.zhongyouzk.top

Ruby: a, b = pair
来源：http://ikm.vehdjk.com

C#:   var (a, b) = pair;
来源：http://qst.wangdashe.top

[C16] 函数 / 方法重载
来源：http://jce.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ohi.sxryk.cn

PHP:  // 无重载
来源：http://mxb.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhl.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://gqr.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kuu.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://rdu.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://qbt.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vsc.jqgfzy.top

================================================================================
来源：http://iol.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://imr.cheryme.top

================================================================================
来源：http://zhq.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://vbs.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sho.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iot.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wcm.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xfo.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://myy.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://pgr.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://txr.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bea.jiagoushi.top

[D02] 追加元素到末尾
来源：http://zwk.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hxa.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rwx.jqgufenzy.top

JS:   arr.push(4);
来源：http://ugw.guowangkeji.top

TS:   arr.push(4);
来源：http://naf.yuxming.cn

Java: list.add(4);
来源：http://hye.havefunace.top

Go:   arr = append(arr, 4)
来源：http://etr.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://hee.yvedp.cn

C#:   list.Add(4);
来源：http://xtu.cucudq.cn


<!-- 参考信息 -->