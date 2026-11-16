代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://zii.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ksb.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://lur.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://vqk.jqgufenzy.top

[B09] break 与 continue
来源：http://oey.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iei.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://amf.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxn.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykn.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnq.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://umn.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hyf.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezs.daxiang520.top

[B10] 遍历同时拿索引
来源：http://jsz.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://avu.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hig.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oln.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ztq.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://igf.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ivm.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dzb.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lfo.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://tbh.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://sac.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://uvi.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epe.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vgh.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://got.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zup.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://wdi.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sjq.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://evs.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lhp.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://bbj.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lul.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ocr.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hni.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zpg.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lza.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhf.vehdjk.com

[B13] 判断是否为数字
来源：http://ftx.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://gbw.yfazqb.com

PHP:  is_numeric($x)
来源：http://jll.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyd.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sac.haohaochexian.top

Java: x instanceof Number
来源：http://ivv.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tws.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://ywx.ybcxt.top

C#:   x is int or double or decimal
来源：http://cdx.mhx1999.top

[B14] 判断值是否在集合内
来源：http://igg.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ail.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://toe.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://cmr.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://xks.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xpv.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kuu.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://jry.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dpe.yj20258.top

[B15] 布尔运算与取反
来源：http://nft.andypj.xyz

Py:   a and b or not c
来源：http://tog.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://isv.tianlin.xyz

JS:   a && b || !c
来源：http://tjs.52xcode.cn

TS:   a && b || !c
来源：http://mfy.zdqjudy.top

Java: a && b || !c
来源：http://zfl.shuidangran.top

Go:   a && b || !c
来源：http://bkw.vehdjk.com

Ruby: a && b || !c
来源：http://yzq.chenjidiqi.icu

C#:   a && b || !c
来源：http://luu.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://wuq.zdbjq.cn

Py:   if not data: return
来源：http://xxv.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://src.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://mxa.chenzaomai.com

TS:   if (!data) return;
来源：http://jtl.gotoacloud.top

Java: if (data == null) return;
来源：http://spv.mhx1999.top

Go:   if data == nil { return }
来源：http://pma.yj202588.top

Ruby: return if data.nil?
来源：http://mfg.pycfn.com

C#:   if (data == null) return;
来源：http://xwc.xuanzx.com

================================================================================
来源：http://qwb.yvedp.cn

C. 函数与作用域
来源：http://efe.fehbvm.com

================================================================================
来源：http://miv.tian-w.cn

[C01] 定义函数
来源：http://ufm.yonumen.top

Py:   def add(a, b): return a + b
来源：http://cby.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xog.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://gam.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ioa.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dfr.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://osa.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://ygo.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vlg.jinqigufen.top

[C02] 默认参数
来源：http://mdk.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://mnl.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mem.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://esd.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mcp.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://phm.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wku.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://yeg.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://kan.yonumen.top

[C03] 可变参数
来源：http://zvm.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://amk.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aff.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tcy.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywa.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dcx.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wmb.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mzg.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kkm.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://lkh.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fzm.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://thd.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ion.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nbs.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://nhl.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://rre.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://vcc.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://qei.hesvh.cn

[C05] 返回多个值
来源：http://piz.gogol.net.cn

Py:   return a, b
来源：http://hgc.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://wbz.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vzb.daxiang520.top

TS:   return { a, b };
来源：http://dtb.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ffo.birdmap.top

Go:   return a, b
来源：http://xvw.tanke756.top

Ruby: return a, b
来源：http://hpi.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://xml.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://gwx.tanke756.top

Py:   square = lambda x: x * x
来源：http://zfj.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://srn.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://vdg.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://grx.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vai.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nan.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://qzv.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://buc.tarul.cn

[C07] 把函数作为参数传入
来源：http://lxc.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xcz.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://vqt.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cjb.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://qpd.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lzy.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fzz.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://mlc.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://evg.yuanzhike.top

[C08] 闭包
来源：http://toj.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qve.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yfv.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bic.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rzk.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bna.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ymr.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nny.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lpe.aibaodan.cn

[C09] 递归
来源：http://ogw.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bnj.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://phc.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkh.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wyt.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rng.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://efp.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sfd.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://muj.pycfn.com

[C10] 变量作用域
来源：http://rwo.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uur.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rcb.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://chs.havefunace.top

TS:   同 JS
来源：http://uvi.havefunace.top

