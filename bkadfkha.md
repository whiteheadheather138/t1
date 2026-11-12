代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://utq.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmy.yangfankeji.com

[B03] switch / match / case
来源：http://wfy.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://izh.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sqs.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://okg.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xls.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://waj.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cym.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gky.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lhe.cucudq.cn

[B04] for 计数循环
来源：http://oqt.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://uwn.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zod.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjm.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kqj.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rkw.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oeq.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://ihi.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mzn.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://aob.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://tgd.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ysd.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hri.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qdw.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://niz.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iay.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://vtc.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hdr.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://ctk.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pqy.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rsl.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ycp.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wsf.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ooi.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qdp.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mld.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://csi.ywan-chungtsiang.top

[B07] while 循环
来源：http://jps.cucudq.cn

Py:   while i < 10: i += 1
来源：http://kqm.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://dyh.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://wwb.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://but.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://qol.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nml.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://ywg.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://cpm.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://jys.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://keb.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rph.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://jxx.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://eys.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://sdh.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bfc.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://kig.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://ihe.chenlongwang.top

[B09] break 与 continue
来源：http://xvr.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://axh.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dlj.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbg.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyk.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://awi.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xal.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zho.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goo.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://tfr.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cxj.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lif.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bec.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ria.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fzy.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fgz.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dcw.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ceh.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://ccn.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://xmp.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://lkp.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yih.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxb.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aml.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ckp.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://qtc.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vij.iojbl.cn

[B12] 跳出多层循环
来源：http://jny.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://reu.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qsd.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iam.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wrx.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://arw.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bbd.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dov.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xxm.52xcode.cn

[B13] 判断是否为数字
来源：http://uzr.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://noj.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://vlb.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dma.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dvy.cashguo.top

Java: x instanceof Number
来源：http://eny.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qvr.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://tbs.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://mll.xinyue.icu

[B14] 判断值是否在集合内
来源：http://mjv.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hwm.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bbu.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://cxj.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://xyc.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zyl.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vjd.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tmc.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ekb.jianghu66.top

[B15] 布尔运算与取反
来源：http://bhz.chenlongwang.top

Py:   a and b or not c
来源：http://pce.meibo888.top

PHP:  $a && $b || !$c
来源：http://uqd.jlsjyb.cn

JS:   a && b || !c
来源：http://shc.yangfankeji.com

TS:   a && b || !c
来源：http://pze.fzhhl.top

Java: a && b || !c
来源：http://yck.jinqigfzy.top

Go:   a && b || !c
来源：http://dlz.sufxvd.cn

Ruby: a && b || !c
来源：http://ici.cdnleiting.top

C#:   a && b || !c
来源：http://pnj.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://iuv.jlsjyb.cn

Py:   if not data: return
来源：http://brt.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://xlz.daria6918.cn

JS:   if (!data) return;
来源：http://jdg.jyoumei.cn

TS:   if (!data) return;
来源：http://skq.hysaishi.cn

Java: if (data == null) return;
来源：http://mlf.yfazqb.com

Go:   if data == nil { return }
来源：http://vgv.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://jvm.ydzc1.top

C#:   if (data == null) return;
来源：http://dcg.zhoulong.xyz

================================================================================
来源：http://eot.aibaodan.cn

C. 函数与作用域
来源：http://bvv.jinqigufen.top

================================================================================
来源：http://cfl.jinyuanbaomall.cn

[C01] 定义函数
来源：http://wbq.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://fve.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbv.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://xrp.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgw.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://khn.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://utq.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://mcz.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://frh.yuanzhike.top

[C02] 默认参数
来源：http://cvm.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://lxh.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jfu.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xpl.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://egd.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oca.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zoq.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://xvh.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://hlb.sweek.top

[C03] 可变参数
来源：http://cwd.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://mgu.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tgy.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sig.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://frr.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bkc.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kxn.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lya.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ksw.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://hpd.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsn.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qgx.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fqj.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgu.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://zym.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://dai.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://sgu.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://kmt.52xcode.cn

