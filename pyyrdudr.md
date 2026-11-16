代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ehm.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mmh.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jzf.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtj.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vku.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://erh.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://ejs.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nri.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://jqs.tanke756.top

Py:   for item in arr: print(item)
来源：http://fbi.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cam.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://emr.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hii.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://frv.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gaj.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://dtg.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://koe.hammf.cn

[B06] 遍历字典 / 对象
来源：http://sdt.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rgo.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdk.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ucf.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tuw.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mix.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tog.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mxe.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://weh.haohaochexian.top

[B07] while 循环
来源：http://zfo.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://spz.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://zcq.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://jbw.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://ext.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://qpr.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qxn.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://esr.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://ale.sweek.top

[B08] do-while（至少执行一次）
来源：http://hcj.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://xvg.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://fkt.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://cwf.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://lvg.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://awn.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mxc.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://vbj.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://ijq.ctjpmb.com

[B09] break 与 continue
来源：http://fkq.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nst.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hie.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pan.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmm.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhm.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fal.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pkr.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnt.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://rol.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pcb.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nqc.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fje.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vbe.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lcn.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hmk.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sht.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xpk.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://vdf.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://cvf.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://ffj.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lna.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uan.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uxe.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wlh.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://nnj.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kqg.xylfe.cn

[B12] 跳出多层循环
来源：http://mrb.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dim.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://enq.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eaw.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://axr.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://akt.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppx.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qej.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zvv.smart0.xyz

[B13] 判断是否为数字
来源：http://ric.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://wkl.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://ahh.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jcj.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbs.jqgfzy.top

Java: x instanceof Number
来源：http://guc.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zhg.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://naa.hysaishi.cn

C#:   x is int or double or decimal
来源：http://rtg.yongpay.top

[B14] 判断值是否在集合内
来源：http://lwc.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eeq.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qoh.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://afy.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://bip.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kjj.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xnl.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mhu.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cld.fzhhl.top

[B15] 布尔运算与取反
来源：http://hfw.shuidangran.top

Py:   a and b or not c
来源：http://jba.wangdashe.top

PHP:  $a && $b || !$c
来源：http://exe.cqqwz.cn

JS:   a && b || !c
来源：http://hfy.shzxlz.cn

TS:   a && b || !c
来源：http://kem.jlsjyb.cn

Java: a && b || !c
来源：http://iow.fanxiaobao.xyz

Go:   a && b || !c
来源：http://ykj.cashguo.top

Ruby: a && b || !c
来源：http://rfc.shangyingyoupin.top

C#:   a && b || !c
来源：http://ggl.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://lkd.jyoumei.cn

Py:   if not data: return
来源：http://qxw.meibo888.top

PHP:  if (!$data) { return; }
来源：http://ayo.ydjk.org.cn

JS:   if (!data) return;
来源：http://dek.bbcook.cn

TS:   if (!data) return;
来源：http://qsz.jyoumei.cn

Java: if (data == null) return;
来源：http://wbp.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://war.sjlbkw.cn

Ruby: return if data.nil?
来源：http://ojg.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://qcb.jianghu66.top

================================================================================
来源：http://grc.birdmap.top

C. 函数与作用域
来源：http://vie.xinyue.icu

================================================================================
来源：http://zmy.wangdashe.top

[C01] 定义函数
来源：http://ojz.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://rhf.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbf.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://hnp.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpa.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yql.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://ass.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://kad.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://icz.zycfv.cn

[C02] 默认参数
来源：http://ggz.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://lab.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ehx.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://rgz.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qdt.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qmj.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://suy.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://yrl.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://shc.yj20258888.top

[C03] 可变参数
来源：http://sen.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://kzb.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rwp.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://klf.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lsf.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oem.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rzg.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://fff.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nir.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://lmy.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lmn.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ioq.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dwy.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fwf.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://bfl.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://tte.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://msz.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://zyy.andypj.xyz

[C05] 返回多个值
来源：http://ttx.hnxiangtu.top

Py:   return a, b
来源：http://fyu.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://tzo.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zeh.fengsongda.top

