代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndk.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://utp.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lss.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vul.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nbb.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfa.shanyushiyangtech.top

[B03] switch / match / case
来源：http://dkl.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pqg.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ckj.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fck.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nec.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bkg.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tbt.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oow.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zip.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://ppf.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://hzg.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wfe.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cds.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eww.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lmy.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zkm.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://djz.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xnv.havefunace.top

[B05] 遍历数组 / 列表
来源：http://gvx.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://yrd.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ajw.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ugf.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tar.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vel.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sim.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://qgt.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bwz.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://hrh.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pax.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ihy.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zge.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pni.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pee.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://glk.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lyt.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://enl.jqgfzy.top

[B07] while 循环
来源：http://hkw.fengsongda.top

Py:   while i < 10: i += 1
来源：http://hwf.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vry.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://weq.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://kbu.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://aif.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kow.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://caf.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://cah.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://sbt.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://hfb.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zci.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://cly.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://izk.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://lim.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qsx.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ong.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://btg.hongshengwenyu.top

[B09] break 与 continue
来源：http://zom.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hpc.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://swe.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xds.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbp.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzo.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://avc.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ube.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsi.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://tfs.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pcc.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://srl.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxk.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xij.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uhz.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjn.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://whu.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hob.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://cub.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://bwh.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://mrh.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tdy.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obi.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hya.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iod.xylfe.cn

Ruby: (0...10).step(2).to_a
来源：http://prz.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iqh.hysaishi.cn

[B12] 跳出多层循环
来源：http://qqn.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wdh.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vho.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://agj.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfa.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ecz.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dsu.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ggl.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nif.nwbrower.top

[B13] 判断是否为数字
来源：http://bzu.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://lbg.hammf.cn

PHP:  is_numeric($x)
来源：http://hwh.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wto.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://woj.redwolf501.top

Java: x instanceof Number
来源：http://gwh.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hcs.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://qtr.nanxinkj.top

C#:   x is int or double or decimal
来源：http://hrl.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://wan.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bpg.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oit.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://okx.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://gmk.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dli.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bnh.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://vwh.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jhs.sxryk.cn

[B15] 布尔运算与取反
来源：http://rxj.fengsongda.top

Py:   a and b or not c
来源：http://fjv.xylfe.cn

PHP:  $a && $b || !$c
来源：http://djb.shangyingyoupin.top

JS:   a && b || !c
来源：http://xak.vqdsnc.cn

TS:   a && b || !c
来源：http://lgs.epnwcf.com

Java: a && b || !c
来源：http://tje.hysaishi.cn

Go:   a && b || !c
来源：http://gan.andypj.xyz

Ruby: a && b || !c
来源：http://bzb.zdbjq.cn

C#:   a && b || !c
来源：http://din.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://diu.shanyushiyangkeji.top

Py:   if not data: return
来源：http://fqb.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://aar.zdqjudy.top

JS:   if (!data) return;
来源：http://ssj.yangfankeji.com

TS:   if (!data) return;
来源：http://wgr.tian-w.cn

Java: if (data == null) return;
来源：http://klh.gzhubu.top

Go:   if data == nil { return }
来源：http://fmj.chenzaomai.com

Ruby: return if data.nil?
来源：http://hiz.sjlbkw.cn

C#:   if (data == null) return;
来源：http://nfy.daria6918.cn

================================================================================
来源：http://rjj.jinghuilouyu.cn

C. 函数与作用域
来源：http://nqo.zhiwuduotai.top

================================================================================
来源：http://mbo.jyoumei.cn

[C01] 定义函数
来源：http://kkj.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://exp.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgp.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://upt.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwm.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hwz.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://ugv.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://btf.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iof.fzhhl.top

[C02] 默认参数
来源：http://sfe.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://ept.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pov.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hsp.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cey.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dxa.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xpf.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://wed.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://qfj.yj20258.top

