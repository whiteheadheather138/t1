代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nnx.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://urw.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwp.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eln.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qwd.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dte.shzxlz.cn

[B03] switch / match / case
来源：http://iet.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uwp.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lny.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ixa.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlq.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wil.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qar.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://izl.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lct.vqdsnc.cn

[B04] for 计数循环
来源：http://jvw.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://dwl.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uhu.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wtm.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lks.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vpv.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://orq.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://fzv.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uww.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://rbs.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://jcy.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tbd.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://jan.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://anq.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fll.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://beu.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://qnk.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yvb.tarul.cn

[B06] 遍历字典 / 对象
来源：http://yns.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://utd.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wit.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxt.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rmu.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gxi.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffb.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hid.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epd.xuetiantiany.cn

[B07] while 循环
来源：http://mwj.mhx1999.top

Py:   while i < 10: i += 1
来源：http://jxc.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://fbk.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://yqf.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://ceo.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://leu.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vph.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://rbn.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://wig.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://daz.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://rcj.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hdr.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://hzd.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://pvw.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://zbz.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://swm.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fhr.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://erh.hnqzz.top

[B09] break 与 continue
来源：http://bin.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whl.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gci.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isg.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndy.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mkj.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vbm.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lfp.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxm.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://aun.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fwj.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xfa.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jud.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wje.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pcj.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uby.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pbu.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hvr.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://lrg.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://rok.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://eai.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jim.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gza.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zqv.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vzb.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://zap.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jtl.shuidangran.top

[B12] 跳出多层循环
来源：http://lif.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qkx.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://muv.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xya.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dgr.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gtc.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://scx.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qom.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mqd.xuanzx.com

[B13] 判断是否为数字
来源：http://pql.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://nhw.daria6918.cn

PHP:  is_numeric($x)
来源：http://fyq.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://log.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayo.wangshuangyany.cn

Java: x instanceof Number
来源：http://hsd.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hhb.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://rza.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://zoz.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://ywx.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hzk.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yfo.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://wys.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://ruk.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://otw.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jxb.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://csp.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mrk.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://act.yj20258.top

Py:   a and b or not c
来源：http://abr.ybcxt.top

PHP:  $a && $b || !$c
来源：http://jyv.gotoacloud.top

JS:   a && b || !c
来源：http://zgt.xuetiantiany.cn

TS:   a && b || !c
来源：http://yrp.zhongyouzk.top

Java: a && b || !c
来源：http://skk.cashguo.top

Go:   a && b || !c
来源：http://wiu.tarul.cn

Ruby: a && b || !c
来源：http://ujl.jinqigufen.top

C#:   a && b || !c
来源：http://nts.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://ftj.0kj1m.cn

Py:   if not data: return
来源：http://baw.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://fda.havefunace.top

JS:   if (!data) return;
来源：http://ehz.kuanghao11.cn

TS:   if (!data) return;
来源：http://yrj.bjfxy.top

Java: if (data == null) return;
来源：http://csg.xuanzx.com

Go:   if data == nil { return }
来源：http://zdw.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://qlp.daxiang520.top

C#:   if (data == null) return;
来源：http://wzk.chenjidiqi.icu

================================================================================
来源：http://riv.hysaishi.cn

C. 函数与作用域
来源：http://tzk.uphjek.com

================================================================================
来源：http://ics.ppjwa.cn

[C01] 定义函数
来源：http://ita.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://ryq.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ogg.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ulq.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://avd.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vir.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nhp.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://mhe.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://urf.shangyingyoupin.top

[C02] 默认参数
来源：http://twg.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://zlh.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pkt.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://bhu.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://voy.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://faj.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://taf.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://vxn.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://myk.gaohongyu789.top

[C03] 可变参数
来源：http://abo.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://nnl.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bto.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://trj.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jal.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fug.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kyg.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://edo.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gfq.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://ces.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lrs.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fbr.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ztl.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wqv.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://asp.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://qhf.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://dog.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://svi.9152youxi.cn

[C05] 返回多个值
来源：http://uvn.guowangkeji.top

Py:   return a, b
来源：http://ubl.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://isq.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vfx.wangshuangyany.cn

TS:   return { a, b };
来源：http://rar.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ork.zhengqikj.top

Go:   return a, b
来源：http://aza.jianghu66.top

Ruby: return a, b
来源：http://mif.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://vsl.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://mnb.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://pim.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ufs.yuanzhike.top

JS:   const square = x => x * x;
来源：http://ttw.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://tta.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://scn.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fsc.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://yxm.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ngt.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://vly.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dnw.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://reu.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qjt.hcnkem.com

TS:   arr.map(String)
来源：http://ahy.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ubf.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://voo.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://rdv.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://quh.cucudq.cn

[C08] 闭包
来源：http://aqq.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://odz.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sch.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bln.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mlr.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kpl.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sbz.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wlu.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xix.zhoulong.xyz

[C09] 递归
来源：http://sij.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rny.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pez.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxo.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqu.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tde.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fyj.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctm.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkg.sjlbkw.cn

[C10] 变量作用域
来源：http://hjt.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://umx.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kkf.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zka.ivvv.top

TS:   同 JS
来源：http://adk.c1oappe.top

Java: 方法内为块级作用域
来源：http://lmj.birdmap.top

Go:   花括号块级作用域
来源：http://vpv.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sbj.fanxiaobao.xyz

C#:   块级作用域
来源：http://swm.zhixingplan.top

[C11] 模块导入与导出
来源：http://xwd.xinyue.icu

Py:   from module import func
来源：http://tzg.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zys.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://iwd.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lyg.yueranfly.top

Java: import java.util.List;
来源：http://njk.zhongyouzk.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmo.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://kpe.guowangkeji.top

C#:   using System.Text;
来源：http://imh.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://foz.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://sqi.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://cco.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://ydn.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://neb.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yag.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://axj.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://xhn.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hez.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://yri.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aer.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vje.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qvz.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyc.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qsj.yj20258888.top

Go:   func add(a, b int) int
来源：http://xzp.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ald.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://icf.bjfxy.top

[C14] 泛型函数
来源：http://qml.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xpu.feifeiyinyue.top

PHP:  // 无泛型
来源：http://mgf.hammf.cn

JS:   // 无泛型
来源：http://ffh.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fuo.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fpp.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uaf.hfpthk.cn

Ruby: # 无泛型
来源：http://djz.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tbn.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://pvs.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tcz.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://pfr.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jna.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmu.sufxvd.cn

Java: // 无解构
来源：http://biw.0kj1m.cn

Go:   // 无解构
来源：http://jja.hfpthk.cn

Ruby: a, b = pair
来源：http://bsg.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://msh.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://jxy.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vhd.vehdjk.com

PHP:  // 无重载
来源：http://xfn.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xsr.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://jir.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kth.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://rtw.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://msk.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oks.shzxlz.cn

================================================================================
来源：http://nad.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://kpw.daria6918.cn

================================================================================
来源：http://lpx.cashguo.top

[D01] 创建数组 / 列表
来源：http://bat.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljh.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yyw.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbh.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qth.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hvp.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://jeb.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://ext.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cqt.ehwqpu.com

[D02] 追加元素到末尾
来源：http://dwn.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yfc.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mgh.zdbjq.cn

JS:   arr.push(4);
来源：http://hqj.hongshengwenyu.top

TS:   arr.push(4);
来源：http://qbl.mhx1999.top

Java: list.add(4);
来源：http://tkh.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://odd.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zws.zhoulong.xyz

C#:   list.Add(4);
来源：http://iul.zhixingplan.top


<!-- 参考信息 -->