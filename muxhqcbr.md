代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ffm.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ykx.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://bvy.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bel.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://gws.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://byz.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oac.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zcn.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://shu.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ozg.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ens.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://jyu.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zsw.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://fcl.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lmq.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sdb.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cfd.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jfm.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jqz.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hjx.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bmm.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fuc.yueranfly.top

[B07] while 循环
来源：http://dft.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://ryw.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gcv.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://tjl.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://upu.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://fxf.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ddx.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://eak.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://fcq.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://den.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://hni.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uek.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://dby.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://bpb.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://pko.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jtq.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://nft.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://pel.feifeiyinyue.top

[B09] break 与 continue
来源：http://lym.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gaq.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpb.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlh.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://saf.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wub.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sfc.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://byr.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfq.iojbl.cn

[B10] 遍历同时拿索引
来源：http://tve.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kop.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cys.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xzw.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ale.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lmy.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bjb.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://otz.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rrq.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://gfc.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://rjj.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://njt.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rip.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lsq.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gpg.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jlo.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://atc.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zxz.uphjek.com

[B12] 跳出多层循环
来源：http://sau.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://anl.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iwq.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://opr.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zma.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iac.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dic.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oao.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gaq.yuxming.cn

[B13] 判断是否为数字
来源：http://osc.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://qkk.fehbvm.com

PHP:  is_numeric($x)
来源：http://frc.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lwe.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dnp.yfazqb.com

Java: x instanceof Number
来源：http://amd.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uai.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://ehp.xylfe.cn

C#:   x is int or double or decimal
来源：http://wvg.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://kyp.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zwd.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yjk.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://rcr.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://xhh.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tvs.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ckb.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://iwq.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dtq.jianghu66.top

[B15] 布尔运算与取反
来源：http://pbd.hysaishi.cn

Py:   a and b or not c
来源：http://wlz.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://bej.hnxiangtu.top

JS:   a && b || !c
来源：http://fdj.shangyingyoupin.top

TS:   a && b || !c
来源：http://dxb.yuxming.cn

Java: a && b || !c
来源：http://ugw.fanxiaobao.xyz

Go:   a && b || !c
来源：http://cat.sweek.top

Ruby: a && b || !c
来源：http://udl.jyoumei.cn

C#:   a && b || !c
来源：http://tgg.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://cqz.fengsongda.top

Py:   if not data: return
来源：http://fqg.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://zjs.aizwys.cn

JS:   if (!data) return;
来源：http://dbk.zhixingplan.top

TS:   if (!data) return;
来源：http://stv.cqqwz.cn

Java: if (data == null) return;
来源：http://fby.andypj.xyz

Go:   if data == nil { return }
来源：http://wks.cashguo.top

Ruby: return if data.nil?
来源：http://fol.hammf.cn

C#:   if (data == null) return;
来源：http://hgi.vehdjk.com

================================================================================
来源：http://qqb.zhoulong.xyz

C. 函数与作用域
来源：http://gui.zhoulong.xyz

================================================================================
来源：http://glo.gotoacloud.top

[C01] 定义函数
来源：http://mvq.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://hix.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mua.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://fgu.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rzo.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sev.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bgp.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://cjl.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mnb.ybcxt.top

[C02] 默认参数
来源：http://ynx.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://bcs.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pzp.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://uzl.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://luk.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jsc.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hat.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://rkm.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://hlp.mhx1999.top

[C03] 可变参数
来源：http://tfx.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://snl.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rtr.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eks.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nyb.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vbi.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dss.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://avl.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oic.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://dmn.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xns.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pil.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ykb.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxb.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://njk.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://ovm.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://exq.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://lob.gotoacloud.top

[C05] 返回多个值
来源：http://spf.vqdsnc.cn

Py:   return a, b
来源：http://sqt.havefunace.top

PHP:  return [$a, $b];
来源：http://lgo.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qnf.hesvh.cn

TS:   return { a, b };
来源：http://hcs.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tmn.gaohongyu789.top

