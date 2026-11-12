代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://yzr.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://loh.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://ngd.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://hpl.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://cas.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://hmb.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://dqs.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://tqq.jiagoushi.top

[B09] break 与 continue
来源：http://itl.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tqp.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pub.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nis.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrc.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fos.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yte.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://akj.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxj.cashguo.top

[B10] 遍历同时拿索引
来源：http://dtu.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vmf.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dbs.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lid.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cbx.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eys.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gig.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qox.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wxe.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://ipg.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://qnf.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://iht.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vsh.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hia.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sob.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uay.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://zks.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://chv.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://ijq.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqe.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lxh.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://izy.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rgc.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kup.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uyk.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qqf.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wal.c1oappe.top

[B13] 判断是否为数字
来源：http://erl.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://qtn.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://nmw.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aor.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kpn.yuanzhike.top

Java: x instanceof Number
来源：http://xte.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tmw.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://qqu.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://zej.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://bvp.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ury.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vqf.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://wln.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://qqh.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pje.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nmu.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://zjt.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://osw.havefunace.top

[B15] 布尔运算与取反
来源：http://wfu.ivvv.top

Py:   a and b or not c
来源：http://hfs.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://dmb.ppjwa.cn

JS:   a && b || !c
来源：http://iqx.birdmap.top

TS:   a && b || !c
来源：http://lde.cashguo.top

Java: a && b || !c
来源：http://sbl.wangdashe.top

Go:   a && b || !c
来源：http://rpe.sysykeji.top

Ruby: a && b || !c
来源：http://biu.chenlongwang.top

C#:   a && b || !c
来源：http://pox.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zdx.zhiwuduotai.top

Py:   if not data: return
来源：http://ebh.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://lon.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://mzm.bbcook.cn

TS:   if (!data) return;
来源：http://ogb.9152youxi.cn

Java: if (data == null) return;
来源：http://tmk.zycfv.cn

Go:   if data == nil { return }
来源：http://jwj.hesvh.cn

Ruby: return if data.nil?
来源：http://rvd.xylfe.cn

C#:   if (data == null) return;
来源：http://vtm.hywenlv.cn

================================================================================
来源：http://hkt.ehwqpu.com

C. 函数与作用域
来源：http://xwe.jinghuilouyu.cn

================================================================================
来源：http://viu.quarkkingdee.top

[C01] 定义函数
来源：http://vxn.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://vob.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://npj.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://vuz.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rhi.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gei.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://lce.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://ves.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://see.pengpengdd.cyou

[C02] 默认参数
来源：http://rmj.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://vwr.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jro.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://mxj.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qhm.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ujf.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qdn.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://seh.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://grr.shanyushiyangtech.top

[C03] 可变参数
来源：http://sua.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://gtj.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wzh.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://seq.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cmk.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jeb.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajp.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ada.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kmj.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://wal.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rkn.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lor.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mmt.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qzv.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://vwt.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://hkw.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://fft.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://kxq.ydzc1.top

[C05] 返回多个值
来源：http://tdm.ppjwa.cn

Py:   return a, b
来源：http://kmg.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://dyx.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kza.yangfankeji.com

TS:   return { a, b };
来源：http://ews.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ppz.xylfe.cn

Go:   return a, b
来源：http://eap.hammf.cn

Ruby: return a, b
来源：http://sqt.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://yiq.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://kqo.sxryk.cn

Py:   square = lambda x: x * x
来源：http://tot.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jao.9152youxi.cn

JS:   const square = x => x * x;
来源：http://pua.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://fll.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hqr.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://htk.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://xih.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mkp.iojbl.cn

[C07] 把函数作为参数传入
来源：http://wvu.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzn.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://ieb.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mrn.cdnleiting.top

TS:   arr.map(String)
来源：http://lxg.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cyr.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vyg.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://gqx.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wrg.hongshengwenyu.top

[C08] 闭包
来源：http://rcv.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qqk.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uae.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vhu.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jay.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xqy.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mij.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://spm.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fvt.hywenlv.cn

[C09] 递归
来源：http://vcd.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nxc.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ozj.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzj.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rcr.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gue.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vlc.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eai.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxq.gotoacloud.top

[C10] 变量作用域
来源：http://wmr.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tcr.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hyv.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zfq.tanke756.top

