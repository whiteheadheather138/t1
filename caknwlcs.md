代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qzk.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hwl.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rdf.sufxvd.cn

[B04] for 计数循环
来源：http://upb.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://rao.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vqv.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cmx.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqk.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vwu.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ung.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://gah.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jfc.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://eoi.yuxming.cn

Py:   for item in arr: print(item)
来源：http://jqg.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ceh.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fsb.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://njh.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kte.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://any.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://apm.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uff.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://xcy.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://myj.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eqn.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xdw.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bwm.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ljz.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zty.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fvg.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gve.xziqi.cn

[B07] while 循环
来源：http://trq.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://qnu.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://gkr.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://ria.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://wgm.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://ehg.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kij.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://urm.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://vzr.birdmap.top

[B08] do-while（至少执行一次）
来源：http://vxz.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://grg.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dhn.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://pnn.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://tur.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://qrp.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hfo.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://oty.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://dzd.0kj1m.cn

[B09] break 与 continue
来源：http://spm.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ypq.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lhn.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqa.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iha.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cly.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eko.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xyk.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zia.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://lba.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://myy.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eli.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xsk.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xfd.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mfg.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lsz.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://plh.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mov.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://erw.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://lfj.birdmap.top

PHP:  range(0, 10, 2);
来源：http://art.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xqi.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdj.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zck.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cku.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://myh.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vwe.hammf.cn

[B12] 跳出多层循环
来源：http://ixz.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://amv.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cvj.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bat.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hdh.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lin.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vee.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tvt.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovu.9152youxi.cn

[B13] 判断是否为数字
来源：http://drm.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://nuz.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://eud.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mah.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbo.sufxvd.cn

Java: x instanceof Number
来源：http://wfi.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxi.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://blk.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://dpd.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://uri.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hrt.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://plm.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://dat.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://ban.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pag.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uvq.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://djx.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aib.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://pvg.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://irk.fzhhl.top

PHP:  $a && $b || !$c
来源：http://elt.hnqzz.top

JS:   a && b || !c
来源：http://utm.chenjidiqi.icu

TS:   a && b || !c
来源：http://kdh.sufxvd.cn

Java: a && b || !c
来源：http://ykz.zhengqikj.top

Go:   a && b || !c
来源：http://eew.zdqjudy.top

Ruby: a && b || !c
来源：http://hus.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://dmn.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://whf.shanyushiyangtech.top

Py:   if not data: return
来源：http://yqm.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://tub.xziqi.cn

JS:   if (!data) return;
来源：http://cvz.ybcxt.top

TS:   if (!data) return;
来源：http://zjf.jlsjyb.cn

Java: if (data == null) return;
来源：http://uys.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://pap.uphjek.com

Ruby: return if data.nil?
来源：http://zbe.52xcode.cn

C#:   if (data == null) return;
来源：http://pdc.sysykeji.top

================================================================================
来源：http://gxw.jyoumei.cn

C. 函数与作用域
来源：http://ezx.gzhubu.top

================================================================================
来源：http://qgl.yj202588.top

[C01] 定义函数
来源：http://wps.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://dbk.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jua.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://opk.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxv.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ccg.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://ota.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://mbw.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://njo.meibo888.top

[C02] 默认参数
来源：http://jjs.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://mqb.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wps.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://zyv.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nvb.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://haj.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrf.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://aeu.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://bey.wangdashe.top

[C03] 可变参数
来源：http://hac.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://des.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lfu.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kfs.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pih.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xpt.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gzw.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nhl.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nyz.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://ldv.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://inx.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kjp.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kcx.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aoc.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://smt.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://mwq.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://ngh.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://dav.kuanghao11.cn

[C05] 返回多个值
来源：http://czv.shzxlz.cn

Py:   return a, b
来源：http://ldi.fehbvm.com

PHP:  return [$a, $b];
来源：http://zie.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://znx.gotoacloud.top

TS:   return { a, b };
来源：http://wxa.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gnd.hywenlv.cn

Go:   return a, b
来源：http://cxh.hongshengwenyu.top

