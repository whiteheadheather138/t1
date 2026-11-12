代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fhw.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kid.bbcook.cn

[B03] switch / match / case
来源：http://wpl.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wig.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rsy.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sdo.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kfk.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wzg.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wvu.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://obq.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qhe.dianchejie.cn

[B04] for 计数循环
来源：http://sbq.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://kyg.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uts.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hzt.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://elo.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pzd.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jbg.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://vem.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rkq.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://byp.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://vau.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gng.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://btk.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ydh.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vin.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xgk.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://dav.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qpn.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://tci.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://agq.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cly.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qsq.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jav.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://anm.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rir.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xxn.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nyg.kuanghao11.cn

[B07] while 循环
来源：http://epz.yj202588.top

Py:   while i < 10: i += 1
来源：http://cel.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://cda.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://gou.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://sgq.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://jqb.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://drv.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://bsf.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://xbn.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://jlx.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://tjk.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iwv.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://evg.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://xwo.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://iup.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fgo.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vrj.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://ruc.uphjek.com

[B09] break 与 continue
来源：http://ljg.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pcp.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://psc.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eld.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bef.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oni.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://clg.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://twp.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gyj.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://zez.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iik.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvp.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oeb.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hou.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vgq.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fbo.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ayv.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://apd.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://kjf.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://ynq.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://xkt.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpm.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://foi.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dqd.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://paw.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://lng.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fyo.ivvv.top

[B12] 跳出多层循环
来源：http://bku.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hvb.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jcm.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wcr.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cmd.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uyr.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ajp.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rdi.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://crc.tanke756.top

[B13] 判断是否为数字
来源：http://dlt.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://mah.hfpthk.cn

PHP:  is_numeric($x)
来源：http://kcu.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqs.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://owv.guannengcc.top

Java: x instanceof Number
来源：http://xhi.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ytz.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://dso.ppjwa.cn

C#:   x is int or double or decimal
来源：http://eyh.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://lop.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xvg.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://omw.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://zvv.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vnb.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bwk.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ake.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://tpp.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dmx.nwbrower.top

[B15] 布尔运算与取反
来源：http://gfe.chenzaomai.com

Py:   a and b or not c
来源：http://mks.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://oji.fengsongda.top

JS:   a && b || !c
来源：http://eox.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://oip.9152youxi.cn

Java: a && b || !c
来源：http://axb.xinyue.icu

Go:   a && b || !c
来源：http://zmh.ivvv.top

Ruby: a && b || !c
来源：http://ona.shangyingyoupin.top

C#:   a && b || !c
来源：http://ncz.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rkk.0kj1m.cn

Py:   if not data: return
来源：http://ofq.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://shd.cdnleiting.top

JS:   if (!data) return;
来源：http://kvw.sjlbkw.cn

TS:   if (!data) return;
来源：http://xmm.yonumen.top

Java: if (data == null) return;
来源：http://pqa.hnxiangtu.top

Go:   if data == nil { return }
来源：http://yvu.aizwys.cn

Ruby: return if data.nil?
来源：http://hez.hcnkem.com

C#:   if (data == null) return;
来源：http://fki.yuanzhike.top

================================================================================
来源：http://rbb.yueranfly.top

C. 函数与作用域
来源：http://shc.dianchejie.cn

================================================================================
来源：http://ilo.yfazqb.com

[C01] 定义函数
来源：http://opd.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://jhu.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzm.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://afc.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqk.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ylp.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://myz.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://ntv.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qxk.jinghuilouyu.cn

[C02] 默认参数
来源：http://vny.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://fxu.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iya.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fwp.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://obf.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://wku.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gfv.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://guu.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://psj.ivvv.top

[C03] 可变参数
来源：http://uhf.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://ldx.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vnv.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ehq.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nmv.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nyb.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uro.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nxg.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://klc.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://akm.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yze.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sgu.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ukh.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awj.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://yin.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://wxs.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://her.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://yqw.zdqjudy.top

[C05] 返回多个值
来源：http://jre.pengpengdd.cyou

Py:   return a, b
来源：http://ftz.fengsongda.top

PHP:  return [$a, $b];
来源：http://maf.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zor.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://pno.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhy.zdbjq.cn

Go:   return a, b
来源：http://kak.ybcxt.top

Ruby: return a, b
来源：http://jor.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://sbk.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://oyo.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://xip.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bsy.sysykeji.top

JS:   const square = x => x * x;
来源：http://vai.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://qmf.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dqb.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://hbh.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://gfa.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wnh.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://tmr.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://glf.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://abd.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rls.redwolf501.top

TS:   arr.map(String)
来源：http://wmb.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tnr.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://osn.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://lks.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://min.hesvh.cn

[C08] 闭包
来源：http://adt.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hvb.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oec.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jwm.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qhj.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zwu.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jua.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sdy.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ybe.ppjwa.cn

[C09] 递归
来源：http://oor.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yoh.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qgl.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pbl.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uro.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://efu.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lyw.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://czs.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dca.fktsv.cn

[C10] 变量作用域
来源：http://vku.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nwl.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qhk.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cuw.shanyushiyangkeji.top

TS:   同 JS
来源：http://ugs.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://qxz.sysykeji.top

Go:   花括号块级作用域
来源：http://itm.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wyx.pycfn.com

C#:   块级作用域
来源：http://sig.yj20258888.top

[C11] 模块导入与导出
来源：http://jzu.haohaochexian.top

Py:   from module import func
来源：http://ooc.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pym.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hex.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wra.fktsv.cn

Java: import java.util.List;
来源：http://irf.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://isq.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://ity.aizwys.cn

C#:   using System.Text;
来源：http://tpa.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://rwz.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://qto.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://ync.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://xdl.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://xgs.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qzo.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://iya.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://rca.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tjj.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://koq.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fgp.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ius.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iuy.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdn.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hww.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://zmz.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ddy.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tqi.xziqi.cn

[C14] 泛型函数
来源：http://vzp.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qyf.hfpthk.cn

PHP:  // 无泛型
来源：http://fqw.hnqzz.top

JS:   // 无泛型
来源：http://jmv.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dof.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qve.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xzs.jiagoushi.top

Ruby: # 无泛型
来源：http://gmx.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gde.yueranfly.top

[C15] 解构 / 展开参数
来源：http://sdk.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://viy.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://sma.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ktu.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzy.tarul.cn

Java: // 无解构
来源：http://ani.sxryk.cn

Go:   // 无解构
来源：http://iai.iojbl.cn

Ruby: a, b = pair
来源：http://ran.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://pmv.tarul.cn

[C16] 函数 / 方法重载
来源：http://bcw.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://atj.ehwqpu.com

PHP:  // 无重载
来源：http://ird.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gmi.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://fnv.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://inr.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://klu.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://sab.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xlu.chenzaomai.com

================================================================================
来源：http://sow.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://mqw.xingfuxueyuan.xyz

================================================================================
来源：http://kma.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://gqg.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vua.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zgs.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dqs.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jkg.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xlm.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://pnt.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://odl.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://utl.jinqigufen.top

[D02] 追加元素到末尾
来源：http://qmi.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nsj.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ehs.zhoulong.xyz

JS:   arr.push(4);
来源：http://stc.havefunace.top

TS:   arr.push(4);
来源：http://pbj.cucudq.cn

Java: list.add(4);
来源：http://sau.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://jij.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://ict.ehwqpu.com

C#:   list.Add(4);
来源：http://tcw.uphjek.com

[D03] 在指定位置插入元素
来源：http://krr.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://atv.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://erl.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eyt.daria6918.cn


<!-- 参考信息 -->