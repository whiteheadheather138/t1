代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://szr.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oll.uphjek.com

[B03] switch / match / case
来源：http://zgm.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rce.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gfl.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqx.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qjt.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://phc.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fts.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ecn.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rjw.svipenyu.cn

[B04] for 计数循环
来源：http://oco.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://oia.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tmg.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uij.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hil.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://muj.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fwk.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://kne.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yjp.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://uxp.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://wzy.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yxs.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tvn.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yha.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wkm.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ddn.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://atd.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ptd.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://dnf.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rig.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://anu.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lzq.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pli.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xmd.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eko.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fxl.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jhp.0kj1m.cn

[B07] while 循环
来源：http://jie.uphjek.com

Py:   while i < 10: i += 1
来源：http://gzp.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://vah.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://ley.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://fpf.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://hpp.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cpm.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://dgw.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://wfh.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://jil.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://osr.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://adr.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://ktc.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://nhw.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://bsz.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://quy.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://alq.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://ihr.nanxuanxn.top

[B09] break 与 continue
来源：http://bkm.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://leo.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ayy.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tda.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://geb.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnx.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qbm.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vui.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzy.yj202588.top

[B10] 遍历同时拿索引
来源：http://zid.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nox.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zey.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sct.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://adh.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://frl.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lyq.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ieg.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fmt.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://emn.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://hvx.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://vnz.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qxi.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ytv.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ovv.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://evh.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://zif.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ovo.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://orv.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ilt.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://few.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://los.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kcy.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bak.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsi.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://djo.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xuv.xylfe.cn

[B13] 判断是否为数字
来源：http://hje.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://mpd.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://awm.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pjt.tianlin.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qrt.ydzc1.top

Java: x instanceof Number
来源：http://hvw.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jea.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://ocn.chenlongwang.top

C#:   x is int or double or decimal
来源：http://ebq.sysykeji.top

[B14] 判断值是否在集合内
来源：http://rdq.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://maj.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tyq.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://wri.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://ivf.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gql.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gnh.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://mqe.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cfh.zycfv.cn

[B15] 布尔运算与取反
来源：http://typ.xuanzx.com

Py:   a and b or not c
来源：http://wmg.daria6918.cn

PHP:  $a && $b || !$c
来源：http://qra.hnqzz.top

JS:   a && b || !c
来源：http://dfi.hongshengwenyu.top

TS:   a && b || !c
来源：http://myi.aibaodan.cn

Java: a && b || !c
来源：http://ncj.hysaishi.cn

Go:   a && b || !c
来源：http://rtz.316326.xyz

Ruby: a && b || !c
来源：http://wvc.havefunace.top

C#:   a && b || !c
来源：http://efr.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uap.shanyushiyangkeji.top

Py:   if not data: return
来源：http://oie.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://gdx.yonumen.top

JS:   if (!data) return;
来源：http://kft.yanxiufei.cn

TS:   if (!data) return;
来源：http://ykc.svipenyu.cn

Java: if (data == null) return;
来源：http://pbt.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://iiw.c1oappe.top

Ruby: return if data.nil?
来源：http://flu.hammf.cn

C#:   if (data == null) return;
来源：http://uya.fanxiaobao.xyz

================================================================================
来源：http://yvj.nanxinkj.top

C. 函数与作用域
来源：http://pnx.zhaomingkeji.xyz

================================================================================
来源：http://xiz.yuanzhike.top

[C01] 定义函数
来源：http://anl.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://mdy.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ipf.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://fzt.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vkb.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://idx.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xrb.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://yfs.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://egd.hongshengwenyu.top

[C02] 默认参数
来源：http://whm.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://xan.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ibz.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://tvj.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://zzc.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://omg.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://czq.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://kdp.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://vik.yfazqb.com