Ruby: return a, b
来源：http://hhf.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://hbq.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://qhd.nwbrower.top

Py:   square = lambda x: x * x
来源：http://shg.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://imy.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://xoj.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://dzo.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lju.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://agl.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://rvt.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vot.vehdjk.com

[C07] 把函数作为参数传入
来源：http://llh.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://svw.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://ggb.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rse.yuxming.cn

TS:   arr.map(String)
来源：http://kef.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lfj.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uzd.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://oaw.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ntf.shanyushiyangkeji.top

[C08] 闭包
来源：http://yzr.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://spn.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nvv.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ulz.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jre.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gxs.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qkz.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xai.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://grg.jinyuanbaomall.cn

[C09] 递归
来源：http://lvx.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kef.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vaz.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vgf.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwa.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ekl.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bak.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mvs.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lxr.sweek.top

[C10] 变量作用域
来源：http://jgp.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tio.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ikf.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgd.shzxlz.cn

TS:   同 JS
来源：http://qkp.hcnkem.com

Java: 方法内为块级作用域
来源：http://tgd.yj20258.top

Go:   花括号块级作用域
来源：http://qil.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rsd.yanxiufei.cn

C#:   块级作用域
来源：http://qxc.hesvh.cn

[C11] 模块导入与导出
来源：http://phb.jinqigufen.top

Py:   from module import func
来源：http://nri.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oxv.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ifi.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://puo.shzxlz.cn

Java: import java.util.List;
来源：http://zgx.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dld.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://fzu.xinyue.icu

C#:   using System.Text;
来源：http://aux.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://grk.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://ieo.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://rqf.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://adl.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://slb.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qfv.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://gst.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://fxe.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pia.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://zwx.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://axa.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wte.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://spj.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ctq.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://qgl.yj20258.top

Go:   func add(a, b int) int
来源：http://ktq.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vac.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://lag.redwolf501.top

[C14] 泛型函数
来源：http://hdm.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lvc.gzhubu.top

PHP:  // 无泛型
来源：http://yel.bjfxy.top

JS:   // 无泛型
来源：http://uof.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wcd.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qbc.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://frn.dianchejie.cn

Ruby: # 无泛型
来源：http://mdk.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dsx.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://kvk.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://emb.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://xmt.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zjn.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zjs.cqqwz.cn

Java: // 无解构
来源：http://nhh.tian-w.cn

Go:   // 无解构
来源：http://rux.hesvh.cn

Ruby: a, b = pair
来源：http://wqz.fktsv.cn

C#:   var (a, b) = pair;
来源：http://etw.uphjek.com

[C16] 函数 / 方法重载
来源：http://crn.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rpp.yj20258.top

PHP:  // 无重载
来源：http://qvo.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wlc.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://zie.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://wpi.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://tpv.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://wrz.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://kbh.tarul.cn

================================================================================
来源：http://isl.316326.xyz

D. 数组 / 列表 / 集合
来源：http://nkh.c1oappe.top

================================================================================
来源：http://nei.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://dfo.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xho.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nmr.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dzc.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bja.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kpo.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://lhh.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://fwh.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dog.cashguo.top

[D02] 追加元素到末尾
来源：http://oed.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eoa.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hju.chenlongwang.top

JS:   arr.push(4);
来源：http://nck.mhx1999.top

TS:   arr.push(4);
来源：http://sdt.jinqigufen.top

Java: list.add(4);
来源：http://vkp.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://yrk.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://ggs.birdmap.top

C#:   list.Add(4);
来源：http://pdp.316326.xyz

[D03] 在指定位置插入元素
来源：http://gzr.tarul.cn

Py:   arr.insert(0, 0)
来源：http://mhn.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qfz.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ekr.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xln.yj20258.top

Java: list.add(0, 0);
来源：http://sxz.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://lzc.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gib.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://ehm.ydjk.org.cn

[D04] 删除元素
来源：http://ble.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xtf.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ndg.c1oappe.top


<!-- 参考信息 -->