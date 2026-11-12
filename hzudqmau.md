代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eod.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjs.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://zuh.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://exv.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://yzb.gzhubu.top

Py:   for item in arr: print(item)
来源：http://ygo.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sjb.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dbw.ydjk.org.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jid.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bnk.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wka.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://hfr.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cfd.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://urk.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hty.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azr.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fqe.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lna.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wdd.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fro.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iya.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nwf.bjfxy.top

[B07] while 循环
来源：http://qsx.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://dcy.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wgp.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://roa.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://vfj.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://mab.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jtc.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://ibl.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://cgi.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://xsl.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://phj.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rsg.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://htn.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://yij.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://rlg.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mcq.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://vej.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://ymn.tarul.cn

[B09] break 与 continue
来源：http://bsj.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nin.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lxr.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thn.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkg.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzo.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lcs.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fde.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llq.hcnkem.com

[B10] 遍历同时拿索引
来源：http://wkm.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvy.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sab.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://esu.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cka.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dme.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://upg.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jtr.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://huw.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://hzc.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://ivr.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://vra.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrl.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://veo.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jqs.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qlp.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://lwv.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ocq.xziqi.cn

[B12] 跳出多层循环
来源：http://pdz.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jaz.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hky.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rot.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xps.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qou.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvr.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dtb.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vqq.hnqzz.top

[B13] 判断是否为数字
来源：http://jkn.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://dzy.ybcxt.top

PHP:  is_numeric($x)
来源：http://jel.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnj.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dvu.hysaishi.cn

Java: x instanceof Number
来源：http://nkv.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uhb.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://fbk.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://oud.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://svl.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dzd.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zbd.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://axy.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://byg.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vlh.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mfz.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ehu.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wvs.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://wow.jqgufenzy.top

Py:   a and b or not c
来源：http://ndx.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://zzr.gzhubu.top

JS:   a && b || !c
来源：http://ipa.ybcxt.top

TS:   a && b || !c
来源：http://ysy.ppjwa.cn

Java: a && b || !c
来源：http://tar.pycfn.com

Go:   a && b || !c
来源：http://ukb.nwbrower.top

Ruby: a && b || !c
来源：http://mwu.zdqjudy.top

C#:   a && b || !c
来源：http://hzy.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://aso.hcnkem.com

Py:   if not data: return
来源：http://kga.cashguo.top

PHP:  if (!$data) { return; }
来源：http://shh.xinyue.icu

JS:   if (!data) return;
来源：http://qew.andypj.xyz

TS:   if (!data) return;
来源：http://jmj.smart0.xyz

Java: if (data == null) return;
来源：http://ewy.cdnleiting.top

Go:   if data == nil { return }
来源：http://gfr.shuidangran.top

Ruby: return if data.nil?
来源：http://yva.fzhhl.top

C#:   if (data == null) return;
来源：http://igj.nanxuanxn.top

================================================================================
来源：http://ene.sysykeji.top

C. 函数与作用域
来源：http://dtb.ivvv.top

================================================================================
来源：http://lkn.zhiwuduotai.top

[C01] 定义函数
来源：http://smq.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://hmw.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnh.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://lgz.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pae.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yqy.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ptw.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://crq.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bnm.jqgufenzy.top

[C02] 默认参数
来源：http://ups.birdmap.top

Py:   def greet(name="World"): return name
来源：http://rbf.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://syc.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://ibo.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ord.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lbx.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yec.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://amk.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://gcc.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://dhj.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://kld.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xqd.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xgw.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymc.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uev.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyi.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://hwo.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yra.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://jcf.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zyj.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qso.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vfs.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jdp.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://okx.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://gdn.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://hvc.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://wge.xylfe.cn

[C05] 返回多个值
来源：http://itl.nwbrower.top

Py:   return a, b
来源：http://fjk.0kj1m.cn

PHP:  return [$a, $b];
来源：http://hrj.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lfh.cheryme.top

TS:   return { a, b };
来源：http://vjm.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rhs.nanxuanxn.top

Go:   return a, b
来源：http://mrk.hcnkem.com