[C03] 可变参数
来源：http://nlf.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://ijs.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qbm.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wim.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wfr.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dpk.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://csa.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://uop.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mxs.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://aqw.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ujp.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ove.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uor.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://crc.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://mlc.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://vym.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://ksb.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://cif.cqqwz.cn

[C05] 返回多个值
来源：http://tho.zdbjq.cn

Py:   return a, b
来源：http://xda.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://slb.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://soz.yuanzhike.top

TS:   return { a, b };
来源：http://ukl.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vue.sjlbkw.cn

Go:   return a, b
来源：http://skc.wangshuangyany.cn

Ruby: return a, b
来源：http://cuu.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://sga.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://opw.tian-w.cn

Py:   square = lambda x: x * x
来源：http://uyb.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pbu.tianlin.xyz

JS:   const square = x => x * x;
来源：http://gbf.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://iba.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hzt.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://gyk.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://pyn.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://ydx.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://kqe.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://emf.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ccl.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cgs.yangfankeji.com

TS:   arr.map(String)
来源：http://ltf.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xgz.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mbp.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://qwb.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ovr.jiagoushi.top

[C08] 闭包
来源：http://okg.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://coo.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sxm.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://agy.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ohp.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hii.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pvs.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jju.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlj.hesvh.cn

[C09] 递归
来源：http://zoh.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpu.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rmw.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zym.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rre.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wyr.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pgb.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jfj.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xju.fzhhl.top

[C10] 变量作用域
来源：http://rxa.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xtt.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csd.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hdl.shzxlz.cn

TS:   同 JS
来源：http://ejf.shzxlz.cn

Java: 方法内为块级作用域
来源：http://xyd.chenlongwang.top

Go:   花括号块级作用域
来源：http://egc.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://alp.ydzc1.top

C#:   块级作用域
来源：http://tsj.iojbl.cn

[C11] 模块导入与导出
来源：http://tfv.pengpengdd.cyou

Py:   from module import func
来源：http://nkr.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hmk.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gfv.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ttv.jinghuilouyu.cn

Java: import java.util.List;
来源：http://etu.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lnc.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ght.gzhubu.top

C#:   using System.Text;
来源：http://zgs.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://xat.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://cdm.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://xkz.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://zzs.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://xxc.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wsb.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://cgy.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://trr.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rtx.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://mae.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fnw.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyn.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hdj.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mac.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lfw.xziqi.cn

Go:   func add(a, b int) int
来源：http://lhh.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ibg.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://czm.hywenlv.cn

[C14] 泛型函数
来源：http://cnd.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fvo.yangfankeji.com

PHP:  // 无泛型
来源：http://cjr.zhengqikj.top

JS:   // 无泛型
来源：http://iwm.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vgz.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://emq.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kjb.gogol.net.cn

Ruby: # 无泛型
来源：http://lva.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pib.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://jnh.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cea.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ylg.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ula.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eal.hongshengwenyu.top

Java: // 无解构
来源：http://mqy.jiagoushi.top

Go:   // 无解构
来源：http://vrv.xinyue.icu

Ruby: a, b = pair
来源：http://pbs.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://lrj.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://xqm.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yrm.sufxvd.cn

PHP:  // 无重载
来源：http://trd.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://agc.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://wyb.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zzd.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://sgn.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://ntt.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lcw.jinyuanbaomall.cn

================================================================================
来源：http://qlk.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://jta.bbcook.cn

================================================================================
来源：http://ext.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://msd.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fxc.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mdh.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tgv.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yiq.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nyv.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://dhq.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://bky.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gsh.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://dqi.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mlx.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szz.nanxinkj.top

JS:   arr.push(4);
来源：http://rvt.yonumen.top

TS:   arr.push(4);
来源：http://xsg.9152youxi.cn

Java: list.add(4);
来源：http://cdc.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://qzw.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://ztj.hysaishi.cn

C#:   list.Add(4);
来源：http://jud.9152youxi.cn


<!-- 参考信息 -->