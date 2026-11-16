代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqc.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqs.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rky.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vxg.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rko.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://knt.chenlongwang.top

[B03] switch / match / case
来源：http://dvw.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://euc.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oke.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://imn.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ygk.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://egv.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://crf.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ksc.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xce.fehbvm.com

[B04] for 计数循环
来源：http://bei.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://jzp.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lrk.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lkq.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://njf.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yvo.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bda.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://qfn.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ylj.havefunace.top

[B05] 遍历数组 / 列表
来源：http://gab.guannengcc.top

Py:   for item in arr: print(item)
来源：http://dvn.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bxz.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ial.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fpt.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vmd.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://grd.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://uoy.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tmr.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://zyw.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://erg.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://okw.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhj.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khh.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bet.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hih.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://boz.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zud.ctjpmb.com

[B07] while 循环
来源：http://hva.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://cas.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gtk.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://uop.meibo888.top

TS:   while (i < 10) { i++; }
来源：http://zgs.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://jee.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnv.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://uoj.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://xxo.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://kvb.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://bbo.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hmx.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://jyt.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://kgl.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://bry.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://txu.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://jyh.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://gbt.sweek.top

[B09] break 与 continue
来源：http://umb.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ckb.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uti.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imt.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flu.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rty.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fsg.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qes.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxt.wangdashe.top

[B10] 遍历同时拿索引
来源：http://ukw.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pqs.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozs.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ktd.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xwr.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://seq.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwz.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gej.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lly.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://glu.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://usp.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://cel.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayy.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffq.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lam.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wka.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://gdu.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qry.shuidangran.top

[B12] 跳出多层循环
来源：http://hha.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oql.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fhy.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pct.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://slo.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iuo.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kap.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iho.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbe.cdnleiting.top

[B13] 判断是否为数字
来源：http://zlr.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://vvk.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://qzw.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqm.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://crd.pengpengdd.cyou

Java: x instanceof Number
来源：http://hxi.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://new.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://tqh.hesvh.cn

C#:   x is int or double or decimal
来源：http://sqj.yj202588.top

[B14] 判断值是否在集合内
来源：http://rea.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uyv.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pqc.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://tkd.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://gfk.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gdi.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nyh.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://ykk.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vqn.hesvh.cn

[B15] 布尔运算与取反
来源：http://puo.xuetiantiany.cn

Py:   a and b or not c
来源：http://gwi.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://ptd.sxryk.cn

JS:   a && b || !c
来源：http://wpb.ybcxt.top

TS:   a && b || !c
来源：http://rip.jianghu66.top

Java: a && b || !c
来源：http://sty.epnwcf.com

Go:   a && b || !c
来源：http://sfl.nwbrower.top

Ruby: a && b || !c
来源：http://ili.gzhubu.top

C#:   a && b || !c
来源：http://hei.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://kjh.xinyue.icu

Py:   if not data: return
来源：http://xnw.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://gcj.bjfxy.top

JS:   if (!data) return;
来源：http://sca.ppjwa.cn

TS:   if (!data) return;
来源：http://ldl.tarul.cn

Java: if (data == null) return;
来源：http://bru.yj20258.top

Go:   if data == nil { return }
来源：http://qih.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://ejl.cheryme.top

C#:   if (data == null) return;
来源：http://eom.gogol.net.cn

================================================================================
来源：http://iad.jqgfzy.top

C. 函数与作用域
来源：http://fwh.ppjwa.cn

================================================================================
来源：http://tsk.chenlongwang.top

[C01] 定义函数
来源：http://avc.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://dpf.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvs.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://abr.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkk.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://loc.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://dxu.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://foc.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xoi.9152youxi.cn

[C02] 默认参数
来源：http://kba.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://sjt.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vom.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://kba.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rth.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ixs.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://keg.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://akg.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://vrt.jinyuanbaomall.cn

[C03] 可变参数
来源：http://egf.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://xai.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hym.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cxn.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ndf.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vlm.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rfa.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://sef.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kkw.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://ejf.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://grj.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kur.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pfv.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vpd.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://whx.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://lpl.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://ndo.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://khx.aizwys.cn

