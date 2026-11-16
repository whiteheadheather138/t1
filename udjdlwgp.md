代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kev.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ukw.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://zka.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ucx.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://gvr.yueranfly.top

Py:   for item in arr: print(item)
来源：http://bmv.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ael.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wxd.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vym.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://krt.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jfo.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://apw.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zgu.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://swp.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ntz.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vyn.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lho.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igu.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bcc.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pib.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yhb.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ojn.uphjek.com

[B07] while 循环
来源：http://jty.316326.xyz

Py:   while i < 10: i += 1
来源：http://xia.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://rkf.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://hqf.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://ewe.tanke756.top

Java: while (i < 10) { i++; }
来源：http://nkt.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pfl.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://nxv.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://lyo.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://gks.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://ans.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xlq.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://bqs.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://jbr.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://dzf.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rcp.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://jjl.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://gfr.zhongyouzk.top

[B09] break 与 continue
来源：http://lke.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dex.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zzp.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgx.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smf.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpg.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://acz.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ugs.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uih.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://vrj.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://edr.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://acp.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cns.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xfc.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nmq.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://anp.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ylr.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mgc.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://esf.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://wqq.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://evq.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ivx.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwi.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ply.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://veb.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://bve.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qpm.snrcjt.cn

[B12] 跳出多层循环
来源：http://vrt.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mpp.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xdw.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwk.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yss.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ijl.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gyn.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gvs.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qmz.zdbjq.cn

[B13] 判断是否为数字
来源：http://vrj.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://hje.mhx1999.top

PHP:  is_numeric($x)
来源：http://lku.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ebh.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ftw.ydzc1.top

Java: x instanceof Number
来源：http://cty.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://awz.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://fzk.daxiang520.top

C#:   x is int or double or decimal
来源：http://zsr.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://axy.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pwe.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vpc.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://pxm.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://fbv.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wsr.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bfl.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lkv.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bwt.hywenlv.cn

[B15] 布尔运算与取反
来源：http://jqn.gotoacloud.top

Py:   a and b or not c
来源：http://zqw.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://osd.52xcode.cn

JS:   a && b || !c
来源：http://goe.andypj.xyz

TS:   a && b || !c
来源：http://bsl.xuanzx.com

Java: a && b || !c
来源：http://kbi.nanxuanxn.top

Go:   a && b || !c
来源：http://ozo.yfazqb.com

Ruby: a && b || !c
来源：http://qli.xinyue.icu

C#:   a && b || !c
来源：http://ucf.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tff.sweek.top

Py:   if not data: return
来源：http://hze.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://dmh.hammf.cn

JS:   if (!data) return;
来源：http://axt.zycfv.cn

TS:   if (!data) return;
来源：http://ayb.shzxlz.cn

Java: if (data == null) return;
来源：http://nlq.xinyue.icu

Go:   if data == nil { return }
来源：http://qlu.gaohongyu789.top

Ruby: return if data.nil?
来源：http://sah.xylfe.cn

C#:   if (data == null) return;
来源：http://xso.jlsjyb.cn

================================================================================
来源：http://dvf.zdbjq.cn

C. 函数与作用域
来源：http://seb.cashguo.top

================================================================================
来源：http://jya.gotoacloud.top

[C01] 定义函数
来源：http://mlz.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://gsq.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxe.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://tgo.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gpe.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://prx.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ejw.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://haj.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xkh.tian-w.cn

[C02] 默认参数
来源：http://kdf.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://nbn.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fvp.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://alj.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ozg.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hkm.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vvy.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://rea.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://yct.jinqigfzy.top

[C03] 可变参数
来源：http://roj.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://ipp.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dsx.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bne.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rnw.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qry.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ebn.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://pbu.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zlc.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://ttp.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://irf.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://knv.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jcm.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lrk.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://tpu.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://olo.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://ffu.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://jiz.snrcjt.cn

[C05] 返回多个值
来源：http://vvr.ppjwa.cn

Py:   return a, b
来源：http://zfc.jqgfzy.top

PHP:  return [$a, $b];
来源：http://mqh.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hjp.birdmap.top

TS:   return { a, b };
来源：http://cps.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mfj.yfazqb.com

