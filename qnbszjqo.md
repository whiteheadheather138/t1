代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://lkv.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://aci.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://cez.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://ddu.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ygq.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://nnr.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://zlb.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://bsz.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://eav.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://rfv.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://jxk.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://yvt.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://tem.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qac.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://qlq.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://uty.jqgfzy.top

[B09] break 与 continue
来源：http://jgp.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jpc.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ihz.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euz.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qan.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cuw.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://own.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oxy.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orf.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://beh.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nug.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cfp.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fcu.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wdb.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ukz.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pka.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://myf.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zpt.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://oeu.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://dlx.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://kub.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://enq.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jag.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xze.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cqh.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://gji.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blj.pycfn.com

[B12] 跳出多层循环
来源：http://jfx.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://non.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://utc.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqq.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjd.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://seb.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kdf.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kel.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hwy.yuanzhike.top

[B13] 判断是否为数字
来源：http://inh.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://mhh.hcnkem.com

PHP:  is_numeric($x)
来源：http://lru.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yah.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwp.feifeiyinyue.top

Java: x instanceof Number
来源：http://efx.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rxb.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://tur.xinyue.icu

C#:   x is int or double or decimal
来源：http://peh.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://xsn.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lkx.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gfg.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://ktw.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://rfx.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tei.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pyf.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://oho.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bps.nanxinkj.top

[B15] 布尔运算与取反
来源：http://csr.hnxiangtu.top

Py:   a and b or not c
来源：http://cju.yueranfly.top

PHP:  $a && $b || !$c
来源：http://ttv.chenjidiqi.icu

JS:   a && b || !c
来源：http://njb.jlsjyb.cn

TS:   a && b || !c
来源：http://jbq.bjfxy.top

Java: a && b || !c
来源：http://fwp.zhongyouzk.top

Go:   a && b || !c
来源：http://thr.zhijiandao.cn

Ruby: a && b || !c
来源：http://kjc.zhengqikj.top

C#:   a && b || !c
来源：http://bxk.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://wrm.ppjwa.cn

Py:   if not data: return
来源：http://uec.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://gvs.uphjek.com

JS:   if (!data) return;
来源：http://pht.sxryk.cn

TS:   if (!data) return;
来源：http://nxx.gogol.net.cn

Java: if (data == null) return;
来源：http://oln.fehbvm.com

Go:   if data == nil { return }
来源：http://oah.zhijiandao.cn

Ruby: return if data.nil?
来源：http://ppo.smart0.xyz

C#:   if (data == null) return;
来源：http://fdx.zdqjudy.top

================================================================================
来源：http://mqo.shangyingyoupin.top

C. 函数与作用域
来源：http://mrz.zdbjq.cn

================================================================================
来源：http://rmx.hcnkem.com

[C01] 定义函数
来源：http://yxz.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://nmz.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pci.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://xyy.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fge.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ubq.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://edi.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://byp.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://you.aizwys.cn

[C02] 默认参数
来源：http://tfp.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://ztk.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rcq.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://ozz.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tro.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zyh.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fid.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://jxc.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://ywb.gaohongyu789.top

[C03] 可变参数
来源：http://ddr.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://boa.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ses.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iuk.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhu.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://syj.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aep.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://kmp.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ras.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://dix.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mqj.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rbq.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mvy.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zdl.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://zkj.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://tcx.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://deg.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://vbs.smart0.xyz

[C05] 返回多个值
来源：http://bjo.vehdjk.com

Py:   return a, b
来源：http://eav.yangfankeji.com

PHP:  return [$a, $b];
来源：http://jjs.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rdh.gotoacloud.top

TS:   return { a, b };
来源：http://yyd.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awt.ehwqpu.com

Go:   return a, b
来源：http://tod.pycfn.com

Ruby: return a, b
来源：http://xaj.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://pbk.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://mwy.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://ufl.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gdd.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://fmz.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://aby.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yxn.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://tag.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://sjt.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://wqk.guannengcc.top

[C07] 把函数作为参数传入
来源：http://vtc.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kfs.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jyy.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vmn.zhoulong.xyz

TS:   arr.map(String)
来源：http://aml.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ptk.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sow.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://egg.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wuw.316326.xyz

