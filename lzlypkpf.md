代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aer.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dub.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mku.tarul.cn

[B04] for 计数循环
来源：http://oyt.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://ijw.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dyy.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bgw.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tfd.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://txp.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yit.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://exi.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vki.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://lyl.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://uip.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pyf.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yrd.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yml.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://djs.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kzg.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://vuw.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hcd.birdmap.top

[B06] 遍历字典 / 对象
来源：http://iid.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wvi.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ona.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlm.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igl.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zle.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rlh.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qwf.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://urn.jianghu66.top

[B07] while 循环
来源：http://xbc.jianghu66.top

Py:   while i < 10: i += 1
来源：http://ztc.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://upz.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://paf.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://auo.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://jlu.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngb.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://yqm.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://nqs.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://lry.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://acx.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aak.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://vax.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://wge.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://rdc.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bzn.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://ofn.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://wiw.yuxming.cn

[B09] break 与 continue
来源：http://fsb.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ole.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uxi.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fco.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bce.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubi.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vcj.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wwc.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqe.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://gja.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yoh.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://csa.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cvz.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vyu.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lnk.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zhn.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lrb.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xvh.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://nyn.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://hob.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://vov.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgv.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://buy.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jtd.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rqg.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://srw.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zyj.chenlongwang.top

[B12] 跳出多层循环
来源：http://stn.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vhl.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nwb.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://orp.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://shc.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ufb.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fra.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zby.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iqj.nanxuanxn.top

[B13] 判断是否为数字
来源：http://jzt.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://qly.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://zvv.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyw.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://voh.fehbvm.com

Java: x instanceof Number
来源：http://iap.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ghf.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://zej.cucudq.cn

C#:   x is int or double or decimal
来源：http://gcs.meibo888.top

[B14] 判断值是否在集合内
来源：http://nqx.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sod.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://erd.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://mxh.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://zwz.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dze.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qio.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ltl.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mfk.wangdashe.top

[B15] 布尔运算与取反
来源：http://bhg.316326.xyz

Py:   a and b or not c
来源：http://emn.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://qcz.shuidangran.top

JS:   a && b || !c
来源：http://wzx.cucudq.cn

TS:   a && b || !c
来源：http://kdq.0kj1m.cn

Java: a && b || !c
来源：http://fdv.sufxvd.cn

Go:   a && b || !c
来源：http://aho.snrcjt.cn

Ruby: a && b || !c
来源：http://kfd.zhiwuduotai.top

C#:   a && b || !c
来源：http://ion.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://dcn.jqgufenzy.top

Py:   if not data: return
来源：http://gmb.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://phg.andypj.xyz

JS:   if (!data) return;
来源：http://uqp.hysaishi.cn

TS:   if (!data) return;
来源：http://cnv.zhiwuduotai.top

Java: if (data == null) return;
来源：http://jha.yongpay.top

Go:   if data == nil { return }
来源：http://omg.jqgufenzy.top

Ruby: return if data.nil?
来源：http://jij.xziqi.cn

C#:   if (data == null) return;
来源：http://vce.fehbvm.com

================================================================================
来源：http://dal.tarul.cn

C. 函数与作用域
来源：http://vvo.fanxiaobao.xyz

================================================================================
来源：http://tgz.bjfxy.top

[C01] 定义函数
来源：http://qrs.hammf.cn

Py:   def add(a, b): return a + b
来源：http://uqu.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltm.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://nkh.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ycy.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://irv.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://enm.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://mjv.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://otq.sysykeji.top

[C02] 默认参数
来源：http://jbj.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://frb.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://muc.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://kfz.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://krd.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://npw.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://evh.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://bce.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://eti.zhengqikj.top

[C03] 可变参数
来源：http://kul.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://pqy.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lhf.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nip.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtt.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ojp.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ugh.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://ubl.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tow.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://iju.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tyo.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hni.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cso.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sre.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://dav.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://dpe.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://jwy.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://bfg.gaohongyu789.top