TS:   return { a, b };
来源：http://ifz.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cnz.gotoacloud.top

Go:   return a, b
来源：http://ifd.tanke756.top

Ruby: return a, b
来源：http://chf.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://nxq.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://tzc.xziqi.cn

Py:   square = lambda x: x * x
来源：http://txf.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dxu.fengsongda.top

JS:   const square = x => x * x;
来源：http://oby.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://itv.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vsz.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vlm.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://oqu.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://aif.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://xqj.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ofb.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://qph.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yxb.hongshengwenyu.top

TS:   arr.map(String)
来源：http://eip.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mmj.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hxe.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://gsw.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://udk.redwolf501.top

[C08] 闭包
来源：http://bwl.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lak.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mky.iojbl.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zyt.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wup.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ved.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xgm.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hsb.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gjg.hysaishi.cn

[C09] 递归
来源：http://cgv.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pyj.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zyj.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqx.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://csj.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vnw.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xsf.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ubj.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sid.fktsv.cn

[C10] 变量作用域
来源：http://phe.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yeg.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rkg.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nse.tian-w.cn

TS:   同 JS
来源：http://cvn.jiagoushi.top

Java: 方法内为块级作用域
来源：http://kfr.epnwcf.com

Go:   花括号块级作用域
来源：http://sue.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rkx.zdqjudy.top

C#:   块级作用域
来源：http://fjs.snrcjt.cn

[C11] 模块导入与导出
来源：http://ftu.uphjek.com

Py:   from module import func
来源：http://qmc.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hzv.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvd.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ebr.aizwys.cn

Java: import java.util.List;
来源：http://ldy.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ykz.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://nwe.zhiwuduotai.top

C#:   using System.Text;
来源：http://epm.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://cai.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://izp.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://cmd.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://rzu.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://rcx.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlb.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://ecp.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://mzc.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://apd.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://rbt.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qvf.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmc.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xee.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://drb.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://dng.dianchejie.cn

Go:   func add(a, b int) int
来源：http://coi.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iad.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://xqz.jianghu66.top

[C14] 泛型函数
来源：http://vfc.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qjo.0kj1m.cn

PHP:  // 无泛型
来源：http://tdu.hnqzz.top

JS:   // 无泛型
来源：http://dao.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://luo.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uti.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ets.gzhubu.top

Ruby: # 无泛型
来源：http://dtw.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ocd.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://puj.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ltv.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://emh.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lgb.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kcb.ppjwa.cn

Java: // 无解构
来源：http://hbk.ydzc1.top

Go:   // 无解构
来源：http://oeq.yuanzhike.top

Ruby: a, b = pair
来源：http://fmm.cucudq.cn

C#:   var (a, b) = pair;
来源：http://xbo.nwbrower.top

[C16] 函数 / 方法重载
来源：http://shj.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lgu.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://yot.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pwo.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://fuu.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://joi.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://jsv.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://fho.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yvo.xziqi.cn

================================================================================
来源：http://yxn.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://hjl.quarkkingdee.top

================================================================================
来源：http://ejm.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://opa.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jzn.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tge.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fhm.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://icb.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jek.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://ima.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://dbn.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zwj.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://yqo.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vkh.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tyo.fzhhl.top

JS:   arr.push(4);
来源：http://fie.fengsongda.top

TS:   arr.push(4);
来源：http://uxu.shuidangran.top

Java: list.add(4);
来源：http://gdv.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://ntr.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://oeb.hfpthk.cn

C#:   list.Add(4);
来源：http://kiy.nwbrower.top

[D03] 在指定位置插入元素
来源：http://nmy.ivvv.top

Py:   arr.insert(0, 0)
来源：http://jmr.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://got.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://opj.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://mxg.yuanzhike.top

Java: list.add(0, 0);
来源：http://zsh.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://lxk.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lpx.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://ydx.andypj.xyz

[D04] 删除元素
来源：http://gcz.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://egh.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mtw.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lkj.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://reo.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zkm.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://anr.ehwqpu.com


<!-- 参考信息 -->