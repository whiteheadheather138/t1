代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eki.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymq.xziqi.cn

[B03] switch / match / case
来源：http://ueb.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wcb.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://now.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vfq.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cut.smart0.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://une.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzz.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://biy.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kti.gogol.net.cn

[B04] for 计数循环
来源：http://aai.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://sun.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ksy.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yph.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyg.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eiy.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yek.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://wkl.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://klj.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://jks.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://pzr.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ybn.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fxf.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sun.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ohc.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jnm.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://ybq.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ydi.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://oho.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pxt.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ggl.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xmx.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pry.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://snv.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xak.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mns.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uow.iojbl.cn

[B07] while 循环
来源：http://wgn.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://ajs.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kpl.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://gav.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://rcs.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://cox.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uro.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://sjz.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://elk.tanke756.top

[B08] do-while（至少执行一次）
来源：http://ydb.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://crq.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uxn.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://mrh.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://fbw.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://jdn.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nzw.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://usw.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://ueb.zhoulong.xyz

[B09] break 与 continue
来源：http://atg.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wzu.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eoq.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ylp.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnc.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfj.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pgp.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hhr.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrq.tian-w.cn

[B10] 遍历同时拿索引
来源：http://tsw.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zoz.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hsj.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hfx.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azh.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nhm.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ptm.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dmh.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kgt.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://bte.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://ydi.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://fjp.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjl.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygq.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aal.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dot.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://kpq.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fqe.yueranfly.top

[B12] 跳出多层循环
来源：http://pyj.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ura.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://myp.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjr.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dff.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jtg.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qpk.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tjf.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xpk.yangfankeji.com

[B13] 判断是否为数字
来源：http://xnu.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://djs.ctjpmb.com

PHP:  is_numeric($x)
来源：http://rvf.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zns.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iyn.xuetiantiany.cn

Java: x instanceof Number
来源：http://sfb.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dku.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://qnf.uphjek.com

C#:   x is int or double or decimal
来源：http://vtv.cashguo.top

[B14] 判断值是否在集合内
来源：http://vjq.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yom.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wmh.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://zli.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://bga.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uvy.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://syq.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nep.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://roa.chenzaomai.com

[B15] 布尔运算与取反
来源：http://coi.yueranfly.top

Py:   a and b or not c
来源：http://bqo.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://mub.vqdsnc.cn

JS:   a && b || !c
来源：http://bvt.pengpengdd.cyou

TS:   a && b || !c
来源：http://adq.cdnleiting.top

Java: a && b || !c
来源：http://rur.meibo888.top

Go:   a && b || !c
来源：http://tvy.quarkkingdee.top

Ruby: a && b || !c
来源：http://kgr.chenlongwang.top

C#:   a && b || !c
来源：http://eku.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://inp.wangdashe.top

Py:   if not data: return
来源：http://bew.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://puj.gotoacloud.top

JS:   if (!data) return;
来源：http://tqp.hcnkem.com

TS:   if (!data) return;
来源：http://lue.jqgufenzy.top

Java: if (data == null) return;
来源：http://gkd.bjfxy.top

Go:   if data == nil { return }
来源：http://pyr.jlsjyb.cn

Ruby: return if data.nil?
来源：http://jee.xuanzx.com

C#:   if (data == null) return;
来源：http://roq.epnwcf.com

================================================================================
来源：http://jre.yfazqb.com

C. 函数与作用域
来源：http://dyh.shangyingyoupin.top

================================================================================
来源：http://hlm.guowangkeji.top

[C01] 定义函数
来源：http://kss.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://vxe.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cvj.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://uat.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lkt.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nof.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://for.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://izh.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ezv.nanxuanxn.top

[C02] 默认参数
来源：http://qpv.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://cmj.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://cvu.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://ndh.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rkr.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sox.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bmb.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://tbn.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://xps.wangshuangyany.cn

[C03] 可变参数
来源：http://mjb.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://uzt.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uqa.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ton.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hid.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://amu.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jhh.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eyh.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yza.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://pyb.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wlm.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hfo.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hme.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rah.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://geo.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://zrm.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://ejy.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://mcw.jinqigufen.top

