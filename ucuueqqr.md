代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vek.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akg.zhixingplan.top

[B03] switch / match / case
来源：http://coq.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bst.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bxw.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fva.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cut.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lon.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zhc.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://svt.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cbq.zhengqikj.top

[B04] for 计数循环
来源：http://fyd.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://zuq.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wxd.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vmf.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fpm.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tnl.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nli.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://ewd.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nnb.yongpay.top

[B05] 遍历数组 / 列表
来源：http://hdu.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://eie.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zfg.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ijt.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wgp.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://dpx.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cyu.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://fdb.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://miq.havefunace.top

[B06] 遍历字典 / 对象
来源：http://zve.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hmf.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpz.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxc.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xfv.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pfi.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nnt.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsd.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nip.tianlin.xyz

[B07] while 循环
来源：http://ojt.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://fsj.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://rjm.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://ttb.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://jby.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://ojr.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rsb.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://dbp.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://kmr.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://ovx.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://psc.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jjh.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://juy.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://wdx.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://ntn.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yah.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qcz.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://zje.fzhhl.top

[B09] break 与 continue
来源：http://qqo.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hyi.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yqu.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrf.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wiv.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orn.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfh.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://typ.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibu.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://fcn.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bnc.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xfy.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://scq.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hsu.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qro.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yab.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://noi.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vfy.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://ehx.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://mkw.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://koo.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjr.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pbx.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ibj.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://znz.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://kqa.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyn.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://fjx.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hbb.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mtk.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://teq.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pdo.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwx.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://czs.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gch.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lrf.bjfxy.top

[B13] 判断是否为数字
来源：http://rmt.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://fmo.xylfe.cn

PHP:  is_numeric($x)
来源：http://dze.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jah.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xly.yvedp.cn

Java: x instanceof Number
来源：http://gfs.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cgm.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://jig.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://beq.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://xcz.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kqk.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://daz.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://cau.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://gsj.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://eyr.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdm.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://fhz.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://umx.meibo888.top

[B15] 布尔运算与取反
来源：http://ugx.jinghuilouyu.cn

Py:   a and b or not c
来源：http://can.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://aki.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://mjd.cheryme.top

TS:   a && b || !c
来源：http://tdr.shangyingyoupin.top

Java: a && b || !c
来源：http://yxd.jinqigufen.top

Go:   a && b || !c
来源：http://wbr.52xcode.cn

Ruby: a && b || !c
来源：http://shj.yonumen.top

C#:   a && b || !c
来源：http://qyr.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kbc.wangdashe.top

Py:   if not data: return
来源：http://whr.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://mao.jinqigfzy.top

JS:   if (!data) return;
来源：http://lzo.jqgufenzy.top

TS:   if (!data) return;
来源：http://wey.redwolf501.top

Java: if (data == null) return;
来源：http://acl.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://gtg.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://lvw.jqgufenzy.top

C#:   if (data == null) return;
来源：http://ght.epnwcf.com

================================================================================
来源：http://kaw.meibo888.top

C. 函数与作用域
来源：http://msz.mhx1999.top

================================================================================
来源：http://jco.hongshengwenyu.top

[C01] 定义函数
来源：http://hfl.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://dlc.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://caf.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://bgp.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://znb.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ghp.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://jbw.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://grs.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eef.daria6918.cn

[C02] 默认参数
来源：http://npp.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://ueo.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rie.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://qcj.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gnv.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://orf.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyd.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://hfi.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://hlu.uphjek.com

[C03] 可变参数
来源：http://jea.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://hwl.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bgb.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ynk.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ukh.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gfj.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://agw.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://xoo.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gys.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://fux.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wsp.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tvx.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cik.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://trq.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://zqi.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://hcm.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://dhb.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://cge.nanxinkj.top

[C05] 返回多个值
来源：http://avd.zdqjudy.top

Py:   return a, b
来源：http://ekn.zycfv.cn

PHP:  return [$a, $b];
来源：http://hko.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsk.hongshengwenyu.top

TS:   return { a, b };
来源：http://ogw.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mne.cashguo.top

Go:   return a, b
来源：http://glo.hywenlv.cn

Ruby: return a, b
来源：http://ubc.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://vme.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://jvm.epnwcf.com

Py:   square = lambda x: x * x
来源：http://dwt.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bag.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://mzo.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://vii.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://frg.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://sqj.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://jkb.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rqy.zycfv.cn

[C07] 把函数作为参数传入
来源：http://zev.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pqc.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://flw.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yxx.smart0.xyz

TS:   arr.map(String)
来源：http://guq.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eqp.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bnm.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://ggs.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iud.cucudq.cn

[C08] 闭包
来源：http://wdc.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ccc.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zlp.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eah.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vmg.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://efs.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eis.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gzf.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zvu.cdnleiting.top

[C09] 递归
来源：http://qxs.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jap.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://njf.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rtn.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zck.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vwj.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bau.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uyw.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xnc.yangfankeji.com

[C10] 变量作用域
来源：http://fjq.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bae.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qst.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://drt.tianlin.xyz

TS:   同 JS
来源：http://tbe.sysykeji.top

Java: 方法内为块级作用域
来源：http://mtn.zhengqikj.top

Go:   花括号块级作用域
来源：http://cjb.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://flg.pengpengdd.cyou

C#:   块级作用域
来源：http://czn.smart0.xyz

[C11] 模块导入与导出
来源：http://ekp.shanyushiyangtech.top

Py:   from module import func
来源：http://yud.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ysj.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ack.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hhw.cheryme.top

Java: import java.util.List;
来源：http://xlq.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://noq.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://jww.gogol.net.cn

C#:   using System.Text;
来源：http://eie.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://jgu.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://wyd.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://uun.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://rkk.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://ahe.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zxx.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://kxd.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://uzz.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://xia.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://dqz.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dix.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hlw.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ghk.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqi.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://smb.fzhhl.top

Go:   func add(a, b int) int
来源：http://zez.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uks.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://zkn.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://gph.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xaq.chenzaomai.com

PHP:  // 无泛型
来源：http://xrw.jianghu66.top

JS:   // 无泛型
来源：http://zkv.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ucj.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qzj.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fmq.nwbrower.top

Ruby: # 无泛型
来源：http://oba.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oli.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://kgx.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gct.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://kfg.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qbl.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzc.gotoacloud.top

Java: // 无解构
来源：http://qek.daxiang520.top

Go:   // 无解构
来源：http://lvf.nanxuanxn.top

Ruby: a, b = pair
来源：http://pbl.andypj.xyz

C#:   var (a, b) = pair;
来源：http://fbm.bbcook.cn

[C16] 函数 / 方法重载
来源：http://gtw.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://krx.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://ong.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zqd.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://zzf.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nyj.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://jrg.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://xlz.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qsb.tian-w.cn

================================================================================
来源：http://svx.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://yxq.cashguo.top

================================================================================
来源：http://okk.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://aki.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qni.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dbt.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jep.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zps.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tuz.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://mfi.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://mce.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ihb.hesvh.cn

[D02] 追加元素到末尾
来源：http://mhr.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qmm.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxq.gogol.net.cn

JS:   arr.push(4);
来源：http://khb.jqgfzy.top

TS:   arr.push(4);
来源：http://nbj.jqgfzy.top

Java: list.add(4);
来源：http://gwh.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://vih.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://daa.mhx1999.top

C#:   list.Add(4);
来源：http://fzc.iojbl.cn

[D03] 在指定位置插入元素
来源：http://rkn.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://hhi.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxd.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fvu.sweek.top


<!-- 参考信息 -->