[C05] 返回多个值
来源：http://pet.xinyue.icu

Py:   return a, b
来源：http://owr.9152youxi.cn

PHP:  return [$a, $b];
来源：http://zye.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://czk.yj20258.top

TS:   return { a, b };
来源：http://yez.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zej.gotoacloud.top

Go:   return a, b
来源：http://keg.nanxuanxn.top

Ruby: return a, b
来源：http://ojh.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ztx.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://jdb.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://blc.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jvv.hfpthk.cn

JS:   const square = x => x * x;
来源：http://dwh.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://mco.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cxc.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://imx.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://jve.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oce.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://wik.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://too.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://nor.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uyp.chenlongwang.top

TS:   arr.map(String)
来源：http://cjn.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mxj.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tpd.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://lbg.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kof.ivvv.top

[C08] 闭包
来源：http://xws.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iue.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cfn.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dlv.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://avk.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://okd.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bpw.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xyr.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://thq.ydzc1.top

[C09] 递归
来源：http://euu.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pxm.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ktc.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltv.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://off.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xgj.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cra.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zqp.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qnb.bjfxy.top

[C10] 变量作用域
来源：http://kuf.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ipt.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fhi.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zlm.yuxming.cn

TS:   同 JS
来源：http://hsz.xylfe.cn

Java: 方法内为块级作用域
来源：http://gvo.sweek.top

Go:   花括号块级作用域
来源：http://fwh.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mmh.dashuyun.cn

C#:   块级作用域
来源：http://pfx.zhoulong.xyz

[C11] 模块导入与导出
来源：http://tcx.gzhubu.top

Py:   from module import func
来源：http://qqa.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://usa.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bdm.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://srx.birdmap.top

Java: import java.util.List;
来源：http://jud.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sng.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://hwi.sufxvd.cn

C#:   using System.Text;
来源：http://yhg.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://iwi.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://bni.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://suz.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://pqh.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://qtv.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rbw.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://lnt.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://rit.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vup.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://kak.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ygc.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sen.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mnb.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tov.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aqf.iojbl.cn

Go:   func add(a, b int) int
来源：http://ydu.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://glb.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vuj.hnqzz.top

[C14] 泛型函数
来源：http://idn.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://msm.cqqwz.cn

PHP:  // 无泛型
来源：http://rte.52xcode.cn

JS:   // 无泛型
来源：http://gym.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kuf.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://evj.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hya.andypj.xyz

Ruby: # 无泛型
来源：http://qsd.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xyo.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://hvd.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yix.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://zjl.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kqh.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ddj.tarul.cn

Java: // 无解构
来源：http://lov.ehwqpu.com

Go:   // 无解构
来源：http://wju.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://skj.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://kir.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://bub.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tsm.yvedp.cn

PHP:  // 无重载
来源：http://wwj.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ojm.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://xko.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xbn.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://esv.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://oeq.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://egd.vqdsnc.cn

================================================================================
来源：http://ovf.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://poo.gaohongyu789.top

================================================================================
来源：http://xwr.guannengcc.top

[D01] 创建数组 / 列表
来源：http://hia.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ord.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://moe.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nsj.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://phj.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ant.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://jmh.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://bdz.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lkv.gotoacloud.top

[D02] 追加元素到末尾
来源：http://ykx.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lfx.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://thk.jyoumei.cn

JS:   arr.push(4);
来源：http://qaa.zhengqikj.top

TS:   arr.push(4);
来源：http://yzp.yueranfly.top

Java: list.add(4);
来源：http://tfd.uphjek.com

Go:   arr = append(arr, 4)
来源：http://jdg.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://bhe.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://gvh.yongpay.top

[D03] 在指定位置插入元素
来源：http://umq.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://jpn.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://npe.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cdh.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://tcq.snrcjt.cn

Java: list.add(0, 0);
来源：http://zzs.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://ctl.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eus.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://ilk.ppjwa.cn

[D04] 删除元素
来源：http://inb.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pqg.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bom.zycfv.cn


<!-- 参考信息 -->