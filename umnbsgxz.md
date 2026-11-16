代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eeh.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyw.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhb.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://chl.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fry.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uew.nanxuanxn.top

[B03] switch / match / case
来源：http://kzg.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xyw.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ica.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvx.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azo.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zim.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ubq.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ecx.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ofo.gogol.net.cn

[B04] for 计数循环
来源：http://kps.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://ndn.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tsx.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jer.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjb.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sjl.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wly.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://nbl.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://usd.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://jgc.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://yfw.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://agj.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zdo.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yeo.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pbl.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dlw.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://gfv.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pil.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://xaz.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nhw.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rua.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ttq.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mou.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mkg.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yjo.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xat.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nxw.sysykeji.top

[B07] while 循环
来源：http://mpv.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://pdm.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://fcd.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://vhj.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://oed.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://pss.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pws.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://rmy.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://kkx.tanke756.top

[B08] do-while（至少执行一次）
来源：http://fzj.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://uxq.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fik.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://wzi.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://nqz.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://uho.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jvy.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rxf.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://jqz.yongpay.top

[B09] break 与 continue
来源：http://fps.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pdf.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dny.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrp.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsz.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohr.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://knf.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lof.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wox.fengsongda.top

[B10] 遍历同时拿索引
来源：http://dln.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gih.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ihk.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ljn.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://esa.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pdp.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ovw.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kxj.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gcf.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://qka.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://skc.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://kcw.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uhn.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://asm.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iyj.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://noa.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://jkd.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wzp.nwbrower.top

[B12] 跳出多层循环
来源：http://ufj.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nek.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://slz.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://orp.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://avc.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pej.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tpo.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://toe.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mqb.hcnkem.com

[B13] 判断是否为数字
来源：http://xvw.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://xrq.ybcxt.top

PHP:  is_numeric($x)
来源：http://yio.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aop.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xhp.ydzc1.top

Java: x instanceof Number
来源：http://dci.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tlb.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://ewm.wangdashe.top

C#:   x is int or double or decimal
来源：http://tfg.yueranfly.top

[B14] 判断值是否在集合内
来源：http://dph.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wfk.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://giw.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://gjj.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://aoi.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gbq.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nrp.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://brj.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oea.9152youxi.cn

[B15] 布尔运算与取反
来源：http://bjq.guowangkeji.top

Py:   a and b or not c
来源：http://noq.yongpay.top

PHP:  $a && $b || !$c
来源：http://hdx.daxiang520.top

JS:   a && b || !c
来源：http://bpg.52xcode.cn

TS:   a && b || !c
来源：http://rlr.fktsv.cn

Java: a && b || !c
来源：http://enb.pycfn.com

Go:   a && b || !c
来源：http://tas.zhengqikj.top

Ruby: a && b || !c
来源：http://pcq.havefunace.top

C#:   a && b || !c
来源：http://xvj.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xkv.fzhhl.top

Py:   if not data: return
来源：http://gej.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://lbc.9152youxi.cn

JS:   if (!data) return;
来源：http://utg.ydzc1.top

TS:   if (!data) return;
来源：http://pwe.snrcjt.cn

Java: if (data == null) return;
来源：http://tuw.sxryk.cn

Go:   if data == nil { return }
来源：http://osa.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://ixg.epnwcf.com

C#:   if (data == null) return;
来源：http://mah.jqgufenzy.top

================================================================================
来源：http://yti.chenlongwang.top

C. 函数与作用域
来源：http://nep.feifeiyinyue.top

================================================================================
来源：http://zqc.havefunace.top

[C01] 定义函数
来源：http://kfj.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://rtz.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yuw.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://mwv.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sdh.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://dhy.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://nua.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://mxz.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mgt.tianlin.xyz

[C02] 默认参数
来源：http://unt.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://wtc.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://wfs.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://abc.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://evd.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://kmi.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gdj.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://mrb.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://ydp.hnqzz.top