[C05] 返回多个值
来源：http://fkv.nanxuanxn.top

Py:   return a, b
来源：http://igg.gogol.net.cn

PHP:  return [$a, $b];
来源：http://bmd.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lzs.cheryme.top

TS:   return { a, b };
来源：http://etz.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yly.cucudq.cn

Go:   return a, b
来源：http://que.chenlongwang.top

Ruby: return a, b
来源：http://dee.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://qod.cheryme.top

[C06] 匿名函数 / lambda
来源：http://una.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://abi.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qdr.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://yav.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://uvm.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xin.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ssb.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://ugg.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sha.tian-w.cn

[C07] 把函数作为参数传入
来源：http://jys.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hku.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://txc.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kjq.xylfe.cn

TS:   arr.map(String)
来源：http://jog.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://guf.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bem.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://nlj.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kqw.xylfe.cn

[C08] 闭包
来源：http://avb.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbg.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cof.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yxy.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aor.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mor.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://itc.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyx.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dpe.52xcode.cn

[C09] 递归
来源：http://mey.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpb.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lel.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cqr.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqz.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zmq.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yxi.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pzg.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mfg.svipenyu.cn

[C10] 变量作用域
来源：http://ozx.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://prd.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tho.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://img.nanxinkj.top

TS:   同 JS
来源：http://jel.jyoumei.cn

Java: 方法内为块级作用域
来源：http://qpq.dashuyun.cn

Go:   花括号块级作用域
来源：http://ehd.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxf.zycfv.cn

C#:   块级作用域
来源：http://ubb.zycfv.cn

[C11] 模块导入与导出
来源：http://rlh.hammf.cn

Py:   from module import func
来源：http://ffr.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wax.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ykw.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bqe.yuanzhike.top

Java: import java.util.List;
来源：http://xmn.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hsq.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://kpl.wangdashe.top

C#:   using System.Text;
来源：http://czz.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://tgq.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://tux.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://zwj.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://njd.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://vmq.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://slb.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://pwk.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://qxj.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ihh.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://orf.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kcp.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kgn.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uwr.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xvj.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://rak.jqgfzy.top

Go:   func add(a, b int) int
来源：http://iut.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://luq.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://anp.hfpthk.cn

[C14] 泛型函数
来源：http://lcj.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ewi.tanke756.top

PHP:  // 无泛型
来源：http://egu.dashuyun.cn

JS:   // 无泛型
来源：http://ssk.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zzi.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://inj.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jjn.uphjek.com

Ruby: # 无泛型
来源：http://rfo.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ahq.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://hth.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fiu.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://fsv.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kxd.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://brc.havefunace.top

Java: // 无解构
来源：http://pfu.jinqigfzy.top

Go:   // 无解构
来源：http://xmd.sxryk.cn

Ruby: a, b = pair
来源：http://fzm.sweek.top

C#:   var (a, b) = pair;
来源：http://hvr.tian-w.cn

[C16] 函数 / 方法重载
来源：http://hsb.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://euz.feifeiyinyue.top

PHP:  // 无重载
来源：http://raj.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ylk.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://gpb.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xmx.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://llh.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://igq.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fco.tian-w.cn

================================================================================
来源：http://lpo.havefunace.top

D. 数组 / 列表 / 集合
来源：http://gxn.daria6918.cn

================================================================================
来源：http://vbk.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://jyk.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zst.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bac.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ajc.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ehq.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ljz.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://bro.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://icv.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vnn.andypj.xyz

[D02] 追加元素到末尾
来源：http://lps.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fsl.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rqe.gotoacloud.top

JS:   arr.push(4);
来源：http://fcq.cucudq.cn

TS:   arr.push(4);
来源：http://hik.shangyingyoupin.top

Java: list.add(4);
来源：http://hic.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://mwo.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://akg.fzhhl.top

C#:   list.Add(4);
来源：http://vqn.yvedp.cn

[D03] 在指定位置插入元素
来源：http://uzn.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://ruv.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yvb.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qfg.gotoacloud.top


<!-- 参考信息 -->