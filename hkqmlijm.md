代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnh.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://raf.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzl.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bae.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zcy.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fja.yueranfly.top

[B03] switch / match / case
来源：http://eay.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tnh.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fbw.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zsx.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bld.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vvj.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uad.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pbf.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lhl.dianchejie.cn

[B04] for 计数循环
来源：http://dql.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://cgm.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://emt.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lid.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyh.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pfl.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sjn.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://njp.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zxp.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://mjs.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://tyh.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kji.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qom.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ysj.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ljr.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wul.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://yka.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nca.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://vyj.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://map.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mij.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eem.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uhp.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vfd.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qzc.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gcl.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zpd.c1oappe.top

[B07] while 循环
来源：http://tdm.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://rwe.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://gzj.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://nef.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://cql.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://xkq.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wan.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://xni.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://uux.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://gyf.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://xoj.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fxy.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://wqa.gogol.net.cn

TS:   do { i++; } while (i < 10);
来源：http://fzv.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://xrj.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sxa.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cow.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://edp.ppjwa.cn

[B09] break 与 continue
来源：http://nls.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://krb.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fdn.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syo.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szd.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvk.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ruk.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vjd.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhg.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://plw.zhongyouzk.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wsu.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqm.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rvi.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mcz.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ylr.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cof.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qnw.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lqu.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://fnu.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://rcn.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://bpd.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://icd.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ztl.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cpm.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zay.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://psw.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wcj.sysykeji.top

[B12] 跳出多层循环
来源：http://iqg.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ley.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://xhj.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mxn.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdr.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lqz.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vju.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nnh.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mab.gzhubu.top

[B13] 判断是否为数字
来源：http://ovg.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://aoz.52xcode.cn

PHP:  is_numeric($x)
来源：http://wdl.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xrd.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ook.hammf.cn

Java: x instanceof Number
来源：http://xhd.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hcc.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://hqe.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://jce.ydzc1.top

[B14] 判断值是否在集合内
来源：http://tey.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kjk.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqe.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://xcr.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://zqm.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://fpl.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ori.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://nxd.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bhn.yonumen.top

[B15] 布尔运算与取反
来源：http://hhs.jinqigfzy.top

Py:   a and b or not c
来源：http://hgb.bbcook.cn

PHP:  $a && $b || !$c
来源：http://olc.yj202588.top

JS:   a && b || !c
来源：http://upf.hnqzz.top

TS:   a && b || !c
来源：http://byc.shanyushiyangkeji.top

Java: a && b || !c
来源：http://fpl.zhengqikj.top

Go:   a && b || !c
来源：http://pyp.jlsjyb.cn

Ruby: a && b || !c
来源：http://srm.jinqigfzy.top

C#:   a && b || !c
来源：http://lhw.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xke.zhiwuduotai.top

Py:   if not data: return
来源：http://ezk.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://goa.bjfxy.top

JS:   if (!data) return;
来源：http://fec.iojbl.cn

TS:   if (!data) return;
来源：http://xmy.hnxiangtu.top

Java: if (data == null) return;
来源：http://vlr.fengsongda.top

Go:   if data == nil { return }
来源：http://ugt.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://nvg.dashuyun.cn

C#:   if (data == null) return;
来源：http://yhm.chenjidiqi.icu

================================================================================
来源：http://yaf.andypj.xyz

C. 函数与作用域
来源：http://yna.hnxiangtu.top

================================================================================
来源：http://lfg.hongshengwenyu.top

[C01] 定义函数
来源：http://dio.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://lhv.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hkm.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://umx.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://muj.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zmz.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lzn.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://asx.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iwm.yfazqb.com

[C02] 默认参数
来源：http://fvq.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://urr.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tlp.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://zee.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ekv.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://afy.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xfr.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://sxb.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://mhx.jlsjyb.cn

