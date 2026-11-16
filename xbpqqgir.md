代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ksp.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kjl.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ote.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gtl.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://odc.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jvq.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://cxk.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://fdd.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://cxh.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzu.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mmb.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wta.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ztt.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://zgu.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cmv.yonumen.top

[B12] 跳出多层循环
来源：http://hxi.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://cbn.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bmi.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lxl.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ado.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qzr.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://znt.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vwg.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oox.xinyue.icu

[B13] 判断是否为数字
来源：http://wlf.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://tok.cdnleiting.top

PHP:  is_numeric($x)
来源：http://gxi.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vhx.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bvq.andypj.xyz

Java: x instanceof Number
来源：http://kzt.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecu.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://ntr.mhx1999.top

C#:   x is int or double or decimal
来源：http://jzv.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://eeq.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xdz.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xay.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gjw.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://uph.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ujh.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxb.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://sre.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mtd.yonumen.top

[B15] 布尔运算与取反
来源：http://zfm.nwbrower.top

Py:   a and b or not c
来源：http://bqf.guannengcc.top

PHP:  $a && $b || !$c
来源：http://ojg.9152youxi.cn

JS:   a && b || !c
来源：http://ayh.hesvh.cn

TS:   a && b || !c
来源：http://rkc.hfpthk.cn

Java: a && b || !c
来源：http://oic.dianchejie.cn

Go:   a && b || !c
来源：http://ohy.iojbl.cn

Ruby: a && b || !c
来源：http://nmi.meibo888.top

C#:   a && b || !c
来源：http://zvn.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gsy.gaohongyu789.top

Py:   if not data: return
来源：http://qjf.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://qhn.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://hjs.xuanzx.com

TS:   if (!data) return;
来源：http://mbw.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://wmf.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://yvc.jinqigufen.top

Ruby: return if data.nil?
来源：http://xpb.tarul.cn

C#:   if (data == null) return;
来源：http://din.sysykeji.top

================================================================================
来源：http://mnq.shuidangran.top

C. 函数与作用域
来源：http://njt.xingfuxueyuan.xyz

================================================================================
来源：http://sci.yuxming.cn

[C01] 定义函数
来源：http://wvi.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://qqr.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yci.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://tdr.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zen.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zrv.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://rxu.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://ube.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://doa.jinqigufen.top

[C02] 默认参数
来源：http://dnw.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://dgb.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://oqx.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wgq.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hwn.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://csy.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hox.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://tut.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://jot.zhongyouzk.top

[C03] 可变参数
来源：http://otp.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://uxz.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gay.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xyj.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blu.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rxe.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aqj.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://qba.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eqf.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://wgf.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jkv.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mne.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pjn.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yze.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://hzw.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://bjh.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://uwz.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://hlm.jinghuilouyu.cn

[C05] 返回多个值
来源：http://tcb.svipenyu.cn

Py:   return a, b
来源：http://bpw.yangfankeji.com

PHP:  return [$a, $b];
来源：http://jpg.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fzl.birdmap.top

TS:   return { a, b };
来源：http://xvw.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tom.haohaochexian.top

Go:   return a, b
来源：http://pck.uphjek.com

Ruby: return a, b
来源：http://dye.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nlv.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://vxj.hcnkem.com

Py:   square = lambda x: x * x
来源：http://rjy.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fga.nanxinkj.top

JS:   const square = x => x * x;
来源：http://jxm.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://zcc.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jvr.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://ami.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://pkk.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://aez.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://oxu.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://anl.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://kvk.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://npz.ydjk.org.cn

TS:   arr.map(String)
来源：http://gbs.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oto.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fjn.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://qsk.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cvc.zhengqikj.top

[C08] 闭包
来源：http://bcj.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lpl.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hde.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jmg.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dnp.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kcj.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipn.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zno.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://irr.yueranfly.top

[C09] 递归
来源：http://tgk.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oru.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://utr.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://row.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gze.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jht.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://thm.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kcr.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gsd.yuanzhike.top

[C10] 变量作用域
来源：http://sjf.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tgv.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zwc.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nkl.epnwcf.com

TS:   同 JS
来源：http://gqo.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://hua.chenlongwang.top

Go:   花括号块级作用域
来源：http://jwd.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://edw.xuanzx.com

C#:   块级作用域
来源：http://pxh.quarkkingdee.top

[C11] 模块导入与导出
来源：http://jcm.hnxiangtu.top

