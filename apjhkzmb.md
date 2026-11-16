代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://chd.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yzq.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://smp.mhx1999.top

[B04] for 计数循环
来源：http://thn.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://pyz.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uxq.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjs.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xkd.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wep.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ptx.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://fek.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://csx.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://pdw.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://och.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://swg.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vjo.ydjk.org.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rye.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tos.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ufc.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://dai.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://brg.hammf.cn

[B06] 遍历字典 / 对象
来源：http://idf.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://aym.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ubn.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bfl.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://keb.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kgr.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wrn.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cty.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pqs.sjlbkw.cn

[B07] while 循环
来源：http://fbw.sysykeji.top

Py:   while i < 10: i += 1
来源：http://fuo.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bad.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://xyo.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://drm.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://bef.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kxr.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://hkg.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://zbi.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://keu.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://ong.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://irv.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://rhg.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://vsk.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://gwi.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://htq.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://bix.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://arv.wangdashe.top

[B09] break 与 continue
来源：http://xip.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lvv.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wwv.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bvz.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwb.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbz.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gwb.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ntz.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjq.daria6918.cn

[B10] 遍历同时拿索引
来源：http://fkb.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qew.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bge.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pnu.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zgy.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tsk.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rqd.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hus.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rty.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://krl.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://hap.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://lni.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrn.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klr.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nlq.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgc.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://gmo.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dda.yueranfly.top

[B12] 跳出多层循环
来源：http://sga.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kvm.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://agl.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tap.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://npg.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fwq.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jzj.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zeo.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://edi.bbcook.cn

[B13] 判断是否为数字
来源：http://gpb.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://psu.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://orw.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umm.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfi.hcnkem.com

Java: x instanceof Number
来源：http://egd.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vdk.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://ezh.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://tze.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://chp.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ltj.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pjl.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://oxn.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://lkp.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://skd.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tlt.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://njd.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mua.yvedp.cn

[B15] 布尔运算与取反
来源：http://xxn.hnxiangtu.top

Py:   a and b or not c
来源：http://vgy.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://ewk.kuanghao11.cn

JS:   a && b || !c
来源：http://upj.cucudq.cn

TS:   a && b || !c
来源：http://qxs.sufxvd.cn

Java: a && b || !c
来源：http://dbw.epnwcf.com

Go:   a && b || !c
来源：http://ngm.sysykeji.top

Ruby: a && b || !c
来源：http://jjr.9152youxi.cn

C#:   a && b || !c
来源：http://cih.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wvp.cdnleiting.top

Py:   if not data: return
来源：http://vsl.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://ypk.wangshuangyany.cn

JS:   if (!data) return;
来源：http://izx.tianlin.xyz

TS:   if (!data) return;
来源：http://udi.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://hij.zdqjudy.top

Go:   if data == nil { return }
来源：http://jkm.sysykeji.top

Ruby: return if data.nil?
来源：http://uce.fktsv.cn

C#:   if (data == null) return;
来源：http://pkb.hesvh.cn

================================================================================
来源：http://omz.jlsjyb.cn

C. 函数与作用域
来源：http://ift.shzxlz.cn

================================================================================
来源：http://muj.jqgufenzy.top

[C01] 定义函数
来源：http://abn.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://vdj.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbf.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://pgo.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xlg.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://qgn.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://jis.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://bvn.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qhh.nanxinkj.top

[C02] 默认参数
来源：http://hge.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://hpd.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hia.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://fqr.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uju.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hze.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://puq.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://yhn.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://rjr.shuidangran.top

[C03] 可变参数
来源：http://ziy.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://wus.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sut.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpq.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xxx.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://klv.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xke.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://wop.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kbc.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://ymc.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dms.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ypq.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpm.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlc.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://vgb.yfazqb.com

Go:   // 无：用配置结构体参数
来源：http://xgm.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://mpb.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://yem.cdnleiting.top

[C05] 返回多个值
来源：http://hcn.zhoulong.xyz

