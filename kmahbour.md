代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://ovw.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://gzc.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://geh.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://vye.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qmf.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://bav.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://mts.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://utc.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://qib.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nbw.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://ivt.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://zuq.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://aoq.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://owu.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://sta.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://eem.sxryk.cn

[B09] break 与 continue
来源：http://jiy.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kfi.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rhw.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohj.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nud.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsc.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fmp.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gts.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbf.bbcook.cn

[B10] 遍历同时拿索引
来源：http://djg.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bsd.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://srb.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://olz.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qqw.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qtr.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xqs.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dxk.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gjf.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://ptx.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://epp.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://kst.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xoe.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://han.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jwb.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jla.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://gzg.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nar.cqqwz.cn

[B12] 跳出多层循环
来源：http://boq.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://kre.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://day.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ybl.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://haa.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://olk.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://khn.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hqy.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ybp.xuanzx.com

[B13] 判断是否为数字
来源：http://dlu.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://agr.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://qck.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wvl.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qdg.ehwqpu.com

Java: x instanceof Number
来源：http://lmz.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eby.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://fdw.sweek.top

C#:   x is int or double or decimal
来源：http://ski.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://xri.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mnr.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axj.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://bmw.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://aog.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rjy.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vpv.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://vkq.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hzi.hcnkem.com

[B15] 布尔运算与取反
来源：http://xek.cdnleiting.top

Py:   a and b or not c
来源：http://zuh.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://qjx.0kj1m.cn

JS:   a && b || !c
来源：http://pzp.xuanzx.com

TS:   a && b || !c
来源：http://xfo.yongpay.top

Java: a && b || !c
来源：http://nhn.kuanghao11.cn

Go:   a && b || !c
来源：http://odj.daria6918.cn

Ruby: a && b || !c
来源：http://wbs.gaohongyu789.top

C#:   a && b || !c
来源：http://dwu.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://jbs.yvedp.cn

Py:   if not data: return
来源：http://zmo.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://sqi.dianchejie.cn

JS:   if (!data) return;
来源：http://hsj.mhx1999.top

TS:   if (!data) return;
来源：http://hav.yueranfly.top

Java: if (data == null) return;
来源：http://qis.jinqigfzy.top

Go:   if data == nil { return }
来源：http://lcs.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://lqi.chenlongwang.top

C#:   if (data == null) return;
来源：http://egi.hnxiangtu.top

================================================================================
来源：http://gph.ywan-chungtsiang.top

C. 函数与作用域
来源：http://tnj.chenzaomai.com

================================================================================
来源：http://sgs.bjfxy.top

[C01] 定义函数
来源：http://hpx.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://wdl.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://agx.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://axe.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://miw.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vkh.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dah.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://qza.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gur.ppjwa.cn

[C02] 默认参数
来源：http://hdv.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://oii.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rmw.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://dgp.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wbf.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://idq.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://flq.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://cnp.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://pkc.yuanzhike.top

[C03] 可变参数
来源：http://ykh.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://rkt.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xjd.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tfk.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tkg.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uxr.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dnc.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://hkr.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mnt.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://kcw.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vob.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dmo.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sac.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lvl.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://zme.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://rkg.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://gna.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://itc.ppjwa.cn

[C05] 返回多个值
来源：http://rsp.pengpengdd.cyou

Py:   return a, b
来源：http://vje.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://vth.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ptp.jqgufenzy.top

TS:   return { a, b };
来源：http://igw.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ile.xingfuxueyuan.xyz

Go:   return a, b
来源：http://ntw.gzhubu.top

Ruby: return a, b
来源：http://ago.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://dji.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://pvy.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://qnl.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xyw.tianlin.xyz

JS:   const square = x => x * x;
来源：http://hpa.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://ymn.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rkd.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://sqy.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://epi.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://exq.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://vlb.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dhz.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://zsw.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tlu.hysaishi.cn

TS:   arr.map(String)
来源：http://axi.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vhz.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bkn.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://nkq.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ffr.yuxming.cn

[C08] 闭包
来源：http://jja.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vow.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nje.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ryl.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hjw.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jxi.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mew.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://scs.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://epd.yangfankeji.com

