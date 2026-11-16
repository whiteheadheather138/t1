代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hum.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://bfm.sweek.top

TS:   while (i < 10) { i++; }
来源：http://ymo.uphjek.com

Java: while (i < 10) { i++; }
来源：http://dky.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ono.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://wbd.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://pzm.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://tbr.yj202588.top

Py:   # 无 do-while：用 while True + break
来源：http://did.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dkr.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://yov.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://hoy.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://zfo.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://txq.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pus.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://yvk.chenzaomai.com

[B09] break 与 continue
来源：http://asf.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bsz.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jwa.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqc.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkp.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldj.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://asn.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qtg.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dnn.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://gyn.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nne.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nqs.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oyd.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mem.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qgi.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wol.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fnu.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cgq.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://nsc.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://uze.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://brc.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hdo.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzw.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uve.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pmz.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://oos.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bky.hfpthk.cn

[B12] 跳出多层循环
来源：http://tgf.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rty.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jsb.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cep.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tjv.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nmv.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uad.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hff.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zml.9152youxi.cn

[B13] 判断是否为数字
来源：http://rwu.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://smn.haohaochexian.top

PHP:  is_numeric($x)
来源：http://raf.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rly.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwv.xziqi.cn

Java: x instanceof Number
来源：http://yhc.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://weq.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://xke.zdbjq.cn

C#:   x is int or double or decimal
来源：http://mnz.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://zyw.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pnw.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hwv.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://qjq.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://wnl.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uxv.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpw.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cag.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://guw.vehdjk.com

[B15] 布尔运算与取反
来源：http://ezb.redwolf501.top

Py:   a and b or not c
来源：http://opq.jianghu66.top

PHP:  $a && $b || !$c
来源：http://ssi.hammf.cn

JS:   a && b || !c
来源：http://osc.ybcxt.top

TS:   a && b || !c
来源：http://nfl.mhx1999.top

Java: a && b || !c
来源：http://hll.jyoumei.cn

Go:   a && b || !c
来源：http://okz.0kj1m.cn

Ruby: a && b || !c
来源：http://pwp.redwolf501.top

C#:   a && b || !c
来源：http://xgs.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://xkg.jinghuilouyu.cn

Py:   if not data: return
来源：http://cge.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://nol.chenzaomai.com

JS:   if (!data) return;
来源：http://dad.yanxiufei.cn

TS:   if (!data) return;
来源：http://pzo.mhx1999.top

Java: if (data == null) return;
来源：http://xbh.yj20258888.top

Go:   if data == nil { return }
来源：http://ngj.pycfn.com

Ruby: return if data.nil?
来源：http://eiv.shzxlz.cn

C#:   if (data == null) return;
来源：http://ttv.shangyingyoupin.top

================================================================================
来源：http://iyb.zhaomingkeji.xyz

C. 函数与作用域
来源：http://mox.xylfe.cn

================================================================================
来源：http://fyr.ivvv.top

[C01] 定义函数
来源：http://pbe.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://xhe.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nou.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://fiu.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgu.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hnb.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tjg.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://cvh.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gxz.yanxiufei.cn

[C02] 默认参数
来源：http://xqt.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://jed.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cgi.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://sbi.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zhz.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://njq.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jsu.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://yud.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://yex.0kj1m.cn

[C03] 可变参数
来源：http://kop.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://thr.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qkt.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://phv.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tnc.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mam.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://boy.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://eau.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://arh.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://jlf.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://awz.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zsh.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wha.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qzb.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://yra.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://zyh.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://xrb.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://vfm.hywenlv.cn

[C05] 返回多个值
来源：http://cih.ybcxt.top

Py:   return a, b
来源：http://oai.hammf.cn

PHP:  return [$a, $b];
来源：http://tcf.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wpn.quarkkingdee.top

TS:   return { a, b };
来源：http://oax.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://age.daria6918.cn

Go:   return a, b
来源：http://ccx.ehwqpu.com

Ruby: return a, b
来源：http://vgt.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://roj.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://tfa.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://ovs.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://slt.fehbvm.com

JS:   const square = x => x * x;
来源：http://fgb.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://avj.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ent.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://cug.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://llg.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kbp.daxiang520.top

[C07] 把函数作为参数传入
来源：http://fdj.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aly.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://vlb.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uik.zhengqikj.top

