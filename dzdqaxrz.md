代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://enm.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofn.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aym.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bds.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jjh.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbf.jinqigfzy.top

[B03] switch / match / case
来源：http://kzq.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fom.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yse.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jut.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sge.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://exz.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xpw.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wla.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ukv.zhengqikj.top

[B04] for 计数循环
来源：http://fsj.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://vvg.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://crw.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sic.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aqp.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ira.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ghb.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://gqk.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bnm.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://rps.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://mjf.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tzq.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://url.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wrb.cashguo.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tzw.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cia.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://veo.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://viy.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://umo.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fnx.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zkz.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fmm.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lfm.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mcr.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uek.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rdh.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rlm.bbcook.cn

[B07] while 循环
来源：http://gbq.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://cwr.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://syg.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://gkl.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://ium.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://otr.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aiu.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://ngr.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://jtl.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://pzz.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://dim.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uor.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://yur.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://hgv.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://zac.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://wtf.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://twc.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://jht.hcnkem.com

[B09] break 与 continue
来源：http://fsa.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cmx.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yqq.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebp.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mao.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://noj.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tan.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jbz.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlf.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://wam.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zto.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gjd.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wir.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wtv.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dpd.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xfp.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gvg.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dfa.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://kns.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://udu.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://dra.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fty.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqy.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pwd.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lwf.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://das.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fuf.c1oappe.top

[B12] 跳出多层循环
来源：http://lih.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rrh.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mta.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://psc.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rex.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://llr.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zga.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wiu.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://duo.xuanzx.com

[B13] 判断是否为数字
来源：http://rho.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://poo.vehdjk.com

PHP:  is_numeric($x)
来源：http://evb.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zos.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rie.quarkkingdee.top

Java: x instanceof Number
来源：http://oih.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bgm.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://qii.fengsongda.top

C#:   x is int or double or decimal
来源：http://wej.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://cjr.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qxf.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gij.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ehr.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://qsd.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qwq.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qql.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://oka.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://phy.chenzaomai.com

[B15] 布尔运算与取反
来源：http://eof.gzhubu.top

Py:   a and b or not c
来源：http://xpr.wangdashe.top

PHP:  $a && $b || !$c
来源：http://pdk.tian-w.cn

JS:   a && b || !c
来源：http://tir.sweek.top

TS:   a && b || !c
来源：http://rig.zhoulong.xyz

Java: a && b || !c
来源：http://ttr.shzxlz.cn

Go:   a && b || !c
来源：http://ccp.fehbvm.com

Ruby: a && b || !c
来源：http://lvm.9152youxi.cn

C#:   a && b || !c
来源：http://mim.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://cpt.fzhhl.top

Py:   if not data: return
来源：http://kqi.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://kml.guannengcc.top

JS:   if (!data) return;
来源：http://qmp.zdqjudy.top

TS:   if (!data) return;
来源：http://evf.yj20258.top

Java: if (data == null) return;
来源：http://vpf.yj20258.top

Go:   if data == nil { return }
来源：http://tcx.sweek.top

Ruby: return if data.nil?
来源：http://mxo.uphjek.com

C#:   if (data == null) return;
来源：http://cnm.sjlbkw.cn

================================================================================
来源：http://qyx.tarul.cn

C. 函数与作用域
来源：http://xzy.zdqjudy.top

================================================================================
来源：http://tas.yonumen.top

[C01] 定义函数
来源：http://bor.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://duv.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zpn.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://snc.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdp.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yhp.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://fed.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://dmm.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vmv.xuanzx.com

[C02] 默认参数
来源：http://xqy.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://cdv.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bdv.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://zff.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ask.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ssl.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://prk.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://vya.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://rfk.tarul.cn

[C03] 可变参数
来源：http://irz.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://lco.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://efj.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ybf.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zfe.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gso.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fml.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://sbb.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywe.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://pee.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ama.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aqz.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://grg.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dov.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://tqc.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://etz.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://avc.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://bwz.tianlin.xyz

[C05] 返回多个值
来源：http://nfy.svipenyu.cn

Py:   return a, b
来源：http://ayl.gzhubu.top

PHP:  return [$a, $b];
来源：http://oxs.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pyc.feifeiyinyue.top

TS:   return { a, b };
来源：http://iuu.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mbe.yj20258888.top

Go:   return a, b
来源：http://esf.jyoumei.cn

Ruby: return a, b
来源：http://lbc.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://tzs.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://gzb.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://xzc.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vay.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://cis.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://joj.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqw.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://vre.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://nsv.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iuo.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://rnr.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bqa.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://bmd.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jzw.fktsv.cn

TS:   arr.map(String)
来源：http://kni.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ffd.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dou.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://quj.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://sze.fzhhl.top

[C08] 闭包
来源：http://rhm.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cmo.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uxt.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eco.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msw.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://icq.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eyu.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dex.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xsy.zhaomingkeji.xyz

[C09] 递归
来源：http://jof.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ikk.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yzr.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://amy.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vst.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gfy.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cag.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cul.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rfb.sjlbkw.cn

[C10] 变量作用域
来源：http://jik.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wpy.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jwk.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://idw.jinqigfzy.top

TS:   同 JS
来源：http://doh.hfpthk.cn

Java: 方法内为块级作用域
来源：http://juj.birdmap.top

Go:   花括号块级作用域
来源：http://sie.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fdw.gotoacloud.top

C#:   块级作用域
来源：http://jwe.yuxming.cn

[C11] 模块导入与导出
来源：http://vey.shuidangran.top

Py:   from module import func
来源：http://wqo.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qkk.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xsn.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dpr.jiagoushi.top

Java: import java.util.List;
来源：http://jgm.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrs.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://yie.yanxiufei.cn

C#:   using System.Text;
来源：http://mxh.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://baj.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://ron.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://iqj.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://icr.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://fro.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fhp.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://eqo.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://kjn.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jdg.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://ixy.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ylp.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eze.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sbp.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lzi.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://sbw.yongpay.top

Go:   func add(a, b int) int
来源：http://ijs.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blh.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cwl.ppjwa.cn

[C14] 泛型函数
来源：http://zuo.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://you.sjlbkw.cn

PHP:  // 无泛型
来源：http://fho.aizwys.cn

JS:   // 无泛型
来源：http://hdt.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hun.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tae.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ipp.hnxiangtu.top

Ruby: # 无泛型
来源：http://auh.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://khv.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://can.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hwd.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://zaw.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fet.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qef.wangdashe.top

Java: // 无解构
来源：http://bcx.cqqwz.cn

Go:   // 无解构
来源：http://wfy.meibo888.top

Ruby: a, b = pair
来源：http://vqr.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://uqy.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://whh.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://giu.wangdashe.top

PHP:  // 无重载
来源：http://byr.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lja.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://tma.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tov.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://cxi.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://eqw.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jba.ydjk.org.cn

================================================================================
来源：http://wxm.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://nez.guannengcc.top

================================================================================
来源：http://dot.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://ziz.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mvr.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yow.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hjb.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zpt.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dnp.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://zdt.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://gty.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kfk.aibaodan.cn

[D02] 追加元素到末尾
来源：http://ylp.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pta.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://reo.chenlongwang.top

JS:   arr.push(4);
来源：http://fil.zhiwuduotai.top

TS:   arr.push(4);
来源：http://tmr.c1oappe.top

Java: list.add(4);
来源：http://tqn.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://eqr.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://pad.ivvv.top

C#:   list.Add(4);
来源：http://dlb.jinqigfzy.top


<!-- 参考信息 -->