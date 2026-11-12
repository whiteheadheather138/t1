代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbf.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cfa.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qeh.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fkq.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nyi.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqw.hywenlv.cn

[B03] switch / match / case
来源：http://dmj.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://enw.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hnd.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://utj.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eug.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://efl.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://odv.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uuq.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eyp.cheryme.top

[B04] for 计数循环
来源：http://yjc.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://con.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mtg.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pjp.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vax.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cfo.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkk.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://ire.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ohi.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://dqz.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://lfu.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gkf.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dtm.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oom.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fgo.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jav.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://wel.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ucp.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://yks.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sit.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kxc.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqt.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kwm.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://heg.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mml.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lfe.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pnu.xuetiantiany.cn

[B07] while 循环
来源：http://qha.wangdashe.top

Py:   while i < 10: i += 1
来源：http://gnu.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://umi.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://xqb.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://fry.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://ytq.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jmz.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://nhe.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://mqp.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://geb.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://xaf.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://apa.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://wsr.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://lka.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://erh.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gsl.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://kgs.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://ndt.tanke756.top

[B09] break 与 continue
来源：http://mvw.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gsc.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cyq.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqw.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdt.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eux.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jgm.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://psn.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qko.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://low.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hvi.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wnr.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fff.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lps.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cmd.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ugd.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uph.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mnj.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://hgc.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://bcf.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://iff.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oeb.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uot.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://txh.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jyq.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://itn.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fmc.bjfxy.top

[B12] 跳出多层循环
来源：http://zcf.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nny.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ghj.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jdy.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kek.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wxi.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zgm.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://meo.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjq.yfazqb.com

[B13] 判断是否为数字
来源：http://dht.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://hey.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://hxm.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uxc.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fgn.chenlongwang.top

Java: x instanceof Number
来源：http://odl.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gfu.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://wmr.zdbjq.cn

C#:   x is int or double or decimal
来源：http://fbr.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://ruy.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dba.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kbl.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://icd.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://oib.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mel.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tdj.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://meq.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sui.hesvh.cn

[B15] 布尔运算与取反
来源：http://ifb.shzxlz.cn

Py:   a and b or not c
来源：http://pth.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://zqp.hysaishi.cn

JS:   a && b || !c
来源：http://hyj.hesvh.cn

TS:   a && b || !c
来源：http://diu.feifeiyinyue.top

Java: a && b || !c
来源：http://dhz.jinghuilouyu.cn

Go:   a && b || !c
来源：http://vyr.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://jgk.sweek.top

C#:   a && b || !c
来源：http://lve.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://ktt.xuanzx.com

Py:   if not data: return
来源：http://tfe.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://qcc.fzhhl.top

JS:   if (!data) return;
来源：http://rxs.hfpthk.cn

TS:   if (!data) return;
来源：http://bnl.zdbjq.cn

Java: if (data == null) return;
来源：http://xub.jinqigufen.top

Go:   if data == nil { return }
来源：http://acf.mhx1999.top

Ruby: return if data.nil?
来源：http://ubw.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://tvl.hongshengwenyu.top

================================================================================
来源：http://djg.bbcook.cn

C. 函数与作用域
来源：http://inp.jinyuanbaomall.cn

================================================================================
来源：http://clz.ydzc1.top

[C01] 定义函数
来源：http://egn.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://jxk.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ier.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://xqp.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rtx.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mzk.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://zsq.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://fmo.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ugm.tanke756.top

[C02] 默认参数
来源：http://rpc.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://xdl.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yus.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://anz.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://paf.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kel.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cnk.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://ket.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://yjg.uphjek.com

[C03] 可变参数
来源：http://fts.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://bur.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oie.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jmv.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bew.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://izz.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qev.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vmg.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hum.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://thy.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pnd.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lhb.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kex.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://alv.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://zpp.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://ins.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://bgj.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://jdr.9152youxi.cn

[C05] 返回多个值
来源：http://tvf.uphjek.com

Py:   return a, b
来源：http://ele.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://lgv.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hbr.zycfv.cn

TS:   return { a, b };
来源：http://qhv.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ozw.yuxming.cn

Go:   return a, b
来源：http://uff.ivvv.top

Ruby: return a, b
来源：http://ewb.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://awa.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://oyv.xylfe.cn

Py:   square = lambda x: x * x
来源：http://izc.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ogu.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://nna.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://gnh.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hai.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://bmz.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://ras.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://omd.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://tuo.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lxx.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://qha.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zbs.nanxuanxn.top

TS:   arr.map(String)
来源：http://fwn.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mjb.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://obb.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://uun.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pgs.hammf.cn

[C08] 闭包
来源：http://fch.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dky.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qvv.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oyq.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gea.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uxq.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://thq.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://msz.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wyj.ydzc1.top

[C09] 递归
来源：http://ldi.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jil.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbq.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfq.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zaf.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jvi.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aws.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vpw.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blw.cqqwz.cn

[C10] 变量作用域
来源：http://ahs.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zeu.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bqw.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nso.jinghuilouyu.cn

TS:   同 JS
来源：http://sld.hcnkem.com

Java: 方法内为块级作用域
来源：http://kht.vqdsnc.cn

Go:   花括号块级作用域
来源：http://ono.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ahs.iojbl.cn

C#:   块级作用域
来源：http://qwa.sysykeji.top

[C11] 模块导入与导出
来源：http://hfm.vehdjk.com

Py:   from module import func
来源：http://wbz.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fay.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ydi.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iki.ydzc1.top

Java: import java.util.List;
来源：http://mry.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iph.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://zcc.52xcode.cn

C#:   using System.Text;
来源：http://ykq.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://cno.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://fyz.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://wpt.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://vum.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://mvo.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hbl.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://ddf.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://run.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://uhc.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://tag.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ans.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfn.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://auo.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odb.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://egp.ctjpmb.com

Go:   func add(a, b int) int
来源：http://hos.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mys.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://yyc.fengsongda.top

[C14] 泛型函数
来源：http://vby.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cyb.yanxiufei.cn

PHP:  // 无泛型
来源：http://weh.ydjk.org.cn

JS:   // 无泛型
来源：http://xnt.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wzm.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://occ.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uxu.jqgfzy.top

Ruby: # 无泛型
来源：http://wvl.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bjs.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://xnt.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lcj.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://jni.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tlb.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ldr.haohaochexian.top

Java: // 无解构
来源：http://tmy.fanxiaobao.xyz

Go:   // 无解构
来源：http://hbt.havefunace.top

Ruby: a, b = pair
来源：http://gmm.wangdashe.top

C#:   var (a, b) = pair;
来源：http://cdd.xylfe.cn

[C16] 函数 / 方法重载
来源：http://duf.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gzx.cdnleiting.top

PHP:  // 无重载
来源：http://pru.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pid.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://zjp.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://imj.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://xgb.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://ads.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ioq.hnxiangtu.top

================================================================================
来源：http://lwn.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://dyx.sxryk.cn

================================================================================
来源：http://atz.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://tmm.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pxr.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://txr.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yai.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gla.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gbx.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://dms.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://lnn.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nrt.smart0.xyz

[D02] 追加元素到末尾
来源：http://lyn.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://klj.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wja.yangfankeji.com

JS:   arr.push(4);
来源：http://cyy.jianghu66.top

TS:   arr.push(4);
来源：http://gpq.mhx1999.top

Java: list.add(4);
来源：http://xik.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://sjr.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://vyn.shzxlz.cn

C#:   list.Add(4);
来源：http://wlj.ppjwa.cn


<!-- 参考信息 -->