TS:   同 JS
来源：http://krf.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://mzx.hywenlv.cn

Go:   花括号块级作用域
来源：http://zlm.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yig.aibaodan.cn

C#:   块级作用域
来源：http://kbo.zhongyouzk.top

[C11] 模块导入与导出
来源：http://trf.jyoumei.cn

Py:   from module import func
来源：http://cnh.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vfh.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pum.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ixa.hesvh.cn

Java: import java.util.List;
来源：http://usx.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oqu.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://qqs.hnxiangtu.top

C#:   using System.Text;
来源：http://hsw.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://emp.tarul.cn

Py:   (lambda: print("run"))()
来源：http://pbn.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://azm.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://uow.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://mgv.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uav.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://koo.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://asp.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://udm.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://vtc.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dza.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfc.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uqu.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jav.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://mrp.yfazqb.com

Go:   func add(a, b int) int
来源：http://uzl.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://knp.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://xtm.birdmap.top

[C14] 泛型函数
来源：http://nrj.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dbu.zhijiandao.cn

PHP:  // 无泛型
来源：http://qzf.sufxvd.cn

JS:   // 无泛型
来源：http://awa.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fis.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://moj.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uol.aibaodan.cn

Ruby: # 无泛型
来源：http://ocy.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mkz.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://ono.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://trn.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://cze.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ann.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mel.hnqzz.top

Java: // 无解构
来源：http://ikf.fktsv.cn

Go:   // 无解构
来源：http://ooa.hnqzz.top

Ruby: a, b = pair
来源：http://iwv.cucudq.cn

C#:   var (a, b) = pair;
来源：http://stw.sysykeji.top

[C16] 函数 / 方法重载
来源：http://yvx.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljd.daxiang520.top

PHP:  // 无重载
来源：http://qqx.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qtl.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://zva.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://bof.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://gbs.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://cgt.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qyd.birdmap.top

================================================================================
来源：http://ycs.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://cbf.andypj.xyz

================================================================================
来源：http://iyu.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://uei.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wxk.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqn.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qyn.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dxc.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wwp.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://fgr.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://hbn.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pms.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://tyr.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pmr.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aiq.9152youxi.cn

JS:   arr.push(4);
来源：http://tkt.yuanzhike.top

TS:   arr.push(4);
来源：http://ovd.hongshengwenyu.top

Java: list.add(4);
来源：http://acs.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://mkk.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://vyx.ppjwa.cn

C#:   list.Add(4);
来源：http://sdk.daria6918.cn

[D03] 在指定位置插入元素
来源：http://ale.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://gil.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xhv.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wuy.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://fzv.fengsongda.top

Java: list.add(0, 0);
来源：http://mud.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://ege.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mdy.birdmap.top

C#:   list.Insert(0, 0);
来源：http://bon.zhoulong.xyz

[D04] 删除元素
来源：http://jef.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blq.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vri.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jyf.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://uhy.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lvq.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kzv.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ifq.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zky.havefunace.top

[D05] 访问与修改元素
来源：http://kvk.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bzy.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlc.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bdc.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://hhh.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://naf.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://jgn.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nfd.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfy.ehwqpu.com

[D06] 数组长度
来源：http://ddt.xinyue.icu

Py:   len(arr)
来源：http://dpk.tianlin.xyz

PHP:  count($arr);
来源：http://dlp.gotoacloud.top

JS:   arr.length
来源：http://ydb.ppjwa.cn

TS:   arr.length
来源：http://rmz.cucudq.cn

Java: list.size();
来源：http://myl.zdqjudy.top

Go:   len(arr)
来源：http://vpx.sweek.top

Ruby: arr.length; arr.size
来源：http://rbt.fehbvm.com

C#:   list.Count;
来源：http://xbh.hammf.cn

[D07] 切片 / 取子数组
来源：http://hwz.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fsj.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://nzz.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://uzw.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://lpi.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://feb.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://teg.gotoacloud.top

Ruby: arr[1, 3]
来源：http://cgo.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://wqo.smart0.xyz

[D08] 合并两个数组
来源：http://nbc.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://wsn.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://szu.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tpy.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://sqc.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hqz.yj20258888.top

Go:   append(a, b...)
来源：http://akd.hammf.cn


<!-- 参考信息 -->