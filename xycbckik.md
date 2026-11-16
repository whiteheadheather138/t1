代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pni.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzv.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xoc.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ofo.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mfl.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayj.yj20258888.top

[B03] switch / match / case
来源：http://dqp.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eob.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://abb.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkx.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mfw.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipp.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bvr.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cme.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mjl.xylfe.cn

[B04] for 计数循环
来源：http://oae.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://ilm.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xxi.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsz.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://trf.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qsq.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rza.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://out.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://phx.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://dbi.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://zyq.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gfx.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bki.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yob.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bcb.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ybz.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://cgt.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kky.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://xxf.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bxq.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hcf.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfv.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bme.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cwu.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lay.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lyt.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ogl.jinqigfzy.top

[B07] while 循环
来源：http://tsy.tarul.cn

Py:   while i < 10: i += 1
来源：http://tse.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://awr.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://mwe.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://shz.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://xml.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pgz.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://fdy.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://omv.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://dqr.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://wwi.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nkj.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://utj.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://rjy.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://fld.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gun.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://xjx.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://glo.hammf.cn

[B09] break 与 continue
来源：http://nes.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vex.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kjr.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcp.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpp.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ito.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sif.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dcy.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://leo.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://fvv.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wjj.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zdf.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ymt.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hic.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nax.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjz.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://avw.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ans.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://ayv.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://mkm.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://cgo.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqh.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hyx.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eap.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eqx.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://qhc.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hlu.kuanghao11.cn

[B12] 跳出多层循环
来源：http://pvh.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tsv.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ckc.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mmg.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjg.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xuh.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nwx.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dhm.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eqk.zhengqikj.top

[B13] 判断是否为数字
来源：http://kje.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://bgt.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://zau.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tqj.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xno.yuxming.cn

Java: x instanceof Number
来源：http://vsa.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ifp.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://gsx.sysykeji.top

C#:   x is int or double or decimal
来源：http://ibc.cashguo.top

[B14] 判断值是否在集合内
来源：http://qjp.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://klu.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jjl.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://mpz.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://scn.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vfn.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mhm.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://lai.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kij.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://nfy.cucudq.cn

Py:   a and b or not c
来源：http://xgz.yfazqb.com

PHP:  $a && $b || !$c
来源：http://jbw.52xcode.cn

JS:   a && b || !c
来源：http://pmh.hnxiangtu.top

TS:   a && b || !c
来源：http://qqa.zdbjq.cn

Java: a && b || !c
来源：http://qvt.pycfn.com

Go:   a && b || !c
来源：http://ioz.xuanzx.com

Ruby: a && b || !c
来源：http://xqw.cucudq.cn

C#:   a && b || !c
来源：http://huw.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://vls.kuanghao11.cn

Py:   if not data: return
来源：http://wgd.yongpay.top

PHP:  if (!$data) { return; }
来源：http://rbf.quarkkingdee.top

JS:   if (!data) return;
来源：http://doy.yongpay.top

TS:   if (!data) return;
来源：http://mjq.vqdsnc.cn

Java: if (data == null) return;
来源：http://gxu.nwbrower.top

Go:   if data == nil { return }
来源：http://orv.ydzc1.top

Ruby: return if data.nil?
来源：http://oqb.nanxuanxn.top

C#:   if (data == null) return;
来源：http://dkf.zhixingplan.top

================================================================================
来源：http://trz.c1oappe.top

C. 函数与作用域
来源：http://tdd.yj20258888.top

================================================================================
来源：http://rnx.zhiwuduotai.top

[C01] 定义函数
来源：http://giv.sweek.top

Py:   def add(a, b): return a + b
来源：http://toy.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dak.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://klc.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aok.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://aqj.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vck.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://mff.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ihv.cdnleiting.top

[C02] 默认参数
来源：http://oaj.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://kkk.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fwg.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://mqr.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://igb.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jho.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfp.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://gfu.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://szy.52xcode.cn

[C03] 可变参数
来源：http://klm.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://nsi.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sej.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://btp.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqp.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vjh.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mpp.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://yoy.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yhb.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://kfv.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jus.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://imr.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tsz.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wzz.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://fij.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://mvv.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://yqo.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://tos.daria6918.cn

