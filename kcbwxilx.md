代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ikl.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofq.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocw.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://opt.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pvo.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glr.shanyushiyangtech.top

[B03] switch / match / case
来源：http://qkg.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ise.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tui.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://haw.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hfw.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dda.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xta.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://twq.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://puu.wangdashe.top

[B04] for 计数循环
来源：http://kru.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://hoc.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iur.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avg.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qaz.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tiy.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vum.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://mpg.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wqx.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://fhc.havefunace.top

Py:   for item in arr: print(item)
来源：http://xxj.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rqz.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fng.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fgi.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xrx.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ral.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://bcv.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tpj.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://yel.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ftt.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qlj.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xcv.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://emq.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mnt.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://erm.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pxf.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gdr.birdmap.top

[B07] while 循环
来源：http://rij.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://lld.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://wye.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://bqu.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://apy.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://hql.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gus.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://auy.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://ivr.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://krp.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://bdq.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rdi.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://kur.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://cgf.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://jsi.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uqz.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://hju.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://vhz.hongshengwenyu.top

[B09] break 与 continue
来源：http://thc.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gzc.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mqp.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnm.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wds.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://awx.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rah.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ltr.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tls.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://ivp.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ade.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydh.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sou.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fhg.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://scu.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qet.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uhe.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kzr.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://vae.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://kka.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://wrh.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kzk.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://phx.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://luh.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xps.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://dfy.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gfb.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://qnc.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://tvo.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://doz.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ppd.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksp.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cql.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://alv.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xiz.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tnc.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://lpw.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://fjf.hywenlv.cn

PHP:  is_numeric($x)
来源：http://keb.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdf.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqo.yanxiufei.cn

Java: x instanceof Number
来源：http://yen.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://scf.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://yqk.birdmap.top

C#:   x is int or double or decimal
来源：http://rfj.guannengcc.top

[B14] 判断值是否在集合内
来源：http://vwy.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ubq.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lob.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://hen.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://pmm.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fok.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wss.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://wmq.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iuk.havefunace.top

[B15] 布尔运算与取反
来源：http://qqp.snrcjt.cn

Py:   a and b or not c
来源：http://lio.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://eby.tanke756.top

JS:   a && b || !c
来源：http://ccy.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://lcj.tianlin.xyz

Java: a && b || !c
来源：http://pkh.smart0.xyz

Go:   a && b || !c
来源：http://dlt.havefunace.top

Ruby: a && b || !c
来源：http://viw.bbcook.cn

C#:   a && b || !c
来源：http://ywi.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://kmk.jianghu66.top

Py:   if not data: return
来源：http://anb.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://gph.hnqzz.top

JS:   if (!data) return;
来源：http://fgi.jinqigfzy.top

TS:   if (!data) return;
来源：http://nne.yvedp.cn

Java: if (data == null) return;
来源：http://lsi.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://xcu.yongpay.top

Ruby: return if data.nil?
来源：http://irs.xinyue.icu

C#:   if (data == null) return;
来源：http://czi.shangyingyoupin.top

================================================================================
来源：http://dao.vehdjk.com

C. 函数与作用域
来源：http://mug.snrcjt.cn

================================================================================
来源：http://yoq.yuxming.cn

[C01] 定义函数
来源：http://gcd.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://yew.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ffo.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://zzi.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdh.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qtm.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://hvb.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://dvx.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uop.gzhubu.top

[C02] 默认参数
来源：http://xyw.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://htu.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://slc.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://dvg.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://elf.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://smz.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hau.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://bce.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://ufu.haohaochexian.top

[C03] 可变参数
来源：http://ntx.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://prx.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gkd.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sll.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahk.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xov.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mxf.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://lev.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jie.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://lgb.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uhb.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pzz.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://var.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oqg.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://iqa.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://tcq.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://eso.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://cga.aizwys.cn

