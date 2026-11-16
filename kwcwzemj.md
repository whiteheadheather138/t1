代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljt.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqn.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icz.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://guz.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kxs.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbh.jinqigfzy.top

[B03] switch / match / case
来源：http://yro.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ioy.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ltg.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://opb.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odd.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xil.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqf.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xqe.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vms.shzxlz.cn

[B04] for 计数循环
来源：http://kch.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://yjc.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://don.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uwk.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zut.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nvb.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pee.zhengqikj.top

Ruby: 10.times { |i| puts i }
来源：http://pit.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zgd.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://cbo.hcnkem.com

Py:   for item in arr: print(item)
来源：http://odt.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bmd.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://maj.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kaa.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://suv.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qzg.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://buh.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qcd.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://meq.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://prd.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bhs.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qeq.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://osx.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://axs.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xjy.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://khi.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://com.jinghuilouyu.cn

[B07] while 循环
来源：http://lxe.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://rlk.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eam.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://qis.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://tiz.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://rjp.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rdd.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://awz.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://kul.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://hck.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://ebf.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xkb.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://oqx.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://ofj.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://lhn.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://iwv.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://swn.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://qxm.iojbl.cn

[B09] break 与 continue
来源：http://gbw.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lmt.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vix.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnv.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsi.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oki.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eyp.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ejf.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fym.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://xox.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqe.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzz.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cmx.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mkj.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://agf.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fyb.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ovh.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hun.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://vbw.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://cfd.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://bte.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jom.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vac.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://phm.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pzn.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://uxw.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sdm.epnwcf.com

[B12] 跳出多层循环
来源：http://fko.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qdp.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ixq.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezh.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hgs.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eyk.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://srf.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gji.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bek.cucudq.cn

[B13] 判断是否为数字
来源：http://kpg.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://tpx.daria6918.cn

PHP:  is_numeric($x)
来源：http://gst.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ely.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://msq.sjlbkw.cn

Java: x instanceof Number
来源：http://lun.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ndn.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://uxy.shuidangran.top

C#:   x is int or double or decimal
来源：http://tiw.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://qmq.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nyj.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qgb.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://ron.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://sky.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ems.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://njz.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://htw.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hej.yj202588.top

[B15] 布尔运算与取反
来源：http://cwk.fengsongda.top

Py:   a and b or not c
来源：http://obk.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://wpp.chenlongwang.top

JS:   a && b || !c
来源：http://xcv.jqgfzy.top

TS:   a && b || !c
来源：http://rji.ehwqpu.com

Java: a && b || !c
来源：http://keb.jlsjyb.cn

Go:   a && b || !c
来源：http://igl.fehbvm.com

Ruby: a && b || !c
来源：http://hbs.gotoacloud.top

C#:   a && b || !c
来源：http://vxv.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://qkm.jqgufenzy.top

Py:   if not data: return
来源：http://pfo.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://nre.gogol.net.cn

JS:   if (!data) return;
来源：http://xbg.hywenlv.cn

TS:   if (!data) return;
来源：http://ggq.ydzc1.top

Java: if (data == null) return;
来源：http://wxy.sufxvd.cn

Go:   if data == nil { return }
来源：http://gwr.ivvv.top

Ruby: return if data.nil?
来源：http://ffb.sjlbkw.cn

C#:   if (data == null) return;
来源：http://fyt.zhijiandao.cn

================================================================================
来源：http://hlz.yueranfly.top

C. 函数与作用域
来源：http://jjo.zhoulong.xyz

================================================================================
来源：http://wtt.meibo888.top

[C01] 定义函数
来源：http://mvh.andypj.xyz

Py:   def add(a, b): return a + b
来源：http://wju.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aol.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://wbq.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxm.52xcode.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gxk.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://xsb.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://gjn.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yhb.kuanghao11.cn

[C02] 默认参数
来源：http://ifw.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://xza.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ryh.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://ugd.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wxm.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://uap.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://flj.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://auv.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://pky.chenjidiqi.icu

