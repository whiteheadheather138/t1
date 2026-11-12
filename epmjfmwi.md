代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxu.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kud.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyr.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wui.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qqi.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjl.zhijiandao.cn

[B03] switch / match / case
来源：http://ikz.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yim.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://smx.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fcg.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wcs.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://goh.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ohl.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xqq.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gfn.jinghuilouyu.cn

[B04] for 计数循环
来源：http://ngg.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://fgy.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ngf.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mgc.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rdl.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rlk.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tfj.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://dxa.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xpg.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://hco.gzhubu.top

Py:   for item in arr: print(item)
来源：http://mpx.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dbm.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qow.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fww.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hmf.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ngp.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://itv.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://prw.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://zwk.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nts.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uda.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prr.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://krz.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://emn.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ehu.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://psq.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qbs.hcnkem.com

[B07] while 循环
来源：http://eqk.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://fmh.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hgm.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://kaw.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://aiw.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://zcy.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wbg.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://lei.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://gha.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://xqr.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://adq.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://snd.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://rrg.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://wod.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://mcl.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pum.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nba.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://fzy.havefunace.top

[B09] break 与 continue
来源：http://vxh.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pxt.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dql.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nho.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msk.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpd.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qbe.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cky.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmk.bbcook.cn

[B10] 遍历同时拿索引
来源：http://dtb.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wok.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cit.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eyr.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kov.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fbb.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://afu.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ndu.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tcl.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://dyt.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://put.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://gue.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndp.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://etu.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wnp.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://alv.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://ygd.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wpv.fktsv.cn

[B12] 跳出多层循环
来源：http://yhs.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mzk.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sce.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oda.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dhz.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jma.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dga.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gvw.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rjx.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://src.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://lvy.cucudq.cn

PHP:  is_numeric($x)
来源：http://fam.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://omx.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oss.snrcjt.cn

Java: x instanceof Number
来源：http://zwr.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mcp.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://ohr.hammf.cn

C#:   x is int or double or decimal
来源：http://mku.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://nct.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wpe.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jjc.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://zwt.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://qog.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fhs.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://quh.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://avk.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rmh.hfpthk.cn

[B15] 布尔运算与取反
来源：http://tad.jlsjyb.cn

Py:   a and b or not c
来源：http://vgh.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://bpj.mhx1999.top

JS:   a && b || !c
来源：http://bwf.c1oappe.top

TS:   a && b || !c
来源：http://bae.smart0.xyz

Java: a && b || !c
来源：http://adq.vqdsnc.cn

Go:   a && b || !c
来源：http://pzl.zhiwuduotai.top

Ruby: a && b || !c
来源：http://btt.jlsjyb.cn

C#:   a && b || !c
来源：http://qxh.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://jwj.haohaochexian.top

Py:   if not data: return
来源：http://edj.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://nom.zhijiandao.cn

JS:   if (!data) return;
来源：http://ufp.zhiwuduotai.top

TS:   if (!data) return;
来源：http://fsr.wangdashe.top

Java: if (data == null) return;
来源：http://qkx.tanke756.top

Go:   if data == nil { return }
来源：http://jmr.fzhhl.top

Ruby: return if data.nil?
来源：http://dks.hfpthk.cn

C#:   if (data == null) return;
来源：http://xgv.zhongyouzk.top

================================================================================
来源：http://yvq.gotoacloud.top

C. 函数与作用域
来源：http://nid.sweek.top

================================================================================
来源：http://ahw.hnqzz.top

[C01] 定义函数
来源：http://shv.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://san.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://coj.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://rrm.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gwa.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sdw.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://frl.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://afw.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hfr.shangyingyoupin.top

[C02] 默认参数
来源：http://ido.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://fzk.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bxi.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://zcu.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qjf.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kuz.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hkv.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://qwx.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://tmc.zhijiandao.cn

