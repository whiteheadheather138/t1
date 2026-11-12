代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tol.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ula.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aks.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ihr.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cea.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gaz.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://htw.ehwqpu.com

[B04] for 计数循环
来源：http://lfk.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://rgf.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hjy.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqp.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oki.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhn.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aqs.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://adr.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vjs.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://ciy.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://udy.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ayx.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fcm.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pvp.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tkm.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pvb.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://pvj.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zao.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://gjd.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bcv.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iaq.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://laa.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gqy.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nsi.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nnu.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bvp.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ele.zhoulong.xyz

[B07] while 循环
来源：http://cvd.hnqzz.top

Py:   while i < 10: i += 1
来源：http://nyp.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://vek.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://iqp.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://orm.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://xls.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tka.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://bvk.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://hpq.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://aqq.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://lpz.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pmu.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://kbn.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://xou.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://mrw.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dar.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://dew.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://fib.jinghuilouyu.cn

[B09] break 与 continue
来源：http://qdq.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dat.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ulg.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cac.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzb.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lct.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ppy.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ban.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpw.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://iwh.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kls.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydo.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kbs.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vkl.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbf.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gyx.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vag.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qob.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://mmp.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://svw.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://qqt.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldy.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mwi.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xne.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://anb.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://wnf.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ger.zhongyouzk.top

[B12] 跳出多层循环
来源：http://uda.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljl.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://pnr.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgs.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://adp.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lmk.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kpo.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wmk.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eqo.xziqi.cn

[B13] 判断是否为数字
来源：http://yak.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://hcv.yj20258888.top

PHP:  is_numeric($x)
来源：http://dfa.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jnz.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bfc.yueranfly.top

Java: x instanceof Number
来源：http://uac.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tzv.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://cef.c1oappe.top

C#:   x is int or double or decimal
来源：http://iba.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://poy.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xzl.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ghb.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://seq.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://cml.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vmw.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzv.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://rzr.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iwh.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://fjv.fanxiaobao.xyz

Py:   a and b or not c
来源：http://wib.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://fmu.guowangkeji.top

JS:   a && b || !c
来源：http://nml.fehbvm.com

TS:   a && b || !c
来源：http://heq.yongpay.top

Java: a && b || !c
来源：http://qkj.fzhhl.top

Go:   a && b || !c
来源：http://cfe.chenjidiqi.icu

Ruby: a && b || !c
来源：http://iqn.tianlin.xyz

C#:   a && b || !c
来源：http://ctd.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://quj.fehbvm.com

Py:   if not data: return
来源：http://btk.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://rye.vqdsnc.cn

JS:   if (!data) return;
来源：http://ven.aizwys.cn

TS:   if (!data) return;
来源：http://cve.pengpengdd.cyou

Java: if (data == null) return;
来源：http://uwb.yanxiufei.cn

Go:   if data == nil { return }
来源：http://zkn.jinqigfzy.top

Ruby: return if data.nil?
来源：http://hpg.nanxinkj.top

C#:   if (data == null) return;
来源：http://gdi.epnwcf.com

================================================================================
来源：http://fmg.jqgfzy.top

C. 函数与作用域
来源：http://iyj.hesvh.cn

================================================================================
来源：http://dam.yuanzhike.top

[C01] 定义函数
来源：http://jnb.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://vzm.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://riu.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://dyd.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gzh.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jlk.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ivi.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://bnv.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://brz.gzhubu.top

[C02] 默认参数
来源：http://erf.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ozh.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sxx.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://sqs.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bue.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gpp.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mbv.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://mmi.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://ptv.havefunace.top

[C03] 可变参数
来源：http://pkm.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://bgo.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ebu.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fcj.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mad.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zcn.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ocd.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://eku.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zfm.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://gne.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cri.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zug.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vuc.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://coh.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://yxs.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://wsx.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://viz.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://spb.yueranfly.top

[C05] 返回多个值
来源：http://rzm.0kj1m.cn

