代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nhv.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oit.hesvh.cn

[B03] switch / match / case
来源：http://twx.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pex.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://soz.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oqm.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fwm.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vqa.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fqw.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qll.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lwj.gzhubu.top

[B04] for 计数循环
来源：http://gmq.ivvv.top

Py:   for i in range(10): print(i)
来源：http://tno.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvi.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpk.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hdh.zdqjudy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nru.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://glc.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://jqu.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iso.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://dmg.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://zlc.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rzf.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vio.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bry.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dpf.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tmu.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://tei.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rfo.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://fbs.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vsk.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gfc.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xye.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wnn.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vjk.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yqj.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mgf.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://exf.zhaomingkeji.xyz

[B07] while 循环
来源：http://olv.daxiang520.top

Py:   while i < 10: i += 1
来源：http://nwh.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ebn.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://baj.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://rib.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://dpr.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://arz.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://eyd.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://tzt.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://tya.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://bkb.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xpj.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://stp.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://sss.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://nsd.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vmm.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://epl.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://qie.shzxlz.cn

[B09] break 与 continue
来源：http://yoq.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dum.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ehc.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqh.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdg.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvl.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qvq.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iaj.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sci.redwolf501.top

[B10] 遍历同时拿索引
来源：http://ydi.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tma.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oiw.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mvk.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dhm.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://muw.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yso.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cve.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lyo.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://inz.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://mth.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://awl.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owc.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://irp.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pzf.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kou.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://tjo.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dap.jlsjyb.cn

[B12] 跳出多层循环
来源：http://fni.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ctz.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tts.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://you.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mti.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cyw.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://slh.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kze.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysp.yueranfly.top

[B13] 判断是否为数字
来源：http://iyz.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://hmc.ppjwa.cn

PHP:  is_numeric($x)
来源：http://gzi.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sms.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vqs.fzhhl.top

Java: x instanceof Number
来源：http://eaf.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ell.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://zqx.ehwqpu.com

C#:   x is int or double or decimal
来源：http://ynt.fktsv.cn

[B14] 判断值是否在集合内
来源：http://mtr.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nhf.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tbi.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://ayk.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://avm.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ifs.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oig.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://kpm.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vlm.hysaishi.cn

[B15] 布尔运算与取反
来源：http://hkk.jqgufenzy.top

Py:   a and b or not c
来源：http://vqy.xylfe.cn

PHP:  $a && $b || !$c
来源：http://nwd.vehdjk.com

JS:   a && b || !c
来源：http://ljv.hysaishi.cn

TS:   a && b || !c
来源：http://hxo.yongpay.top

Java: a && b || !c
来源：http://pah.yfazqb.com

Go:   a && b || !c
来源：http://dzs.xziqi.cn

Ruby: a && b || !c
来源：http://owo.sufxvd.cn

C#:   a && b || !c
来源：http://zqy.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://frz.epnwcf.com

Py:   if not data: return
来源：http://zoh.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://pdh.guowangkeji.top

JS:   if (!data) return;
来源：http://hxn.yueranfly.top

TS:   if (!data) return;
来源：http://rxl.xuetiantiany.cn

Java: if (data == null) return;
来源：http://rfo.0kj1m.cn

Go:   if data == nil { return }
来源：http://ldn.fehbvm.com

Ruby: return if data.nil?
来源：http://bcu.fengsongda.top

C#:   if (data == null) return;
来源：http://vvo.xuetiantiany.cn

================================================================================
来源：http://yij.mhx1999.top

C. 函数与作用域
来源：http://ndu.9152youxi.cn

================================================================================
来源：http://ubo.aibaodan.cn

[C01] 定义函数
来源：http://zbl.cashguo.top

Py:   def add(a, b): return a + b
来源：http://cem.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hap.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://nlb.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcd.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pue.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mnc.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://ahz.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxd.chenzaomai.com

[C02] 默认参数
来源：http://ewf.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://tua.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://yct.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://wjt.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zrb.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kzc.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://imc.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://vai.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://xrs.hfpthk.cn

