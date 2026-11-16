代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qoy.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pby.fktsv.cn

[B03] switch / match / case
来源：http://fxf.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cza.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mco.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://itb.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fko.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dcs.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qqm.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://opl.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tiv.guowangkeji.top

[B04] for 计数循环
来源：http://eqv.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://hvs.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vkr.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ape.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://whh.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://att.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vxp.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://kqs.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ucf.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://ozv.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://yjq.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://paf.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uzk.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kaw.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://imr.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gcb.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://spd.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tkg.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://xcb.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dpu.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zkb.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://put.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frx.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qqm.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jeb.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://csp.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://thd.xuanzx.com

[B07] while 循环
来源：http://dym.daria6918.cn

Py:   while i < 10: i += 1
来源：http://hiw.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kag.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://rne.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://tnx.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://bly.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xji.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://pdx.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://env.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://veu.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://eaf.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ybp.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://ddd.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://xyy.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://vla.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://esa.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://peq.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://gil.daxiang520.top

[B09] break 与 continue
来源：http://aem.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ouv.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yvd.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxb.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkj.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdt.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://myc.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zid.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idb.fengsongda.top

[B10] 遍历同时拿索引
来源：http://qcz.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nmd.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rtu.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://swv.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tsz.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yaz.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eui.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xzy.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lzh.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://jqb.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://uay.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://lwi.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zci.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rao.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://itd.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://spl.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://dmh.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://plk.jinqigufen.top

[B12] 跳出多层循环
来源：http://zbc.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://apz.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rhq.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fru.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jwc.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fmf.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jlb.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gbj.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xdr.sysykeji.top

[B13] 判断是否为数字
来源：http://ybh.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://svs.dashuyun.cn

PHP:  is_numeric($x)
来源：http://wqu.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wur.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipp.guowangkeji.top

Java: x instanceof Number
来源：http://tdn.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ajw.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://van.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://kab.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://aqv.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lfl.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ody.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://pdb.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://lch.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://efc.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://noy.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://qhf.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tdn.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://qix.xylfe.cn

Py:   a and b or not c
来源：http://wpb.cashguo.top

PHP:  $a && $b || !$c
来源：http://syc.svipenyu.cn

JS:   a && b || !c
来源：http://cbp.daxiang520.top

TS:   a && b || !c
来源：http://vfk.guowangkeji.top

Java: a && b || !c
来源：http://ced.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://hee.hfpthk.cn

Ruby: a && b || !c
来源：http://rcl.cashguo.top

C#:   a && b || !c
来源：http://wpf.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://orr.chenzaomai.com

Py:   if not data: return
来源：http://erj.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://ulj.zdqjudy.top

JS:   if (!data) return;
来源：http://hic.daxiang520.top

TS:   if (!data) return;
来源：http://tbo.nanxinkj.top

Java: if (data == null) return;
来源：http://uhe.hesvh.cn

Go:   if data == nil { return }
来源：http://vtq.kuanghao11.cn

Ruby: return if data.nil?
来源：http://adz.hcnkem.com

C#:   if (data == null) return;
来源：http://wsg.ydzc1.top

================================================================================
来源：http://plu.bbcook.cn

C. 函数与作用域
来源：http://mls.cheryme.top

================================================================================
来源：http://xsj.shuidangran.top

[C01] 定义函数
来源：http://sij.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://jvr.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vtb.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://ffu.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vxq.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://syz.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://cxz.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://hao.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ftr.yuanzhike.top

[C02] 默认参数
来源：http://ttm.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://kab.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cea.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://gnv.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sbd.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zup.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://trg.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://qdl.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://knm.pengpengdd.cyou

[C03] 可变参数
来源：http://get.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://uyw.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tre.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzo.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pdb.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jkh.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://imp.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eal.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fid.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://wyg.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://avt.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ccq.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tat.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ybt.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://nnf.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://zxu.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://vvg.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://tny.chenjidiqi.icu

[C05] 返回多个值
来源：http://nbf.mhx1999.top

Py:   return a, b
来源：http://fcu.yongpay.top

PHP:  return [$a, $b];
来源：http://xbs.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tdz.hnxiangtu.top

TS:   return { a, b };
来源：http://tmx.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wam.fanxiaobao.xyz

Go:   return a, b
来源：http://gyc.sxryk.cn

Ruby: return a, b
来源：http://vzg.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://gbu.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://glz.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://wow.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://sen.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://nlg.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://fkc.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://urg.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://mag.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://blm.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jjx.fktsv.cn

[C07] 把函数作为参数传入
来源：http://ana.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ayc.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oxt.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qyd.cashguo.top

TS:   arr.map(String)
来源：http://jbb.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ifi.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mgf.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://vgo.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kio.zhengqikj.top

[C08] 闭包
来源：http://ula.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lxz.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pcv.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dhx.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hxe.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qzv.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hsx.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wmh.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://svb.tanke756.top

[C09] 递归
来源：http://ljp.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yso.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jle.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnf.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gjz.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cti.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pnr.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yat.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://caj.gogol.net.cn

[C10] 变量作用域
来源：http://fgs.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qhs.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tqo.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nqb.hysaishi.cn

TS:   同 JS
来源：http://aki.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://myi.yfazqb.com

Go:   花括号块级作用域
来源：http://tqu.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hkk.gotoacloud.top

C#:   块级作用域
来源：http://uop.c1oappe.top

[C11] 模块导入与导出
来源：http://dtt.yj202588.top

Py:   from module import func
来源：http://okz.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://pvs.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://uhm.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mnl.ctjpmb.com

Java: import java.util.List;
来源：http://que.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kxd.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://awb.wangshuangyany.cn

C#:   using System.Text;
来源：http://tqx.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://yul.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://qyb.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://lza.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://sjk.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://qhs.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hpa.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://kno.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://qpx.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xrl.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://txb.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cab.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlk.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lxs.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezd.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zgl.ydzc1.top

Go:   func add(a, b int) int
来源：http://osv.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ymi.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pet.cheryme.top

[C14] 泛型函数
来源：http://kzr.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dwn.zhoulong.xyz

PHP:  // 无泛型
来源：http://xry.yongpay.top

JS:   // 无泛型
来源：http://dym.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebb.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nhe.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ofi.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://qzv.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hjb.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://omz.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://llg.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://aqm.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://syu.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vul.jinghuilouyu.cn

Java: // 无解构
来源：http://jup.316326.xyz

Go:   // 无解构
来源：http://kdf.sweek.top

Ruby: a, b = pair
来源：http://qbr.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://aym.yj20258.top

[C16] 函数 / 方法重载
来源：http://mjx.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qzo.xuetiantiany.cn

PHP:  // 无重载
来源：http://gpr.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mqb.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://mzg.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://djy.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://vwy.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://bob.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ouk.gogol.net.cn

================================================================================
来源：http://ceg.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://ogg.shanyushiyangkeji.top

================================================================================
来源：http://clb.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://bnx.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqz.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hra.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wmk.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ukh.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sdp.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://ncw.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://fkf.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mso.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://doq.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pwp.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sch.bjfxy.top

JS:   arr.push(4);
来源：http://osc.dianchejie.cn

TS:   arr.push(4);
来源：http://ywg.fanxiaobao.xyz

Java: list.add(4);
来源：http://xwj.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://ynu.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://nbr.dashuyun.cn

C#:   list.Add(4);
来源：http://soc.ybcxt.top

[D03] 在指定位置插入元素
来源：http://sbp.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://dcr.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://khr.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bfq.svipenyu.cn


<!-- 参考信息 -->