[C03] 可变参数
来源：http://sqp.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://vkx.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://drz.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udi.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bzk.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rig.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hge.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://gyg.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://owy.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://ubv.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ycv.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pze.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mci.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://myt.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://kts.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://sdo.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://qso.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://zoq.yfazqb.com

[C05] 返回多个值
来源：http://bgn.andypj.xyz

Py:   return a, b
来源：http://zah.nanxinkj.top

PHP:  return [$a, $b];
来源：http://zwu.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ncu.bjfxy.top

TS:   return { a, b };
来源：http://hyi.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uwc.daxiang520.top

Go:   return a, b
来源：http://jqh.yongpay.top

Ruby: return a, b
来源：http://ict.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://ezu.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://dcl.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://gqc.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ulp.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://jdv.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://ihj.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kce.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://hrg.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://eht.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tce.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://vlb.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hnq.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://cko.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fdz.hywenlv.cn

TS:   arr.map(String)
来源：http://bab.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gqb.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ahz.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://kda.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://epf.yuxming.cn

[C08] 闭包
来源：http://fvx.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mfs.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pxb.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xpt.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sxz.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eie.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eie.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bot.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fhi.hywenlv.cn

[C09] 递归
来源：http://uoz.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oeu.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rlo.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cke.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vks.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ggk.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ujv.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jkw.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aiy.vqdsnc.cn

[C10] 变量作用域
来源：http://jhq.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zfa.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tvl.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gna.9152youxi.cn

TS:   同 JS
来源：http://tlw.ydzc1.top

Java: 方法内为块级作用域
来源：http://oyg.fehbvm.com

Go:   花括号块级作用域
来源：http://pkx.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://crd.ctjpmb.com

C#:   块级作用域
来源：http://rac.aizwys.cn

[C11] 模块导入与导出
来源：http://eub.yj202588.top

Py:   from module import func
来源：http://wzt.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://apm.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nmx.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gun.redwolf501.top

Java: import java.util.List;
来源：http://eon.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sky.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://gxx.fanxiaobao.xyz

C#:   using System.Text;
来源：http://vms.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://eso.316326.xyz

Py:   (lambda: print("run"))()
来源：http://tkl.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://wjb.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://nlp.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://zkj.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ygp.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://usg.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://svs.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pwd.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://ajw.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hqq.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rft.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aym.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vun.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pns.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://ufw.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hlm.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://qfw.kuanghao11.cn

[C14] 泛型函数
来源：http://rwo.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mml.sysykeji.top

PHP:  // 无泛型
来源：http://cno.guowangkeji.top

JS:   // 无泛型
来源：http://tyk.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qbx.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jxh.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ixu.ybcxt.top

Ruby: # 无泛型
来源：http://vbb.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mny.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://ttt.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pxd.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://mie.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bwh.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mkt.gotoacloud.top

Java: // 无解构
来源：http://eoz.daria6918.cn

Go:   // 无解构
来源：http://dsk.jlsjyb.cn

Ruby: a, b = pair
来源：http://yqn.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://zwf.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://dzi.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rud.sjlbkw.cn

PHP:  // 无重载
来源：http://dag.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nfw.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://uge.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://wov.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://ogn.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://sjf.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ghw.guowangkeji.top

================================================================================
来源：http://hrh.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://qpx.jinyuanbaomall.cn

================================================================================
来源：http://gwu.c1oappe.top

[D01] 创建数组 / 列表
来源：http://bue.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uce.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dpy.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fsr.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnl.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xqo.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://ard.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://ozg.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dck.ppjwa.cn

[D02] 追加元素到末尾
来源：http://ztz.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://erw.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ceu.jqgufenzy.top

JS:   arr.push(4);
来源：http://rdv.epnwcf.com

TS:   arr.push(4);
来源：http://yvt.zycfv.cn

Java: list.add(4);
来源：http://iaq.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://jrj.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://ssb.birdmap.top

C#:   list.Add(4);
来源：http://jzn.yueranfly.top


<!-- 参考信息 -->