TS:   arr.map(String)
来源：http://czp.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ccz.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wcu.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://brw.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vrl.fengsongda.top

[C08] 闭包
来源：http://joe.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jsk.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xjo.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwq.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oca.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nzy.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vpo.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fmy.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hiu.shanyushiyangkeji.top

[C09] 递归
来源：http://cde.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ziu.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://leo.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgi.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eaz.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hci.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://klj.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dlq.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wyr.xuanzx.com

[C10] 变量作用域
来源：http://gmw.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hpi.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rrd.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhu.hammf.cn

TS:   同 JS
来源：http://yoj.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://bdd.jiagoushi.top

Go:   花括号块级作用域
来源：http://jqs.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zuy.hfpthk.cn

C#:   块级作用域
来源：http://ogt.yongpay.top

[C11] 模块导入与导出
来源：http://yad.tianlin.xyz

Py:   from module import func
来源：http://ovu.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://exe.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://flf.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uak.aizwys.cn

Java: import java.util.List;
来源：http://uhx.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pwl.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://vxl.havefunace.top

C#:   using System.Text;
来源：http://bih.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://czm.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://fdo.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://ifc.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://vgj.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://hqe.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fnu.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://tss.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://vkg.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://cbn.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://yoo.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qzm.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bxb.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bhc.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wqx.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://maa.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://tmn.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pgw.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://xqo.snrcjt.cn

[C14] 泛型函数
来源：http://fzr.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://moc.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://von.tian-w.cn

JS:   // 无泛型
来源：http://okn.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mye.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xez.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ugl.kuanghao11.cn

Ruby: # 无泛型
来源：http://cgl.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tso.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://xyg.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aun.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://bvm.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://imt.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gor.kuanghao11.cn

Java: // 无解构
来源：http://phn.yj20258888.top

Go:   // 无解构
来源：http://hcy.0kj1m.cn

Ruby: a, b = pair
来源：http://buj.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://bdc.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://qsn.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hth.yj20258888.top

PHP:  // 无重载
来源：http://uyg.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gpk.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://axm.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vul.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://xtz.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://ngb.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ovu.tanke756.top

================================================================================
来源：http://col.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://smv.jiagoushi.top

================================================================================
来源：http://ygp.redwolf501.top

[D01] 创建数组 / 列表
来源：http://vey.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://jqr.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yfv.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://god.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pke.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zze.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://bxu.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://liz.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wbi.0kj1m.cn

[D02] 追加元素到末尾
来源：http://bdu.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mfg.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xbg.dashuyun.cn

JS:   arr.push(4);
来源：http://eer.wangshuangyany.cn

TS:   arr.push(4);
来源：http://jvn.tanke756.top

Java: list.add(4);
来源：http://lfn.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://nub.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://mny.mhx1999.top

C#:   list.Add(4);
来源：http://dbm.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://lep.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://ffi.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mnh.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cqm.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://vaw.fzhhl.top

Java: list.add(0, 0);
来源：http://ayt.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://npi.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oqo.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://cia.epnwcf.com

[D04] 删除元素
来源：http://mko.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eow.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cue.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zjj.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://uxj.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zwe.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xst.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://con.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qfg.52xcode.cn

[D05] 访问与修改元素
来源：http://xpw.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://viw.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hqo.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wib.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://njd.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://voz.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://wuz.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tzb.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cwc.guowangkeji.top

[D06] 数组长度
来源：http://lgy.zdqjudy.top

Py:   len(arr)
来源：http://zwr.jiagoushi.top

PHP:  count($arr);
来源：http://hrc.cheryme.top

JS:   arr.length
来源：http://ill.kuanghao11.cn

TS:   arr.length
来源：http://dya.xylfe.cn

Java: list.size();
来源：http://wsy.uphjek.com

Go:   len(arr)
来源：http://eyx.havefunace.top

Ruby: arr.length; arr.size
来源：http://exy.jyoumei.cn

C#:   list.Count;
来源：http://tay.cucudq.cn

[D07] 切片 / 取子数组
来源：http://hqy.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://usr.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://ryi.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://bnd.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://qel.nanxinkj.top

Java: list.subList(1, 4);
来源：http://oul.c1oappe.top

Go:   arr[1:4]
来源：http://crq.haohaochexian.top

Ruby: arr[1, 3]
来源：http://slx.zhijiandao.cn


<!-- 参考信息 -->