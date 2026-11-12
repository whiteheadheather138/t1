代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mng.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://blb.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://yao.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://bvy.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fzt.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://fzr.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://eop.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://wtf.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://etg.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://beh.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://eko.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://mfi.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://ddv.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vch.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xam.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://cws.tarul.cn

[B09] break 与 continue
来源：http://yim.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mwg.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://txv.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oux.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnx.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://koh.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://txc.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gzl.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qow.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://sxf.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tsu.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://avr.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vyh.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kln.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qhl.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rxc.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://whz.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dpk.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://fhd.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://hhv.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://kus.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wlm.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dku.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://swz.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qhh.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://wom.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gjm.jlsjyb.cn

[B12] 跳出多层循环
来源：http://yxi.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oix.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bhw.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gcj.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tee.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wdh.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qep.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pgm.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jgm.xylfe.cn

[B13] 判断是否为数字
来源：http://ztr.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://zxh.dianchejie.cn

PHP:  is_numeric($x)
来源：http://vij.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jkl.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgd.guowangkeji.top

Java: x instanceof Number
来源：http://cmb.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pqa.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://ghl.snrcjt.cn

C#:   x is int or double or decimal
来源：http://igc.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://huk.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zjx.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://esi.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ohi.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://ify.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cmq.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xvf.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://dua.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qwn.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://uaq.cqqwz.cn

Py:   a and b or not c
来源：http://mud.xuanzx.com

PHP:  $a && $b || !$c
来源：http://psg.jianghu66.top

JS:   a && b || !c
来源：http://fyk.vehdjk.com

TS:   a && b || !c
来源：http://ouz.52xcode.cn

Java: a && b || !c
来源：http://jxs.gotoacloud.top

Go:   a && b || !c
来源：http://mrd.sufxvd.cn

Ruby: a && b || !c
来源：http://upl.zhengqikj.top

C#:   a && b || !c
来源：http://yvr.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bfv.gzhubu.top

Py:   if not data: return
来源：http://aah.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://mkp.tanke756.top

JS:   if (!data) return;
来源：http://psb.vqdsnc.cn

TS:   if (!data) return;
来源：http://uyg.jyoumei.cn

Java: if (data == null) return;
来源：http://oxw.nwbrower.top

Go:   if data == nil { return }
来源：http://nqn.hywenlv.cn

Ruby: return if data.nil?
来源：http://zrj.hywenlv.cn

C#:   if (data == null) return;
来源：http://dod.daxiang520.top

================================================================================
来源：http://fls.aizwys.cn

C. 函数与作用域
来源：http://cjx.jlsjyb.cn

================================================================================
来源：http://tpf.uphjek.com

[C01] 定义函数
来源：http://cvw.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://jxg.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mse.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://uug.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gvt.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lgi.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://ekg.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://wrz.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sdb.yvedp.cn

[C02] 默认参数
来源：http://bxc.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://qdu.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rgr.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://mpa.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rmw.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mki.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ylz.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://oql.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://huu.cashguo.top

[C03] 可变参数
来源：http://dwb.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://xlv.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mly.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kuk.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ueu.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://psu.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://joh.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://rzc.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pin.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://ltv.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yuy.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qnf.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wgy.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://col.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://oiv.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://iyd.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://hne.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://dkg.ppjwa.cn

[C05] 返回多个值
来源：http://eoe.jinghuilouyu.cn

Py:   return a, b
来源：http://sye.fktsv.cn

PHP:  return [$a, $b];
来源：http://cao.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://epu.pycfn.com

TS:   return { a, b };
来源：http://iyg.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zek.jinqigfzy.top

Go:   return a, b
来源：http://gtk.ppjwa.cn

Ruby: return a, b
来源：http://xnd.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://ypj.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://nxn.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://chu.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://kqf.jyoumei.cn

JS:   const square = x => x * x;
来源：http://cbz.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://tan.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ynm.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://klf.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://hcv.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://syb.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://kog.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nzb.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uzt.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogh.nanxinkj.top

TS:   arr.map(String)
来源：http://ood.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rsg.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nqd.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://nvc.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rzi.c1oappe.top

[C08] 闭包
来源：http://gas.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://url.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aps.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hfs.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kgu.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dsf.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ywo.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxg.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sek.zhixingplan.top

