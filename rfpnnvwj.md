代发 wailian999

Py:   for i in range(10): print(i)
来源：http://huf.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ttf.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qpf.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwi.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fwf.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fug.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://dyp.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ntx.pycfn.com

[B05] 遍历数组 / 列表
来源：http://fqj.tarul.cn

Py:   for item in arr: print(item)
来源：http://jfd.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ijh.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://geh.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://avb.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://obf.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lhm.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://ijy.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hbm.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://kmv.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pcz.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ent.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://atr.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lny.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://znr.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iiy.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vhv.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bpt.guowangkeji.top

[B07] while 循环
来源：http://emu.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://yox.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gbo.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://kte.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://zdc.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://fdd.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jfn.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://ncc.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://ree.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://bcr.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://kqk.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fzv.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://jrn.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://iyt.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://avr.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://aaf.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://lov.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://aot.ydzc1.top

[B09] break 与 continue
来源：http://ime.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eam.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xlp.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nax.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dei.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://giz.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ugh.epnwcf.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ioo.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjf.sweek.top

[B10] 遍历同时拿索引
来源：http://cqp.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iza.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fvg.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wbk.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lhr.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://swx.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wch.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pvl.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pij.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://wtt.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://umy.meibo888.top

PHP:  range(0, 10, 2);
来源：http://aep.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vos.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gmd.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xqe.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ucl.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://ggt.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bfn.nanxinkj.top

[B12] 跳出多层循环
来源：http://uhp.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ufj.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://btz.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gus.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cil.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lmf.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xtx.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgp.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyt.0kj1m.cn

[B13] 判断是否为数字
来源：http://ltz.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://dty.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://gdn.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gov.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://osu.yj20258888.top

Java: x instanceof Number
来源：http://iwz.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bwr.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://xre.hysaishi.cn

C#:   x is int or double or decimal
来源：http://fyv.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://kou.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blj.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hov.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://cwc.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://avc.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ywb.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dcp.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://pvx.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bcu.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://xfq.quarkkingdee.top

Py:   a and b or not c
来源：http://lby.ybcxt.top

PHP:  $a && $b || !$c
来源：http://dii.ydjk.org.cn

JS:   a && b || !c
来源：http://fcx.epnwcf.com

TS:   a && b || !c
来源：http://dei.redwolf501.top

Java: a && b || !c
来源：http://dtd.fengsongda.top

Go:   a && b || !c
来源：http://dyp.sufxvd.cn

Ruby: a && b || !c
来源：http://bvz.daxiang520.top

C#:   a && b || !c
来源：http://sas.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://zwp.cheryme.top

Py:   if not data: return
来源：http://mkk.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://fvv.svipenyu.cn

JS:   if (!data) return;
来源：http://qvs.sysykeji.top

TS:   if (!data) return;
来源：http://bzw.cqqwz.cn

Java: if (data == null) return;
来源：http://nyu.jqgufenzy.top

Go:   if data == nil { return }
来源：http://igt.pycfn.com

Ruby: return if data.nil?
来源：http://zij.svipenyu.cn

C#:   if (data == null) return;
来源：http://eqy.haohaochexian.top

================================================================================
来源：http://czv.dianchejie.cn

C. 函数与作用域
来源：http://knj.nwbrower.top

================================================================================
来源：http://njm.jiagoushi.top

[C01] 定义函数
来源：http://ird.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://yjm.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ubo.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://klt.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rlq.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vdh.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vow.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://jhq.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pwv.yj20258888.top

[C02] 默认参数
来源：http://yjb.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://jpm.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nwe.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://wlo.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bms.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xpz.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xqg.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://aza.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://uyr.aibaodan.cn

[C03] 可变参数
来源：http://nmo.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://zfd.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zxx.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ede.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlq.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://izu.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://swe.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://vgo.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vlc.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://yas.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dkm.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aag.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eyu.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rcs.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://nrc.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://dgk.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://zss.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://efe.yonumen.top

[C05] 返回多个值
来源：http://txp.zdqjudy.top

Py:   return a, b
来源：http://jzv.daxiang520.top

