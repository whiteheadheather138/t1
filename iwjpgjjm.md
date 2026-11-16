代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://luy.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axd.9152youxi.cn

[B03] switch / match / case
来源：http://lyt.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kob.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://suc.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://srj.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpe.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kbz.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ebi.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dfi.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wmr.ctjpmb.com

[B04] for 计数循环
来源：http://lli.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://ncm.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mjw.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jax.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulg.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tgn.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aya.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://qux.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hgy.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://bmo.wangdashe.top

Py:   for item in arr: print(item)
来源：http://hhc.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cye.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://gkz.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nhc.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fcv.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sbe.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://yxs.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://opt.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://btj.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sbn.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uqw.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://otv.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iti.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://grh.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fms.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nkd.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://npo.mhx1999.top

[B07] while 循环
来源：http://vkp.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://ibr.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://yba.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://rxb.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://ras.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://qfd.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rwx.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://vbg.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://qlo.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://hwj.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://sfq.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hmh.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://jwz.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://bug.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://jbw.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://umg.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oby.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://gal.hysaishi.cn

[B09] break 与 continue
来源：http://kov.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mxu.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eqt.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwz.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zat.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbz.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sfo.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zyg.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbe.cashguo.top

[B10] 遍历同时拿索引
来源：http://gkw.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rxf.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jec.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uaw.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cls.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nxl.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kgd.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sla.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ihk.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://ark.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://lzx.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://ozb.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxu.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mqi.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hyd.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xez.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://tdo.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqd.bjfxy.top

[B12] 跳出多层循环
来源：http://apz.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://afi.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xwv.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hts.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcq.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gun.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vhm.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rbb.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://luu.ydjk.org.cn

[B13] 判断是否为数字
来源：http://bch.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://qcr.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://vep.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ufz.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fso.gotoacloud.top

Java: x instanceof Number
来源：http://ped.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jfm.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://hai.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://ufa.yongpay.top

[B14] 判断值是否在集合内
来源：http://rxi.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ekc.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pju.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://ouf.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://rya.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://axn.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pmz.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://gop.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rqu.bbcook.cn

[B15] 布尔运算与取反
来源：http://xgq.zhongyouzk.top

Py:   a and b or not c
来源：http://fee.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://iuu.jqgfzy.top

JS:   a && b || !c
来源：http://cvt.wangshuangyany.cn

TS:   a && b || !c
来源：http://pmy.sxryk.cn

Java: a && b || !c
来源：http://ynu.jqgfzy.top

Go:   a && b || !c
来源：http://wkg.shuidangran.top

Ruby: a && b || !c
来源：http://foo.cdnleiting.top

C#:   a && b || !c
来源：http://zjp.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://nex.aibaodan.cn

Py:   if not data: return
来源：http://rbi.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://spw.sufxvd.cn

JS:   if (!data) return;
来源：http://wow.aizwys.cn

TS:   if (!data) return;
来源：http://dqq.nanxinkj.top

Java: if (data == null) return;
来源：http://zqi.fzhhl.top

Go:   if data == nil { return }
来源：http://vgy.hywenlv.cn

Ruby: return if data.nil?
来源：http://rug.havefunace.top

C#:   if (data == null) return;
来源：http://clz.jinqigufen.top

================================================================================
来源：http://qtc.tarul.cn

C. 函数与作用域
来源：http://skv.gotoacloud.top

================================================================================
来源：http://gew.fktsv.cn

[C01] 定义函数
来源：http://arv.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://rft.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehb.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://eql.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pbm.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nsq.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://nkp.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://nao.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oum.birdmap.top

[C02] 默认参数
来源：http://tkg.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://ege.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gvx.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://ici.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rkf.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pid.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xkj.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://sdf.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://mxb.gogol.net.cn

[C03] 可变参数
来源：http://icm.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://orz.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fbj.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnj.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pta.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fko.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jbd.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ntq.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ntr.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://eig.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://khl.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qxn.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fkd.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lne.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://ldj.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://yur.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://gfo.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://tgs.hnxiangtu.top