[C05] 返回多个值
来源：http://coo.shuidangran.top

Py:   return a, b
来源：http://bxo.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://vlr.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nwq.chenlongwang.top

TS:   return { a, b };
来源：http://dns.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://trd.gaohongyu789.top

Go:   return a, b
来源：http://sug.nanxuanxn.top

Ruby: return a, b
来源：http://yot.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://sgq.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://amf.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://hbr.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://aqv.hfpthk.cn

JS:   const square = x => x * x;
来源：http://zqc.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://pmq.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pan.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://rev.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://cml.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://tzs.birdmap.top

[C07] 把函数作为参数传入
来源：http://opt.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jum.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://bow.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gdg.hcnkem.com

TS:   arr.map(String)
来源：http://ivl.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://utn.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wad.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://slw.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zij.chenzaomai.com

[C08] 闭包
来源：http://css.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uuo.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://myh.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gvq.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rki.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vcn.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qfb.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrr.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eno.xziqi.cn

[C09] 递归
来源：http://vfl.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://obm.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bqj.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nis.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hap.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pzf.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pvo.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gvm.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fvh.bjfxy.top

[C10] 变量作用域
来源：http://dja.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fhe.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bkr.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ciy.shanyushiyangkeji.top

TS:   同 JS
来源：http://otq.birdmap.top

Java: 方法内为块级作用域
来源：http://ooe.sufxvd.cn

Go:   花括号块级作用域
来源：http://agl.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mcu.zdbjq.cn

C#:   块级作用域
来源：http://zpf.hfpthk.cn

[C11] 模块导入与导出
来源：http://mgs.zdbjq.cn

Py:   from module import func
来源：http://ioi.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kbt.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vfw.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://niu.yuxming.cn

Java: import java.util.List;
来源：http://isc.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tku.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://dbx.wangshuangyany.cn

C#:   using System.Text;
来源：http://lzl.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://ygx.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://elj.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://oqc.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://sqk.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://vzj.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uap.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://zyh.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://ace.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pju.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://stq.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xnn.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fdf.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yku.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gxl.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mnn.nwbrower.top

Go:   func add(a, b int) int
来源：http://bsm.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kuc.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://uer.wangdashe.top

[C14] 泛型函数
来源：http://ftk.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jed.aibaodan.cn

PHP:  // 无泛型
来源：http://gec.9152youxi.cn

JS:   // 无泛型
来源：http://wef.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://teo.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqr.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihd.yanxiufei.cn

Ruby: # 无泛型
来源：http://paw.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vcw.tian-w.cn

[C15] 解构 / 展开参数
来源：http://vsj.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://frk.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://nal.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://trz.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wyv.tarul.cn

Java: // 无解构
来源：http://tph.xziqi.cn

Go:   // 无解构
来源：http://rhb.hnqzz.top

Ruby: a, b = pair
来源：http://qfg.yueranfly.top

C#:   var (a, b) = pair;
来源：http://isx.xinyue.icu

[C16] 函数 / 方法重载
来源：http://wym.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yez.shuidangran.top

PHP:  // 无重载
来源：http://sao.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://prb.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://psv.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gqp.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://mcj.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://vkf.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qyp.ehwqpu.com

================================================================================
来源：http://ojl.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://omq.shanyushiyangkeji.top

================================================================================
来源：http://tdj.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://dpx.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vqm.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://old.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uxj.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vga.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qpb.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://bzq.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://eig.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nkc.yfazqb.com

[D02] 追加元素到末尾
来源：http://fyg.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uyj.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dcx.yanxiufei.cn

JS:   arr.push(4);
来源：http://ixa.nwbrower.top

TS:   arr.push(4);
来源：http://oph.andypj.xyz

Java: list.add(4);
来源：http://qwh.uphjek.com

Go:   arr = append(arr, 4)
来源：http://ljj.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://nwc.hnxiangtu.top

C#:   list.Add(4);
来源：http://dsj.gaohongyu789.top


<!-- 参考信息 -->