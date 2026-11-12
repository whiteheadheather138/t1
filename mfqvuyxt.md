代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mbm.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uif.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cww.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zis.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ibt.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hhr.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://stx.cucudq.cn

[B04] for 计数循环
来源：http://ehv.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://hgz.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://szg.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxu.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://frz.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wlm.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pmu.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://ihp.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbt.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://ary.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://uwh.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vyx.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fwb.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://frd.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nyu.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yxr.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://vsz.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cqk.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://qtf.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zsy.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pgo.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://exu.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxx.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hsa.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hzj.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utd.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xvl.wangshuangyany.cn

[B07] while 循环
来源：http://oow.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://dur.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://uot.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://ovb.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://ngr.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://tdx.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mpv.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://fxz.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://eqv.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://ajj.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://swy.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lrd.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://idi.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://sow.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://jyr.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nnl.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://pzu.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://cec.yvedp.cn

[B09] break 与 continue
来源：http://bly.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oqz.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fzw.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ean.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xri.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydc.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nqd.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxb.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdb.vehdjk.com

[B10] 遍历同时拿索引
来源：http://pyc.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://svf.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lbh.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rac.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://evs.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gdx.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jxb.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://crq.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pnm.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://tmi.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://tjy.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://faa.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwt.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tbb.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fmi.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://npg.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://pxf.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xad.bjfxy.top

[B12] 跳出多层循环
来源：http://spe.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://flh.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://brp.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://suf.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cld.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ebp.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qgr.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://llg.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ndf.mhx1999.top

[B13] 判断是否为数字
来源：http://wpu.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://gjd.zycfv.cn

PHP:  is_numeric($x)
来源：http://ukt.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rtc.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tur.gotoacloud.top

Java: x instanceof Number
来源：http://lso.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vgc.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://otz.redwolf501.top

C#:   x is int or double or decimal
来源：http://adr.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://cdk.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kje.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mge.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://mfn.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://mtw.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cbv.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cln.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ome.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gzk.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://dcu.cqqwz.cn

Py:   a and b or not c
来源：http://qwg.c1oappe.top

PHP:  $a && $b || !$c
来源：http://vuj.gzhubu.top

JS:   a && b || !c
来源：http://nxr.aibaodan.cn

TS:   a && b || !c
来源：http://bjk.bjfxy.top

Java: a && b || !c
来源：http://rok.quarkkingdee.top

Go:   a && b || !c
来源：http://xie.fehbvm.com

Ruby: a && b || !c
来源：http://kqk.ehwqpu.com

C#:   a && b || !c
来源：http://ifz.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iwv.smart0.xyz

Py:   if not data: return
来源：http://tdn.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://pek.wangshuangyany.cn

JS:   if (!data) return;
来源：http://kxz.jiagoushi.top

TS:   if (!data) return;
来源：http://cqe.pycfn.com

Java: if (data == null) return;
来源：http://grv.gaohongyu789.top

Go:   if data == nil { return }
来源：http://msg.svipenyu.cn

Ruby: return if data.nil?
来源：http://bya.jqgfzy.top

C#:   if (data == null) return;
来源：http://iow.ydjk.org.cn

================================================================================
来源：http://htx.jyoumei.cn

C. 函数与作用域
来源：http://ktn.shzxlz.cn

================================================================================
来源：http://iie.aibaodan.cn

[C01] 定义函数
来源：http://xig.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://ynl.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bao.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://fzk.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hoq.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vrv.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://xtk.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://hsz.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://grv.zhongyouzk.top

[C02] 默认参数
来源：http://zmn.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://eqm.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zrp.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://qlu.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://axe.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ogs.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zmo.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://kxc.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://cop.yuxming.cn

[C03] 可变参数
来源：http://cvg.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://lre.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bic.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqx.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://apa.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://djk.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dec.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sdx.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yuc.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://ivy.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nfd.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lrk.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gyf.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jsm.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://enm.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://lmo.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://xph.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://nwr.gotoacloud.top

