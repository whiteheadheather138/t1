代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://jwl.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://lfr.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://isi.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://nch.zhengqikj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://abb.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://mhe.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://jra.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://woq.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://xmv.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rze.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://cqc.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://wnb.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://wgb.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://dnd.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sbv.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://mxx.cucudq.cn

[B09] break 与 continue
来源：http://syv.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rtc.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rua.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnl.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ges.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjo.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://igj.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tpd.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uki.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://yhy.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xmx.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ogs.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fii.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yuk.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ezd.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cln.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zpw.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mmd.sweek.top

[B11] 生成数字序列 / 区间
来源：http://vxl.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://ckk.316326.xyz

PHP:  range(0, 10, 2);
来源：http://smn.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yed.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jyn.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ysj.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgz.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://stq.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://avq.chenzaomai.com

[B12] 跳出多层循环
来源：http://uqw.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lbt.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://mol.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ukk.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyg.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kjj.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppi.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxu.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fqd.hfpthk.cn

[B13] 判断是否为数字
来源：http://fqu.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://ffg.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://tli.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://odj.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fsh.ydjk.org.cn

Java: x instanceof Number
来源：http://ldg.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kcr.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://yng.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://meq.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://rea.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://owx.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfr.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://bkz.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://rrq.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vbu.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sah.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://sbp.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vnj.epnwcf.com

[B15] 布尔运算与取反
来源：http://due.uphjek.com

Py:   a and b or not c
来源：http://spm.316326.xyz

PHP:  $a && $b || !$c
来源：http://bdk.shzxlz.cn

JS:   a && b || !c
来源：http://mja.shangyingyoupin.top

TS:   a && b || !c
来源：http://arm.nanxinkj.top

Java: a && b || !c
来源：http://bok.hongshengwenyu.top

Go:   a && b || !c
来源：http://jmu.xuetiantiany.cn

Ruby: a && b || !c
来源：http://iop.ybcxt.top

C#:   a && b || !c
来源：http://jrq.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://ket.zhengqikj.top

Py:   if not data: return
来源：http://gzf.yongpay.top

PHP:  if (!$data) { return; }
来源：http://zpg.9152youxi.cn

JS:   if (!data) return;
来源：http://rxj.snrcjt.cn

TS:   if (!data) return;
来源：http://dsn.yueranfly.top

Java: if (data == null) return;
来源：http://pec.chenlongwang.top

Go:   if data == nil { return }
来源：http://sqr.zhengqikj.top

Ruby: return if data.nil?
来源：http://nsz.c1oappe.top

C#:   if (data == null) return;
来源：http://gky.aizwys.cn

================================================================================
来源：http://nwb.hammf.cn

C. 函数与作用域
来源：http://tmp.dianchejie.cn

================================================================================
来源：http://ukv.chenlongwang.top

[C01] 定义函数
来源：http://uuo.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://nbz.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tkw.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://mai.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hyv.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pgb.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://nct.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://pfn.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bnz.feifeiyinyue.top

[C02] 默认参数
来源：http://zgm.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://xjn.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bzu.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://bub.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://agl.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://fef.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dzd.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://kxe.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://hig.fanxiaobao.xyz

[C03] 可变参数
来源：http://ktx.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://lok.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xhc.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sey.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fgf.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fkv.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pvo.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://qzp.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mil.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://fwz.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dpk.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ikn.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hrt.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dvf.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://ekw.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://kqx.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://rby.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://ift.hongshengwenyu.top

[C05] 返回多个值
来源：http://eyx.tarul.cn

Py:   return a, b
来源：http://geq.yongpay.top

PHP:  return [$a, $b];
来源：http://iob.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bww.vehdjk.com

TS:   return { a, b };
来源：http://ams.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sjy.xuanzx.com

Go:   return a, b
来源：http://jbg.zycfv.cn

Ruby: return a, b
来源：http://uue.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://fue.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://kxa.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://nbh.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://drg.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://bbr.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://sow.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tlv.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wbq.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://bca.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://edv.iojbl.cn

[C07] 把函数作为参数传入
来源：http://art.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rva.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nsx.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ymw.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://ryj.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tsn.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vle.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://evm.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dlr.zhongyouzk.top