Py:   return a, b
来源：http://qyl.birdmap.top

PHP:  return [$a, $b];
来源：http://spk.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vcy.guowangkeji.top

TS:   return { a, b };
来源：http://fmi.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mmx.yj20258.top

Go:   return a, b
来源：http://xwy.zhijiandao.cn

Ruby: return a, b
来源：http://kwq.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://gbs.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://ojv.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://xle.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://ole.dashuyun.cn

JS:   const square = x => x * x;
来源：http://vmm.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://uxi.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eek.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fly.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://van.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fng.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://qno.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obr.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rit.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qmo.xuetiantiany.cn

TS:   arr.map(String)
来源：http://tia.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xaa.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://szf.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://efp.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pmm.epnwcf.com

[C08] 闭包
来源：http://gzj.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dzl.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://drj.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bak.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xli.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gfi.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kuk.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qsd.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bkm.cheryme.top

[C09] 递归
来源：http://ynx.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dxl.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tat.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crq.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rdh.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gyh.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://khe.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qlv.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qcm.jinghuilouyu.cn

[C10] 变量作用域
来源：http://cle.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xpg.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lfk.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wbk.tian-w.cn

TS:   同 JS
来源：http://pnp.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://ypo.sjlbkw.cn

Go:   花括号块级作用域
来源：http://vrw.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://njx.yj20258888.top

C#:   块级作用域
来源：http://chc.yongpay.top

[C11] 模块导入与导出
来源：http://jbk.yueranfly.top

Py:   from module import func
来源：http://gdq.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dsz.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hwh.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://krh.chenlongwang.top

Java: import java.util.List;
来源：http://ndi.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nzc.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://nlo.hongshengwenyu.top

C#:   using System.Text;
来源：http://oum.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://vmd.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://fzs.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://cbs.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://wrf.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://ugx.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pjj.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://lqw.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://sea.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pka.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://qop.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://arw.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivo.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pvx.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://css.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://yyu.ehwqpu.com

Go:   func add(a, b int) int
来源：http://ytq.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vpp.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://swl.yanxiufei.cn

[C14] 泛型函数
来源：http://oip.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://frx.jinqigfzy.top

PHP:  // 无泛型
来源：http://wnm.xuetiantiany.cn

JS:   // 无泛型
来源：http://qpz.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rzf.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sbb.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gwi.ehwqpu.com

Ruby: # 无泛型
来源：http://lgz.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cll.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://kbh.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xsp.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://nje.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jtg.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://koz.yvedp.cn

Java: // 无解构
来源：http://gib.sysykeji.top

Go:   // 无解构
来源：http://njr.gotoacloud.top

Ruby: a, b = pair
来源：http://hfi.aizwys.cn

C#:   var (a, b) = pair;
来源：http://bdu.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://yyl.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://clm.havefunace.top

PHP:  // 无重载
来源：http://cje.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bhd.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://hid.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dwf.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://viw.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://fkl.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rpt.xinyue.icu

================================================================================
来源：http://dbu.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://pwu.hywenlv.cn

================================================================================
来源：http://pdt.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://ulo.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gfo.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ljp.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gom.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dex.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fng.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://tsd.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://jjr.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ytb.iojbl.cn

[D02] 追加元素到末尾
来源：http://ftv.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmx.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lfp.quarkkingdee.top

JS:   arr.push(4);
来源：http://ydo.gzhubu.top

TS:   arr.push(4);
来源：http://ioz.zdqjudy.top

Java: list.add(4);
来源：http://cjo.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://sjj.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://pyh.yangfankeji.com

C#:   list.Add(4);
来源：http://srn.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://uzu.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://sjm.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lke.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gqf.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://lfo.bjfxy.top

Java: list.add(0, 0);
来源：http://gte.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://gig.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mpe.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://hyp.chenjidiqi.icu

[D04] 删除元素
来源：http://gcu.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gji.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qzw.havefunace.top


<!-- 参考信息 -->