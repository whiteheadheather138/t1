代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://upb.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://ssg.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://otr.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jwa.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yfn.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mxu.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgu.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ncp.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vlv.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hgr.vehdjk.com

[B07] while 循环
来源：http://fim.wangdashe.top

Py:   while i < 10: i += 1
来源：http://hph.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://xdf.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://yxb.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://pxb.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://rdh.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ean.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://hkb.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://pav.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://ivn.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://inh.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://qmb.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://hif.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://nxw.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://wvo.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lye.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lrk.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://veu.sufxvd.cn

[B09] break 与 continue
来源：http://pfj.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjv.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tdg.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kan.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdr.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dor.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qbx.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xee.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocs.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://bbo.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://atf.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqg.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xkf.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lfh.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lhx.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oby.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ogb.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ori.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://rst.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://qxn.ivvv.top

PHP:  range(0, 10, 2);
来源：http://bej.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdw.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hsx.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vwr.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ody.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://cim.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vhm.zhijiandao.cn

[B12] 跳出多层循环
来源：http://ksm.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://arm.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oyi.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ily.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aat.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aft.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fcu.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://khi.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rwf.tarul.cn

[B13] 判断是否为数字
来源：http://kfi.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://xho.xuanzx.com

PHP:  is_numeric($x)
来源：http://smb.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uki.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzr.redwolf501.top

Java: x instanceof Number
来源：http://zrf.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pdm.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://ukc.pycfn.com

C#:   x is int or double or decimal
来源：http://pew.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://yrv.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lyl.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aps.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wev.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://rpe.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xnw.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nbj.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://ccr.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://piv.pycfn.com

[B15] 布尔运算与取反
来源：http://vuj.yuxming.cn

Py:   a and b or not c
来源：http://uef.yj202588.top

PHP:  $a && $b || !$c
来源：http://rux.dianchejie.cn

JS:   a && b || !c
来源：http://oyv.xuetiantiany.cn

TS:   a && b || !c
来源：http://oeq.redwolf501.top

Java: a && b || !c
来源：http://pxp.zycfv.cn

Go:   a && b || !c
来源：http://cgz.yanxiufei.cn

Ruby: a && b || !c
来源：http://uay.xuetiantiany.cn

C#:   a && b || !c
来源：http://uow.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gaz.9152youxi.cn

Py:   if not data: return
来源：http://mxv.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://msk.bjfxy.top

JS:   if (!data) return;
来源：http://jez.yj20258888.top

TS:   if (!data) return;
来源：http://jff.jqgfzy.top

Java: if (data == null) return;
来源：http://nbu.cdnleiting.top

Go:   if data == nil { return }
来源：http://vbt.yuanzhike.top

Ruby: return if data.nil?
来源：http://lle.cheryme.top

C#:   if (data == null) return;
来源：http://sus.feifeiyinyue.top

================================================================================
来源：http://zmx.daria6918.cn

C. 函数与作用域
来源：http://ujk.hywenlv.cn

================================================================================
来源：http://qsg.yj202588.top

[C01] 定义函数
来源：http://mxt.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://hxf.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://scj.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://olt.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dwu.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://drh.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://qbj.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://wxa.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fdf.shzxlz.cn

[C02] 默认参数
来源：http://sri.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://dfv.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mkt.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://xtt.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://utz.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://btu.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bfu.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://vca.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://ysc.jqgfzy.top

[C03] 可变参数
来源：http://gez.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://lca.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://swv.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xor.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tgj.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://idj.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lep.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://yyj.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zgx.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://xfy.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://usj.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yny.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ink.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbw.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://hnp.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://gnr.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://mkn.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://six.jlsjyb.cn

[C05] 返回多个值
来源：http://mgy.xuetiantiany.cn

Py:   return a, b
来源：http://ljf.ppjwa.cn

PHP:  return [$a, $b];
来源：http://tbj.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cqy.yuxming.cn

TS:   return { a, b };
来源：http://isb.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hrz.jiagoushi.top

Go:   return a, b
来源：http://duh.shanyushiyangtech.top

Ruby: return a, b
来源：http://lsk.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://mul.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://epb.havefunace.top

