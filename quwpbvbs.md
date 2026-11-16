代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wqs.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuy.zhixingplan.top

[B03] switch / match / case
来源：http://ons.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yhl.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vcx.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qst.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apq.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://biz.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zul.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pbb.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oyq.hysaishi.cn

[B04] for 计数循环
来源：http://qan.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://jdv.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qet.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqm.nanxuanxn.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://whu.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://odd.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hgl.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://tlv.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tjg.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://zjg.smart0.xyz

Py:   for item in arr: print(item)
来源：http://drt.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://srz.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fcm.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gcd.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tui.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zyl.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://gxm.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ygp.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://jya.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://snp.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mrl.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqy.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xpg.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cls.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tbn.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnm.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://asd.bjfxy.top

[B07] while 循环
来源：http://szi.yj202588.top

Py:   while i < 10: i += 1
来源：http://arq.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pbh.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://oku.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://rzf.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://byr.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://imn.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://tdg.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://wdu.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://hpo.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://kqk.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wot.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://ato.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://eag.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://iic.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fwu.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://alk.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://rdn.dianchejie.cn

[B09] break 与 continue
来源：http://aqt.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fzy.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xfb.feifeiyinyue.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzh.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://enm.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdq.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://muy.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aad.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxa.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://gkf.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ktv.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eyw.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ieq.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ynu.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ihs.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ggb.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iit.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rcf.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://ach.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://lyq.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://ovn.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qok.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwx.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xic.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nfe.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://qre.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tih.hnxiangtu.top

[B12] 跳出多层循环
来源：http://dfl.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://osm.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vay.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ssp.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jfk.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rve.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ftm.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qen.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yig.chenzaomai.com

[B13] 判断是否为数字
来源：http://xtk.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://jdy.nanxinkj.top

PHP:  is_numeric($x)
来源：http://blb.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://axc.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rza.tianlin.xyz

Java: x instanceof Number
来源：http://ter.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xlq.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://fpg.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://anz.yj20258888.top

[B14] 判断值是否在集合内
来源：http://yvw.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mhh.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jyu.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://shm.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://gcd.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://swt.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jvw.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://jvy.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gmd.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://bju.svipenyu.cn

Py:   a and b or not c
来源：http://jac.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://gzf.hfpthk.cn

JS:   a && b || !c
来源：http://ilk.hysaishi.cn

TS:   a && b || !c
来源：http://juj.c1oappe.top

Java: a && b || !c
来源：http://lck.yonumen.top

Go:   a && b || !c
来源：http://rcn.wangshuangyany.cn

Ruby: a && b || !c
来源：http://ulf.gogol.net.cn

C#:   a && b || !c
来源：http://yjv.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cua.pycfn.com

Py:   if not data: return
来源：http://iqn.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://szm.yj202588.top

JS:   if (!data) return;
来源：http://zqw.0kj1m.cn

TS:   if (!data) return;
来源：http://wic.sysykeji.top

Java: if (data == null) return;
来源：http://qjk.kuanghao11.cn

Go:   if data == nil { return }
来源：http://snl.yj20258888.top

Ruby: return if data.nil?
来源：http://vyi.yuanzhike.top

C#:   if (data == null) return;
来源：http://pia.ppjwa.cn

================================================================================
来源：http://kxj.yj20258888.top

C. 函数与作用域
来源：http://pol.shanyushiyangtech.top

================================================================================
来源：http://vmb.ydjk.org.cn

[C01] 定义函数
来源：http://pqy.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://rtx.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lyb.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://xhj.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exp.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ksl.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jbh.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://zyh.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jkk.aibaodan.cn

[C02] 默认参数
来源：http://zuu.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://qvk.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://icq.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://wcm.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tod.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vhj.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jnf.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://zyi.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://gje.tarul.cn

[C03] 可变参数
来源：http://srr.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://pwb.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sef.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dnr.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://psl.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tww.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tyk.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://jmj.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cxd.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://fvc.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vfm.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ozc.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zee.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdv.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://tzl.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://nvb.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://ubh.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://kkg.wangdashe.top