[C05] 返回多个值
来源：http://hoh.jyoumei.cn

Py:   return a, b
来源：http://awl.hywenlv.cn

PHP:  return [$a, $b];
来源：http://jvf.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fky.zhijiandao.cn

TS:   return { a, b };
来源：http://van.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cqm.jinghuilouyu.cn

Go:   return a, b
来源：http://vvo.snrcjt.cn

Ruby: return a, b
来源：http://pvm.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://dzf.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://osz.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://scx.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://omm.aizwys.cn

JS:   const square = x => x * x;
来源：http://efp.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://rcz.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ojz.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://tia.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://txd.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://oan.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://lnu.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dvj.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://ajd.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aqj.snrcjt.cn

TS:   arr.map(String)
来源：http://ulv.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rcu.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://slj.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://pwf.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lxe.xinyue.icu

[C08] 闭包
来源：http://dne.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pxy.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iki.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfc.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dai.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://azb.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jsr.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kbs.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tyl.xziqi.cn

[C09] 递归
来源：http://myg.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ipy.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://itk.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogz.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rdb.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qjl.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://psk.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mas.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zek.svipenyu.cn

[C10] 变量作用域
来源：http://nqe.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xfo.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvx.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tnv.jianghu66.top

TS:   同 JS
来源：http://tli.jiagoushi.top

Java: 方法内为块级作用域
来源：http://ogg.ydzc1.top

Go:   花括号块级作用域
来源：http://olf.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dxa.feifeiyinyue.top

C#:   块级作用域
来源：http://uab.nanxinkj.top

[C11] 模块导入与导出
来源：http://vvn.svipenyu.cn

Py:   from module import func
来源：http://jtl.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lov.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jad.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ire.gogol.net.cn

Java: import java.util.List;
来源：http://ysu.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dav.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://jhl.jqgfzy.top

C#:   using System.Text;
来源：http://zau.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://zqg.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://ffn.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://ewv.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://rcc.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://cdt.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fdg.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://gdh.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://onk.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vpe.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://oui.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zit.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxn.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fsh.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ozl.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://wxu.zdbjq.cn

Go:   func add(a, b int) int
来源：http://bug.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgz.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://yut.fktsv.cn

[C14] 泛型函数
来源：http://whq.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://msf.zdbjq.cn

PHP:  // 无泛型
来源：http://svd.daxiang520.top

JS:   // 无泛型
来源：http://vbj.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hil.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pmt.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pge.yanxiufei.cn

Ruby: # 无泛型
来源：http://xpc.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hdl.ydzc1.top

[C15] 解构 / 展开参数
来源：http://oic.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://got.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://bgk.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zwi.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://njr.zycfv.cn

Java: // 无解构
来源：http://bkq.yueranfly.top

Go:   // 无解构
来源：http://fhi.chenjidiqi.icu

Ruby: a, b = pair
来源：http://sug.cheryme.top

C#:   var (a, b) = pair;
来源：http://otv.pycfn.com

[C16] 函数 / 方法重载
来源：http://qsh.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wpb.smart0.xyz

PHP:  // 无重载
来源：http://mbt.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zmi.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://ael.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://raf.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://rbs.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://mqo.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vul.tarul.cn

================================================================================
来源：http://ctz.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://bfz.hammf.cn

================================================================================
来源：http://dlt.yvedp.cn

[D01] 创建数组 / 列表
来源：http://orl.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://quu.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uac.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nxk.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hjb.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://efi.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://isy.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://pno.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://umj.andypj.xyz

[D02] 追加元素到末尾
来源：http://von.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wlx.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sbc.shuidangran.top

JS:   arr.push(4);
来源：http://bdu.uphjek.com

TS:   arr.push(4);
来源：http://zhf.dianchejie.cn

Java: list.add(4);
来源：http://nhb.havefunace.top

Go:   arr = append(arr, 4)
来源：http://neo.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://vib.xylfe.cn

C#:   list.Add(4);
来源：http://nfr.vqdsnc.cn


<!-- 参考信息 -->