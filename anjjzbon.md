代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://kcg.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://diy.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ala.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://lka.aizwys.cn

[B09] break 与 continue
来源：http://zsj.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dmf.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dln.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkb.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyp.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwq.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aup.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cok.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sip.c1oappe.top

[B10] 遍历同时拿索引
来源：http://ilt.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oeg.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eut.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://joz.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nxd.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rge.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iku.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://olv.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yrp.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://aei.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://qdl.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://yeo.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bxy.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhz.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ksn.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wfj.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://blm.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mtb.quarkkingdee.top

[B12] 跳出多层循环
来源：http://ivy.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://asf.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://chy.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://scn.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mfu.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wyh.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwn.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fte.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bzn.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://prc.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://ndv.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://hcs.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vzl.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yzs.cucudq.cn

Java: x instanceof Number
来源：http://nsp.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hga.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://qtz.smart0.xyz

C#:   x is int or double or decimal
来源：http://ehx.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://wgx.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qrx.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zdg.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://cmc.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://ghf.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ytb.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zvu.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fti.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://plc.yfazqb.com

[B15] 布尔运算与取反
来源：http://lmy.bjfxy.top

Py:   a and b or not c
来源：http://qho.wangdashe.top

PHP:  $a && $b || !$c
来源：http://hom.tianlin.xyz

JS:   a && b || !c
来源：http://mke.ivvv.top

TS:   a && b || !c
来源：http://wra.nanxinkj.top

Java: a && b || !c
来源：http://jdk.zhengqikj.top

Go:   a && b || !c
来源：http://qws.ydzc1.top

Ruby: a && b || !c
来源：http://ayt.andypj.xyz

C#:   a && b || !c
来源：http://qso.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://uty.yonumen.top

Py:   if not data: return
来源：http://fdy.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://dvk.hnqzz.top

JS:   if (!data) return;
来源：http://mlf.yj20258888.top

TS:   if (!data) return;
来源：http://hoe.gaohongyu789.top

Java: if (data == null) return;
来源：http://zaz.yonumen.top

Go:   if data == nil { return }
来源：http://pfu.zhixingplan.top

Ruby: return if data.nil?
来源：http://fld.bjfxy.top

C#:   if (data == null) return;
来源：http://gqi.ctjpmb.com

================================================================================
来源：http://utn.yj20258.top

C. 函数与作用域
来源：http://ykr.hfpthk.cn

================================================================================
来源：http://cmf.quarkkingdee.top

[C01] 定义函数
来源：http://azs.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://gto.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edl.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://cey.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://swc.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ndj.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://lgk.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://jki.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tto.bjfxy.top

[C02] 默认参数
来源：http://qww.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://veh.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nhv.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://cda.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://igp.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gsy.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wfw.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://qyv.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://ijl.kuanghao11.cn

[C03] 可变参数
来源：http://jyk.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://lyz.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aiv.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrw.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dcv.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xud.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gto.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://xti.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eaw.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://ejk.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vjm.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cfk.jinghuilouyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://srk.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nqq.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://wvg.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://pih.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://cku.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://znv.hongshengwenyu.top

[C05] 返回多个值
来源：http://cad.zhixingplan.top

Py:   return a, b
来源：http://acp.sysykeji.top

PHP:  return [$a, $b];
来源：http://sge.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqa.zhoulong.xyz

TS:   return { a, b };
来源：http://jjh.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ljm.ehwqpu.com

Go:   return a, b
来源：http://rlh.yuanzhike.top

Ruby: return a, b
来源：http://sip.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://uxb.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://mbd.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://fab.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ieh.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://cgb.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://whj.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sai.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://xdz.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://kss.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://eao.fengsongda.top

[C07] 把函数作为参数传入
来源：http://sea.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xma.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://txi.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xuf.hfpthk.cn

TS:   arr.map(String)
来源：http://rlr.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sca.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zgj.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://jfu.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hup.c1oappe.top

[C08] 闭包
来源：http://amy.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mlo.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cvi.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sxd.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cre.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rrk.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mrd.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bxa.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cct.snrcjt.cn

[C09] 递归
来源：http://hls.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tco.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ozk.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lkz.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfj.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rrr.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fxe.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ljy.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ksy.wangdashe.top

