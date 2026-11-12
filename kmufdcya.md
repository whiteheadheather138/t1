代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yzr.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwv.jyoumei.cn

[B07] while 循环
来源：http://kfk.hammf.cn

Py:   while i < 10: i += 1
来源：http://ogh.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://yty.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://lzv.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://zba.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://rrc.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pxn.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://jej.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://cuc.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://jhz.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://yda.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://smr.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://dqz.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://gyx.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://yaf.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ffa.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://enw.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://bjx.pengpengdd.cyou

[B09] break 与 continue
来源：http://uof.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sfz.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vng.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdb.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukh.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mry.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://efq.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tmm.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snm.xziqi.cn

[B10] 遍历同时拿索引
来源：http://qyo.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ojd.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jmf.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gbf.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dxz.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dox.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yrs.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ygp.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wgq.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://nld.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://tqw.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://lbx.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yjl.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yfc.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dii.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://otp.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://zma.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://brs.sufxvd.cn

[B12] 跳出多层循环
来源：http://psy.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lzs.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://afv.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tya.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xth.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bag.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rqh.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jts.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mwe.jiagoushi.top

[B13] 判断是否为数字
来源：http://xla.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://cih.wangdashe.top

PHP:  is_numeric($x)
来源：http://gvr.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wbu.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuy.tanke756.top

Java: x instanceof Number
来源：http://ses.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hli.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://bgs.zdbjq.cn

C#:   x is int or double or decimal
来源：http://ata.ydzc1.top

[B14] 判断值是否在集合内
来源：http://cob.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vug.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dsz.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://lxp.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://gsh.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hta.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pwm.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nxx.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vjj.cheryme.top

[B15] 布尔运算与取反
来源：http://wty.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://rqm.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://psc.xuanzx.com

JS:   a && b || !c
来源：http://kru.smart0.xyz

TS:   a && b || !c
来源：http://hbd.bjfxy.top

Java: a && b || !c
来源：http://ckj.tarul.cn

Go:   a && b || !c
来源：http://tpf.gzhubu.top

Ruby: a && b || !c
来源：http://gqf.ehwqpu.com

C#:   a && b || !c
来源：http://vpz.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://xhp.zhengqikj.top

Py:   if not data: return
来源：http://kxb.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://lii.nanxinkj.top

JS:   if (!data) return;
来源：http://pub.guowangkeji.top

TS:   if (!data) return;
来源：http://wkc.fengsongda.top

Java: if (data == null) return;
来源：http://khz.zhoulong.xyz

Go:   if data == nil { return }
来源：http://osh.nanxinkj.top

Ruby: return if data.nil?
来源：http://qkn.vehdjk.com

C#:   if (data == null) return;
来源：http://upj.0kj1m.cn

================================================================================
来源：http://yxf.cashguo.top

C. 函数与作用域
来源：http://uyo.yj20258888.top

================================================================================
来源：http://fru.hcnkem.com

[C01] 定义函数
来源：http://ulu.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://lbm.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xiv.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://dgu.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgr.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zjp.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://urh.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://cxl.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://abh.ydzc1.top

[C02] 默认参数
来源：http://mmb.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://noj.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zpq.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://feq.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://cpv.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bsa.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gta.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://odk.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nha.cheryme.top

[C03] 可变参数
来源：http://yku.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://xgi.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ick.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xeg.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zmh.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qeu.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zml.zhongyouzk.top

Ruby: def total(*nums); nums.sum; end
来源：http://mxh.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://caw.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://cld.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mui.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hci.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://deg.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ekz.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://iys.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://qlt.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://nva.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://nsx.fehbvm.com

[C05] 返回多个值
来源：http://cts.wangdashe.top

Py:   return a, b
来源：http://fha.yj202588.top

PHP:  return [$a, $b];
来源：http://mtg.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ndg.snrcjt.cn

TS:   return { a, b };
来源：http://unz.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dij.zdbjq.cn

Go:   return a, b
来源：http://lmg.quarkkingdee.top

Ruby: return a, b
来源：http://eju.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://hzb.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://env.aizwys.cn

Py:   square = lambda x: x * x
来源：http://ouk.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zbl.haohaochexian.top

JS:   const square = x => x * x;
来源：http://atc.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://xxa.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ved.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://cny.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://zsg.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://exv.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://qkq.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ehc.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://bof.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mon.hysaishi.cn