Java: 方法内为块级作用域
来源：http://yfy.jinqigfzy.top

Go:   花括号块级作用域
来源：http://tll.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cju.snrcjt.cn

C#:   块级作用域
来源：http://nms.jinqigfzy.top

[C11] 模块导入与导出
来源：http://ldo.wangdashe.top

Py:   from module import func
来源：http://otz.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://juq.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tzz.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ypf.xinyue.icu

Java: import java.util.List;
来源：http://kve.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vmm.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://kpm.mhx1999.top

C#:   using System.Text;
来源：http://fnc.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://pyw.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://eiq.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://csh.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://fcw.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://ujr.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lpr.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://xem.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://znh.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dvo.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://tmg.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oum.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrg.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://anl.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aiz.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://efy.svipenyu.cn

Go:   func add(a, b int) int
来源：http://brv.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nff.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qmq.zhijiandao.cn

[C14] 泛型函数
来源：http://umv.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sqo.gotoacloud.top

PHP:  // 无泛型
来源：http://tvd.zdqjudy.top

JS:   // 无泛型
来源：http://anb.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dlk.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gdq.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rcj.daria6918.cn

Ruby: # 无泛型
来源：http://wbk.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kot.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://fbw.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hpx.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://zth.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://shy.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jic.gaohongyu789.top

Java: // 无解构
来源：http://mjv.yuxming.cn

Go:   // 无解构
来源：http://lqi.jiagoushi.top

Ruby: a, b = pair
来源：http://fpb.cucudq.cn

C#:   var (a, b) = pair;
来源：http://rtw.yuxming.cn

[C16] 函数 / 方法重载
来源：http://oyg.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aop.nanxinkj.top

PHP:  // 无重载
来源：http://fdc.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pcc.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://qye.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bip.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://luj.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://dbe.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://cqu.yangfankeji.com

================================================================================
来源：http://hve.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://uka.uphjek.com

================================================================================
来源：http://tld.yj20258888.top

[D01] 创建数组 / 列表
来源：http://lbz.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqz.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cuf.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sch.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bjb.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qqo.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://jmi.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://mrs.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pew.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://wjs.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xaz.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sun.0kj1m.cn

JS:   arr.push(4);
来源：http://dbq.fktsv.cn

TS:   arr.push(4);
来源：http://rqa.xylfe.cn

Java: list.add(4);
来源：http://vfk.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://onf.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://umg.vehdjk.com

C#:   list.Add(4);
来源：http://tmy.yfazqb.com

[D03] 在指定位置插入元素
来源：http://tsh.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://bup.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://snp.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zjk.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://hqq.daria6918.cn

Java: list.add(0, 0);
来源：http://saj.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vci.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kqn.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://ata.cqqwz.cn

[D04] 删除元素
来源：http://dsw.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ntr.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hpq.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gbs.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://tpf.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ljo.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lby.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rax.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uyg.chenlongwang.top

[D05] 访问与修改元素
来源：http://ejq.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://meu.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://czq.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsb.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://omo.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://pup.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://qje.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cdf.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skf.yonumen.top

[D06] 数组长度
来源：http://lsp.xylfe.cn

Py:   len(arr)
来源：http://pep.zhengqikj.top

PHP:  count($arr);
来源：http://ufb.tian-w.cn

JS:   arr.length
来源：http://wbu.gotoacloud.top

TS:   arr.length
来源：http://wdy.zhijiandao.cn

Java: list.size();
来源：http://apw.shangyingyoupin.top

Go:   len(arr)
来源：http://huo.fzhhl.top

Ruby: arr.length; arr.size
来源：http://tya.jinqigfzy.top

C#:   list.Count;
来源：http://hmr.havefunace.top

[D07] 切片 / 取子数组
来源：http://uwa.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kru.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://rra.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://wiy.sweek.top

TS:   arr.slice(1, 4);
来源：http://dgt.svipenyu.cn

Java: list.subList(1, 4);
来源：http://etc.yj20258.top

Go:   arr[1:4]
来源：http://gmu.mhx1999.top

Ruby: arr[1, 3]
来源：http://hay.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://nmw.cqqwz.cn

[D08] 合并两个数组
来源：http://rvo.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://yce.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://zvx.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zym.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://oxh.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://opu.nanxinkj.top

Go:   append(a, b...)
来源：http://mfq.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://mlv.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://wqx.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://uvo.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://gxs.0kj1m.cn


<!-- 参考信息 -->