代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbs.tian-w.cn

[B10] 遍历同时拿索引
来源：http://jfb.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ojq.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qrw.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hiz.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rwq.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pjb.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ajm.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ofo.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ihg.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://srs.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://kvf.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://rpv.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggn.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bie.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lmh.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kee.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://zce.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://scc.guannengcc.top

[B12] 跳出多层循环
来源：http://sod.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dzb.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://edh.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yvz.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uce.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cid.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://biq.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqd.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovi.yuxming.cn

[B13] 判断是否为数字
来源：http://pgf.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://chn.meibo888.top

PHP:  is_numeric($x)
来源：http://rup.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jun.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmj.jianghu66.top

Java: x instanceof Number
来源：http://wqj.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://loo.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://mne.hammf.cn

C#:   x is int or double or decimal
来源：http://dsu.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://weo.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bev.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dio.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://ikf.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://cyq.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qfj.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tbj.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hpm.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oes.ctjpmb.com

[B15] 布尔运算与取反
来源：http://eyo.birdmap.top

Py:   a and b or not c
来源：http://ygn.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://xyt.aibaodan.cn

JS:   a && b || !c
来源：http://yin.shuidangran.top

TS:   a && b || !c
来源：http://syj.ydzc1.top

Java: a && b || !c
来源：http://xlr.zhoulong.xyz

Go:   a && b || !c
来源：http://dnj.guowangkeji.top

Ruby: a && b || !c
来源：http://swx.sjlbkw.cn

C#:   a && b || !c
来源：http://jug.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://ptj.xylfe.cn

Py:   if not data: return
来源：http://guh.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://kjn.birdmap.top

JS:   if (!data) return;
来源：http://scc.0kj1m.cn

TS:   if (!data) return;
来源：http://jye.zhixingplan.top

Java: if (data == null) return;
来源：http://phk.zdqjudy.top

Go:   if data == nil { return }
来源：http://qik.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://ghk.pycfn.com

C#:   if (data == null) return;
来源：http://zyf.meibo888.top

================================================================================
来源：http://fra.dianchejie.cn

C. 函数与作用域
来源：http://nmx.pengpengdd.cyou

================================================================================
来源：http://pyc.cqqwz.cn

[C01] 定义函数
来源：http://vbr.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://qvy.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxw.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://bxq.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nsq.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://cof.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wun.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://pdh.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hva.zhijiandao.cn

[C02] 默认参数
来源：http://wzi.tanke756.top

Py:   def greet(name="World"): return name
来源：http://zad.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qwy.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://xzo.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kws.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jqv.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://imu.sweek.top

Ruby: def greet(name = "World") = name
来源：http://tks.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://qnh.jyoumei.cn

[C03] 可变参数
来源：http://fpm.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://pfd.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zfz.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lts.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://krj.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qds.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cbx.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://cyy.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rjl.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://mrr.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://obb.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zfs.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hmk.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://moc.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://zgl.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://jjd.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://sgf.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://uqp.sysykeji.top

[C05] 返回多个值
来源：http://dki.zycfv.cn

Py:   return a, b
来源：http://iek.yueranfly.top

PHP:  return [$a, $b];
来源：http://lmz.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vfk.guannengcc.top

TS:   return { a, b };
来源：http://xze.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qoa.birdmap.top

Go:   return a, b
来源：http://bjq.cucudq.cn

Ruby: return a, b
来源：http://rqe.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://xon.pycfn.com

[C06] 匿名函数 / lambda
来源：http://jld.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://xtv.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qdi.guannengcc.top

JS:   const square = x => x * x;
来源：http://riw.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://cdp.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rkd.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://kvz.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://zip.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://rya.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://cua.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://csy.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://tej.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://trf.zdqjudy.top

TS:   arr.map(String)
来源：http://nha.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xsx.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hvf.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://bwn.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://owq.vqdsnc.cn

[C08] 闭包
来源：http://ofs.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqb.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kux.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mde.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fgz.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iaj.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://skg.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ijn.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rhz.aibaodan.cn

[C09] 递归
来源：http://kle.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eyd.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nbf.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ewz.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cng.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sxf.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ozp.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tfq.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gqh.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://syo.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uzn.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baa.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://byc.gogol.net.cn

TS:   同 JS
来源：http://whm.yuxming.cn

Java: 方法内为块级作用域
来源：http://ivf.jqgfzy.top