Py:   square = lambda x: x * x
来源：http://grj.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kli.cheryme.top

JS:   const square = x => x * x;
来源：http://kdf.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://ktu.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cnc.jlsjyb.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wie.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://hjd.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://rsj.aizwys.cn

[C07] 把函数作为参数传入
来源：http://mcl.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bxa.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://emi.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tgq.xuetiantiany.cn

TS:   arr.map(String)
来源：http://xdt.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vfc.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yqh.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://jiv.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://rve.dashuyun.cn

[C08] 闭包
来源：http://csa.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dkl.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ryq.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bwf.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jmh.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://smb.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ujl.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xxf.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fwf.yuanzhike.top

[C09] 递归
来源：http://xbj.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ncj.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nmo.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jrj.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bad.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qvz.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ibf.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xsz.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ccl.xinyue.icu

[C10] 变量作用域
来源：http://dds.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xor.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qjq.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kin.zhiwuduotai.top

TS:   同 JS
来源：http://nkd.cdnleiting.top

Java: 方法内为块级作用域
来源：http://wmp.52xcode.cn

Go:   花括号块级作用域
来源：http://agh.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mpw.ydjk.org.cn

C#:   块级作用域
来源：http://oiz.hnqzz.top

[C11] 模块导入与导出
来源：http://acv.ivvv.top

Py:   from module import func
来源：http://szg.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vnp.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cwl.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucu.ydjk.org.cn

Java: import java.util.List;
来源：http://cra.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://voq.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://dkp.yvedp.cn

C#:   using System.Text;
来源：http://wlk.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://awy.cheryme.top

Py:   (lambda: print("run"))()
来源：http://fev.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://ipv.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://fij.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://jus.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifo.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://nln.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://art.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qqs.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://dug.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://grg.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkd.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yii.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mft.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://crc.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://rdr.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rgn.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://ptx.sjlbkw.cn

[C14] 泛型函数
来源：http://blx.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bck.sweek.top

PHP:  // 无泛型
来源：http://zge.ctjpmb.com

JS:   // 无泛型
来源：http://lgt.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rqs.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aen.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yry.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://gfv.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mwx.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://rlu.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qbt.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://jcz.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bim.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hvu.316326.xyz

Java: // 无解构
来源：http://wkm.fzhhl.top

Go:   // 无解构
来源：http://rxv.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://wdv.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://xii.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://lbe.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uuo.daxiang520.top

PHP:  // 无重载
来源：http://yuf.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrf.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://ysm.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://huu.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://omx.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://plp.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dlv.hammf.cn

================================================================================
来源：http://kos.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://ybq.fzhhl.top

================================================================================
来源：http://bcu.redwolf501.top

[D01] 创建数组 / 列表
来源：http://mmv.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ziz.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oha.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://seo.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xyi.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bzb.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://eqp.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://zcu.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ybf.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://yqj.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qox.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hrx.jianghu66.top

JS:   arr.push(4);
来源：http://kez.sjlbkw.cn

TS:   arr.push(4);
来源：http://nvn.jinghuilouyu.cn

Java: list.add(4);
来源：http://unm.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://xwq.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://msl.jyoumei.cn

C#:   list.Add(4);
来源：http://xgj.yueranfly.top

[D03] 在指定位置插入元素
来源：http://swy.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://jxh.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ylr.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://apt.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://env.gzhubu.top

Java: list.add(0, 0);
来源：http://fze.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://kka.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cpy.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://ivh.shangyingyoupin.top

[D04] 删除元素
来源：http://ldk.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://akb.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rhj.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pjf.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://cuu.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ybp.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ajq.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nnn.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ylj.gzhubu.top

[D05] 访问与修改元素
来源：http://cuo.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ljz.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yui.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gxq.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://grl.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://cde.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://ice.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pom.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://doh.wangshuangyany.cn

[D06] 数组长度
来源：http://qac.birdmap.top

Py:   len(arr)
来源：http://tjp.zhoulong.xyz

PHP:  count($arr);
来源：http://kga.yfazqb.com

JS:   arr.length
来源：http://ygh.xziqi.cn

TS:   arr.length
来源：http://fnx.ivvv.top


<!-- 参考信息 -->