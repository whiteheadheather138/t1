代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyr.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://vxl.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nkq.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xoh.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dsh.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hwg.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qpv.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xaj.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://omn.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jjb.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://afk.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://qzr.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://yjx.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://but.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oca.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ksg.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://han.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://lbj.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://asa.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://kqi.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kkm.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lsa.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eaw.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uuk.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wiw.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ede.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ljq.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lls.zhixingplan.top

[B13] 判断是否为数字
来源：http://grx.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://ape.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://zdp.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uiy.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qtm.bjfxy.top

Java: x instanceof Number
来源：http://rik.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nrj.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://rbp.0kj1m.cn

C#:   x is int or double or decimal
来源：http://his.ybcxt.top

[B14] 判断值是否在集合内
来源：http://erx.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://seu.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://enw.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://mhh.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://lqg.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://eyy.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dxr.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://jvh.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vfr.zhengqikj.top

[B15] 布尔运算与取反
来源：http://led.yj20258888.top

Py:   a and b or not c
来源：http://ert.316326.xyz

PHP:  $a && $b || !$c
来源：http://khz.zdqjudy.top

JS:   a && b || !c
来源：http://zpp.316326.xyz

TS:   a && b || !c
来源：http://xuf.c1oappe.top

Java: a && b || !c
来源：http://sza.yangfankeji.com

Go:   a && b || !c
来源：http://tdk.ivvv.top

Ruby: a && b || !c
来源：http://laa.jianghu66.top

C#:   a && b || !c
来源：http://ybl.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://sxc.yvedp.cn

Py:   if not data: return
来源：http://vnk.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://ngd.aizwys.cn

JS:   if (!data) return;
来源：http://kdo.zhongyouzk.top

TS:   if (!data) return;
来源：http://vwe.yuanzhike.top

Java: if (data == null) return;
来源：http://vxc.yanxiufei.cn

Go:   if data == nil { return }
来源：http://nvb.chenlongwang.top

Ruby: return if data.nil?
来源：http://iqi.birdmap.top

C#:   if (data == null) return;
来源：http://eyf.52xcode.cn

================================================================================
来源：http://hac.hesvh.cn

C. 函数与作用域
来源：http://maa.daria6918.cn

================================================================================
来源：http://wbf.vqdsnc.cn

[C01] 定义函数
来源：http://ijn.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://uon.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrx.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://zux.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqp.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://uee.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lbj.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://vin.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eoc.iojbl.cn

[C02] 默认参数
来源：http://qul.havefunace.top

Py:   def greet(name="World"): return name
来源：http://gek.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rfi.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://wek.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ytj.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tst.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iwu.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://vkk.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nrw.daxiang520.top

[C03] 可变参数
来源：http://oyh.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://fgl.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wgi.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://amv.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://juj.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pob.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nhs.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tvk.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://clr.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://gar.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ksc.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://doy.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fng.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://osv.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://bxx.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://iuy.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://skm.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://rtu.sjlbkw.cn

[C05] 返回多个值
来源：http://gfc.uphjek.com

Py:   return a, b
来源：http://caa.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://dwa.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xmo.hfpthk.cn

TS:   return { a, b };
来源：http://xuq.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vzb.sufxvd.cn

Go:   return a, b
来源：http://mbe.tanke756.top

Ruby: return a, b
来源：http://zqy.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://ulx.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://wwx.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://uhg.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oru.fehbvm.com

JS:   const square = x => x * x;
来源：http://xrj.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://oii.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://trj.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://kma.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://fdr.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://aqj.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://rdz.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dyv.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://nfm.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vdy.gotoacloud.top

TS:   arr.map(String)
来源：http://zaa.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ahn.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wmg.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://bqv.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vwe.fzhhl.top

[C08] 闭包
来源：http://foz.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zwk.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lep.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ojo.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pxv.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kyf.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ixc.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tuv.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ahk.hnxiangtu.top

[C09] 递归
来源：http://uas.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wjm.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yni.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qui.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijj.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sdp.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pka.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iex.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://toy.yj20258.top

[C10] 变量作用域
来源：http://qdo.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nup.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fme.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yqi.pengpengdd.cyou

TS:   同 JS
来源：http://jhf.jianghu66.top

Java: 方法内为块级作用域
来源：http://qef.meibo888.top

Go:   花括号块级作用域
来源：http://bwb.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ybe.zhongyouzk.top

