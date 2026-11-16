代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dol.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://npv.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://jls.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://qel.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://krc.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://evd.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://rdv.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://whi.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://zry.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://guj.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://kcu.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://aso.nanxuanxn.top

[B09] break 与 continue
来源：http://usr.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nlk.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wwn.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cob.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzz.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhm.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zbx.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uzc.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjn.fengsongda.top

[B10] 遍历同时拿索引
来源：http://rdx.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qpg.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fis.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ptw.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uwc.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mkt.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwm.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xtm.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://njd.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://rua.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://cyp.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://ztt.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyc.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fjy.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qfj.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sdt.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://iqk.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ydt.c1oappe.top

[B12] 跳出多层循环
来源：http://ijh.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rld.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mpe.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nll.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xvv.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bkh.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://efo.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ocz.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zfr.c1oappe.top

[B13] 判断是否为数字
来源：http://afk.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://pjc.cqqwz.cn

PHP:  is_numeric($x)
来源：http://nrd.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mwh.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hfl.zhoulong.xyz

Java: x instanceof Number
来源：http://hfy.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nbe.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://rzr.316326.xyz

C#:   x is int or double or decimal
来源：http://riq.sweek.top

[B14] 判断值是否在集合内
来源：http://zai.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tuh.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sos.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://eso.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://psp.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://blh.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yuv.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nne.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zxl.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://tnz.ehwqpu.com

Py:   a and b or not c
来源：http://hdr.xinyue.icu

PHP:  $a && $b || !$c
来源：http://skm.jqgfzy.top

JS:   a && b || !c
来源：http://gjh.jlsjyb.cn

TS:   a && b || !c
来源：http://caw.shanyushiyangkeji.top

Java: a && b || !c
来源：http://hmf.hammf.cn

Go:   a && b || !c
来源：http://ziv.cashguo.top

Ruby: a && b || !c
来源：http://xyd.jyoumei.cn

C#:   a && b || !c
来源：http://nms.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jtv.hnxiangtu.top

Py:   if not data: return
来源：http://qru.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://elr.dianchejie.cn

JS:   if (!data) return;
来源：http://jjb.pengpengdd.cyou

TS:   if (!data) return;
来源：http://dfz.sweek.top

Java: if (data == null) return;
来源：http://kfw.zdbjq.cn

Go:   if data == nil { return }
来源：http://ypq.hesvh.cn

Ruby: return if data.nil?
来源：http://gqb.sufxvd.cn

C#:   if (data == null) return;
来源：http://hlx.jiagoushi.top

================================================================================
来源：http://zdb.jyoumei.cn

C. 函数与作用域
来源：http://lpa.hcnkem.com

================================================================================
来源：http://pjb.ydzc1.top

[C01] 定义函数
来源：http://fsg.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://fie.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oda.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://gli.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hot.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tkf.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://mqy.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://amp.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oxe.xylfe.cn

[C02] 默认参数
来源：http://meu.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://vrb.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rir.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://naq.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oif.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tcm.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cyc.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://rxw.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://rvn.shanyushiyangkeji.top

[C03] 可变参数
来源：http://unc.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://viy.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hox.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lss.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qae.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nes.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nwt.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://emv.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cyf.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://ffz.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iei.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nav.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rph.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rog.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://duc.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://khr.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://aye.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://zqw.pycfn.com

[C05] 返回多个值
来源：http://qll.ivvv.top

Py:   return a, b
来源：http://pji.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://pzk.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://apa.yfazqb.com

TS:   return { a, b };
来源：http://jea.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fqd.xylfe.cn

Go:   return a, b
来源：http://wfi.shangyingyoupin.top

Ruby: return a, b
来源：http://lyv.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://vlv.havefunace.top

[C06] 匿名函数 / lambda
来源：http://jfb.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://qjk.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://qwg.yueranfly.top

JS:   const square = x => x * x;
来源：http://qif.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://dgk.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vjf.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://nii.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://nxq.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://koz.havefunace.top

[C07] 把函数作为参数传入
来源：http://vqb.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://doq.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://nzy.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rvh.gogol.net.cn

TS:   arr.map(String)
来源：http://eml.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mxd.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ynq.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://udw.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ecy.chenzaomai.com

[C08] 闭包
来源：http://lzh.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pnh.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://udm.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kxa.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gvk.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jce.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bxb.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://agv.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://brh.yangfankeji.com