TS:   arr.map(String)
来源：http://qyp.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jvg.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wqb.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://nph.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ghq.kuanghao11.cn

[C08] 闭包
来源：http://jni.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ima.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blf.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwp.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rzb.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ozm.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xnd.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cps.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qai.xuanzx.com

[C09] 递归
来源：http://dno.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gyi.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wyc.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcp.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wxa.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwk.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upa.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vds.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxq.xylfe.cn

[C10] 变量作用域
来源：http://zzi.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://npo.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qty.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://npm.shuidangran.top

TS:   同 JS
来源：http://mcd.guannengcc.top

Java: 方法内为块级作用域
来源：http://buq.wangdashe.top

Go:   花括号块级作用域
来源：http://qka.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jri.guannengcc.top

C#:   块级作用域
来源：http://ldk.zhongyouzk.top

[C11] 模块导入与导出
来源：http://rjw.fzhhl.top

Py:   from module import func
来源：http://jap.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sij.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cml.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lbb.jinqigfzy.top

Java: import java.util.List;
来源：http://hjl.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hgf.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://xco.svipenyu.cn

C#:   using System.Text;
来源：http://smf.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://zsw.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://zwa.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://ufc.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://now.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://kfd.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ohp.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://kzw.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://jjz.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kvy.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://kjn.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ekt.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gly.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gxo.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kfw.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://upr.cheryme.top

Go:   func add(a, b int) int
来源：http://tzc.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iqh.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ece.hywenlv.cn

[C14] 泛型函数
来源：http://cop.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qqd.fengsongda.top

PHP:  // 无泛型
来源：http://dpp.sufxvd.cn

JS:   // 无泛型
来源：http://sxo.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oxk.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iuh.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ctw.zhijiandao.cn

Ruby: # 无泛型
来源：http://lrj.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://usu.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://mvv.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ysp.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://yei.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bel.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sib.ctjpmb.com

Java: // 无解构
来源：http://zgs.yj202588.top

Go:   // 无解构
来源：http://blv.shzxlz.cn

Ruby: a, b = pair
来源：http://iad.hesvh.cn

C#:   var (a, b) = pair;
来源：http://ywc.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ytu.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qhs.dashuyun.cn

PHP:  // 无重载
来源：http://vik.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zwz.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://olj.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gbg.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://cah.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://djn.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pln.hnqzz.top

================================================================================
来源：http://bit.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://pce.zhoulong.xyz

================================================================================
来源：http://wlz.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://zis.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aje.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://otl.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://njs.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tcz.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujf.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://vhj.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://iku.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://soh.zycfv.cn

[D02] 追加元素到末尾
来源：http://zsr.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://faw.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsg.pycfn.com

JS:   arr.push(4);
来源：http://asp.yuanzhike.top

TS:   arr.push(4);
来源：http://cyv.yueranfly.top

Java: list.add(4);
来源：http://rvm.sweek.top

Go:   arr = append(arr, 4)
来源：http://jzi.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://cub.hfpthk.cn

C#:   list.Add(4);
来源：http://sjg.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://oni.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://cdb.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gsx.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ezx.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://dks.zhongyouzk.top

Java: list.add(0, 0);
来源：http://wcl.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zif.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yoa.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://jun.nwbrower.top

[D04] 删除元素
来源：http://fno.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imf.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dcg.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cza.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://mjn.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pqj.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zgl.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fkh.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gek.jqgfzy.top

[D05] 访问与修改元素
来源：http://cmc.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cbu.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eox.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pzq.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://cdh.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://rmi.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://grr.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fqm.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nva.c1oappe.top

[D06] 数组长度
来源：http://pqf.zhijiandao.cn

Py:   len(arr)
来源：http://nuz.jqgfzy.top

PHP:  count($arr);
来源：http://rtt.0kj1m.cn

JS:   arr.length
来源：http://key.mhx1999.top

TS:   arr.length
来源：http://hjs.dashuyun.cn

Java: list.size();
来源：http://bvj.yuxming.cn

Go:   len(arr)
来源：http://gpd.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://mpr.zhongyouzk.top

C#:   list.Count;
来源：http://zjk.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://ksp.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pdr.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uau.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://jdh.0kj1m.cn


<!-- 参考信息 -->