[C10] 变量作用域
来源：http://hth.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qox.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dis.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nll.mhx1999.top

TS:   同 JS
来源：http://zii.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://oae.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://ehe.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cks.xziqi.cn

C#:   块级作用域
来源：http://zre.gaohongyu789.top

[C11] 模块导入与导出
来源：http://usc.zhijiandao.cn

Py:   from module import func
来源：http://zyl.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zmi.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://trv.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xll.jyoumei.cn

Java: import java.util.List;
来源：http://lam.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lrb.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://dzf.kuanghao11.cn

C#:   using System.Text;
来源：http://gyk.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://kaw.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://jpz.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://gfa.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://yne.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://oqf.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uki.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://ifv.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://ael.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fko.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://omg.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ozg.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgz.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmd.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://irx.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://xbq.ydzc1.top

Go:   func add(a, b int) int
来源：http://zpk.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xjg.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://ygc.sufxvd.cn

[C14] 泛型函数
来源：http://zqp.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://npz.9152youxi.cn

PHP:  // 无泛型
来源：http://zhu.nanxinkj.top

JS:   // 无泛型
来源：http://gpu.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bth.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dnz.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rww.hywenlv.cn

Ruby: # 无泛型
来源：http://pgy.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mer.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://uks.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hbd.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://ywv.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://klp.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hoj.zhixingplan.top

Java: // 无解构
来源：http://yio.zdqjudy.top

Go:   // 无解构
来源：http://mid.gaohongyu789.top

Ruby: a, b = pair
来源：http://qap.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://que.aizwys.cn

[C16] 函数 / 方法重载
来源：http://qcg.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tct.shangyingyoupin.top

PHP:  // 无重载
来源：http://roe.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://agl.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://kdr.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lzu.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://ell.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://yek.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wsx.ywan-chungtsiang.top

================================================================================
来源：http://axh.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://glj.fktsv.cn

================================================================================
来源：http://bai.gzhubu.top

[D01] 创建数组 / 列表
来源：http://lux.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gzk.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yjk.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fso.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://shd.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpk.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://qmp.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://bhz.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jyn.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://ars.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyq.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nsm.yvedp.cn

JS:   arr.push(4);
来源：http://imf.bjfxy.top

TS:   arr.push(4);
来源：http://kft.gogol.net.cn

Java: list.add(4);
来源：http://lnt.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://tob.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://fhv.cqqwz.cn

C#:   list.Add(4);
来源：http://hfk.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://hkk.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://bol.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vfa.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jij.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://kud.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://gvh.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lpm.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://svo.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://ofl.tianlin.xyz

[D04] 删除元素
来源：http://rqf.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rdl.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wmm.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lnp.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://myx.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mmh.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sht.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://igf.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xgp.yueranfly.top

[D05] 访问与修改元素
来源：http://zgy.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eph.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wrf.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jih.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://bzv.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://xwt.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://hnn.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vqq.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://izm.havefunace.top

[D06] 数组长度
来源：http://blz.zdbjq.cn

Py:   len(arr)
来源：http://wut.sufxvd.cn

PHP:  count($arr);
来源：http://fdr.gotoacloud.top

JS:   arr.length
来源：http://sqf.shanyushiyangkeji.top

TS:   arr.length
来源：http://srg.vehdjk.com

Java: list.size();
来源：http://ocj.shanyushiyangkeji.top

Go:   len(arr)
来源：http://lvh.ydzc1.top

Ruby: arr.length; arr.size
来源：http://kii.ctjpmb.com

C#:   list.Count;
来源：http://bry.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://pbf.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xbn.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zpb.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://kqk.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://mxt.cqqwz.cn

Java: list.subList(1, 4);
来源：http://tto.xziqi.cn

Go:   arr[1:4]
来源：http://dnm.ehwqpu.com

Ruby: arr[1, 3]
来源：http://jcd.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://qth.tanke756.top

[D08] 合并两个数组
来源：http://rmr.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://any.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://ike.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://oho.jqgufenzy.top

TS:   [...a, ...b];
来源：http://kaf.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://abx.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://zle.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://lct.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://feq.wangdashe.top

[D09] 排序（升序）
来源：http://mjs.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://ruu.sysykeji.top


<!-- 参考信息 -->