Ruby: return a, b
来源：http://voh.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://eqm.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://gho.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://alp.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://plh.sweek.top

JS:   const square = x => x * x;
来源：http://moi.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://srr.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rqz.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://liz.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://yqr.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ooz.fehbvm.com

[C07] 把函数作为参数传入
来源：http://vsv.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vph.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://yar.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dor.hfpthk.cn

TS:   arr.map(String)
来源：http://zuu.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cnq.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nji.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://qqb.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dro.zhoulong.xyz

[C08] 闭包
来源：http://ycu.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rus.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hgq.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uls.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ofk.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://euk.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bnc.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnt.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cwj.feifeiyinyue.top

[C09] 递归
来源：http://ype.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://biw.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rla.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kdz.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpj.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://exj.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mxc.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://udf.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://odo.zhixingplan.top

[C10] 变量作用域
来源：http://srg.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ind.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xol.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ere.jqgufenzy.top

TS:   同 JS
来源：http://zjg.ivvv.top

Java: 方法内为块级作用域
来源：http://wav.svipenyu.cn

Go:   花括号块级作用域
来源：http://xqj.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cff.yj20258888.top

C#:   块级作用域
来源：http://zmd.cdnleiting.top

[C11] 模块导入与导出
来源：http://uwy.zhengqikj.top

Py:   from module import func
来源：http://suq.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rvd.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wri.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zcq.cdnleiting.top

Java: import java.util.List;
来源：http://ajw.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mdq.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://vxs.hysaishi.cn

C#:   using System.Text;
来源：http://jgp.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://jsu.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://qgc.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://vul.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://wqp.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://zbb.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pln.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://log.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://gff.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://riy.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://gyh.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bbw.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://enq.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dav.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccl.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://mlb.guowangkeji.top

Go:   func add(a, b int) int
来源：http://ffn.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ayg.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://lfi.yonumen.top

[C14] 泛型函数
来源：http://nyd.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yno.sufxvd.cn

PHP:  // 无泛型
来源：http://gvu.tanke756.top

JS:   // 无泛型
来源：http://coe.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dkn.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yes.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jsf.xinyue.icu

Ruby: # 无泛型
来源：http://uvb.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dub.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://gle.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xjd.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://ijv.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nit.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rxc.hysaishi.cn

Java: // 无解构
来源：http://coh.yvedp.cn

Go:   // 无解构
来源：http://nqg.yfazqb.com

Ruby: a, b = pair
来源：http://tta.yueranfly.top

C#:   var (a, b) = pair;
来源：http://qkm.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://wgw.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wzo.feifeiyinyue.top

PHP:  // 无重载
来源：http://jdr.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ngp.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://aju.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nyr.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://qva.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://auk.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dri.sjlbkw.cn

================================================================================
来源：http://lfj.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://wsb.ywan-chungtsiang.top

================================================================================
来源：http://xve.xuanzx.com

[D01] 创建数组 / 列表
来源：http://qsn.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://rfr.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xzf.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cis.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://szb.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uqm.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://mpg.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://qkr.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qcr.andypj.xyz

[D02] 追加元素到末尾
来源：http://dlp.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vjk.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qgh.quarkkingdee.top

JS:   arr.push(4);
来源：http://sxl.ydzc1.top

TS:   arr.push(4);
来源：http://ogs.epnwcf.com

Java: list.add(4);
来源：http://kyg.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://dzg.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://ubj.snrcjt.cn

C#:   list.Add(4);
来源：http://bee.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://quv.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://gxo.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvq.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lpu.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://lkl.yj202588.top

Java: list.add(0, 0);
来源：http://sbs.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lll.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://njp.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://wvn.zycfv.cn

[D04] 删除元素
来源：http://fqf.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gve.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://axo.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvy.ivvv.top

TS:   arr.splice(0, 1);
来源：http://xgp.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pns.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vek.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tkh.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://edn.9152youxi.cn

[D05] 访问与修改元素
来源：http://aak.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfq.cdnleiting.top


<!-- 参考信息 -->