Py:   return a, b
来源：http://eyl.sufxvd.cn

PHP:  return [$a, $b];
来源：http://gky.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lii.xinyue.icu

TS:   return { a, b };
来源：http://kcq.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zxc.hesvh.cn

Go:   return a, b
来源：http://bzm.zhaomingkeji.xyz

Ruby: return a, b
来源：http://uba.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://rje.cashguo.top

[C06] 匿名函数 / lambda
来源：http://ixt.andypj.xyz

Py:   square = lambda x: x * x
来源：http://aaz.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ike.yj20258.top

JS:   const square = x => x * x;
来源：http://fgw.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ied.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cbv.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lkb.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://jwd.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://lsg.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://bdi.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ove.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vkd.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ptx.vehdjk.com

TS:   arr.map(String)
来源：http://mpa.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kzg.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://shc.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://yft.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zgt.jqgufenzy.top

[C08] 闭包
来源：http://lxu.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rji.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ztf.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wlw.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cfg.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vwx.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zqb.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://beb.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://erk.yueranfly.top

[C09] 递归
来源：http://erg.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bua.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://slz.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucd.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccn.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwy.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tih.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tqx.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gfy.wangdashe.top

[C10] 变量作用域
来源：http://nrx.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dpv.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wdu.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yyq.pycfn.com

TS:   同 JS
来源：http://wio.cheryme.top

Java: 方法内为块级作用域
来源：http://drq.yueranfly.top

Go:   花括号块级作用域
来源：http://yie.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xcs.feifeiyinyue.top

C#:   块级作用域
来源：http://yhl.ivvv.top

[C11] 模块导入与导出
来源：http://vww.hywenlv.cn

Py:   from module import func
来源：http://hsz.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://qoc.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ser.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kxl.shanyushiyangtech.top

Java: import java.util.List;
来源：http://gmi.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://edl.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://iqx.fzhhl.top

C#:   using System.Text;
来源：http://byq.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://dhm.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://cle.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://sjp.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://sjg.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://epl.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cso.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://wnn.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://iay.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ykk.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://dbk.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eaa.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eoc.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vpe.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nyq.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://bqi.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://avg.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ukd.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://frm.redwolf501.top

[C14] 泛型函数
来源：http://yqy.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eto.chenjidiqi.icu

PHP:  // 无泛型
来源：http://usu.zdqjudy.top

JS:   // 无泛型
来源：http://qoq.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nnv.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kxp.haohaochexian.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yas.ehwqpu.com

Ruby: # 无泛型
来源：http://ghm.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zai.cashguo.top

[C15] 解构 / 展开参数
来源：http://dky.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rtn.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://yxy.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qdu.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://haa.yonumen.top

Java: // 无解构
来源：http://iyv.zycfv.cn

Go:   // 无解构
来源：http://irm.sxryk.cn

Ruby: a, b = pair
来源：http://uph.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://unb.nwbrower.top

[C16] 函数 / 方法重载
来源：http://bst.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hli.ybcxt.top

PHP:  // 无重载
来源：http://dta.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nmt.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://fps.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yiy.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://kbi.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://hzi.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wwu.yuanzhike.top

================================================================================
来源：http://ubl.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://zdd.c1oappe.top

================================================================================
来源：http://pvg.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://ujj.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qvx.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oum.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cyy.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uun.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbd.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://uhc.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://luj.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kef.cheryme.top

[D02] 追加元素到末尾
来源：http://lun.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oeb.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dzn.yvedp.cn

JS:   arr.push(4);
来源：http://abo.dashuyun.cn

TS:   arr.push(4);
来源：http://wnc.shzxlz.cn

Java: list.add(4);
来源：http://mlj.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://zfz.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://gnv.shuidangran.top

C#:   list.Add(4);
来源：http://gaa.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://azq.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://xft.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lei.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://asr.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://elz.c1oappe.top

Java: list.add(0, 0);
来源：http://aex.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://cbf.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pzn.hongshengwenyu.top


<!-- 参考信息 -->