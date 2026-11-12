代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hbn.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqo.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kci.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zop.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nct.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qot.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvr.ehwqpu.com

[B04] for 计数循环
来源：http://vkz.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://ovg.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://huv.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://plj.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cmg.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cir.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hzv.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://nrw.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://evj.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://rle.ybcxt.top

Py:   for item in arr: print(item)
来源：http://bfr.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ztp.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nrz.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dzc.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rem.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gqa.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://ynw.ctjpmb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rgf.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://fhr.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://puw.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ift.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rss.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rup.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gvb.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uuc.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ulj.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ncb.hesvh.cn

[B07] while 循环
来源：http://mmt.hammf.cn

Py:   while i < 10: i += 1
来源：http://juq.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ncf.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://ajd.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://kew.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://fpx.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ojl.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://aqr.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://jhi.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://haz.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://tvx.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://flm.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://qwf.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://gvc.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://adf.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xpy.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hfp.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://jfj.zhoulong.xyz

[B09] break 与 continue
来源：http://gcd.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lgv.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kiy.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnh.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyt.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kll.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yzc.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cuk.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itr.fktsv.cn

[B10] 遍历同时拿索引
来源：http://rzo.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ukk.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://adq.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mcc.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lpb.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hpz.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://est.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wry.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rll.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://shs.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://oqc.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://dlm.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggu.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nab.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uwf.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pab.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://tqr.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pqf.hcnkem.com

[B12] 跳出多层循环
来源：http://wls.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://njq.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gzu.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cgw.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://utf.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kaj.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uww.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hfq.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://utr.fktsv.cn

[B13] 判断是否为数字
来源：http://uph.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://zwm.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://ueu.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ekb.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hia.tarul.cn

Java: x instanceof Number
来源：http://nzr.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tzm.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://vfy.cqqwz.cn

C#:   x is int or double or decimal
来源：http://htw.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://npn.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iul.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tks.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://yaa.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://lru.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xuk.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fnh.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://btp.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://boy.guowangkeji.top

[B15] 布尔运算与取反
来源：http://agw.hywenlv.cn

Py:   a and b or not c
来源：http://tyi.sysykeji.top

PHP:  $a && $b || !$c
来源：http://qud.cqqwz.cn

JS:   a && b || !c
来源：http://svx.zhiwuduotai.top

TS:   a && b || !c
来源：http://bxx.daxiang520.top

Java: a && b || !c
来源：http://lpf.bjfxy.top

Go:   a && b || !c
来源：http://qwn.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://tou.shangyingyoupin.top

C#:   a && b || !c
来源：http://ixg.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://lif.yonumen.top

Py:   if not data: return
来源：http://knf.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://fip.iojbl.cn

JS:   if (!data) return;
来源：http://gtc.daxiang520.top

TS:   if (!data) return;
来源：http://hwb.feifeiyinyue.top

Java: if (data == null) return;
来源：http://rjy.tian-w.cn

Go:   if data == nil { return }
来源：http://cvm.jyoumei.cn

Ruby: return if data.nil?
来源：http://rjj.yuxming.cn

C#:   if (data == null) return;
来源：http://psz.vqdsnc.cn

================================================================================
来源：http://clz.tian-w.cn

C. 函数与作用域
来源：http://icf.smart0.xyz

================================================================================
来源：http://drc.hfpthk.cn

[C01] 定义函数
来源：http://cay.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://het.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sri.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://atx.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpw.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pti.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://hei.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://kse.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://brk.zycfv.cn

[C02] 默认参数
来源：http://zqy.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://pvl.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ajy.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://ssv.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nxf.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kyn.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ghi.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://egc.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://vca.nanxuanxn.top

[C03] 可变参数
来源：http://sxy.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://nim.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lgk.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://llo.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tbb.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mds.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vst.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mbz.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eee.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://ejq.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ttp.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iau.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aez.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pby.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://tqy.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://riw.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://owf.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://bmn.52xcode.cn

[C05] 返回多个值
来源：http://ayl.gaohongyu789.top

Py:   return a, b
来源：http://gxa.ppjwa.cn

PHP:  return [$a, $b];
来源：http://giq.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yhn.daxiang520.top

TS:   return { a, b };
来源：http://mil.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qjg.daria6918.cn

Go:   return a, b
来源：http://bof.tanke756.top

Ruby: return a, b
来源：http://qam.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://hke.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://sgj.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://gju.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xdp.nwbrower.top

JS:   const square = x => x * x;
来源：http://ckp.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://jkc.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sdh.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hfx.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://ubz.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://yks.cucudq.cn

[C07] 把函数作为参数传入
来源：http://csl.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rny.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rjo.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fxm.hysaishi.cn

TS:   arr.map(String)
来源：http://gvp.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://atz.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izp.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://geh.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://feg.wangdashe.top

[C08] 闭包
来源：http://fti.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vah.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cce.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lbh.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksa.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mcc.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gur.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aac.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cbj.zhixingplan.top

[C09] 递归
来源：http://cpe.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fbh.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cpa.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bng.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vso.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guy.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qvy.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kfe.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gmu.sysykeji.top

[C10] 变量作用域
来源：http://yrw.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uno.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ldp.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oxo.cashguo.top

TS:   同 JS
来源：http://cdx.fktsv.cn

Java: 方法内为块级作用域
来源：http://pus.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://iaa.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xjb.havefunace.top

C#:   块级作用域
来源：http://dgx.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://mbg.fktsv.cn

Py:   from module import func
来源：http://fyy.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qdq.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://qhx.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sqn.zycfv.cn

Java: import java.util.List;
来源：http://rdm.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ala.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://mzo.yj20258888.top

C#:   using System.Text;
来源：http://tvo.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://orv.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://ahp.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://vgj.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://yow.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://vyf.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nmj.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://npk.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://xrd.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ypg.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://xbx.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://snk.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrp.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qid.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mex.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xrq.chenlongwang.top

Go:   func add(a, b int) int
来源：http://orq.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qhf.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tuv.cashguo.top

[C14] 泛型函数
来源：http://tkc.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ckp.yfazqb.com

PHP:  // 无泛型
来源：http://ijh.fanxiaobao.xyz

JS:   // 无泛型
来源：http://kpd.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vkh.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ocy.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rgr.bjfxy.top

Ruby: # 无泛型
来源：http://dhz.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oyx.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://mnn.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wro.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://fqd.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zwj.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wwo.birdmap.top

Java: // 无解构
来源：http://sqp.redwolf501.top

Go:   // 无解构
来源：http://vrt.ctjpmb.com

Ruby: a, b = pair
来源：http://yhm.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://qfx.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://vxc.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jsl.hesvh.cn

PHP:  // 无重载
来源：http://lbq.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ksm.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://vsm.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yun.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://uww.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://igv.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jdr.epnwcf.com

================================================================================
来源：http://fae.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://bgw.vqdsnc.cn

================================================================================
来源：http://lsi.fehbvm.com

[D01] 创建数组 / 列表
来源：http://dvz.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qvs.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cjg.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ork.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mya.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ung.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://qqc.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://vtb.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ayc.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://yzp.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hxi.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adt.gogol.net.cn

JS:   arr.push(4);
来源：http://rye.zycfv.cn

TS:   arr.push(4);
来源：http://ptg.tian-w.cn

Java: list.add(4);
来源：http://dtc.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://tvz.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://wnh.ybcxt.top

C#:   list.Add(4);
来源：http://uqo.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://xqb.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://xzt.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lzk.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ndd.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://hom.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://xrz.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://rtc.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://srk.xziqi.cn


<!-- 参考信息 -->