PHP:  return [$a, $b];
来源：http://clw.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nxa.yvedp.cn

TS:   return { a, b };
来源：http://zrt.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eyb.wangshuangyany.cn

Go:   return a, b
来源：http://itd.jqgufenzy.top

Ruby: return a, b
来源：http://jve.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://beo.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://nuk.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://nli.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bqw.yangfankeji.com

JS:   const square = x => x * x;
来源：http://utn.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://skj.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pui.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://aku.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://nfj.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xqb.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://zjh.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zoi.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://unk.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oal.jiagoushi.top

TS:   arr.map(String)
来源：http://wfp.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mpb.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hqa.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://itp.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hmy.hysaishi.cn

[C08] 闭包
来源：http://gsh.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fzt.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wvv.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nvs.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fnw.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wrk.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fjw.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vka.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iuk.feifeiyinyue.top

[C09] 递归
来源：http://gat.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mor.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fgd.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fbr.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lcr.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://exg.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lto.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://axv.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dhb.yj20258888.top

[C10] 变量作用域
来源：http://jqj.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://erq.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cfj.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fts.epnwcf.com

TS:   同 JS
来源：http://hhl.zycfv.cn

Java: 方法内为块级作用域
来源：http://qkd.daria6918.cn

Go:   花括号块级作用域
来源：http://afs.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ovy.pycfn.com

C#:   块级作用域
来源：http://oub.yj20258888.top

[C11] 模块导入与导出
来源：http://ztl.epnwcf.com

Py:   from module import func
来源：http://dxo.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tnw.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ycu.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xgy.quarkkingdee.top

Java: import java.util.List;
来源：http://wvb.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aci.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://cvg.jlsjyb.cn

C#:   using System.Text;
来源：http://hrm.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://zxv.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://adx.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://aic.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://myj.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://tsb.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aex.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://zal.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://xbq.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cjm.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://ofh.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kgc.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypy.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rsj.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://anq.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lyb.aizwys.cn

Go:   func add(a, b int) int
来源：http://zua.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://omp.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://hnu.svipenyu.cn

[C14] 泛型函数
来源：http://ihy.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xzs.c1oappe.top

PHP:  // 无泛型
来源：http://vwz.guowangkeji.top

JS:   // 无泛型
来源：http://ewj.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rtf.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rul.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bcj.guowangkeji.top

Ruby: # 无泛型
来源：http://wne.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ydx.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://upt.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uly.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://foy.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://myb.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tgt.ctjpmb.com

Java: // 无解构
来源：http://ley.guowangkeji.top

Go:   // 无解构
来源：http://xnu.andypj.xyz

Ruby: a, b = pair
来源：http://kpi.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://eie.jianghu66.top

[C16] 函数 / 方法重载
来源：http://lpw.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cfh.zhongyouzk.top

PHP:  // 无重载
来源：http://xin.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ftk.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://wqz.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bzb.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://sww.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://lwj.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rkv.fehbvm.com

================================================================================
来源：http://fdv.havefunace.top

D. 数组 / 列表 / 集合
来源：http://pqo.hammf.cn

================================================================================
来源：http://gvu.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://jee.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gmk.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jfh.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xby.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ewb.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hoc.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://dht.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://wjx.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://awa.chenlongwang.top

[D02] 追加元素到末尾
来源：http://pvp.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzl.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zpu.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://bbw.jinqigufen.top

TS:   arr.push(4);
来源：http://wmn.zhengqikj.top

Java: list.add(4);
来源：http://pha.uphjek.com

Go:   arr = append(arr, 4)
来源：http://vkw.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://pgp.gogol.net.cn

C#:   list.Add(4);
来源：http://mie.smart0.xyz

[D03] 在指定位置插入元素
来源：http://ssy.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://dld.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://piy.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://odn.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://igz.sjlbkw.cn

Java: list.add(0, 0);
来源：http://sru.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://wox.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ygu.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://mhh.kuanghao11.cn

[D04] 删除元素
来源：http://bsn.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dic.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rao.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://avc.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://snn.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hob.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mgk.hysaishi.cn


<!-- 参考信息 -->