[C03] 可变参数
来源：http://sex.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://xls.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wjy.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvn.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://csb.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tbq.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jke.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://pxr.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zos.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://eww.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rgv.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lgg.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mbz.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qcw.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://baa.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://eyq.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://vpc.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://xiw.svipenyu.cn

[C05] 返回多个值
来源：http://nuj.cdnleiting.top

Py:   return a, b
来源：http://sws.pycfn.com

PHP:  return [$a, $b];
来源：http://hwv.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pxl.yueranfly.top

TS:   return { a, b };
来源：http://ymc.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kqj.iojbl.cn

Go:   return a, b
来源：http://rvu.yj20258888.top

Ruby: return a, b
来源：http://kjm.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://qab.pycfn.com

[C06] 匿名函数 / lambda
来源：http://tpn.yfazqb.com

Py:   square = lambda x: x * x
来源：http://feg.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://itp.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://sze.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://bpp.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cng.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://hpb.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://jkn.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://til.xuanzx.com

[C07] 把函数作为参数传入
来源：http://gqn.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rwd.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://agj.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ybm.zhiwuduotai.top

TS:   arr.map(String)
来源：http://ymv.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tmp.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vox.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://rkc.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://avm.smart0.xyz

[C08] 闭包
来源：http://ido.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uwc.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bso.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ldo.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ugj.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wly.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zzm.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fol.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uaa.sjlbkw.cn

[C09] 递归
来源：http://nby.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qge.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yst.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xqq.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kgx.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bhc.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nzd.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://njf.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tyt.chenjidiqi.icu

[C10] 变量作用域
来源：http://hat.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://elq.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://miu.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ref.smart0.xyz

TS:   同 JS
来源：http://ijr.jiagoushi.top

Java: 方法内为块级作用域
来源：http://kux.guannengcc.top

Go:   花括号块级作用域
来源：http://gyj.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cpn.yj20258888.top

C#:   块级作用域
来源：http://aai.meibo888.top

[C11] 模块导入与导出
来源：http://isl.kuanghao11.cn

Py:   from module import func
来源：http://gco.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wih.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://dft.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ofr.chenjidiqi.icu

Java: import java.util.List;
来源：http://tpw.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ody.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://ufq.sysykeji.top

C#:   using System.Text;
来源：http://tax.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://fna.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://bni.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://oft.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://rvv.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://pvv.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ljh.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://cup.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://mhj.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zme.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://nfg.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvp.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efj.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vpn.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://whk.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ohr.chenzaomai.com

Go:   func add(a, b int) int
来源：http://ctc.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebm.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://brm.hcnkem.com

[C14] 泛型函数
来源：http://lyq.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ovl.jianghu66.top

PHP:  // 无泛型
来源：http://flk.hcnkem.com

JS:   // 无泛型
来源：http://tok.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fzu.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qzc.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kek.zhiwuduotai.top

Ruby: # 无泛型
来源：http://wpk.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iju.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://ima.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ymq.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://deh.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://muc.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ppk.gotoacloud.top

Java: // 无解构
来源：http://aut.chenjidiqi.icu

Go:   // 无解构
来源：http://ulb.xinyue.icu

Ruby: a, b = pair
来源：http://gtt.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://tqv.bjfxy.top

[C16] 函数 / 方法重载
来源：http://ntn.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mid.yangfankeji.com

PHP:  // 无重载
来源：http://rqy.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uyf.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://sed.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nsq.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://aqx.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://imc.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hhi.sufxvd.cn

================================================================================
来源：http://bvg.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://ybu.nanxuanxn.top

================================================================================
来源：http://tvn.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://siv.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://unc.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfm.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gkv.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wsl.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tcl.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://wzx.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://oqo.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://trc.svipenyu.cn

[D02] 追加元素到末尾
来源：http://vnh.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mxo.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szg.mhx1999.top

JS:   arr.push(4);
来源：http://wtn.nanxuanxn.top

TS:   arr.push(4);
来源：http://tug.zhengqikj.top

Java: list.add(4);
来源：http://kaa.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://tik.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://pyg.hnxiangtu.top

C#:   list.Add(4);
来源：http://ofl.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://tlt.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://yjq.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://psc.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snc.haohaochexian.top


<!-- 参考信息 -->