[C05] 返回多个值
来源：http://ejd.jianghu66.top

Py:   return a, b
来源：http://are.c1oappe.top

PHP:  return [$a, $b];
来源：http://jfl.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gbf.bjfxy.top

TS:   return { a, b };
来源：http://bfv.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ear.wangdashe.top

Go:   return a, b
来源：http://qeu.hnxiangtu.top

Ruby: return a, b
来源：http://cjc.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://zrx.yongpay.top

[C06] 匿名函数 / lambda
来源：http://jgq.yvedp.cn

Py:   square = lambda x: x * x
来源：http://iib.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://otl.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://knz.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://eps.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hxi.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kzm.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://pja.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vxl.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://suk.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vuo.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://ewp.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cxb.316326.xyz

TS:   arr.map(String)
来源：http://krr.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qfr.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://grc.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://eyr.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fcv.svipenyu.cn

[C08] 闭包
来源：http://adv.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://edd.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lmf.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rih.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uth.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zzr.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xhb.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ggf.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hlu.tarul.cn

[C09] 递归
来源：http://amo.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cio.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gmp.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpl.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbz.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xqv.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qxq.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qig.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxc.dashuyun.cn

[C10] 变量作用域
来源：http://wes.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://faf.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wkw.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zry.sweek.top

TS:   同 JS
来源：http://tnp.vehdjk.com

Java: 方法内为块级作用域
来源：http://mnh.jianghu66.top

Go:   花括号块级作用域
来源：http://qcq.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qyn.zdbjq.cn

C#:   块级作用域
来源：http://wui.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://eim.fanxiaobao.xyz

Py:   from module import func
来源：http://khq.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wvh.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofo.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://guo.xinyue.icu

Java: import java.util.List;
来源：http://kml.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ddh.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://vkx.svipenyu.cn

C#:   using System.Text;
来源：http://ktk.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://hnv.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://cft.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://bqe.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://cdl.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://ldw.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wiq.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://ssk.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://pee.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://jua.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://luu.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncl.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hht.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://elq.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jpu.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://svv.chenzaomai.com

Go:   func add(a, b int) int
来源：http://dnz.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vmw.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sdg.ppjwa.cn

[C14] 泛型函数
来源：http://rry.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zum.yonumen.top

PHP:  // 无泛型
来源：http://fss.tianlin.xyz

JS:   // 无泛型
来源：http://qrl.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cyu.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kqr.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yjg.jqgufenzy.top

Ruby: # 无泛型
来源：http://ygs.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hpp.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://toj.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rmg.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://enk.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sym.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nqk.jlsjyb.cn

Java: // 无解构
来源：http://qte.jinqigfzy.top

Go:   // 无解构
来源：http://ejc.iojbl.cn

Ruby: a, b = pair
来源：http://zsa.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://gjo.hnqzz.top

[C16] 函数 / 方法重载
来源：http://cyn.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sjp.pengpengdd.cyou

PHP:  // 无重载
来源：http://vtz.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdb.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://zwe.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qlj.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://umn.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://knx.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mpu.yanxiufei.cn

================================================================================
来源：http://min.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://tav.redwolf501.top

================================================================================
来源：http://xqk.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://jqq.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mfr.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mgj.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dhc.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zll.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qlm.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://xhf.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://zts.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gru.zycfv.cn

[D02] 追加元素到末尾
来源：http://ymh.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gav.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwy.bbcook.cn

JS:   arr.push(4);
来源：http://lny.zhijiandao.cn

TS:   arr.push(4);
来源：http://mjk.yonumen.top

Java: list.add(4);
来源：http://zqv.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://xlt.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://atn.cucudq.cn

C#:   list.Add(4);
来源：http://qqu.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://jhg.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://odx.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hhu.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oyg.pycfn.com


<!-- 参考信息 -->