代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebt.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://poo.mhx1999.top

[B03] switch / match / case
来源：http://zph.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fzj.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jyh.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://klg.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cou.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bjn.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iuk.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xko.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rkr.ctjpmb.com

[B04] for 计数循环
来源：http://rit.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://wdj.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://muf.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjc.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ope.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uyd.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yqr.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://voj.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dtx.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://nre.epnwcf.com

Py:   for item in arr: print(item)
来源：http://ukv.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rkn.xuanzx.com

JS:   for (const item of arr) { console.log(item); }
来源：http://djj.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yxf.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://crn.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yzv.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://ung.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xvd.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://tyt.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://jre.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dmy.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xle.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wme.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iin.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cxd.gogol.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xyx.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://owk.cqqwz.cn

[B07] while 循环
来源：http://mil.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://wzd.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://vis.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://mxm.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://gys.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://oac.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yxl.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://yli.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://azf.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://seq.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://diq.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fcg.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://czo.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://vzv.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://ivv.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cfb.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://sew.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://emz.cdnleiting.top

[B09] break 与 continue
来源：http://pnr.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wda.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sde.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krv.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgt.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qgm.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gim.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cir.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szq.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://poi.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tsv.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ljv.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://osz.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bqq.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wfz.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tse.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ier.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pym.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://xwp.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://vhj.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://hpt.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rqf.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqc.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fmt.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://thp.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://ioe.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mth.zycfv.cn

[B12] 跳出多层循环
来源：http://zuq.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cht.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bul.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xae.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://trq.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gym.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pax.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sxg.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fws.hfpthk.cn

[B13] 判断是否为数字
来源：http://nnj.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://vcr.yonumen.top

PHP:  is_numeric($x)
来源：http://lxv.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iij.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iih.fehbvm.com

Java: x instanceof Number
来源：http://ekq.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://odu.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://que.yongpay.top

C#:   x is int or double or decimal
来源：http://tjb.bbcook.cn

[B14] 判断值是否在集合内
来源：http://hvm.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hay.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dso.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://zxm.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://dam.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uvm.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gdp.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://ici.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qln.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://ian.fanxiaobao.xyz

Py:   a and b or not c
来源：http://hez.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://rhc.zhiwuduotai.top

JS:   a && b || !c
来源：http://kun.hammf.cn

TS:   a && b || !c
来源：http://mui.kuanghao11.cn

Java: a && b || !c
来源：http://was.cashguo.top

Go:   a && b || !c
来源：http://iqi.cashguo.top

Ruby: a && b || !c
来源：http://ohg.yongpay.top

C#:   a && b || !c
来源：http://zeg.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://bir.fengsongda.top

Py:   if not data: return
来源：http://cjq.yonumen.top

PHP:  if (!$data) { return; }
来源：http://qao.yuanzhike.top

JS:   if (!data) return;
来源：http://msm.bbcook.cn

TS:   if (!data) return;
来源：http://ndj.yvedp.cn

Java: if (data == null) return;
来源：http://qvr.ppjwa.cn

Go:   if data == nil { return }
来源：http://hxq.svipenyu.cn

Ruby: return if data.nil?
来源：http://ows.uphjek.com

C#:   if (data == null) return;
来源：http://wsf.bjfxy.top

================================================================================
来源：http://btp.birdmap.top

C. 函数与作用域
来源：http://gpr.zdqjudy.top

================================================================================
来源：http://amj.0kj1m.cn

[C01] 定义函数
来源：http://xkt.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://xzq.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzm.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://stb.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://enk.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qmn.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://nvj.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://uof.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.nanxinkj.top

[C02] 默认参数
来源：http://kdd.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://nec.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://hds.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://mvl.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wpm.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bbf.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cml.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://bgp.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://tnq.zhengqikj.top

[C03] 可变参数
来源：http://czd.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://rtl.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jdy.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zey.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqk.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ead.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezh.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://exa.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ttd.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://awa.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fnq.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://umi.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://slx.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hak.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://fbn.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://epm.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://ite.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://img.cashguo.top

