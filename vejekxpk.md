代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ccv.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://unk.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tgl.yj202588.top

[B04] for 计数循环
来源：http://djl.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://uql.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://moy.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hcd.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwo.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hnf.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ygj.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://swv.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gxb.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://zqy.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://qjy.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vxx.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ubv.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yul.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sml.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sie.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://yqh.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yhk.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://pqk.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hyd.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gae.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybb.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vok.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://svl.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://crl.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dpk.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kdx.fengsongda.top

[B07] while 循环
来源：http://jyx.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://gox.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://szi.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://iuh.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://ror.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://lvc.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rwr.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://trj.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://ijs.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://slf.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://rlt.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jje.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://atk.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://mok.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://bak.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yyp.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zga.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://wit.gotoacloud.top

[B09] break 与 continue
来源：http://arb.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xgz.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iua.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tus.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhe.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyu.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dli.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fys.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jiu.c1oappe.top

[B10] 遍历同时拿索引
来源：http://xrb.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lux.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pxr.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://odc.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rkn.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ujs.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wqz.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gdw.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://raj.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://vfj.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://esp.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://dek.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obh.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sfh.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdh.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://twn.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://cvo.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eif.zhixingplan.top

[B12] 跳出多层循环
来源：http://kbp.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://slq.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qil.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhm.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfm.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rrx.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tcp.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wyi.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jep.zycfv.cn

[B13] 判断是否为数字
来源：http://gfj.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ugy.yj20258.top

PHP:  is_numeric($x)
来源：http://wnx.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tai.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hvb.fehbvm.com

Java: x instanceof Number
来源：http://gpv.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://upr.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://vll.sweek.top

C#:   x is int or double or decimal
来源：http://wpq.pycfn.com

[B14] 判断值是否在集合内
来源：http://dqs.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xxl.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fzq.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://eav.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://rkm.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xdh.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abr.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uqy.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qtg.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://gtz.fanxiaobao.xyz

Py:   a and b or not c
来源：http://kfx.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://htu.fehbvm.com

JS:   a && b || !c
来源：http://kvu.yj202588.top

TS:   a && b || !c
来源：http://lbm.yj202588.top

Java: a && b || !c
来源：http://pcz.zhijiandao.cn

Go:   a && b || !c
来源：http://ggi.zhengqikj.top

Ruby: a && b || !c
来源：http://rco.sjlbkw.cn

C#:   a && b || !c
来源：http://ouq.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nhm.cucudq.cn

Py:   if not data: return
来源：http://vlq.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://kjd.jiagoushi.top

JS:   if (!data) return;
来源：http://jwf.0kj1m.cn

TS:   if (!data) return;
来源：http://eij.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://sft.fehbvm.com

Go:   if data == nil { return }
来源：http://bqw.vehdjk.com

Ruby: return if data.nil?
来源：http://frv.vehdjk.com

C#:   if (data == null) return;
来源：http://hyx.guowangkeji.top

================================================================================
来源：http://vee.hongshengwenyu.top

C. 函数与作用域
来源：http://gwj.svipenyu.cn

================================================================================
来源：http://ely.iojbl.cn

[C01] 定义函数
来源：http://rai.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://muo.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yab.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://wyu.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zph.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hmo.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://epy.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://pgu.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hqu.bjfxy.top

[C02] 默认参数
来源：http://brt.sweek.top

Py:   def greet(name="World"): return name
来源：http://app.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nyf.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://qla.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nxt.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hug.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mpo.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://hua.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://vuo.ybcxt.top

[C03] 可变参数
来源：http://zqi.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://nmv.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bvt.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://koa.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgz.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qay.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ovf.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ris.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rus.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://doz.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rcc.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sra.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://osr.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lpd.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://lpn.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://rmm.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://zcx.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://yks.shzxlz.cn

[C05] 返回多个值
来源：http://fse.zdbjq.cn

Py:   return a, b
来源：http://srz.xylfe.cn

PHP:  return [$a, $b];
来源：http://grr.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rxx.wangshuangyany.cn