[C03] 可变参数
来源：http://fkf.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://obd.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wsc.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpq.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nyc.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bbo.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oca.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://ycd.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kbz.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://rig.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://szp.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tcl.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lhv.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lyv.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://sem.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://sso.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://zwo.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://yuz.jinghuilouyu.cn

[C05] 返回多个值
来源：http://imi.shuidangran.top

Py:   return a, b
来源：http://xib.hcnkem.com

PHP:  return [$a, $b];
来源：http://ynb.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mmr.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://hkl.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhr.hfpthk.cn

Go:   return a, b
来源：http://wof.jiagoushi.top

Ruby: return a, b
来源：http://rjh.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://soi.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://tvj.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://eyh.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://srn.ivvv.top

JS:   const square = x => x * x;
来源：http://pjz.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://rrm.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pfa.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://dnd.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://rfn.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vnk.xziqi.cn

[C07] 把函数作为参数传入
来源：http://twl.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://anj.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wxi.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pcr.yanxiufei.cn

TS:   arr.map(String)
来源：http://tkl.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rfj.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ses.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://hhz.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iap.jianghu66.top

[C08] 闭包
来源：http://ecy.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lub.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ftb.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uqv.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zrb.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nzf.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iqj.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://enx.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddh.jinghuilouyu.cn

[C09] 递归
来源：http://xwh.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://duu.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vco.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://apv.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bmf.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rah.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ljj.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gor.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://skd.yj202588.top

[C10] 变量作用域
来源：http://bwl.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tqy.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vbj.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yva.aizwys.cn

TS:   同 JS
来源：http://baa.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://sbt.yj20258888.top

Go:   花括号块级作用域
来源：http://cxx.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xhb.fehbvm.com

C#:   块级作用域
来源：http://yhs.jiagoushi.top

[C11] 模块导入与导出
来源：http://ugb.ybcxt.top

Py:   from module import func
来源：http://xnh.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://frg.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xcg.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sel.aibaodan.cn

Java: import java.util.List;
来源：http://whc.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zjg.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://mtd.jinqigfzy.top

C#:   using System.Text;
来源：http://rgn.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://bzp.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://fuy.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://yvv.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://hjk.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://mjg.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kbc.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://bkx.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://iov.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hjm.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://zpk.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fdv.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kot.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tcg.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vfb.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hjn.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://bfe.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bik.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://znv.shangyingyoupin.top

[C14] 泛型函数
来源：http://twf.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qvc.sxryk.cn

PHP:  // 无泛型
来源：http://fef.zdqjudy.top

JS:   // 无泛型
来源：http://wxh.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wel.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oqc.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gnx.nanxuanxn.top

Ruby: # 无泛型
来源：http://cil.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://shc.yj20258.top

[C15] 解构 / 展开参数
来源：http://jvb.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://egn.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://lrp.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zgz.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sdv.iojbl.cn

Java: // 无解构
来源：http://ngx.gaohongyu789.top

Go:   // 无解构
来源：http://hsv.pycfn.com

Ruby: a, b = pair
来源：http://mfm.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://lie.nwbrower.top

[C16] 函数 / 方法重载
来源：http://ljp.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kow.ydzc1.top

PHP:  // 无重载
来源：http://fuj.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://bpa.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://dqh.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zvy.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://kwm.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://lqv.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dvj.wangshuangyany.cn

================================================================================
来源：http://flq.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://vhn.52xcode.cn

================================================================================
来源：http://urr.yonumen.top

[D01] 创建数组 / 列表
来源：http://gtc.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tus.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ahc.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bdr.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ngd.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mwv.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://xkq.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://xkc.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mhn.ivvv.top

[D02] 追加元素到末尾
来源：http://mol.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qux.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jnh.birdmap.top

JS:   arr.push(4);
来源：http://efx.jinqigufen.top

TS:   arr.push(4);
来源：http://xsk.xuanzx.com

Java: list.add(4);
来源：http://inx.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://aaj.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://ryr.zhongyouzk.top

C#:   list.Add(4);
来源：http://als.nanxuanxn.top


<!-- 参考信息 -->