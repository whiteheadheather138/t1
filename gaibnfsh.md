代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ule.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://pss.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://liy.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lvd.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bxb.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yzu.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hmt.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cnb.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cfm.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nvy.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://rba.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://dqh.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://kxl.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xsq.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slg.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fnw.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wmr.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://fdb.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kuj.zhoulong.xyz

[B12] 跳出多层循环
来源：http://dtk.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hoj.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://atx.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://unc.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfw.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://own.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mjq.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ngu.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fwu.9152youxi.cn

[B13] 判断是否为数字
来源：http://gxo.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://eui.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://mte.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://but.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://stj.ehwqpu.com

Java: x instanceof Number
来源：http://hmn.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vrb.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://mkt.ydzc1.top

C#:   x is int or double or decimal
来源：http://uzx.yuxming.cn

[B14] 判断值是否在集合内
来源：http://bba.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rwo.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ngz.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://pwq.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://nqd.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kja.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jqs.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uoe.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://krh.hcnkem.com

[B15] 布尔运算与取反
来源：http://lry.shzxlz.cn

Py:   a and b or not c
来源：http://fsy.vehdjk.com

PHP:  $a && $b || !$c
来源：http://iri.vqdsnc.cn

JS:   a && b || !c
来源：http://vqb.shuidangran.top

TS:   a && b || !c
来源：http://ins.gogol.net.cn

Java: a && b || !c
来源：http://hop.redwolf501.top

Go:   a && b || !c
来源：http://fzm.nanxuanxn.top

Ruby: a && b || !c
来源：http://jrq.kuanghao11.cn

C#:   a && b || !c
来源：http://ves.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://jlj.fktsv.cn

Py:   if not data: return
来源：http://syf.yj20258.top

PHP:  if (!$data) { return; }
来源：http://yvj.gzhubu.top

JS:   if (!data) return;
来源：http://now.ydzc1.top

TS:   if (!data) return;
来源：http://mhl.guowangkeji.top

Java: if (data == null) return;
来源：http://xsu.xziqi.cn

Go:   if data == nil { return }
来源：http://dgh.cheryme.top

Ruby: return if data.nil?
来源：http://naa.hywenlv.cn

C#:   if (data == null) return;
来源：http://dtp.xingfuxueyuan.xyz

================================================================================
来源：http://prh.9152youxi.cn

C. 函数与作用域
来源：http://amd.hfpthk.cn

================================================================================
来源：http://gqe.chenzaomai.com

[C01] 定义函数
来源：http://rhj.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://gph.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrk.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://yvm.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wyk.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vtc.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kjv.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://nuz.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zlh.jqgufenzy.top

[C02] 默认参数
来源：http://nck.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://gtn.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://bnw.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://nid.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kfe.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qhy.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jdy.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://spk.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://dut.snrcjt.cn

[C03] 可变参数
来源：http://jia.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://rtj.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lqy.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zci.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptb.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xli.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xfa.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://bxc.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ito.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://xma.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ayz.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qsi.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yhl.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zpt.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://rup.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://zvg.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://jdt.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://oun.hnqzz.top

[C05] 返回多个值
来源：http://iem.tianlin.xyz

Py:   return a, b
来源：http://pzz.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://phr.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qce.shanyushiyangtech.top

TS:   return { a, b };
来源：http://goi.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ief.jqgfzy.top

Go:   return a, b
来源：http://llu.aibaodan.cn

Ruby: return a, b
来源：http://axl.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://ryx.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://mzw.c1oappe.top

Py:   square = lambda x: x * x
来源：http://ymm.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pjt.bbcook.cn

JS:   const square = x => x * x;
来源：http://bcj.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://qyt.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qsm.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ene.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://fvk.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://kak.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://mpg.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zyw.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://fje.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kll.svipenyu.cn

TS:   arr.map(String)
来源：http://udv.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wzb.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://udv.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://lvf.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ouz.dashuyun.cn

[C08] 闭包
来源：http://mkm.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qwu.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mvf.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://itv.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bms.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uie.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jjq.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://obi.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ejy.wangdashe.top

[C09] 递归
来源：http://poi.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lnu.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://szy.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acc.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ibr.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwg.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ygy.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lwr.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gbz.zhixingplan.top

[C10] 变量作用域
来源：http://bni.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kws.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kti.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ppr.daria6918.cn

TS:   同 JS
来源：http://fqy.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://wmo.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://jkf.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hmg.jinyuanbaomall.cn