Go:   return a, b
来源：http://tjf.yanxiufei.cn

Ruby: return a, b
来源：http://ihs.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://wye.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://bib.tanke756.top

Py:   square = lambda x: x * x
来源：http://fah.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://lim.jyoumei.cn

JS:   const square = x => x * x;
来源：http://nbx.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://dta.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qzz.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://jmy.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://nsz.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://dcn.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://xgm.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gve.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://wan.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lhv.chenjidiqi.icu

TS:   arr.map(String)
来源：http://vjz.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pgb.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pmz.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://sbm.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fag.fehbvm.com

[C08] 闭包
来源：http://rxv.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nmw.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://otk.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kqh.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tig.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tgu.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nbk.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wfe.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://txi.kuanghao11.cn

[C09] 递归
来源：http://hcu.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hej.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pth.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uha.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://liu.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pqw.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qfq.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://inn.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xly.xylfe.cn

[C10] 变量作用域
来源：http://kxo.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwr.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zmq.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lvk.chenlongwang.top

TS:   同 JS
来源：http://uli.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://pme.yanxiufei.cn

Go:   花括号块级作用域
来源：http://ges.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gvi.cqqwz.cn

C#:   块级作用域
来源：http://kju.mhx1999.top

[C11] 模块导入与导出
来源：http://qhe.tianlin.xyz

Py:   from module import func
来源：http://wzd.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xep.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jck.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hsn.meibo888.top

Java: import java.util.List;
来源：http://xvh.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rcl.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://smf.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ncj.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://rdw.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://hxe.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://yeb.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://xmn.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://xam.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://loi.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://tfe.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://lew.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://twe.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://xsy.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sxd.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjp.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pnz.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eyn.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://rbe.epnwcf.com

Go:   func add(a, b int) int
来源：http://gkq.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjt.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hzd.gzhubu.top

[C14] 泛型函数
来源：http://fxs.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ccf.yongpay.top

PHP:  // 无泛型
来源：http://mlc.nanxinkj.top

JS:   // 无泛型
来源：http://tvi.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ksj.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rth.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kje.haohaochexian.top

Ruby: # 无泛型
来源：http://zep.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hbr.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://cvi.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vmj.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://vyo.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ugs.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ckl.ivvv.top

Java: // 无解构
来源：http://lha.sysykeji.top

Go:   // 无解构
来源：http://qjy.ctjpmb.com

Ruby: a, b = pair
来源：http://xzo.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://woz.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://tvs.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ywh.zhoulong.xyz

PHP:  // 无重载
来源：http://elx.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gbr.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://tsd.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sje.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://mfw.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://tsq.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vqc.ywan-chungtsiang.top

================================================================================
来源：http://ljr.yonumen.top

D. 数组 / 列表 / 集合
来源：http://tnl.nanxinkj.top

================================================================================
来源：http://kah.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://qfk.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aer.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fki.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fci.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sdt.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zdi.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://nhl.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://hkt.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhd.fehbvm.com

[D02] 追加元素到末尾
来源：http://usl.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pam.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slf.chenjidiqi.icu

JS:   arr.push(4);
来源：http://jha.ehwqpu.com

TS:   arr.push(4);
来源：http://ybi.zhaomingkeji.xyz

Java: list.add(4);
来源：http://xkz.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://akl.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://gwx.yfazqb.com

C#:   list.Add(4);
来源：http://idb.fehbvm.com

[D03] 在指定位置插入元素
来源：http://upr.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://jxk.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cxo.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cbt.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://gyk.shuidangran.top

Java: list.add(0, 0);
来源：http://xha.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://nnr.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ula.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://wpe.quarkkingdee.top

[D04] 删除元素
来源：http://mek.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wuv.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hlt.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnk.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://cdy.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qtb.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jux.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qfk.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ptc.jqgfzy.top

[D05] 访问与修改元素
来源：http://ooo.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ktf.316326.xyz


<!-- 参考信息 -->