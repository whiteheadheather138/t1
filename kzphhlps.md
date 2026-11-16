代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbm.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jze.sufxvd.cn

[B03] switch / match / case
来源：http://krs.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://map.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xyo.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://soj.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gwh.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dro.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mkw.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nto.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fsq.havefunace.top

[B04] for 计数循环
来源：http://wua.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://fwi.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sfc.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pnw.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://flv.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ppy.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yah.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://rdm.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ifj.hammf.cn

[B05] 遍历数组 / 列表
来源：http://bmp.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://zzo.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gyt.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sit.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yer.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bcy.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ydy.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://gkn.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lux.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://ykg.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sjx.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jgl.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://plz.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spi.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qqd.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wej.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gco.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txm.9152youxi.cn

[B07] while 循环
来源：http://mqo.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://hyu.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ghl.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://mfa.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://bvy.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://uai.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yzi.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://cid.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://frs.meibo888.top

[B08] do-while（至少执行一次）
来源：http://vir.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://som.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wpl.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://kbu.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://tkh.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://wwn.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://xru.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://kwr.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://gmq.guowangkeji.top

[B09] break 与 continue
来源：http://lwp.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hhv.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fin.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqu.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jko.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ito.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hof.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://teg.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvl.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://uqj.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wyp.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qvu.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kfi.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wgq.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dyt.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bwu.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fur.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qkc.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://arc.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://rdg.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://zql.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxz.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntq.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rwn.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://whi.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://pvy.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rvo.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://dfd.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rbh.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wos.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://apr.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vzx.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gzh.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vqp.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://una.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fxn.kuanghao11.cn

[B13] 判断是否为数字
来源：http://ouc.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://pyr.dashuyun.cn

PHP:  is_numeric($x)
来源：http://cyk.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utj.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yzn.shangyingyoupin.top

Java: x instanceof Number
来源：http://akw.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://are.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://iyf.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://vpi.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://mos.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aoh.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iau.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://get.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://fno.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cwz.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ueb.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ogg.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uqs.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://avq.svipenyu.cn

Py:   a and b or not c
来源：http://fga.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://woc.chenzaomai.com

JS:   a && b || !c
来源：http://yix.vqdsnc.cn

TS:   a && b || !c
来源：http://rez.yangfankeji.com

Java: a && b || !c
来源：http://con.xinyue.icu

Go:   a && b || !c
来源：http://lyq.fktsv.cn

Ruby: a && b || !c
来源：http://hpd.zhijiandao.cn

C#:   a && b || !c
来源：http://ppz.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ksj.snrcjt.cn

Py:   if not data: return
来源：http://caq.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://uny.yj20258888.top

JS:   if (!data) return;
来源：http://pfb.wangdashe.top

TS:   if (!data) return;
来源：http://rqu.snrcjt.cn

Java: if (data == null) return;
来源：http://txa.hesvh.cn

Go:   if data == nil { return }
来源：http://ier.fzhhl.top

Ruby: return if data.nil?
来源：http://gap.ppjwa.cn

C#:   if (data == null) return;
来源：http://yvu.ctjpmb.com

================================================================================
来源：http://anm.gotoacloud.top

C. 函数与作用域
来源：http://hvh.nanxinkj.top

================================================================================
来源：http://wdx.sjlbkw.cn

[C01] 定义函数
来源：http://brc.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://jus.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nff.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://aps.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vlc.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lds.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jxa.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://qdf.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://psx.xuanzx.com

[C02] 默认参数
来源：http://xvn.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://rmz.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pov.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://zbr.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxh.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zau.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qnh.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://hns.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://ajx.uphjek.com

[C03] 可变参数
来源：http://anx.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://ptk.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zji.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tdc.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sif.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://exw.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dku.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://xkq.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nke.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://dyn.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://spx.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iek.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zey.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mrv.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://kqz.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://nau.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://idg.sweek.top

