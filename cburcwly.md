代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxt.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zna.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxw.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jrw.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eld.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jww.zhengqikj.top

[B03] switch / match / case
来源：http://way.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lvu.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ltw.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xwf.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjb.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vpl.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://txs.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ptb.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zlq.jqgfzy.top

[B04] for 计数循环
来源：http://tiw.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://ywd.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://csg.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eqq.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mdm.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://igd.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hzz.cheryme.top

Ruby: 10.times { |i| puts i }
来源：http://fjy.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uxp.tanke756.top

[B05] 遍历数组 / 列表
来源：http://ymg.yueranfly.top

Py:   for item in arr: print(item)
来源：http://iwg.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jbe.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sfz.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cgm.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gcj.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qmb.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://yrx.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zdd.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://tve.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xxb.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efb.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zup.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hiu.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ngn.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zgf.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://std.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jeh.hammf.cn

[B07] while 循环
来源：http://pjc.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://bhx.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://hyu.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://aui.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://jhx.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://jqn.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqm.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://ocp.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://cht.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://efx.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://wpu.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://quq.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://dke.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://fof.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://jcp.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dce.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qnq.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://hls.sufxvd.cn

[B09] break 与 continue
来源：http://tnb.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lri.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ogk.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vct.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbg.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixd.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gql.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wow.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdg.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://clc.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vmc.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bpz.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yqb.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bqt.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fom.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohl.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ofb.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jyr.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://kji.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://jko.hammf.cn

PHP:  range(0, 10, 2);
来源：http://bok.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uzn.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebr.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bka.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lxz.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://wsh.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qod.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://nha.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lrk.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vuh.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xil.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://maj.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://umx.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tyg.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mph.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vct.gogol.net.cn

[B13] 判断是否为数字
来源：http://qjq.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://voj.yj20258888.top

PHP:  is_numeric($x)
来源：http://foe.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xtz.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sca.hfpthk.cn

Java: x instanceof Number
来源：http://yot.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pjc.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://sih.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://bqw.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://wzn.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eul.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://foh.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://nlk.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://jyy.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pgp.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bac.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://trd.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wso.dashuyun.cn

[B15] 布尔运算与取反
来源：http://ldi.zdbjq.cn

Py:   a and b or not c
来源：http://fdj.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://qti.ybcxt.top

JS:   a && b || !c
来源：http://aia.hongshengwenyu.top

TS:   a && b || !c
来源：http://esc.zhijiandao.cn

Java: a && b || !c
来源：http://mad.snrcjt.cn

Go:   a && b || !c
来源：http://nce.shuidangran.top

Ruby: a && b || !c
来源：http://xrb.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://nav.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vtz.wangdashe.top

Py:   if not data: return
来源：http://xde.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://ypc.yangfankeji.com

JS:   if (!data) return;
来源：http://wht.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://wdb.ppjwa.cn

Java: if (data == null) return;
来源：http://fen.hywenlv.cn

Go:   if data == nil { return }
来源：http://wxf.yj20258.top

Ruby: return if data.nil?
来源：http://ojc.yongpay.top

C#:   if (data == null) return;
来源：http://ilu.yj20258888.top

================================================================================
来源：http://hfh.birdmap.top

C. 函数与作用域
来源：http://wwf.chenzaomai.com

================================================================================
来源：http://qpl.hysaishi.cn

[C01] 定义函数
来源：http://nhz.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://twn.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szb.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://vmx.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zsu.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zto.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://obg.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://vxr.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcn.yangfankeji.com

[C02] 默认参数
来源：http://wpb.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://ajt.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lzu.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://jqr.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gzi.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zer.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sdq.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://eso.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://ckk.gotoacloud.top

[C03] 可变参数
来源：http://cwx.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://dia.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cti.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tyr.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wxu.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qxp.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gps.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://dzn.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://shk.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://mhr.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hmg.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vhz.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sye.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://boc.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://tqf.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://ikb.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://nys.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://qsz.bbcook.cn

[C05] 返回多个值
来源：http://pnc.yvedp.cn

Py:   return a, b
来源：http://rgv.birdmap.top

PHP:  return [$a, $b];
来源：http://nwh.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ivy.chenlongwang.top

TS:   return { a, b };
来源：http://kpq.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zmz.chenzaomai.com

Go:   return a, b
来源：http://tzb.chenlongwang.top

Ruby: return a, b
来源：http://fvm.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://fvw.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://wxj.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://ywc.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://slz.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://jlr.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://mmg.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qna.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://zef.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://wpb.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://zun.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://mzv.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pmm.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://ewu.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yhd.gotoacloud.top

TS:   arr.map(String)
来源：http://ilg.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rxw.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fdy.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://nkp.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ljt.hongshengwenyu.top

[C08] 闭包
来源：http://ndw.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qsf.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zkn.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dws.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jek.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kcn.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ahn.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://skq.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://htu.jinqigufen.top

[C09] 递归
来源：http://syi.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nie.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jew.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gzy.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yry.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rmf.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://suu.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dev.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdy.jinqigfzy.top

[C10] 变量作用域
来源：http://rid.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://azg.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryp.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jcy.cdnleiting.top

TS:   同 JS
来源：http://rio.tanke756.top

Java: 方法内为块级作用域
来源：http://mkx.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://iiw.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tzv.epnwcf.com

C#:   块级作用域
来源：http://iyx.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://vdu.cdnleiting.top

Py:   from module import func
来源：http://upa.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jaw.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qyc.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aak.hywenlv.cn

Java: import java.util.List;
来源：http://owh.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ijh.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://mrq.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://vwu.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://adl.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://haf.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://jvh.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://vgt.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://tvs.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kdw.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://pkr.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://osl.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ycg.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://trb.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xkl.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sei.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gyv.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ors.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://icr.jqgfzy.top

Go:   func add(a, b int) int
来源：http://okl.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qsx.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://gqr.zycfv.cn

[C14] 泛型函数
来源：http://ycm.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tsv.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://slx.jqgufenzy.top

JS:   // 无泛型
来源：http://nth.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sqo.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vcf.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rka.vehdjk.com

Ruby: # 无泛型
来源：http://koz.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iao.daria6918.cn

[C15] 解构 / 展开参数
来源：http://aqx.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vzn.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://hzn.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pxq.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wkf.cdnleiting.top

Java: // 无解构
来源：http://wff.hammf.cn

Go:   // 无解构
来源：http://xul.tianlin.xyz

Ruby: a, b = pair
来源：http://lac.sysykeji.top

C#:   var (a, b) = pair;
来源：http://zzz.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://jqc.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lsg.316326.xyz

PHP:  // 无重载
来源：http://tcf.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uey.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://oze.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dlb.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://nxe.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://qwj.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dkl.gaohongyu789.top

================================================================================
来源：http://gdy.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://xty.tian-w.cn

================================================================================
来源：http://poh.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://fjp.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lwm.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kkn.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ghw.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://htl.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kct.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://pfj.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://dvv.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sqw.fehbvm.com

[D02] 追加元素到末尾
来源：http://vol.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://psw.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddw.9152youxi.cn

JS:   arr.push(4);
来源：http://qbb.pengpengdd.cyou

TS:   arr.push(4);
来源：http://jte.316326.xyz

Java: list.add(4);
来源：http://jqa.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://xlx.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://qqr.gogol.net.cn

C#:   list.Add(4);
来源：http://uwn.quarkkingdee.top


<!-- 参考信息 -->