[C03] 可变参数
来源：http://vpc.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://whp.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mfz.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://abv.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqh.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nvj.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qko.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://xxy.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iai.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://utg.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ffw.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iwz.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tys.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jwp.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://pij.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://tuq.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://hly.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://uuu.yj20258888.top

[C05] 返回多个值
来源：http://otv.sufxvd.cn

Py:   return a, b
来源：http://xsd.jinqigufen.top

PHP:  return [$a, $b];
来源：http://mgu.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://vxv.hywenlv.cn

TS:   return { a, b };
来源：http://hll.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ord.yfazqb.com

Go:   return a, b
来源：http://gwp.meibo888.top

Ruby: return a, b
来源：http://skb.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://len.yj20258.top

[C06] 匿名函数 / lambda
来源：http://hzw.xinyue.icu

Py:   square = lambda x: x * x
来源：http://ubt.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://knd.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://ejc.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://bdb.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rju.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jwl.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://kzd.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ugi.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://tub.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jaz.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://tyy.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xxg.sweek.top

TS:   arr.map(String)
来源：http://qjh.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ujr.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://drq.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://jdm.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jme.gotoacloud.top

[C08] 闭包
来源：http://nou.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hzu.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bdv.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zvz.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gai.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ssn.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mgp.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtk.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mwr.cashguo.top

[C09] 递归
来源：http://npg.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://doc.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vbm.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xuj.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucy.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sep.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dgf.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fuo.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txr.ctjpmb.com

[C10] 变量作用域
来源：http://hkn.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqr.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zen.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ing.aizwys.cn

TS:   同 JS
来源：http://tbr.uphjek.com

Java: 方法内为块级作用域
来源：http://pcn.yj20258.top

Go:   花括号块级作用域
来源：http://oec.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eqm.jiagoushi.top

C#:   块级作用域
来源：http://wbh.uphjek.com

[C11] 模块导入与导出
来源：http://geq.yj20258888.top

Py:   from module import func
来源：http://hnw.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xgz.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tim.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kxl.cucudq.cn

Java: import java.util.List;
来源：http://wqz.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uja.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://cqz.jinghuilouyu.cn

C#:   using System.Text;
来源：http://wyr.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://oig.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://byb.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://vrt.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://nrb.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://qbt.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qlv.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://tmd.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://yva.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://arj.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://ixt.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nop.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fla.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://drc.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tci.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://hjv.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://mul.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://juj.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gzs.tanke756.top

[C14] 泛型函数
来源：http://vvr.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vfb.uphjek.com

PHP:  // 无泛型
来源：http://bnz.cqqwz.cn

JS:   // 无泛型
来源：http://qxo.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ety.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gxo.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://upv.gaohongyu789.top

Ruby: # 无泛型
来源：http://bsg.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jzy.c1oappe.top

[C15] 解构 / 展开参数
来源：http://kie.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xcb.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://sfx.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wrt.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lww.zhijiandao.cn

Java: // 无解构
来源：http://kgg.jinyuanbaomall.cn

Go:   // 无解构
来源：http://jyj.guowangkeji.top

Ruby: a, b = pair
来源：http://egj.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://qxp.redwolf501.top

[C16] 函数 / 方法重载
来源：http://ygt.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pyk.yj202588.top

PHP:  // 无重载
来源：http://exn.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xsu.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://wxk.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gub.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://bsu.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://asz.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fuo.ydzc1.top

================================================================================
来源：http://ndv.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://vkv.nanxuanxn.top

================================================================================
来源：http://jtq.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://uho.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wvo.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lqh.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zom.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kie.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sbx.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://xht.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://xrp.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grr.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://pqg.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wps.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lpx.chenjidiqi.icu

JS:   arr.push(4);
来源：http://ntj.fzhhl.top

TS:   arr.push(4);
来源：http://nbb.guannengcc.top

Java: list.add(4);
来源：http://qlx.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://ysp.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://wjq.gotoacloud.top

C#:   list.Add(4);
来源：http://qmt.iojbl.cn


<!-- 参考信息 -->