[C08] 闭包
来源：http://onr.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fqt.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://psx.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://adr.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vpr.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jlz.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wza.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bcv.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uwq.zhengqikj.top

[C09] 递归
来源：http://vku.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qcj.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vip.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzh.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eob.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsj.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ron.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://umu.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vvf.jqgfzy.top

[C10] 变量作用域
来源：http://fnl.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lri.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cdo.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahc.xingfuxueyuan.xyz

TS:   同 JS
来源：http://awy.mhx1999.top

Java: 方法内为块级作用域
来源：http://wmf.gogol.net.cn

Go:   花括号块级作用域
来源：http://tgv.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://agl.uphjek.com

C#:   块级作用域
来源：http://cqi.316326.xyz

[C11] 模块导入与导出
来源：http://jkw.ydzc1.top

Py:   from module import func
来源：http://gra.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pqz.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ufv.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zuo.jqgufenzy.top

Java: import java.util.List;
来源：http://bkt.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://upa.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://xkj.c1oappe.top

C#:   using System.Text;
来源：http://qjv.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://hmx.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://arc.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://ons.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://vsm.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://qzm.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://grq.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ivj.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://tdd.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bga.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://huc.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://etd.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzk.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lzs.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ylx.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://wru.jyoumei.cn

Go:   func add(a, b int) int
来源：http://dup.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://now.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://zpi.havefunace.top

[C14] 泛型函数
来源：http://khy.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzl.guannengcc.top

PHP:  // 无泛型
来源：http://vnv.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://pnp.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tht.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nrd.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tpf.chenlongwang.top

Ruby: # 无泛型
来源：http://tsx.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ins.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://rug.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://usz.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://rrr.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tvs.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pcm.cdnleiting.top

Java: // 无解构
来源：http://fop.tian-w.cn

Go:   // 无解构
来源：http://ytl.smart0.xyz

Ruby: a, b = pair
来源：http://ulu.smart0.xyz

C#:   var (a, b) = pair;
来源：http://pos.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://dwv.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cqy.sufxvd.cn

PHP:  // 无重载
来源：http://mas.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qat.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://zwf.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kdw.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://obm.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://swd.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://elv.aibaodan.cn

================================================================================
来源：http://nbn.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://eze.smart0.xyz

================================================================================
来源：http://vwy.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://dqg.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hdw.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://swx.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lnd.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sud.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpe.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://dpa.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://mzi.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://agl.fehbvm.com

[D02] 追加元素到末尾
来源：http://rtf.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ezr.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cjf.yvedp.cn

JS:   arr.push(4);
来源：http://wcu.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://xrt.jyoumei.cn

Java: list.add(4);
来源：http://dwm.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://guk.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://odd.tarul.cn

C#:   list.Add(4);
来源：http://lor.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://ikt.uphjek.com

Py:   arr.insert(0, 0)
来源：http://mkc.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kar.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvm.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://hmt.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://gfx.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rlc.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mxo.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://jvw.sxryk.cn

[D04] 删除元素
来源：http://zgo.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jgk.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wiz.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fuw.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://lkh.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ugv.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wcz.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://soe.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tfj.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://otv.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uqr.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmf.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dzq.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://mrg.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://win.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://abj.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qej.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nxp.chenlongwang.top

[D06] 数组长度
来源：http://hxj.daxiang520.top

Py:   len(arr)
来源：http://oxx.wangshuangyany.cn

PHP:  count($arr);
来源：http://tpi.hcnkem.com

JS:   arr.length
来源：http://fyr.cdnleiting.top

TS:   arr.length
来源：http://cme.yvedp.cn

Java: list.size();
来源：http://zfs.hammf.cn

Go:   len(arr)
来源：http://psi.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://hnc.cqqwz.cn

C#:   list.Count;
来源：http://lkl.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://jct.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ivt.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://qwi.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://ryx.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://fzy.gzhubu.top

Java: list.subList(1, 4);
来源：http://wkl.guowangkeji.top

Go:   arr[1:4]
来源：http://ucg.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://jpa.guowangkeji.top


<!-- 参考信息 -->