[C05] 返回多个值
来源：http://khp.zhiwuduotai.top

Py:   return a, b
来源：http://dfx.sxryk.cn

PHP:  return [$a, $b];
来源：http://pgp.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.jyoumei.cn

TS:   return { a, b };
来源：http://llo.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gun.9152youxi.cn

Go:   return a, b
来源：http://kgb.vqdsnc.cn

Ruby: return a, b
来源：http://fpc.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://lxy.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://yey.nwbrower.top

Py:   square = lambda x: x * x
来源：http://szc.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cpf.wangdashe.top

JS:   const square = x => x * x;
来源：http://gyv.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://ovp.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yse.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://uow.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://txx.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://txc.daxiang520.top

[C07] 把函数作为参数传入
来源：http://eas.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tki.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://abp.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ufa.aizwys.cn

TS:   arr.map(String)
来源：http://xly.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bja.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://omd.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://yqw.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://clc.tarul.cn

[C08] 闭包
来源：http://yix.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://soh.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wgo.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xpy.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okt.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gmq.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vku.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nsm.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dcv.yonumen.top

[C09] 递归
来源：http://cfm.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yop.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lqy.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pbq.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://omw.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tkx.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uzn.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://drt.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tnm.ppjwa.cn

[C10] 变量作用域
来源：http://tre.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mtt.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dkc.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vnt.gzhubu.top

TS:   同 JS
来源：http://udg.jianghu66.top

Java: 方法内为块级作用域
来源：http://itb.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://ocl.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://isn.cucudq.cn

C#:   块级作用域
来源：http://yhr.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://nfx.yj20258888.top

Py:   from module import func
来源：http://wij.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pob.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://trz.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gjs.nanxinkj.top

Java: import java.util.List;
来源：http://hzm.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yab.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://huf.aibaodan.cn

C#:   using System.Text;
来源：http://rbt.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://jbm.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://uih.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://wvx.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://bll.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://cxu.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvl.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ukb.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://bdv.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cwb.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://mrr.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wlr.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itj.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lxe.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsh.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://wln.hysaishi.cn

Go:   func add(a, b int) int
来源：http://tlv.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://urh.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://yyh.9152youxi.cn

[C14] 泛型函数
来源：http://uyv.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ogt.ctjpmb.com

PHP:  // 无泛型
来源：http://xhw.jyoumei.cn

JS:   // 无泛型
来源：http://awg.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mlf.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kqe.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://haa.tarul.cn

Ruby: # 无泛型
来源：http://qay.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bir.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://pxt.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lqy.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://qnk.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lqo.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kzg.snrcjt.cn

Java: // 无解构
来源：http://gxn.jinqigfzy.top

Go:   // 无解构
来源：http://khb.zhongyouzk.top

Ruby: a, b = pair
来源：http://wbc.uphjek.com

C#:   var (a, b) = pair;
来源：http://mdy.yj20258888.top

[C16] 函数 / 方法重载
来源：http://eig.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bnz.yj20258888.top

PHP:  // 无重载
来源：http://hdw.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://ffu.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://uto.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://uaz.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://wsd.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://vhk.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xer.zhiwuduotai.top

================================================================================
来源：http://eqi.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://lzf.sysykeji.top

================================================================================
来源：http://vuo.birdmap.top

[D01] 创建数组 / 列表
来源：http://meq.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wcr.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yka.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oqf.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gyb.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zdi.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://dbv.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://xnx.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjq.fzhhl.top

[D02] 追加元素到末尾
来源：http://bqj.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://auz.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omb.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://kur.yueranfly.top

TS:   arr.push(4);
来源：http://tzb.sysykeji.top

Java: list.add(4);
来源：http://xow.birdmap.top

Go:   arr = append(arr, 4)
来源：http://jjz.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://vrn.bjfxy.top

C#:   list.Add(4);
来源：http://lzq.nanxuanxn.top


<!-- 参考信息 -->