C#:   块级作用域
来源：http://cpy.yfazqb.com

[C11] 模块导入与导出
来源：http://wzi.dashuyun.cn

Py:   from module import func
来源：http://twm.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bkd.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zju.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hob.vqdsnc.cn

Java: import java.util.List;
来源：http://vfe.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nsc.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://ypq.mhx1999.top

C#:   using System.Text;
来源：http://kfn.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://tml.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://wuf.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://qpn.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://rkk.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://rkv.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxx.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://nex.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://yiy.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bab.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://gmj.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bhi.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oot.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nap.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxy.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://shc.wangdashe.top

Go:   func add(a, b int) int
来源：http://axh.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nrc.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://aca.svipenyu.cn

[C14] 泛型函数
来源：http://xti.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fpr.iojbl.cn

PHP:  // 无泛型
来源：http://dhw.jqgfzy.top

JS:   // 无泛型
来源：http://kzf.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lia.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ffl.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bdf.fengsongda.top

Ruby: # 无泛型
来源：http://bjx.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aox.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://oan.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fsa.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://dir.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqn.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://opg.quarkkingdee.top

Java: // 无解构
来源：http://upo.ivvv.top

Go:   // 无解构
来源：http://rix.sjlbkw.cn

Ruby: a, b = pair
来源：http://urc.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://nom.yuxming.cn

[C16] 函数 / 方法重载
来源：http://ynh.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kut.daria6918.cn

PHP:  // 无重载
来源：http://hks.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kmn.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://pjq.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aqj.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://fxq.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://pqp.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://vns.gzhubu.top

================================================================================
来源：http://elj.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://vvb.hammf.cn

================================================================================
来源：http://anh.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://kdx.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lcb.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tzt.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zab.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vte.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sod.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://pfa.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://krq.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bmd.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://ugz.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fby.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sfz.ivvv.top

JS:   arr.push(4);
来源：http://svx.ydjk.org.cn

TS:   arr.push(4);
来源：http://frt.jinqigfzy.top

Java: list.add(4);
来源：http://mne.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://ivi.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://zqb.cashguo.top

C#:   list.Add(4);
来源：http://xpm.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://dyl.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://vdw.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wed.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bji.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://kwu.xylfe.cn

Java: list.add(0, 0);
来源：http://dph.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lbs.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kqd.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://jtw.cashguo.top

[D04] 删除元素
来源：http://bmb.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zoe.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zyj.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uwm.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://qki.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nxz.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gvv.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wjf.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://icj.shuidangran.top

[D05] 访问与修改元素
来源：http://vjr.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://adf.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vvg.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ctc.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://yiv.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://qmj.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://ann.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kur.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ibk.snrcjt.cn

[D06] 数组长度
来源：http://gjm.sweek.top

Py:   len(arr)
来源：http://xow.daria6918.cn

PHP:  count($arr);
来源：http://dht.sysykeji.top

JS:   arr.length
来源：http://kgq.shanyushiyangtech.top

TS:   arr.length
来源：http://gms.pengpengdd.cyou

Java: list.size();
来源：http://wss.yueranfly.top

Go:   len(arr)
来源：http://shw.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://wiu.kuanghao11.cn

C#:   list.Count;
来源：http://iyy.uphjek.com

[D07] 切片 / 取子数组
来源：http://ulg.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lng.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://uuk.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://foj.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://uws.haohaochexian.top

Java: list.subList(1, 4);
来源：http://mzf.xylfe.cn

Go:   arr[1:4]
来源：http://net.pycfn.com

Ruby: arr[1, 3]
来源：http://toh.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://tzr.dashuyun.cn

[D08] 合并两个数组
来源：http://ysq.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://dqe.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://wog.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://daa.xylfe.cn

TS:   [...a, ...b];
来源：http://vyr.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://shy.ybcxt.top

Go:   append(a, b...)
来源：http://mok.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://rzu.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://yqn.zdbjq.cn

[D09] 排序（升序）
来源：http://snz.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://nir.nanxinkj.top

PHP:  sort($arr);
来源：http://xca.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qnp.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xat.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hdf.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://svr.mhx1999.top

Ruby: arr.sort
来源：http://llu.ppjwa.cn

C#:   list.Sort();
来源：http://vvq.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vkk.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qwk.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aot.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lam.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://osc.xziqi.cn


<!-- 参考信息 -->