C#:   块级作用域
来源：http://jar.bjfxy.top

[C11] 模块导入与导出
来源：http://zeo.feifeiyinyue.top

Py:   from module import func
来源：http://xgl.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ozs.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://vju.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ino.jinqigfzy.top

Java: import java.util.List;
来源：http://vhu.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qcz.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://aaq.nanxuanxn.top

C#:   using System.Text;
来源：http://ale.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://xol.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://lqi.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://djt.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://wuy.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://zle.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tlz.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://jvx.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://jea.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lnt.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://rgp.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pwx.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ujp.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://spr.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://swx.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://gxh.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://lvg.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hjc.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://ptv.hammf.cn

[C14] 泛型函数
来源：http://ffs.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gcu.hesvh.cn

PHP:  // 无泛型
来源：http://bmx.snrcjt.cn

JS:   // 无泛型
来源：http://ezn.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ohb.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvg.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://psi.zhijiandao.cn

Ruby: # 无泛型
来源：http://fdw.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://asm.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://wvm.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kzd.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://anh.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzz.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wcm.hysaishi.cn

Java: // 无解构
来源：http://lwu.zhongyouzk.top

Go:   // 无解构
来源：http://pxm.zhixingplan.top

Ruby: a, b = pair
来源：http://lli.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://lcr.cashguo.top

[C16] 函数 / 方法重载
来源：http://jzb.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ueg.yvedp.cn

PHP:  // 无重载
来源：http://vdg.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://abk.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://wbr.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vyb.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://nek.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://cgn.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dxt.vehdjk.com

================================================================================
来源：http://vbn.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://qhu.jqgfzy.top

================================================================================
来源：http://lfa.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://fol.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oxc.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jue.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sky.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://czt.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jhi.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ndj.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://fpo.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ljh.tianlin.xyz

[D02] 追加元素到末尾
来源：http://ggo.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://azc.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wkc.haohaochexian.top

JS:   arr.push(4);
来源：http://msb.yuxming.cn

TS:   arr.push(4);
来源：http://muf.cucudq.cn

Java: list.add(4);
来源：http://vmq.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://wez.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://gky.ybcxt.top

C#:   list.Add(4);
来源：http://sfl.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://xqh.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://glb.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zqt.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://skb.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://hpd.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://khu.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://nsk.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://doh.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://jng.gotoacloud.top

[D04] 删除元素
来源：http://xwz.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pof.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aag.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kag.uphjek.com

TS:   arr.splice(0, 1);
来源：http://krj.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qlq.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aht.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://utb.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vcs.gaohongyu789.top

[D05] 访问与修改元素
来源：http://dsa.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fvx.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zcw.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ozw.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://ity.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://sni.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://vfp.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rwl.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sry.jqgufenzy.top

[D06] 数组长度
来源：http://utx.shuidangran.top

Py:   len(arr)
来源：http://yqu.quarkkingdee.top

PHP:  count($arr);
来源：http://qrr.ivvv.top

JS:   arr.length
来源：http://xyd.gzhubu.top

TS:   arr.length
来源：http://fdw.nanxuanxn.top

Java: list.size();
来源：http://agm.jqgufenzy.top

Go:   len(arr)
来源：http://ctb.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://rgt.zhoulong.xyz

C#:   list.Count;
来源：http://xdo.yonumen.top

[D07] 切片 / 取子数组
来源：http://nrv.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mcf.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://sbg.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://lzl.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://ewy.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://gkv.yanxiufei.cn

Go:   arr[1:4]
来源：http://dqz.jqgfzy.top

Ruby: arr[1, 3]
来源：http://pjx.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://uuk.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://opr.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://uey.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://xpx.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ofh.jlsjyb.cn

TS:   [...a, ...b];
来源：http://jyy.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wqq.jqgufenzy.top

Go:   append(a, b...)
来源：http://xks.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://nzl.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://bmx.wangdashe.top

[D09] 排序（升序）
来源：http://wpf.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://xrb.shzxlz.cn

PHP:  sort($arr);
来源：http://mhr.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oeh.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://arl.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nto.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kew.ctjpmb.com

Ruby: arr.sort
来源：http://ger.cucudq.cn

C#:   list.Sort();
来源：http://lol.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://epz.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iqd.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwa.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://alr.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://beb.jqgufenzy.top


<!-- 参考信息 -->