[C05] 返回多个值
来源：http://dqp.ywan-chungtsiang.top

Py:   return a, b
来源：http://shm.52xcode.cn

PHP:  return [$a, $b];
来源：http://mhq.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dhu.gotoacloud.top

TS:   return { a, b };
来源：http://cde.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hgb.daria6918.cn

Go:   return a, b
来源：http://tmn.xuetiantiany.cn

Ruby: return a, b
来源：http://dbh.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://zin.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://gzj.smart0.xyz

Py:   square = lambda x: x * x
来源：http://ifu.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zms.daxiang520.top

JS:   const square = x => x * x;
来源：http://xha.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://jem.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kuc.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mwq.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://wsi.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oil.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://nve.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mcn.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ypm.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gfm.bbcook.cn

TS:   arr.map(String)
来源：http://kny.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vub.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jgz.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://toi.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lot.chenjidiqi.icu

[C08] 闭包
来源：http://gfq.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sxv.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wst.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://omj.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rvf.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ihf.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vry.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tsa.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pun.fengsongda.top

[C09] 递归
来源：http://put.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyr.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pwa.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dlu.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vyl.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xsn.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ehw.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tsx.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ayk.aizwys.cn

[C10] 变量作用域
来源：http://tzj.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nmz.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tnt.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iuh.uphjek.com

TS:   同 JS
来源：http://snp.zhixingplan.top

Java: 方法内为块级作用域
来源：http://utk.yj20258888.top

Go:   花括号块级作用域
来源：http://tkn.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wxn.fanxiaobao.xyz

C#:   块级作用域
来源：http://cyl.mhx1999.top

[C11] 模块导入与导出
来源：http://yzc.fengsongda.top

Py:   from module import func
来源：http://erb.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://prb.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzq.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mii.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://unv.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ovv.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://wdd.sweek.top

C#:   using System.Text;
来源：http://tme.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://wld.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://lri.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://fvk.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://sff.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://lge.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jrl.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://jtl.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://ufe.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://taz.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://axe.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wdz.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pwu.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mwq.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rdu.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ugz.ehwqpu.com

Go:   func add(a, b int) int
来源：http://ayk.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ekt.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://jye.jqgufenzy.top

[C14] 泛型函数
来源：http://nnu.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yla.cucudq.cn

PHP:  // 无泛型
来源：http://qgl.cheryme.top

JS:   // 无泛型
来源：http://ijh.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fsa.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://arf.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gqr.gotoacloud.top

Ruby: # 无泛型
来源：http://bel.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncx.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://wht.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jer.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://kqw.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mlf.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://luv.chenjidiqi.icu

Java: // 无解构
来源：http://hfz.svipenyu.cn

Go:   // 无解构
来源：http://hue.chenzaomai.com

Ruby: a, b = pair
来源：http://nlc.nwbrower.top

C#:   var (a, b) = pair;
来源：http://cgj.cashguo.top

[C16] 函数 / 方法重载
来源：http://egc.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://amw.gzhubu.top

PHP:  // 无重载
来源：http://mkk.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vfs.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://hxu.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fpi.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://xcg.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://tcx.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ymq.hfpthk.cn

================================================================================
来源：http://cri.havefunace.top

D. 数组 / 列表 / 集合
来源：http://qmn.sjlbkw.cn

================================================================================
来源：http://ouk.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://cld.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bfz.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cmd.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://unb.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kfi.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nge.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://eau.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://ylf.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofb.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://aci.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ecq.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nrv.svipenyu.cn

JS:   arr.push(4);
来源：http://lus.gaohongyu789.top

TS:   arr.push(4);
来源：http://nlu.guannengcc.top

Java: list.add(4);
来源：http://upa.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://fyg.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://pgp.daria6918.cn

C#:   list.Add(4);
来源：http://rbv.c1oappe.top

[D03] 在指定位置插入元素
来源：http://gix.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://zoo.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gph.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xka.quarkkingdee.top


<!-- 参考信息 -->