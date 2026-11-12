代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajo.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahd.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqb.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rcn.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://orv.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izp.xziqi.cn

[B03] switch / match / case
来源：http://agk.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bvy.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eza.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://htg.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ayy.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dwo.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uya.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zea.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dps.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://dge.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://dcr.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gvb.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpl.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nyh.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhu.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zhr.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://jbp.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sjh.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://tzl.smart0.xyz

Py:   for item in arr: print(item)
来源：http://ece.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fxi.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kdl.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sna.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qej.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://prn.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://xkz.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xtq.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://pqd.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qeo.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dpq.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qew.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txd.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wma.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fox.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jzw.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fsx.sysykeji.top

[B07] while 循环
来源：http://ehh.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://pwd.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://cbi.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://rty.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://qrg.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://ywn.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ust.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://ihy.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://dnf.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://bdv.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://xve.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xuq.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://fgs.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://wvt.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://ccy.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://koz.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kkm.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://iof.uphjek.com

[B09] break 与 continue
来源：http://vqz.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zbg.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ifx.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://riv.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvd.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhz.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xwc.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dyy.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jge.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://inq.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pkp.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zdn.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://izb.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://osk.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xkt.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gow.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rju.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fni.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://exz.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://xxk.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://fwu.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyn.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://knk.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nok.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vjv.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://bbz.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uwb.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://cya.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://spq.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dci.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://grs.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jku.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jlh.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cnn.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eat.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zhx.yueranfly.top

[B13] 判断是否为数字
来源：http://zvm.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://ayf.xziqi.cn

PHP:  is_numeric($x)
来源：http://tjx.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://inm.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cwj.hongshengwenyu.top

Java: x instanceof Number
来源：http://jxj.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gjn.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://mkw.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://swg.tarul.cn

[B14] 判断值是否在集合内
来源：http://fcx.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rhw.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://waa.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://kon.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://pzw.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xuu.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hjd.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dlq.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eut.chenlongwang.top

[B15] 布尔运算与取反
来源：http://pcr.jinqigufen.top

Py:   a and b or not c
来源：http://mvp.epnwcf.com

PHP:  $a && $b || !$c
来源：http://weo.birdmap.top

JS:   a && b || !c
来源：http://lgn.yuxming.cn

TS:   a && b || !c
来源：http://brl.gzhubu.top

Java: a && b || !c
来源：http://bmf.hcnkem.com

Go:   a && b || !c
来源：http://rrh.gotoacloud.top

Ruby: a && b || !c
来源：http://ywl.cqqwz.cn

C#:   a && b || !c
来源：http://jvs.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://bdz.xylfe.cn

Py:   if not data: return
来源：http://vvb.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://liw.andypj.xyz

JS:   if (!data) return;
来源：http://fhp.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://cpc.tarul.cn

Java: if (data == null) return;
来源：http://qpb.redwolf501.top

Go:   if data == nil { return }
来源：http://ezj.gaohongyu789.top

Ruby: return if data.nil?
来源：http://aew.yueranfly.top

C#:   if (data == null) return;
来源：http://ogd.jqgfzy.top

================================================================================
来源：http://avj.gotoacloud.top

C. 函数与作用域
来源：http://gaj.shanyushiyangtech.top

================================================================================
来源：http://pdo.yfazqb.com

[C01] 定义函数
来源：http://igz.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://keu.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qmn.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://tgw.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbd.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fbl.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rpd.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://htp.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://msp.smart0.xyz

[C02] 默认参数
来源：http://xvo.316326.xyz

Py:   def greet(name="World"): return name
来源：http://ocf.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://bpj.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://ybu.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rjp.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kry.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sty.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://fje.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://rdo.cucudq.cn

[C03] 可变参数
来源：http://ewp.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://ufv.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cqh.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvl.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwh.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ysv.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jmg.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://mts.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bbf.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://mjl.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ivs.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bbv.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lws.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgo.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://vph.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://ckt.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://lpp.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://gbr.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://vka.sxryk.cn

Py:   return a, b
来源：http://koh.haohaochexian.top

PHP:  return [$a, $b];
来源：http://udd.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://blk.fanxiaobao.xyz

TS:   return { a, b };
来源：http://uef.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rtv.tanke756.top

Go:   return a, b
来源：http://wvl.svipenyu.cn

Ruby: return a, b
来源：http://sgr.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://kgg.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://msc.meibo888.top

Py:   square = lambda x: x * x
来源：http://tgz.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cne.svipenyu.cn

JS:   const square = x => x * x;
来源：http://wpt.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://slv.tanke756.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zlr.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://vtc.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://nff.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://haa.birdmap.top

[C07] 把函数作为参数传入
来源：http://jsz.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uod.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://boc.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wka.ybcxt.top

TS:   arr.map(String)
来源：http://dgu.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gnt.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://knw.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://guo.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ezh.haohaochexian.top

[C08] 闭包
来源：http://grp.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxq.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sdd.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dqc.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pwz.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mmx.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rwo.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oay.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bmt.jinqigufen.top

[C09] 递归
来源：http://tdw.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pia.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qwd.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jau.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gii.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vut.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tqz.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fpb.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://swv.pengpengdd.cyou

[C10] 变量作用域
来源：http://hqk.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xjk.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qij.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://own.fzhhl.top

TS:   同 JS
来源：http://ybj.tian-w.cn

Java: 方法内为块级作用域
来源：http://bzq.zhengqikj.top

Go:   花括号块级作用域
来源：http://vmw.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rrx.yonumen.top

C#:   块级作用域
来源：http://zql.xuanzx.com

[C11] 模块导入与导出
来源：http://hwt.zdbjq.cn

Py:   from module import func
来源：http://aid.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kul.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ldc.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hlq.cqqwz.cn

Java: import java.util.List;
来源：http://ois.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://swm.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://rqn.yanxiufei.cn

C#:   using System.Text;
来源：http://aab.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://hrl.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://xts.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://ika.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://whs.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://kvf.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oya.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://fcg.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://cqo.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gcy.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://aig.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://upu.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gup.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jem.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jto.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://sid.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://mzg.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bxd.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://czb.havefunace.top

[C14] 泛型函数
来源：http://fib.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ylb.birdmap.top

PHP:  // 无泛型
来源：http://ojz.yj202588.top

JS:   // 无泛型
来源：http://sam.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mun.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://axk.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hxy.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://nhb.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wkr.shuidangran.top

[C15] 解构 / 展开参数
来源：http://wdx.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fjg.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://uyq.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uui.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rhe.redwolf501.top

Java: // 无解构
来源：http://yxk.gzhubu.top

Go:   // 无解构
来源：http://lst.sjlbkw.cn

Ruby: a, b = pair
来源：http://faq.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://izw.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://qfe.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zdj.nanxinkj.top

PHP:  // 无重载
来源：http://tre.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bbx.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://zcx.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cup.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://ydf.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://plx.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eas.bbcook.cn

================================================================================
来源：http://kbt.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://rnv.hammf.cn

================================================================================
来源：http://cak.tanke756.top

[D01] 创建数组 / 列表
来源：http://tpv.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://inl.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qlx.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gkk.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rur.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wes.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://evg.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://amz.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kvh.redwolf501.top

[D02] 追加元素到末尾
来源：http://roq.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ark.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mab.fengsongda.top

JS:   arr.push(4);
来源：http://yxg.bbcook.cn

TS:   arr.push(4);
来源：http://qxx.hongshengwenyu.top

Java: list.add(4);
来源：http://uzd.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://gij.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://whn.zdbjq.cn

C#:   list.Add(4);
来源：http://pgp.316326.xyz


<!-- 参考信息 -->