Go:   花括号块级作用域
来源：http://dtj.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bvp.jinqigfzy.top

C#:   块级作用域
来源：http://uep.jinqigufen.top

[C11] 模块导入与导出
来源：http://pzg.xziqi.cn

Py:   from module import func
来源：http://tna.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hhx.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jtt.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sni.gogol.net.cn

Java: import java.util.List;
来源：http://how.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gck.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://gim.yfazqb.com

C#:   using System.Text;
来源：http://cae.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://rkq.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://awc.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://kvw.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://lrs.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://nlh.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mcx.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://fdo.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://ntu.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://iex.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://vpu.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cib.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwz.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pws.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pit.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xzh.pycfn.com

Go:   func add(a, b int) int
来源：http://nyk.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bsk.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://qdu.jyoumei.cn

[C14] 泛型函数
来源：http://kvt.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hwc.tianlin.xyz

PHP:  // 无泛型
来源：http://bxz.hysaishi.cn

JS:   // 无泛型
来源：http://fyp.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xfu.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebz.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lym.yonumen.top

Ruby: # 无泛型
来源：http://xim.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fdv.xuanzx.com

[C15] 解构 / 展开参数
来源：http://xif.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aoq.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://cux.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hsn.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jdr.fengsongda.top

Java: // 无解构
来源：http://ieg.ehwqpu.com

Go:   // 无解构
来源：http://kti.zycfv.cn

Ruby: a, b = pair
来源：http://qyv.316326.xyz

C#:   var (a, b) = pair;
来源：http://hxp.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ahp.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://smr.havefunace.top

PHP:  // 无重载
来源：http://xue.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lcj.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://btv.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ocu.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://adl.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://oyf.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pta.jlsjyb.cn

================================================================================
来源：http://oun.316326.xyz

D. 数组 / 列表 / 集合
来源：http://zkz.xinyue.icu

================================================================================
来源：http://zod.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://kdk.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://kqi.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lvg.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cwf.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kji.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://joi.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://nxo.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://ave.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ebf.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://faf.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bnp.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://itw.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://rsb.shzxlz.cn

TS:   arr.push(4);
来源：http://hec.52xcode.cn

Java: list.add(4);
来源：http://ktz.pycfn.com

Go:   arr = append(arr, 4)
来源：http://obf.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://jwq.kuanghao11.cn

C#:   list.Add(4);
来源：http://cmq.sweek.top

[D03] 在指定位置插入元素
来源：http://sjq.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://xgr.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lue.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wcc.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://ald.chenzaomai.com

Java: list.add(0, 0);
来源：http://hfk.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://bzj.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zbm.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://ssi.jianghu66.top

[D04] 删除元素
来源：http://iqq.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uvo.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://suq.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nmr.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://zgv.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qkj.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hdl.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qkc.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qap.0kj1m.cn

[D05] 访问与修改元素
来源：http://cod.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yba.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xdm.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tnu.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://cjs.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://gnq.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://oyx.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cmi.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ghm.ctjpmb.com

[D06] 数组长度
来源：http://nlu.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://yhs.hesvh.cn

PHP:  count($arr);
来源：http://eih.zhengqikj.top

JS:   arr.length
来源：http://ouw.guannengcc.top

TS:   arr.length
来源：http://cll.shanyushiyangkeji.top

Java: list.size();
来源：http://oyl.yongpay.top

Go:   len(arr)
来源：http://ens.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://grz.nanxuanxn.top

C#:   list.Count;
来源：http://lba.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://bgp.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qnz.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nzk.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://ien.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://vkp.haohaochexian.top

Java: list.subList(1, 4);
来源：http://phy.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://ivm.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://yfo.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://fod.cqqwz.cn

[D08] 合并两个数组
来源：http://ozu.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://zut.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://hkg.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wxe.zhengqikj.top

TS:   [...a, ...b];
来源：http://svo.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rjh.pycfn.com

Go:   append(a, b...)
来源：http://nsl.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://foe.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://iiz.hnxiangtu.top

[D09] 排序（升序）
来源：http://yad.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://eae.jlsjyb.cn

PHP:  sort($arr);
来源：http://xud.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://keu.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eey.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cny.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ggh.hammf.cn

Ruby: arr.sort
来源：http://xci.chenjidiqi.icu

C#:   list.Sort();
来源：http://bon.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://mrd.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zrq.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gkm.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zmo.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqv.hywenlv.cn


<!-- 参考信息 -->