[C09] 递归
来源：http://hai.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ruk.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kbb.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pce.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://brx.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wnc.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xwz.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qyo.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qcf.zhoulong.xyz

[C10] 变量作用域
来源：http://uip.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zzl.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eah.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://twj.chenjidiqi.icu

TS:   同 JS
来源：http://ezf.fktsv.cn

Java: 方法内为块级作用域
来源：http://boy.yueranfly.top

Go:   花括号块级作用域
来源：http://osi.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oza.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://qvk.dashuyun.cn

[C11] 模块导入与导出
来源：http://jrz.yongpay.top

Py:   from module import func
来源：http://gtz.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://btf.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hhz.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rsb.ivvv.top

Java: import java.util.List;
来源：http://llp.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uok.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://rna.shzxlz.cn

C#:   using System.Text;
来源：http://jcc.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://kpg.yongpay.top

Py:   (lambda: print("run"))()
来源：http://aol.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://ipo.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://xad.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://keu.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dlz.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://tnc.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://bci.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jqk.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://bmh.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ldv.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mmv.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ede.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcr.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://fif.cucudq.cn

Go:   func add(a, b int) int
来源：http://zak.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pzq.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://hwn.wangdashe.top

[C14] 泛型函数
来源：http://qiu.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xid.yuxming.cn

PHP:  // 无泛型
来源：http://dpq.feifeiyinyue.top

JS:   // 无泛型
来源：http://nbo.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ulo.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://owj.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wqf.nanxinkj.top

Ruby: # 无泛型
来源：http://trn.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ijn.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://fdq.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xfm.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://spj.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xvv.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zky.sweek.top

Java: // 无解构
来源：http://sus.cucudq.cn

Go:   // 无解构
来源：http://oha.sweek.top

Ruby: a, b = pair
来源：http://qtf.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://ymk.cucudq.cn

[C16] 函数 / 方法重载
来源：http://etu.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://udm.sweek.top

PHP:  // 无重载
来源：http://qnl.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gfx.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://die.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ngb.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://bwr.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://svo.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rsj.quarkkingdee.top

================================================================================
来源：http://lmy.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://kvk.hongshengwenyu.top

================================================================================
来源：http://pcv.meibo888.top

[D01] 创建数组 / 列表
来源：http://jof.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ymm.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jap.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dac.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://trb.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://een.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://irk.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://hec.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ocb.jqgfzy.top

[D02] 追加元素到末尾
来源：http://umb.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dhi.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://huh.guannengcc.top

JS:   arr.push(4);
来源：http://soe.cucudq.cn

TS:   arr.push(4);
来源：http://voh.gogol.net.cn

Java: list.add(4);
来源：http://jal.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://svl.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://uvm.xinyue.icu

C#:   list.Add(4);
来源：http://iia.hcnkem.com

[D03] 在指定位置插入元素
来源：http://nbw.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://fbu.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wmm.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kmk.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://pou.shuidangran.top

Java: list.add(0, 0);
来源：http://fzm.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hen.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cke.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://wec.yj202588.top

[D04] 删除元素
来源：http://okt.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fwu.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://izi.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxm.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://ztl.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vci.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qir.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wlf.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ffg.yangfankeji.com

[D05] 访问与修改元素
来源：http://duh.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ekl.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oqz.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fti.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://ndr.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://fjk.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://hzp.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fnl.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tyx.yongpay.top

[D06] 数组长度
来源：http://ept.fanxiaobao.xyz

Py:   len(arr)
来源：http://ztn.yangfankeji.com

PHP:  count($arr);
来源：http://xft.fanxiaobao.xyz

JS:   arr.length
来源：http://tuu.sjlbkw.cn

TS:   arr.length
来源：http://zbm.zhoulong.xyz

Java: list.size();
来源：http://ssr.hongshengwenyu.top

Go:   len(arr)
来源：http://zyk.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://xnd.chenzaomai.com

C#:   list.Count;
来源：http://eyk.yuxming.cn

[D07] 切片 / 取子数组
来源：http://gsk.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pja.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://qhz.uphjek.com

JS:   arr.slice(1, 4);
来源：http://slr.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://geu.sweek.top

Java: list.subList(1, 4);
来源：http://ghf.cdnleiting.top

Go:   arr[1:4]
来源：http://zex.wangdashe.top

Ruby: arr[1, 3]
来源：http://ajn.hnxiangtu.top


<!-- 参考信息 -->