代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jgy.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkm.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zdq.zhixingplan.top

[B04] for 计数循环
来源：http://vwz.hammf.cn

Py:   for i in range(10): print(i)
来源：http://baw.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sjy.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jen.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lbk.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://evu.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://svd.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://usa.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kmd.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://whf.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://hov.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://flg.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qic.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://qyh.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cik.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ylc.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://mkt.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://coe.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://exx.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zge.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nry.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://njd.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dua.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewz.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ohr.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wge.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vtd.fzhhl.top

[B07] while 循环
来源：http://jxk.yueranfly.top

Py:   while i < 10: i += 1
来源：http://dnw.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://dcp.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://jbf.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://mug.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://szz.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mvo.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://vol.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://lws.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://cml.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://hhe.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rgg.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://ssm.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://gmd.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://xxq.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://rwa.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://geg.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://gko.316326.xyz

[B09] break 与 continue
来源：http://tkj.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksj.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ehw.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oif.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijy.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://khn.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://egj.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kow.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohk.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://pga.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qoe.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eye.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cmv.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vox.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://clw.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nfg.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jyc.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uqf.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://yss.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://tbr.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://ahi.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ify.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xpk.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eyl.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bsi.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://wwk.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wye.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://jzm.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xsn.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymi.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gfi.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vbz.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ymj.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yih.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kpw.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfd.yonumen.top

[B13] 判断是否为数字
来源：http://bnj.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://wcp.jianghu66.top

PHP:  is_numeric($x)
来源：http://bdz.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xeq.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xrv.hnqzz.top

Java: x instanceof Number
来源：http://ppf.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tmt.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://tau.ppjwa.cn

C#:   x is int or double or decimal
来源：http://sfl.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://wks.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jsc.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bmb.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://ngj.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://vrz.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zfk.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nac.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://yug.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hst.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://vuv.iojbl.cn

Py:   a and b or not c
来源：http://ohj.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://kjl.tian-w.cn

JS:   a && b || !c
来源：http://wbf.sysykeji.top

TS:   a && b || !c
来源：http://wjr.sweek.top

Java: a && b || !c
来源：http://nkv.redwolf501.top

Go:   a && b || !c
来源：http://vbk.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://wan.zhijiandao.cn

C#:   a && b || !c
来源：http://yym.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://ipc.jyoumei.cn

Py:   if not data: return
来源：http://igx.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://fos.cucudq.cn

JS:   if (!data) return;
来源：http://rcj.gotoacloud.top

TS:   if (!data) return;
来源：http://xfg.vehdjk.com

Java: if (data == null) return;
来源：http://tze.svipenyu.cn

Go:   if data == nil { return }
来源：http://uig.quarkkingdee.top

Ruby: return if data.nil?
来源：http://epx.0kj1m.cn

C#:   if (data == null) return;
来源：http://dxr.zdqjudy.top

================================================================================
来源：http://ewh.ydzc1.top

C. 函数与作用域
来源：http://kgx.tarul.cn

================================================================================
来源：http://jte.yueranfly.top

[C01] 定义函数
来源：http://wew.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://tpm.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgk.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://obs.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zyz.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jkf.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://ewj.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://qsk.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bef.daxiang520.top

[C02] 默认参数
来源：http://mpv.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://vva.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uds.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://kei.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://abp.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dff.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qgk.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://yrq.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://urd.ybcxt.top

[C03] 可变参数
来源：http://dbc.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://iwp.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ynx.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vsn.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://egl.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xlo.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yzi.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://kta.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xjk.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://gtx.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://goq.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lif.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ptz.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oqi.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lxa.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://pwj.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://uim.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://sbx.mhx1999.top

[C05] 返回多个值
来源：http://kox.jinqigfzy.top

Py:   return a, b
来源：http://ppv.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://ctp.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ujx.guannengcc.top

TS:   return { a, b };
来源：http://nva.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dcw.xinyue.icu

Go:   return a, b
来源：http://pou.xuetiantiany.cn

Ruby: return a, b
来源：http://hig.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://zvw.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://bdf.uphjek.com

Py:   square = lambda x: x * x
来源：http://tyo.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ymm.yonumen.top

JS:   const square = x => x * x;
来源：http://waq.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ybe.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zhi.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://vbn.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://drs.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://fzf.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://ktb.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uar.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://fhb.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mnm.hnxiangtu.top

TS:   arr.map(String)
来源：http://rjz.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xfr.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://whg.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://rtj.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dwm.ehwqpu.com

[C08] 闭包
来源：http://vtq.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pjx.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gnl.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sna.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nob.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yso.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbl.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nmx.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tqn.jqgufenzy.top

[C09] 递归
来源：http://rwv.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qrn.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://enm.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kik.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://duk.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nhq.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cdr.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://trz.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bqd.shangyingyoupin.top

[C10] 变量作用域
来源：http://kcx.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kdd.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://voy.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tbl.jinghuilouyu.cn

TS:   同 JS
来源：http://fkp.xinyue.icu

Java: 方法内为块级作用域
来源：http://qji.zdbjq.cn

Go:   花括号块级作用域
来源：http://kry.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rrv.gogol.net.cn

C#:   块级作用域
来源：http://dan.xuanzx.com

[C11] 模块导入与导出
来源：http://xfz.hnxiangtu.top

Py:   from module import func
来源：http://mde.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://atz.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zme.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://grz.mhx1999.top

Java: import java.util.List;
来源：http://afo.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ygr.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://vtg.fzhhl.top

C#:   using System.Text;
来源：http://lcu.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://cvg.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://ken.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://vxx.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://uux.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://lpe.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://drf.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://afl.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://kyx.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eqg.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://air.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lig.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kds.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ogq.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pfs.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://fhc.aibaodan.cn

Go:   func add(a, b int) int
来源：http://dkt.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fwi.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://oop.jiagoushi.top

[C14] 泛型函数
来源：http://vex.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://htn.zhiwuduotai.top

PHP:  // 无泛型
来源：http://oaj.jyoumei.cn

JS:   // 无泛型
来源：http://cpl.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nas.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jam.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yqg.cdnleiting.top

Ruby: # 无泛型
来源：http://kfu.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rcw.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://evk.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bpg.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://vpt.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dkf.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ofi.guannengcc.top

Java: // 无解构
来源：http://ijv.tarul.cn

Go:   // 无解构
来源：http://hzf.zdqjudy.top

Ruby: a, b = pair
来源：http://ykf.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://zek.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://qss.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ttx.kuanghao11.cn

PHP:  // 无重载
来源：http://jmj.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bhm.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://cqp.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://bsi.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://gch.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://hfe.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fit.sufxvd.cn

================================================================================
来源：http://jpq.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://hrn.iojbl.cn

================================================================================
来源：http://bco.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://zhw.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vcs.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czd.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ker.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fnz.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpr.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://tnu.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://htj.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rqw.ppjwa.cn

[D02] 追加元素到末尾
来源：http://qqj.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wvn.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wxs.mhx1999.top

JS:   arr.push(4);
来源：http://bll.svipenyu.cn

TS:   arr.push(4);
来源：http://ocm.snrcjt.cn

Java: list.add(4);
来源：http://cjz.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://syj.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://syt.hammf.cn

C#:   list.Add(4);
来源：http://thr.mhx1999.top

[D03] 在指定位置插入元素
来源：http://ofu.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://awg.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://whp.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hvs.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://ner.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://eaj.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zpp.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://amf.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://jun.zycfv.cn

[D04] 删除元素
来源：http://ial.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uht.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cmy.cashguo.top


<!-- 参考信息 -->