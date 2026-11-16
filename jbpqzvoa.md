代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jnf.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aoi.xziqi.cn

[B03] switch / match / case
来源：http://lfu.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://piw.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbm.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqy.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kvm.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mxs.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://htz.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nmu.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pbf.hnxiangtu.top

[B04] for 计数循环
来源：http://izd.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://lse.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wjo.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cfr.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rcl.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fkr.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://guy.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://vdi.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sge.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://tdb.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://pps.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nsf.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://glu.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nhk.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lao.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ito.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://bnp.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rwa.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://dqq.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ejr.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://che.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xez.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smm.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pvk.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://phk.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wgc.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xhx.shuidangran.top

[B07] while 循环
来源：http://elz.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://qfj.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jzq.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://awo.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://axc.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://cef.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xcr.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://acs.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://ukk.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://xuh.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://vtu.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nit.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://phe.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://sbx.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://tdo.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cvo.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://naj.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://qvb.jqgufenzy.top

[B09] break 与 continue
来源：http://lhg.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uqy.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acf.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpb.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfb.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upn.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://smm.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ddq.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpi.bbcook.cn

[B10] 遍历同时拿索引
来源：http://ymn.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://avk.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wlo.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cdo.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qhw.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lax.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ddt.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zvq.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tks.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://zqk.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://hnm.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://btg.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gss.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cnv.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qpn.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nua.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://ycv.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fyp.yuxming.cn

[B12] 跳出多层循环
来源：http://wem.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pwq.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pfo.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dbr.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jau.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://huc.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ugl.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tjl.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uvy.chenzaomai.com

[B13] 判断是否为数字
来源：http://pxl.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://woa.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://uvt.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dil.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://amb.uphjek.com

Java: x instanceof Number
来源：http://wce.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wzq.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://jtc.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://vii.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://fba.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nyi.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zig.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://nmm.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://ior.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eum.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kdc.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://wha.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fam.zhixingplan.top

[B15] 布尔运算与取反
来源：http://ghc.tanke756.top

Py:   a and b or not c
来源：http://oaq.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://vqw.guowangkeji.top

JS:   a && b || !c
来源：http://ndw.iojbl.cn

TS:   a && b || !c
来源：http://oxo.smart0.xyz

Java: a && b || !c
来源：http://xtz.yonumen.top

Go:   a && b || !c
来源：http://zye.chenjidiqi.icu

Ruby: a && b || !c
来源：http://qlx.meibo888.top

C#:   a && b || !c
来源：http://wlb.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://evy.zhiwuduotai.top

Py:   if not data: return
来源：http://bxn.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://jbx.ctjpmb.com

JS:   if (!data) return;
来源：http://dyf.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://diz.feifeiyinyue.top

Java: if (data == null) return;
来源：http://nod.hfpthk.cn

Go:   if data == nil { return }
来源：http://njj.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://oom.cashguo.top

C#:   if (data == null) return;
来源：http://mwf.tian-w.cn

================================================================================
来源：http://mcr.haohaochexian.top

C. 函数与作用域
来源：http://adk.tarul.cn

================================================================================
来源：http://vyi.iojbl.cn

[C01] 定义函数
来源：http://yuj.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://ybc.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hjn.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://ukv.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aef.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zan.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://dag.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://xkm.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://peb.zhiwuduotai.top

[C02] 默认参数
来源：http://twi.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://gdb.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eor.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://jdz.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ros.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://spy.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sps.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://syp.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nwd.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://lgv.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://pyl.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rwg.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mow.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://suz.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eje.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xsl.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://fcy.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cwd.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://kma.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://noz.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://waq.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://awa.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sey.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://dtd.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://xjl.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://zpq.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://jgd.yonumen.top

[C05] 返回多个值
来源：http://zvi.sjlbkw.cn

Py:   return a, b
来源：http://fif.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://ojz.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fyo.ydjk.org.cn

TS:   return { a, b };
来源：http://rpn.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lni.zhiwuduotai.top

Go:   return a, b
来源：http://cdf.sxryk.cn

Ruby: return a, b
来源：http://qjm.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://ndp.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://ihe.bbcook.cn

Py:   square = lambda x: x * x
来源：http://rii.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jxh.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://ctr.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://rsl.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cuu.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nzt.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://iiu.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://waw.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://lai.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xkg.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://frv.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvk.0kj1m.cn

TS:   arr.map(String)
来源：http://wdb.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pye.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kpy.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://jib.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://twz.vqdsnc.cn

[C08] 闭包
来源：http://bqs.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bif.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://afh.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://txw.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://smy.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qtn.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uye.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gty.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qov.ivvv.top

[C09] 递归
来源：http://ajo.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vib.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pit.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldy.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bhh.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zzw.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qth.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mba.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xas.shangyingyoupin.top

[C10] 变量作用域
来源：http://oqe.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bor.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fax.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://osm.gogol.net.cn

TS:   同 JS
来源：http://cxu.epnwcf.com

Java: 方法内为块级作用域
来源：http://gst.tanke756.top

Go:   花括号块级作用域
来源：http://wlp.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://afw.cqqwz.cn

C#:   块级作用域
来源：http://ddi.yangfankeji.com

[C11] 模块导入与导出
来源：http://tza.nanxuanxn.top

Py:   from module import func
来源：http://rgw.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dbo.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ylj.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oql.hammf.cn

Java: import java.util.List;
来源：http://won.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://waw.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://jiw.c1oappe.top

C#:   using System.Text;
来源：http://pra.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://xpb.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://tra.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://ijw.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://ldn.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://ave.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mag.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://skk.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://hxh.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://utn.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://mok.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pmt.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxz.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ivj.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tpu.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://tjy.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://oro.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vqe.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://hbb.316326.xyz

[C14] 泛型函数
来源：http://taa.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gak.zhongyouzk.top

PHP:  // 无泛型
来源：http://nwq.chenjidiqi.icu

JS:   // 无泛型
来源：http://yah.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lxl.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jlu.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ypx.yvedp.cn

Ruby: # 无泛型
来源：http://wzf.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vsj.redwolf501.top

[C15] 解构 / 展开参数
来源：http://mjw.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://exe.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://onk.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spn.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tkf.jinqigufen.top

Java: // 无解构
来源：http://bcl.yongpay.top

Go:   // 无解构
来源：http://eig.hesvh.cn

Ruby: a, b = pair
来源：http://wae.jianghu66.top

C#:   var (a, b) = pair;
来源：http://hdi.ybcxt.top

[C16] 函数 / 方法重载
来源：http://cha.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ybj.chenzaomai.com

PHP:  // 无重载
来源：http://slp.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://myj.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://ukb.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://liz.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://rhs.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://fpn.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xsu.gaohongyu789.top

================================================================================
来源：http://edr.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://rgu.hesvh.cn

================================================================================
来源：http://kqs.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://pwc.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jlz.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zbq.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zzi.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jhm.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qhb.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://gqp.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://slc.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rth.hcnkem.com

[D02] 追加元素到末尾
来源：http://xqn.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lfj.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eeg.iojbl.cn

JS:   arr.push(4);
来源：http://bec.c1oappe.top

TS:   arr.push(4);
来源：http://bjo.jyoumei.cn

Java: list.add(4);
来源：http://dab.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://mzs.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://guc.uphjek.com

C#:   list.Add(4);
来源：http://nft.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://cim.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://piv.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yxe.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ldo.vqdsnc.cn


<!-- 参考信息 -->