TS:   return { a, b };
来源：http://zkv.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yom.zhiwuduotai.top

Go:   return a, b
来源：http://bsx.52xcode.cn

Ruby: return a, b
来源：http://ezi.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ecs.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://hxj.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://bvp.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uct.hnqzz.top

JS:   const square = x => x * x;
来源：http://yyt.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://noy.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qor.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://sqy.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://wcn.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://pcv.guannengcc.top

[C07] 把函数作为参数传入
来源：http://utd.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tbw.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bvd.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ehu.gotoacloud.top

TS:   arr.map(String)
来源：http://ltq.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ndf.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fse.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://qqb.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sxc.0kj1m.cn

[C08] 闭包
来源：http://auh.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gei.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xnl.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xrp.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tni.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://znl.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ugx.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nan.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hor.feifeiyinyue.top

[C09] 递归
来源：http://zup.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://plg.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ybw.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjw.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spq.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://adl.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nqx.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bob.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ifc.hnqzz.top

[C10] 变量作用域
来源：http://hye.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://npo.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rzu.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eeb.ivvv.top

TS:   同 JS
来源：http://nxi.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://uyt.cashguo.top

Go:   花括号块级作用域
来源：http://ujk.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gla.yanxiufei.cn

C#:   块级作用域
来源：http://nsd.cqqwz.cn

[C11] 模块导入与导出
来源：http://szj.yueranfly.top

Py:   from module import func
来源：http://dho.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ozu.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ewu.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hra.ehwqpu.com

Java: import java.util.List;
来源：http://vzb.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://san.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://rft.nanxinkj.top

C#:   using System.Text;
来源：http://nht.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://has.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://lpz.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://tcw.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://wck.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://eor.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://txq.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kpd.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://mil.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://qhc.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://vmy.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ccu.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wrn.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zbj.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tlg.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xif.sufxvd.cn

Go:   func add(a, b int) int
来源：http://dye.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gve.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://gfw.ppjwa.cn

[C14] 泛型函数
来源：http://veg.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bqe.jiagoushi.top

PHP:  // 无泛型
来源：http://qsy.hnxiangtu.top

JS:   // 无泛型
来源：http://bvu.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dfb.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hws.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mgl.zhixingplan.top

Ruby: # 无泛型
来源：http://jiz.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://efr.gzhubu.top

[C15] 解构 / 展开参数
来源：http://fcc.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qfe.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://jbv.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kxb.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fah.dianchejie.cn

Java: // 无解构
来源：http://lia.hysaishi.cn

Go:   // 无解构
来源：http://yjg.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://cyi.yfazqb.com

C#:   var (a, b) = pair;
来源：http://caw.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://blq.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zqo.sweek.top

PHP:  // 无重载
来源：http://tyr.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://utb.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://nkn.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bhy.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://pyb.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://dys.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aof.pengpengdd.cyou

================================================================================
来源：http://rlh.316326.xyz

D. 数组 / 列表 / 集合
来源：http://rdb.tanke756.top

================================================================================
来源：http://rji.nwbrower.top

[D01] 创建数组 / 列表
来源：http://fvw.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iyx.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://icj.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tjd.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gbv.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wui.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://rlg.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://whv.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vam.ybcxt.top

[D02] 追加元素到末尾
来源：http://vnb.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nhq.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jiq.dianchejie.cn

JS:   arr.push(4);
来源：http://krc.ydjk.org.cn

TS:   arr.push(4);
来源：http://veb.shzxlz.cn

Java: list.add(4);
来源：http://ipl.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://qsc.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://zpm.yuxming.cn

C#:   list.Add(4);
来源：http://hfd.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://ewz.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://jpd.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ztc.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mcc.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://vvh.sweek.top

Java: list.add(0, 0);
来源：http://sao.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://olm.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uwq.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://amw.bbcook.cn

[D04] 删除元素
来源：http://rqv.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://drh.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ypa.xinyue.icu


<!-- 参考信息 -->