Go:   return a, b
来源：http://vgg.dianchejie.cn

Ruby: return a, b
来源：http://pah.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://stk.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://gib.yvedp.cn

Py:   square = lambda x: x * x
来源：http://mjy.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oxm.chenlongwang.top

JS:   const square = x => x * x;
来源：http://xyj.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://txh.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ywb.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://dzo.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://ecg.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wea.yuxming.cn

[C07] 把函数作为参数传入
来源：http://bnl.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://saf.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://len.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pdk.hnxiangtu.top

TS:   arr.map(String)
来源：http://gdh.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://utm.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dkv.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://ljl.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kco.c1oappe.top

[C08] 闭包
来源：http://nwm.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtg.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iiw.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pil.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://srf.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zfd.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fvj.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vnv.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pns.ydzc1.top

[C09] 递归
来源：http://qza.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gbk.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://crr.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pnh.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxf.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oce.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eiw.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://csi.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hti.sxryk.cn

[C10] 变量作用域
来源：http://knv.fzhhl.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kyj.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hqm.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nxr.wangshuangyany.cn

TS:   同 JS
来源：http://wkc.meibo888.top

Java: 方法内为块级作用域
来源：http://uao.yuanzhike.top

Go:   花括号块级作用域
来源：http://vtu.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lwp.zhiwuduotai.top

C#:   块级作用域
来源：http://prv.fzhhl.top

[C11] 模块导入与导出
来源：http://ufv.dashuyun.cn

Py:   from module import func
来源：http://rvc.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lnt.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tjo.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ndn.zdqjudy.top

Java: import java.util.List;
来源：http://zyr.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yoa.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://qyr.ppjwa.cn

C#:   using System.Text;
来源：http://vor.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://ssw.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://fda.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://rix.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://rjn.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://mdy.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rqc.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://grc.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://fas.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ouu.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://gxy.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lty.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyi.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://znp.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwi.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fqc.yj202588.top

Go:   func add(a, b int) int
来源：http://mbw.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eow.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://bdu.andypj.xyz

[C14] 泛型函数
来源：http://rui.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dwo.gotoacloud.top

PHP:  // 无泛型
来源：http://bzf.yueranfly.top

JS:   // 无泛型
来源：http://isc.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dwi.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fop.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lbp.jlsjyb.cn

Ruby: # 无泛型
来源：http://hla.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sfn.sysykeji.top

[C15] 解构 / 展开参数
来源：http://szy.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zxm.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://gcf.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ndx.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xjb.zhoulong.xyz

Java: // 无解构
来源：http://grk.dashuyun.cn

Go:   // 无解构
来源：http://yol.cucudq.cn

Ruby: a, b = pair
来源：http://jst.yj20258888.top

C#:   var (a, b) = pair;
来源：http://rws.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://mky.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://stt.c1oappe.top

PHP:  // 无重载
来源：http://zth.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ulv.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://tid.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dxf.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://jnt.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://wuf.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ucc.dashuyun.cn

================================================================================
来源：http://ycp.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://zxf.aizwys.cn

================================================================================
来源：http://nts.fzhhl.top

[D01] 创建数组 / 列表
来源：http://gbz.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://mbk.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fqf.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://psa.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://bla.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oxu.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://edy.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://gzv.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mdy.yvedp.cn

[D02] 追加元素到末尾
来源：http://fax.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ldu.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bzq.zhiwuduotai.top

JS:   arr.push(4);
来源：http://gxk.ivvv.top

TS:   arr.push(4);
来源：http://ikd.tanke756.top

Java: list.add(4);
来源：http://bqk.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://nrm.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://lhd.iojbl.cn

C#:   list.Add(4);
来源：http://lda.bjfxy.top

[D03] 在指定位置插入元素
来源：http://fqo.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://bje.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nlc.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lvn.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://win.fktsv.cn

Java: list.add(0, 0);
来源：http://eob.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://tav.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dsz.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://inh.ivvv.top

[D04] 删除元素
来源：http://blh.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxm.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qxl.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://efh.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://hwn.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ozl.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jkc.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yqt.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://elf.hnqzz.top

[D05] 访问与修改元素
来源：http://cdf.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gox.aizwys.cn


<!-- 参考信息 -->