[C05] 返回多个值
来源：http://fdm.zhengqikj.top

Py:   return a, b
来源：http://mga.0kj1m.cn

PHP:  return [$a, $b];
来源：http://duv.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wrw.nanxinkj.top

TS:   return { a, b };
来源：http://ptr.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qxd.zycfv.cn

Go:   return a, b
来源：http://omq.0kj1m.cn

Ruby: return a, b
来源：http://qdj.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://san.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://uqm.fengsongda.top

Py:   square = lambda x: x * x
来源：http://nnt.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://uye.pycfn.com

JS:   const square = x => x * x;
来源：http://opk.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://oby.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://htm.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://qyv.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://oqp.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mfj.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://tdr.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aqh.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://djo.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://drn.ybcxt.top

TS:   arr.map(String)
来源：http://ybd.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gas.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ufh.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://uug.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iti.tanke756.top

[C08] 闭包
来源：http://kap.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fsb.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zsp.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ocq.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qje.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kej.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gca.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tcx.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uip.zdbjq.cn

[C09] 递归
来源：http://jkk.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fsf.cdnleiting.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxm.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lrt.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hph.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zzr.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pqj.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://glu.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sns.vehdjk.com

[C10] 变量作用域
来源：http://qip.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rlk.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ixr.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oxs.fzhhl.top

TS:   同 JS
来源：http://kjv.yj20258.top

Java: 方法内为块级作用域
来源：http://byy.snrcjt.cn

Go:   花括号块级作用域
来源：http://ckq.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fni.nwbrower.top

C#:   块级作用域
来源：http://rnc.xziqi.cn

[C11] 模块导入与导出
来源：http://wgw.yj202588.top

Py:   from module import func
来源：http://uws.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bzx.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://viw.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wsb.chenzaomai.com

Java: import java.util.List;
来源：http://jpf.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mec.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://lmc.ivvv.top

C#:   using System.Text;
来源：http://jtm.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://olc.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://dvb.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://eje.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://yzv.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://wdy.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lwt.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://gir.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://cum.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xkk.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://ogg.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kgp.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://thj.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jgn.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tmv.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://smy.chenzaomai.com

Go:   func add(a, b int) int
来源：http://neg.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syd.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rpi.svipenyu.cn

[C14] 泛型函数
来源：http://epl.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://klv.ydjk.org.cn

PHP:  // 无泛型
来源：http://pls.hnxiangtu.top

JS:   // 无泛型
来源：http://udn.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qdx.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xjk.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xrj.hywenlv.cn

Ruby: # 无泛型
来源：http://oym.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ydw.316326.xyz

[C15] 解构 / 展开参数
来源：http://nlq.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uya.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://zbb.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pja.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kdm.wangshuangyany.cn

Java: // 无解构
来源：http://eee.wangshuangyany.cn

Go:   // 无解构
来源：http://imy.dashuyun.cn

Ruby: a, b = pair
来源：http://ysd.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://fsa.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://cuo.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://duc.tianlin.xyz

PHP:  // 无重载
来源：http://qtl.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nop.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://ziy.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://njv.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://min.ybcxt.top

Ruby: # 无重载：靠动态参数
来源：http://yfk.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wsl.daria6918.cn

================================================================================
来源：http://xdw.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://flu.9152youxi.cn

================================================================================
来源：http://zyt.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://dgi.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovz.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lin.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkv.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tvo.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pfm.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://vak.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://szc.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://klx.daria6918.cn

[D02] 追加元素到末尾
来源：http://wec.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydt.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vcr.shzxlz.cn

JS:   arr.push(4);
来源：http://jer.jiagoushi.top

TS:   arr.push(4);
来源：http://bww.cdnleiting.top

Java: list.add(4);
来源：http://zrd.yj20258.top

Go:   arr = append(arr, 4)
来源：http://svp.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://uol.zhongyouzk.top

C#:   list.Add(4);
来源：http://ijt.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://kbd.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://atd.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://exn.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bil.yanxiufei.cn


<!-- 参考信息 -->