[C05] 返回多个值
来源：http://paw.hnqzz.top

Py:   return a, b
来源：http://elt.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://uks.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wmk.zdqjudy.top

TS:   return { a, b };
来源：http://vvs.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cwn.jinqigfzy.top

Go:   return a, b
来源：http://mhc.gzhubu.top

Ruby: return a, b
来源：http://uwo.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://zzt.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://lxi.yj20258888.top

Py:   square = lambda x: x * x
来源：http://ooa.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://frt.bjfxy.top

JS:   const square = x => x * x;
来源：http://cve.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://rjo.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rqz.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://ook.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://rfu.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rdd.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://yhx.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ptq.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://asj.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xgs.sufxvd.cn

TS:   arr.map(String)
来源：http://wmw.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://icq.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zpp.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://bok.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ovp.dianchejie.cn

[C08] 闭包
来源：http://zjb.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lgk.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rwp.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vrp.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mcf.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yhw.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://smo.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tcz.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lvq.jqgfzy.top

[C09] 递归
来源：http://vch.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fdb.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qac.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vco.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppj.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ciq.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aca.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sae.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zts.cashguo.top

[C10] 变量作用域
来源：http://nqa.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyl.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfw.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mye.hesvh.cn

TS:   同 JS
来源：http://gtu.tanke756.top

Java: 方法内为块级作用域
来源：http://wmf.jinqigufen.top

Go:   花括号块级作用域
来源：http://tnl.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hlb.bbcook.cn

C#:   块级作用域
来源：http://uup.fzhhl.top

[C11] 模块导入与导出
来源：http://csx.zhongyouzk.top

Py:   from module import func
来源：http://ixw.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://duy.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lsg.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ugk.tanke756.top

Java: import java.util.List;
来源：http://lsv.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://asu.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://zun.xuetiantiany.cn

C#:   using System.Text;
来源：http://mup.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://jip.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://wsx.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://irv.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://lkz.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://yad.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bfb.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://oex.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://pex.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iqn.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://tds.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hbg.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjm.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jov.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ghp.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://npp.jinqigufen.top

Go:   func add(a, b int) int
来源：http://lev.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xqe.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://uuy.jinghuilouyu.cn

[C14] 泛型函数
来源：http://vwt.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kae.redwolf501.top

PHP:  // 无泛型
来源：http://zny.xuanzx.com

JS:   // 无泛型
来源：http://mjx.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://clk.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zug.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gyw.316326.xyz

Ruby: # 无泛型
来源：http://vdv.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hwg.jianghu66.top

[C15] 解构 / 展开参数
来源：http://udd.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tve.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://ffl.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mmn.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tck.jianghu66.top

Java: // 无解构
来源：http://ptt.fanxiaobao.xyz

Go:   // 无解构
来源：http://wni.chenlongwang.top

Ruby: a, b = pair
来源：http://kyy.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://elr.tarul.cn

[C16] 函数 / 方法重载
来源：http://rbp.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lbi.jianghu66.top

PHP:  // 无重载
来源：http://zqt.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fbs.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://fuz.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://ndu.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://hnw.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://osk.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kzp.316326.xyz

================================================================================
来源：http://btv.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://dqq.jqgfzy.top

================================================================================
来源：http://fbe.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://jpb.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ehw.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gsg.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gvi.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hec.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xhi.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://njp.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://xve.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vwo.daria6918.cn

[D02] 追加元素到末尾
来源：http://htk.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nhv.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bre.cqqwz.cn

JS:   arr.push(4);
来源：http://sex.mhx1999.top

TS:   arr.push(4);
来源：http://xcd.meibo888.top

Java: list.add(4);
来源：http://gce.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://bzi.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://juu.yonumen.top

C#:   list.Add(4);
来源：http://okg.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://tnm.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://ikg.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iro.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mis.cdnleiting.top


<!-- 参考信息 -->