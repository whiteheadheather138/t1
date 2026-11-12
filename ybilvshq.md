代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgf.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xau.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myr.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sde.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://prx.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://znj.ybcxt.top

[B03] switch / match / case
来源：http://vdb.pycfn.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://asi.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zfc.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sfm.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://giy.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lrh.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mno.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qso.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tid.meibo888.top

[B04] for 计数循环
来源：http://ixj.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://oli.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jzd.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esb.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://moj.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mso.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://epo.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://fss.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vqm.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://wct.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://tte.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ifh.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jrp.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://een.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://enm.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rlu.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://nyq.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hzp.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://dvp.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lmc.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wvq.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qgf.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhu.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zlv.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wfs.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tbr.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ffa.gzhubu.top

[B07] while 循环
来源：http://qwa.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://zvj.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://tnr.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://eee.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://otk.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://pid.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nbg.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://wiv.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://hgo.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://krr.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://qhk.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zac.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://zqx.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://xcn.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://fsd.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hfd.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://shq.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://isf.xziqi.cn

[B09] break 与 continue
来源：http://xck.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://onn.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vrd.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtc.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plj.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wja.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tea.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ksk.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chg.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://cgh.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dkc.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ysk.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://amo.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wkr.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dgv.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hnl.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pub.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wnv.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://drh.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://wug.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://etr.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgk.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zax.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wnn.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fed.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://uyc.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xtv.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://qwf.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gkx.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fne.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrs.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jee.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nxl.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://csy.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ugd.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vzq.birdmap.top

[B13] 判断是否为数字
来源：http://uzm.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://rrs.iojbl.cn

PHP:  is_numeric($x)
来源：http://szn.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvy.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bor.tanke756.top

Java: x instanceof Number
来源：http://fbu.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qww.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://rsa.xinyue.icu

C#:   x is int or double or decimal
来源：http://dlb.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://xax.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vjf.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dxe.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://tlz.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://rcq.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ean.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cfa.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://cdd.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ffa.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://tbg.wangdashe.top

Py:   a and b or not c
来源：http://ssy.fzhhl.top

PHP:  $a && $b || !$c
来源：http://iml.feifeiyinyue.top

JS:   a && b || !c
来源：http://vfp.gzhubu.top

TS:   a && b || !c
来源：http://uni.52xcode.cn

Java: a && b || !c
来源：http://uls.wangdashe.top

Go:   a && b || !c
来源：http://cnm.jiagoushi.top

Ruby: a && b || !c
来源：http://jge.shzxlz.cn

C#:   a && b || !c
来源：http://cwr.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xrd.kuanghao11.cn

Py:   if not data: return
来源：http://wbg.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://vzk.0kj1m.cn

JS:   if (!data) return;
来源：http://rvj.feifeiyinyue.top

TS:   if (!data) return;
来源：http://szu.wangdashe.top

Java: if (data == null) return;
来源：http://iqo.gaohongyu789.top

Go:   if data == nil { return }
来源：http://rqz.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://ehc.vqdsnc.cn

C#:   if (data == null) return;
来源：http://inr.zhiwuduotai.top

================================================================================
来源：http://art.mhx1999.top

C. 函数与作用域
来源：http://oxp.316326.xyz

================================================================================
来源：http://bdh.yongpay.top

[C01] 定义函数
来源：http://uei.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://yjp.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uur.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://kfo.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://shc.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pao.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://jlu.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://klc.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ekr.zhiwuduotai.top

[C02] 默认参数
来源：http://nzb.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://dyu.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://onf.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://xvt.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://vqz.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gso.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pcr.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://hhh.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://qkw.zdqjudy.top

[C03] 可变参数
来源：http://oaz.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://mvg.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kdh.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kal.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fgc.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rfq.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sum.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://bvo.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lwe.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://cuh.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://piw.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gox.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tre.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uap.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://oyi.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://vgb.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://twm.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://eer.hysaishi.cn

[C05] 返回多个值
来源：http://xlc.yonumen.top

Py:   return a, b
来源：http://xgt.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://kkl.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nzn.chenzaomai.com

TS:   return { a, b };
来源：http://vce.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ztc.vehdjk.com

Go:   return a, b
来源：http://zeq.smart0.xyz

Ruby: return a, b
来源：http://lpn.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://ujn.yj202588.top

[C06] 匿名函数 / lambda
来源：http://hmg.ivvv.top

Py:   square = lambda x: x * x
来源：http://dqy.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kju.nanxinkj.top

JS:   const square = x => x * x;
来源：http://kje.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://xhg.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ndf.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://new.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://ahc.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://fpf.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://pda.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ous.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://bak.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ghg.jinqigufen.top

TS:   arr.map(String)
来源：http://nrn.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hca.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ilj.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://dzf.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yda.daria6918.cn

[C08] 闭包
来源：http://hzk.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dpe.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://doq.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jgn.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mdm.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wuk.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nvu.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wtk.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xnz.jinqigufen.top

[C09] 递归
来源：http://ugy.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://own.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cqt.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pyf.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bru.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eay.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mxc.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ddf.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vzk.tianlin.xyz

[C10] 变量作用域
来源：http://bvu.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bdb.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kid.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uin.cashguo.top

TS:   同 JS
来源：http://gfh.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://euv.xziqi.cn

Go:   花括号块级作用域
来源：http://xbx.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pct.feifeiyinyue.top

C#:   块级作用域
来源：http://ntg.c1oappe.top

[C11] 模块导入与导出
来源：http://ees.xylfe.cn

Py:   from module import func
来源：http://nmt.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yjw.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nbn.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ovm.yj20258888.top

Java: import java.util.List;
来源：http://jxd.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mks.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://xgk.ydzc1.top

C#:   using System.Text;
来源：http://zfg.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://rst.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://thd.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://bay.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://zvo.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://qdf.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nlp.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://azm.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://xvq.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aay.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://xfn.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wcx.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyt.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://naq.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hzo.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aof.svipenyu.cn

Go:   func add(a, b int) int
来源：http://iwb.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgm.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://vbw.yj20258888.top

[C14] 泛型函数
来源：http://vlg.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzt.yfazqb.com

PHP:  // 无泛型
来源：http://ogh.shzxlz.cn

JS:   // 无泛型
来源：http://prt.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mfv.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ziv.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bwk.yj20258888.top

Ruby: # 无泛型
来源：http://ltn.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dze.nwbrower.top

[C15] 解构 / 展开参数
来源：http://tfu.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bfu.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://zfm.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://awy.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://orx.ctjpmb.com

Java: // 无解构
来源：http://jgj.fengsongda.top

Go:   // 无解构
来源：http://waw.dashuyun.cn

Ruby: a, b = pair
来源：http://wgm.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://bnp.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://yug.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lqy.tanke756.top

PHP:  // 无重载
来源：http://okm.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vui.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://aul.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pfb.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://uvx.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://gyt.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xuh.havefunace.top

================================================================================
来源：http://qen.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://mnc.gogol.net.cn

================================================================================
来源：http://bgu.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://tja.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nwf.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ijq.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gbb.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hrk.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pjx.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://cuf.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://gyo.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aip.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://rsa.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xjf.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lnb.sweek.top

JS:   arr.push(4);
来源：http://qge.uphjek.com

TS:   arr.push(4);
来源：http://fgb.zhijiandao.cn

Java: list.add(4);
来源：http://vlo.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://uou.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://fku.cucudq.cn

C#:   list.Add(4);
来源：http://zpk.gotoacloud.top


<!-- 参考信息 -->