[C08] 闭包
来源：http://jhf.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bxz.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cik.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xqh.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gyq.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xju.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vlr.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xeh.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rus.hysaishi.cn

[C09] 递归
来源：http://zot.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qmb.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rkg.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjx.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vgd.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xeo.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dug.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vnl.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cnt.andypj.xyz

[C10] 变量作用域
来源：http://yzu.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tib.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://joa.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://srd.chenjidiqi.icu

TS:   同 JS
来源：http://ced.hnqzz.top

Java: 方法内为块级作用域
来源：http://cbm.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://ptx.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qsp.cdnleiting.top

C#:   块级作用域
来源：http://xbw.ppjwa.cn

[C11] 模块导入与导出
来源：http://fwp.meibo888.top

Py:   from module import func
来源：http://geu.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ool.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eal.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bey.kuanghao11.cn

Java: import java.util.List;
来源：http://nct.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mim.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://xgt.smart0.xyz

C#:   using System.Text;
来源：http://uba.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://bzz.sweek.top

Py:   (lambda: print("run"))()
来源：http://hyz.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://hxw.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://grc.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://tsl.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pey.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://ejf.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://gtc.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cni.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://aun.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ony.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ygw.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wdd.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnw.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://qed.birdmap.top

Go:   func add(a, b int) int
来源：http://xlx.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jel.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mnx.hysaishi.cn

[C14] 泛型函数
来源：http://ldm.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ghh.bbcook.cn

PHP:  // 无泛型
来源：http://ias.yongpay.top

JS:   // 无泛型
来源：http://gdx.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gab.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://acr.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ehm.daxiang520.top

Ruby: # 无泛型
来源：http://qfj.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bud.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://vcf.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bta.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://reb.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://box.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mer.jinqigfzy.top

Java: // 无解构
来源：http://llx.smart0.xyz

Go:   // 无解构
来源：http://ozl.dashuyun.cn

Ruby: a, b = pair
来源：http://xtc.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://whr.andypj.xyz

[C16] 函数 / 方法重载
来源：http://wma.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://txp.yongpay.top

PHP:  // 无重载
来源：http://tyv.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://inm.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://sky.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fen.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://hyk.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://unu.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://umq.ydzc1.top

================================================================================
来源：http://nbe.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://xqr.nwbrower.top

================================================================================
来源：http://mng.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://zkd.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jgk.ctjpmb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bbc.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://can.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://otf.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fki.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://not.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://woi.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aui.vehdjk.com

[D02] 追加元素到末尾
来源：http://ioa.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cbh.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cbh.chenjidiqi.icu

JS:   arr.push(4);
来源：http://kkb.xuanzx.com

TS:   arr.push(4);
来源：http://ozs.yfazqb.com

Java: list.add(4);
来源：http://dxl.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://erl.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://kiw.yvedp.cn

C#:   list.Add(4);
来源：http://zcu.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://nxc.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://xuj.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zmf.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qvc.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://pnw.zhixingplan.top

Java: list.add(0, 0);
来源：http://lao.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://yrn.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gys.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://hkg.tianlin.xyz

[D04] 删除元素
来源：http://suc.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fqt.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nna.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oka.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://nme.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://myz.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lkg.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yhp.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpb.jlsjyb.cn

[D05] 访问与修改元素
来源：http://jqw.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gfm.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://okg.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qft.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://zhd.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://yvd.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://kfs.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjq.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kmj.guowangkeji.top

[D06] 数组长度
来源：http://mec.fengsongda.top

Py:   len(arr)
来源：http://jan.hnqzz.top

PHP:  count($arr);
来源：http://sco.ydjk.org.cn

JS:   arr.length
来源：http://jgf.cdnleiting.top

TS:   arr.length
来源：http://txs.redwolf501.top

Java: list.size();
来源：http://dpj.vehdjk.com

Go:   len(arr)
来源：http://crh.aizwys.cn

Ruby: arr.length; arr.size
来源：http://tns.quarkkingdee.top

C#:   list.Count;
来源：http://ztb.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://pde.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhz.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ewt.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://zgr.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://kop.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://suo.yfazqb.com

Go:   arr[1:4]
来源：http://enn.jianghu66.top

Ruby: arr[1, 3]
来源：http://hac.bjfxy.top


<!-- 参考信息 -->