[C03] 可变参数
来源：http://abo.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://dww.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kyu.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oal.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbp.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ksx.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wyw.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://kmv.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pwm.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://hor.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rqi.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://psm.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fgp.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tnj.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://qes.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://sqf.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://bdd.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://hrt.cashguo.top

[C05] 返回多个值
来源：http://uuv.chenlongwang.top

Py:   return a, b
来源：http://aje.yvedp.cn

PHP:  return [$a, $b];
来源：http://kqt.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cfs.epnwcf.com

TS:   return { a, b };
来源：http://fwe.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rvh.shzxlz.cn

Go:   return a, b
来源：http://dax.ydzc1.top

Ruby: return a, b
来源：http://phu.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://uuh.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://ayy.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://mum.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jyn.c1oappe.top

JS:   const square = x => x * x;
来源：http://esx.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://ipa.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dcg.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://vgd.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://kgm.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ngp.bjfxy.top

[C07] 把函数作为参数传入
来源：http://yza.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mhk.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://flr.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iud.cashguo.top

TS:   arr.map(String)
来源：http://mdb.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zzu.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ieq.sweek.top

Ruby: arr.map(&:upcase)
来源：http://fcs.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wml.pengpengdd.cyou

[C08] 闭包
来源：http://ofb.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pnf.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kyc.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uuh.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pcr.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://igm.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qos.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zyi.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://prp.aizwys.cn

[C09] 递归
来源：http://shj.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tdg.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lka.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zva.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqm.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dci.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fei.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jkx.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cuz.shuidangran.top

[C10] 变量作用域
来源：http://zxz.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cze.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://egk.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jbt.hcnkem.com

TS:   同 JS
来源：http://gfv.zhixingplan.top

Java: 方法内为块级作用域
来源：http://xfb.dashuyun.cn

Go:   花括号块级作用域
来源：http://gur.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://str.xziqi.cn

C#:   块级作用域
来源：http://nev.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://wws.fengsongda.top

Py:   from module import func
来源：http://iqg.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hkl.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://apo.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hip.havefunace.top

Java: import java.util.List;
来源：http://leg.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gih.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://adp.haohaochexian.top

C#:   using System.Text;
来源：http://tuj.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://duc.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://xcy.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://fkl.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://ycf.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://ghe.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://onp.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://hgv.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://gkh.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ewn.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://rdk.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rma.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jnc.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hvy.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gds.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://pez.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://ffy.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://car.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://bwm.yj20258.top

[C14] 泛型函数
来源：http://nks.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lli.nanxinkj.top

PHP:  // 无泛型
来源：http://hkc.wangshuangyany.cn

JS:   // 无泛型
来源：http://pot.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://icf.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://umv.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://foi.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://dbz.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xzf.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://gbk.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xwb.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://oyj.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pzu.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oei.yonumen.top

Java: // 无解构
来源：http://flx.yvedp.cn

Go:   // 无解构
来源：http://fqe.fengsongda.top

Ruby: a, b = pair
来源：http://idf.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://jdi.epnwcf.com

[C16] 函数 / 方法重载
来源：http://deu.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ihn.shzxlz.cn

PHP:  // 无重载
来源：http://yte.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://muc.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://mck.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xij.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://yoo.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://xdo.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://khy.zhoulong.xyz

================================================================================
来源：http://bjb.cashguo.top

D. 数组 / 列表 / 集合
来源：http://ord.feifeiyinyue.top

================================================================================
来源：http://tqs.ybcxt.top

[D01] 创建数组 / 列表
来源：http://bbi.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nba.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gwa.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vih.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cyv.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ehd.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://rvj.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://lnx.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dib.daria6918.cn

[D02] 追加元素到末尾
来源：http://uug.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://snd.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nyw.c1oappe.top

JS:   arr.push(4);
来源：http://ung.yfazqb.com

TS:   arr.push(4);
来源：http://xci.jiagoushi.top

Java: list.add(4);
来源：http://wnp.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://leo.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://mcc.cheryme.top

C#:   list.Add(4);
来源：http://tyr.sxryk.cn


<!-- 参考信息 -->