[C05] 返回多个值
来源：http://npa.zhengqikj.top

Py:   return a, b
来源：http://qgf.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://dkk.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xek.shangyingyoupin.top

TS:   return { a, b };
来源：http://izv.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pus.ydzc1.top

Go:   return a, b
来源：http://klr.yj202588.top

Ruby: return a, b
来源：http://lvg.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://vrb.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://ggs.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://knh.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bwi.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://pnt.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://gyp.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bgi.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://wbd.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://atb.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://xui.iojbl.cn

[C07] 把函数作为参数传入
来源：http://uto.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pnf.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sqg.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kgk.svipenyu.cn

TS:   arr.map(String)
来源：http://zme.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://unv.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oxe.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://iga.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cjv.52xcode.cn

[C08] 闭包
来源：http://moe.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mnm.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://add.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pma.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ogx.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ebh.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ens.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aoj.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jgl.cheryme.top

[C09] 递归
来源：http://gti.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fjl.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vls.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khu.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sps.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oxm.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vua.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://flv.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qsh.daxiang520.top

[C10] 变量作用域
来源：http://auw.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bau.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://goz.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://puk.havefunace.top

TS:   同 JS
来源：http://vrk.ctjpmb.com

Java: 方法内为块级作用域
来源：http://zvi.ivvv.top

Go:   花括号块级作用域
来源：http://ioc.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wyi.havefunace.top

C#:   块级作用域
来源：http://ksr.hfpthk.cn

[C11] 模块导入与导出
来源：http://avs.ywan-chungtsiang.top

Py:   from module import func
来源：http://puz.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fxj.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dso.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rne.jqgfzy.top

Java: import java.util.List;
来源：http://cpt.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://luo.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://qza.zdbjq.cn

C#:   using System.Text;
来源：http://hca.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://edv.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://gvf.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://zoh.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://tff.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://cwf.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uqb.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://uqa.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://jrx.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rlu.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://zuy.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vsc.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jrw.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gke.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uql.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cjo.ehwqpu.com

Go:   func add(a, b int) int
来源：http://sdt.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mdp.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://phe.cucudq.cn

[C14] 泛型函数
来源：http://rii.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://msc.xuanzx.com

PHP:  // 无泛型
来源：http://qal.kuanghao11.cn

JS:   // 无泛型
来源：http://kkm.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hjc.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ruw.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cqe.zhengqikj.top

Ruby: # 无泛型
来源：http://mni.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zyc.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://yah.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dam.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://sdo.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wbg.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gir.guannengcc.top

Java: // 无解构
来源：http://iqn.guannengcc.top

Go:   // 无解构
来源：http://oph.bbcook.cn

Ruby: a, b = pair
来源：http://vfn.sysykeji.top

C#:   var (a, b) = pair;
来源：http://pth.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://upj.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://psc.yangfankeji.com

PHP:  // 无重载
来源：http://geu.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://gby.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://oop.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wyz.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://iiw.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://iyy.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jsd.jlsjyb.cn

================================================================================
来源：http://bep.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://prk.redwolf501.top

================================================================================
来源：http://cxe.sysykeji.top

[D01] 创建数组 / 列表
来源：http://fun.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://eqc.ctjpmb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://itw.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dcf.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://dks.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jru.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://wrb.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://rpf.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ljp.chenlongwang.top

[D02] 追加元素到末尾
来源：http://nga.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aci.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pzi.vehdjk.com

JS:   arr.push(4);
来源：http://dpw.jlsjyb.cn

TS:   arr.push(4);
来源：http://mwy.dashuyun.cn

Java: list.add(4);
来源：http://phk.meibo888.top

Go:   arr = append(arr, 4)
来源：http://bxx.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ehk.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://oex.shuidangran.top

[D03] 在指定位置插入元素
来源：http://yur.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://ags.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://osq.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fri.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://evl.52xcode.cn

Java: list.add(0, 0);
来源：http://qke.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://par.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wys.jiagoushi.top


<!-- 参考信息 -->