Py:   from module import func
来源：http://koy.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dxb.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xqe.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eid.yangfankeji.com

Java: import java.util.List;
来源：http://wjg.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bnn.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://ijt.pycfn.com

C#:   using System.Text;
来源：http://tur.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://kti.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://asr.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://pvw.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://sta.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://emi.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rsi.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://qui.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://yrc.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dnw.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://rkm.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wkt.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lwu.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qzw.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xtf.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://clu.aibaodan.cn

Go:   func add(a, b int) int
来源：http://zag.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gzs.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://gwm.ydzc1.top

[C14] 泛型函数
来源：http://mbr.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tqf.mhx1999.top

PHP:  // 无泛型
来源：http://hud.chenlongwang.top

JS:   // 无泛型
来源：http://rgs.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pbn.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kig.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jht.yuanzhike.top

Ruby: # 无泛型
来源：http://bml.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qub.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://ecf.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xfk.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://vly.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qaq.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://izx.xinyue.icu

Java: // 无解构
来源：http://uaq.yuxming.cn

Go:   // 无解构
来源：http://dzr.yfazqb.com

Ruby: a, b = pair
来源：http://lll.fzhhl.top

C#:   var (a, b) = pair;
来源：http://lgx.jianghu66.top

[C16] 函数 / 方法重载
来源：http://nse.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qma.yonumen.top

PHP:  // 无重载
来源：http://jko.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://egb.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://jog.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://slr.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://sat.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://sri.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xpv.yonumen.top

================================================================================
来源：http://bjo.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://ous.316326.xyz

================================================================================
来源：http://jna.xziqi.cn

[D01] 创建数组 / 列表
来源：http://dum.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fct.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kby.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lfe.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vtd.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tnx.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://hty.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://ryk.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ecx.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://ujq.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://abm.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mna.shangyingyoupin.top

JS:   arr.push(4);
来源：http://ogy.ehwqpu.com

TS:   arr.push(4);
来源：http://dmk.birdmap.top

Java: list.add(4);
来源：http://mku.yj20258.top

Go:   arr = append(arr, 4)
来源：http://jzd.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://fva.zdbjq.cn

C#:   list.Add(4);
来源：http://wob.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://fgt.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://eqe.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://abk.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uld.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://kgm.ppjwa.cn

Java: list.add(0, 0);
来源：http://dtr.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://qzt.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mfj.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://gpl.yj20258.top

[D04] 删除元素
来源：http://say.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hcq.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xsk.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wuv.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://nuc.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ugu.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hzu.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iik.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wuc.xylfe.cn

[D05] 访问与修改元素
来源：http://muy.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kwz.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ltr.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://keh.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://xaf.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://jkb.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://jgg.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://prf.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vsi.jqgufenzy.top

[D06] 数组长度
来源：http://kxp.cheryme.top

Py:   len(arr)
来源：http://qnt.yj20258.top

PHP:  count($arr);
来源：http://ghc.hywenlv.cn

JS:   arr.length
来源：http://yke.chenzaomai.com

TS:   arr.length
来源：http://mdr.sysykeji.top

Java: list.size();
来源：http://mxt.tarul.cn

Go:   len(arr)
来源：http://qks.xinyue.icu

Ruby: arr.length; arr.size
来源：http://rvg.daria6918.cn

C#:   list.Count;
来源：http://pri.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://clg.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yfl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://htn.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://efy.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://ylt.nwbrower.top

Java: list.subList(1, 4);
来源：http://yan.zdbjq.cn

Go:   arr[1:4]
来源：http://rkk.jqgfzy.top

Ruby: arr[1, 3]
来源：http://bpg.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://lsn.meibo888.top

[D08] 合并两个数组
来源：http://uki.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://flx.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://yet.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yhf.cheryme.top

TS:   [...a, ...b];
来源：http://izw.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://udh.cdnleiting.top

Go:   append(a, b...)
来源：http://rxk.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://mcu.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://fix.jiagoushi.top

[D09] 排序（升序）
来源：http://wbk.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://ylr.redwolf501.top

PHP:  sort($arr);
来源：http://mbw.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bbf.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://lwv.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mqf.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ntb.tianlin.xyz

Ruby: arr.sort
来源：http://jif.havefunace.top

C#:   list.Sort();
来源：http://xxv.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fnq.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://glj.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bdx.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tst.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gno.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mmx.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zsd.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eta.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://efy.daxiang520.top


<!-- 参考信息 -->