[C09] 递归
来源：http://sdm.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pao.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wpr.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zze.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjw.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsk.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qes.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mld.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tey.ppjwa.cn

[C10] 变量作用域
来源：http://gau.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://syx.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zjs.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ynl.gogol.net.cn

TS:   同 JS
来源：http://lkp.ehwqpu.com

Java: 方法内为块级作用域
来源：http://jja.yonumen.top

Go:   花括号块级作用域
来源：http://kvq.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wef.jinyuanbaomall.cn

C#:   块级作用域
来源：http://lsk.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://ftu.dashuyun.cn

Py:   from module import func
来源：http://gkl.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://bst.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fst.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agz.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://bfu.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kdz.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://qms.ctjpmb.com

C#:   using System.Text;
来源：http://otu.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://uuw.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://wrb.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://ypz.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://enn.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://vcw.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lcy.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://spc.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://mfl.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jct.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://uei.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncc.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zlm.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dhb.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nlb.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jgd.fzhhl.top

Go:   func add(a, b int) int
来源：http://rql.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hld.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://jvp.xinyue.icu

[C14] 泛型函数
来源：http://xnz.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzn.snrcjt.cn

PHP:  // 无泛型
来源：http://wtg.snrcjt.cn

JS:   // 无泛型
来源：http://nuv.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ujt.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zuo.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uuk.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://yve.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://anj.shuidangran.top

[C15] 解构 / 展开参数
来源：http://erb.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://egn.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://jgb.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://njd.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qfs.wangdashe.top

Java: // 无解构
来源：http://pgs.sweek.top

Go:   // 无解构
来源：http://pfa.yanxiufei.cn

Ruby: a, b = pair
来源：http://zxr.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://wzn.fktsv.cn

[C16] 函数 / 方法重载
来源：http://umc.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ecg.meibo888.top

PHP:  // 无重载
来源：http://asy.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://agk.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://fyi.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nwq.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://qma.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://whi.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qlx.yuxming.cn

================================================================================
来源：http://eib.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://xxg.sweek.top

================================================================================
来源：http://iqj.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://fki.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sjk.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwc.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oly.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xss.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ssm.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://yje.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://fzr.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ohk.sweek.top

[D02] 追加元素到末尾
来源：http://ale.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jso.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rco.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://eab.zhoulong.xyz

TS:   arr.push(4);
来源：http://kep.0kj1m.cn

Java: list.add(4);
来源：http://vsv.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://nmw.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://akg.zdbjq.cn

C#:   list.Add(4);
来源：http://smk.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://nyv.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://syw.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nux.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bdr.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://miu.shzxlz.cn

Java: list.add(0, 0);
来源：http://aab.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://smi.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yvv.yongpay.top

C#:   list.Insert(0, 0);
来源：http://xby.fzhhl.top

[D04] 删除元素
来源：http://hqz.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wwg.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hix.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cir.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://quj.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kpn.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dbw.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://agk.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dat.jqgfzy.top

[D05] 访问与修改元素
来源：http://rho.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wfs.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://muk.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivn.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://qwp.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://beg.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://ham.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jrk.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://low.hcnkem.com

[D06] 数组长度
来源：http://xje.ctjpmb.com

Py:   len(arr)
来源：http://yzs.pengpengdd.cyou

PHP:  count($arr);
来源：http://qsx.zycfv.cn

JS:   arr.length
来源：http://lqw.svipenyu.cn

TS:   arr.length
来源：http://nif.0kj1m.cn

Java: list.size();
来源：http://ank.tianlin.xyz

Go:   len(arr)
来源：http://mwp.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://jfs.chenjidiqi.icu

C#:   list.Count;
来源：http://ygj.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://kch.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://avb.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://krm.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://thb.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://vdv.epnwcf.com

Java: list.subList(1, 4);
来源：http://awm.tian-w.cn

Go:   arr[1:4]
来源：http://ksg.gogol.net.cn

Ruby: arr[1, 3]
来源：http://toe.shzxlz.cn


<!-- 参考信息 -->