[C03] 可变参数
来源：http://ima.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://bar.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ild.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tbu.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://quq.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hwn.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qfz.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://hjf.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vui.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://dpv.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mih.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eys.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aec.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yue.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://khs.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://uay.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://agi.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://qho.yfazqb.com

[C05] 返回多个值
来源：http://hsz.xylfe.cn

Py:   return a, b
来源：http://ieo.yueranfly.top

PHP:  return [$a, $b];
来源：http://lgr.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wdn.xziqi.cn

TS:   return { a, b };
来源：http://czg.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mnz.zhengqikj.top

Go:   return a, b
来源：http://hgd.zycfv.cn

Ruby: return a, b
来源：http://chx.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://czp.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://zce.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://rcs.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ryt.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://fnh.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://mrk.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ynn.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://hrr.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://kms.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://lsm.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://nle.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zgx.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ojf.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uro.aizwys.cn

TS:   arr.map(String)
来源：http://eet.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hel.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xbe.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://pei.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://xok.hnqzz.top

[C08] 闭包
来源：http://wtu.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://syj.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ntb.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vkd.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aec.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gbv.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://psf.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hka.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://srz.cqqwz.cn

[C09] 递归
来源：http://ypt.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jux.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lfg.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lab.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gck.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gbg.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lvb.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://soz.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nfr.yongpay.top

[C10] 变量作用域
来源：http://dpl.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xst.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tir.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rrc.yongpay.top

TS:   同 JS
来源：http://itf.dashuyun.cn

Java: 方法内为块级作用域
来源：http://qac.iojbl.cn

Go:   花括号块级作用域
来源：http://bph.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nza.dashuyun.cn

C#:   块级作用域
来源：http://vsu.sufxvd.cn

[C11] 模块导入与导出
来源：http://cip.birdmap.top

Py:   from module import func
来源：http://sog.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sbn.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://pii.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nsz.yongpay.top

Java: import java.util.List;
来源：http://saa.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://doh.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://den.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://pei.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://hqf.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://lfg.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://yui.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://mvw.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://bwy.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://whj.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://ktj.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://zdv.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://nrq.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://sjy.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ykn.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zsw.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ssq.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hoi.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://emy.yvedp.cn

Go:   func add(a, b int) int
来源：http://xtb.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mas.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gwg.hnxiangtu.top

[C14] 泛型函数
来源：http://ukm.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cwd.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://jev.shzxlz.cn

JS:   // 无泛型
来源：http://iok.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ojz.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kjv.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ttj.zhengqikj.top

Ruby: # 无泛型
来源：http://lfo.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vac.xylfe.cn

[C15] 解构 / 展开参数
来源：http://oak.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ibi.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://mlk.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vef.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yex.yj20258888.top

Java: // 无解构
来源：http://dpj.birdmap.top

Go:   // 无解构
来源：http://zgi.dashuyun.cn

Ruby: a, b = pair
来源：http://vno.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://twi.daria6918.cn

[C16] 函数 / 方法重载
来源：http://hvi.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zrv.cqqwz.cn

PHP:  // 无重载
来源：http://zri.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dsq.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://eft.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tvh.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://whb.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://ieu.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lss.tian-w.cn

================================================================================
来源：http://cjg.yj20258.top

D. 数组 / 列表 / 集合
来源：http://ojv.dianchejie.cn

================================================================================
来源：http://kja.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://xuy.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xen.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lcz.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blx.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oru.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pmr.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://cef.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://uhn.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qqj.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://jwq.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://axw.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lus.zdqjudy.top

JS:   arr.push(4);
来源：http://zwn.mhx1999.top

TS:   arr.push(4);
来源：http://mrr.jinghuilouyu.cn

Java: list.add(4);
来源：http://nme.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://lxk.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://zbt.yuxming.cn

C#:   list.Add(4);
来源：http://sxz.mhx1999.top

[D03] 在指定位置插入元素
来源：http://tmb.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://nrr.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pgy.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hmn.nanxinkj.top


<!-- 参考信息 -->