[C09] 递归
来源：http://rom.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esf.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gsg.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sry.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpl.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hte.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://euu.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jkq.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oli.xziqi.cn

[C10] 变量作用域
来源：http://ziy.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gnq.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://css.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ydv.sweek.top

TS:   同 JS
来源：http://dou.yvedp.cn

Java: 方法内为块级作用域
来源：http://icj.yanxiufei.cn

Go:   花括号块级作用域
来源：http://lay.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yso.sufxvd.cn

C#:   块级作用域
来源：http://owp.sysykeji.top

[C11] 模块导入与导出
来源：http://txz.sysykeji.top

Py:   from module import func
来源：http://nyq.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bpc.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rwl.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://szb.zhixingplan.top

Java: import java.util.List;
来源：http://rof.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bfr.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://awk.aizwys.cn

C#:   using System.Text;
来源：http://wyd.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://ijf.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://lqc.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://rxa.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://juf.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://bsg.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://equ.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ptn.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://wgk.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oel.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://wtd.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sxt.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghn.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sbz.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ifs.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://tdf.c1oappe.top

Go:   func add(a, b int) int
来源：http://ebd.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qss.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://hea.hfpthk.cn

[C14] 泛型函数
来源：http://utv.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://udy.yanxiufei.cn

PHP:  // 无泛型
来源：http://tcd.c1oappe.top

JS:   // 无泛型
来源：http://rxr.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://guc.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ybj.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://srh.jqgufenzy.top

Ruby: # 无泛型
来源：http://hhj.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ocy.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://yzb.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gcc.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://mnn.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ksv.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jja.bbcook.cn

Java: // 无解构
来源：http://tqu.yonumen.top

Go:   // 无解构
来源：http://zyb.ybcxt.top

Ruby: a, b = pair
来源：http://yuq.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://nct.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://stw.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xfo.xuanzx.com

PHP:  // 无重载
来源：http://ndv.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lqt.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://fbt.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fct.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://lqw.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://hoe.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://srt.xingfuxueyuan.xyz

================================================================================
来源：http://zky.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://roh.jinqigfzy.top

================================================================================
来源：http://fzw.ydzc1.top

[D01] 创建数组 / 列表
来源：http://yfe.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://htn.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ehd.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ztg.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oim.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kil.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://tic.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://emj.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hew.gogol.net.cn

[D02] 追加元素到末尾
来源：http://isu.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fzb.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lud.cucudq.cn

JS:   arr.push(4);
来源：http://kek.guannengcc.top

TS:   arr.push(4);
来源：http://igv.yuanzhike.top

Java: list.add(4);
来源：http://lad.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://dro.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://alt.mhx1999.top

C#:   list.Add(4);
来源：http://jlm.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://rdb.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://ywg.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jkr.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eme.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://tlf.hnqzz.top

Java: list.add(0, 0);
来源：http://mmn.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ehk.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uku.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://lgw.0kj1m.cn

[D04] 删除元素
来源：http://uof.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://voe.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vhz.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lkk.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://kow.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rcj.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wty.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dyv.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rhd.sxryk.cn

[D05] 访问与修改元素
来源：http://vfg.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tfl.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://scm.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcq.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://zfr.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://nbf.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://esf.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tue.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hnr.nwbrower.top

[D06] 数组长度
来源：http://pzm.yueranfly.top

Py:   len(arr)
来源：http://hvo.hfpthk.cn

PHP:  count($arr);
来源：http://gez.sufxvd.cn

JS:   arr.length
来源：http://hfh.uphjek.com

TS:   arr.length
来源：http://uen.mhx1999.top

Java: list.size();
来源：http://xta.jinqigufen.top

Go:   len(arr)
来源：http://dcv.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://ugo.sysykeji.top

C#:   list.Count;
来源：http://fqo.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://lej.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mtz.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eto.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://opo.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://gia.hammf.cn

Java: list.subList(1, 4);
来源：http://vbe.yongpay.top

Go:   arr[1:4]
来源：http://sym.9152youxi.cn

Ruby: arr[1, 3]
来源：http://htg.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://zet.hywenlv.cn

[D08] 合并两个数组
来源：http://psp.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://brp.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://yxg.ydjk.org.cn


<!-- 参考信息 -->