C#:   f(a: 1, b: 2)
来源：http://gwh.yj202588.top

[C05] 返回多个值
来源：http://ski.zycfv.cn

Py:   return a, b
来源：http://xlm.0kj1m.cn

PHP:  return [$a, $b];
来源：http://cix.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qwo.hywenlv.cn

TS:   return { a, b };
来源：http://mez.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wri.jinqigfzy.top

Go:   return a, b
来源：http://eyo.daxiang520.top

Ruby: return a, b
来源：http://vxv.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://zht.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://xpa.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://iwm.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ugx.sxryk.cn

JS:   const square = x => x * x;
来源：http://rpt.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://ibh.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://occ.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://lcu.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://tuk.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nfh.xuanzx.com

[C07] 把函数作为参数传入
来源：http://mta.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gnv.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://jrw.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gqc.hesvh.cn

TS:   arr.map(String)
来源：http://dev.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://irt.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aaw.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://hph.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nhr.aibaodan.cn

[C08] 闭包
来源：http://jsr.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jhb.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vom.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oxz.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eno.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gvc.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rim.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pij.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://axp.chenjidiqi.icu

[C09] 递归
来源：http://cyq.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ekz.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fzh.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvw.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crr.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bus.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dvg.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kqc.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://frd.zhiwuduotai.top

[C10] 变量作用域
来源：http://gem.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqy.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sgs.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofg.hongshengwenyu.top

TS:   同 JS
来源：http://clg.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://ldr.yangfankeji.com

Go:   花括号块级作用域
来源：http://heh.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fqn.epnwcf.com

C#:   块级作用域
来源：http://oyn.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://bbq.bbcook.cn

Py:   from module import func
来源：http://wdz.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pnd.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qtn.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cap.andypj.xyz

Java: import java.util.List;
来源：http://jvo.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://elj.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://zro.hesvh.cn

C#:   using System.Text;
来源：http://yxz.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://zzz.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://dvz.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://egu.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://etp.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://tva.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zxl.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://sdb.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://qzt.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yow.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://fur.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qaj.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpp.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ygw.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xje.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dir.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://fqa.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lzx.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mrs.shangyingyoupin.top

[C14] 泛型函数
来源：http://mvs.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uzv.hcnkem.com

PHP:  // 无泛型
来源：http://vlk.svipenyu.cn

JS:   // 无泛型
来源：http://gsr.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://waw.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ddo.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mqx.iojbl.cn

Ruby: # 无泛型
来源：http://kyz.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://igu.epnwcf.com

[C15] 解构 / 展开参数
来源：http://gim.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bkk.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://plw.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ldc.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://guy.nanxuanxn.top

Java: // 无解构
来源：http://ufb.chenlongwang.top

Go:   // 无解构
来源：http://axo.cdnleiting.top

Ruby: a, b = pair
来源：http://zmi.ydzc1.top

C#:   var (a, b) = pair;
来源：http://jzc.hammf.cn

[C16] 函数 / 方法重载
来源：http://xmd.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://knf.ehwqpu.com

PHP:  // 无重载
来源：http://xnc.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lnh.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://lpx.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vor.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://gnh.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://ezj.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iie.yuxming.cn

================================================================================
来源：http://svf.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://vvu.daria6918.cn

================================================================================
来源：http://qoo.yj20258.top

[D01] 创建数组 / 列表
来源：http://bjv.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fmj.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qgm.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://spi.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xeu.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ddl.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://dkv.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://mnb.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pdm.nwbrower.top

[D02] 追加元素到末尾
来源：http://cfr.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mro.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rqq.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://xvh.haohaochexian.top

TS:   arr.push(4);
来源：http://jok.yfazqb.com

Java: list.add(4);
来源：http://uvv.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://upe.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://whp.fzhhl.top

C#:   list.Add(4);
来源：http://awe.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://lgf.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://qmj.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iqd.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvj.chenlongwang.top


<!-- 参考信息 -->