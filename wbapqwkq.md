代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cze.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tmc.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lnd.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qyv.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxs.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://ibw.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvp.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udb.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://osf.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://evr.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tnh.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fcf.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://roy.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lle.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://qtx.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://bfa.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://ruw.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xkl.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ouo.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://omo.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qtn.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://kmg.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xip.jqgfzy.top

[B12] 跳出多层循环
来源：http://cbi.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://kew.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lbh.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cgd.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fpz.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://miv.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mkc.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ypz.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jno.ivvv.top

[B13] 判断是否为数字
来源：http://zmi.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://zfd.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://hnf.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wrr.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xet.yueranfly.top

Java: x instanceof Number
来源：http://wai.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://olq.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://ewa.yangfankeji.com

C#:   x is int or double or decimal
来源：http://npn.316326.xyz

[B14] 判断值是否在集合内
来源：http://svu.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tqq.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oqd.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://ikg.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://pth.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rhx.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ysg.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://uns.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gmp.bjfxy.top

[B15] 布尔运算与取反
来源：http://vuw.nwbrower.top

Py:   a and b or not c
来源：http://tux.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://rlu.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://sbt.jlsjyb.cn

TS:   a && b || !c
来源：http://kqk.wangshuangyany.cn

Java: a && b || !c
来源：http://syw.cdnleiting.top

Go:   a && b || !c
来源：http://xqz.ivvv.top

Ruby: a && b || !c
来源：http://xjl.jyoumei.cn

C#:   a && b || !c
来源：http://xea.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bfg.zhengqikj.top

Py:   if not data: return
来源：http://lqo.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://npz.gotoacloud.top

JS:   if (!data) return;
来源：http://xkn.shuidangran.top

TS:   if (!data) return;
来源：http://gms.jqgfzy.top

Java: if (data == null) return;
来源：http://kjd.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://rwo.ehwqpu.com

Ruby: return if data.nil?
来源：http://ykr.jyoumei.cn

C#:   if (data == null) return;
来源：http://mtu.shanyushiyangkeji.top

================================================================================
来源：http://oss.epnwcf.com

C. 函数与作用域
来源：http://tiv.yj20258888.top

================================================================================
来源：http://vnk.iojbl.cn

[C01] 定义函数
来源：http://lmo.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://sda.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgy.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://ekp.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xmy.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ohh.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://zpf.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://axs.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nfj.guowangkeji.top

[C02] 默认参数
来源：http://lfg.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://bhy.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jfv.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://aip.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vxd.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xhp.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vrk.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://kwi.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://crf.yuanzhike.top

[C03] 可变参数
来源：http://xlf.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://qmw.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ajp.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ijs.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pvb.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hyz.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jme.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://hia.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jgm.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://zcw.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gah.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yia.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sie.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgk.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://nda.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://odv.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://qmx.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://fys.feifeiyinyue.top

[C05] 返回多个值
来源：http://xlp.jqgufenzy.top

Py:   return a, b
来源：http://moj.guowangkeji.top

PHP:  return [$a, $b];
来源：http://pbz.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qqw.cucudq.cn

TS:   return { a, b };
来源：http://wbx.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ink.pengpengdd.cyou

Go:   return a, b
来源：http://inu.hammf.cn

Ruby: return a, b
来源：http://dxc.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://dpv.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://whk.vehdjk.com

Py:   square = lambda x: x * x
来源：http://qdi.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://ldm.aizwys.cn

JS:   const square = x => x * x;
来源：http://pzg.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://rkp.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qtf.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gfx.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://civ.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://qlj.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://gli.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zkk.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://fed.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sqh.meibo888.top

TS:   arr.map(String)
来源：http://yzg.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fmb.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://esu.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://zkt.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://gdg.chenzaomai.com

[C08] 闭包
来源：http://nod.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nic.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zdw.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ukw.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hsm.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sbp.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lea.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jzp.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yjr.cheryme.top

[C09] 递归
来源：http://okm.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wyg.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gkb.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvm.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wkt.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cyy.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xql.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rqs.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pys.yvedp.cn

[C10] 变量作用域
来源：http://chf.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tzg.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rvc.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://otj.zycfv.cn

TS:   同 JS
来源：http://tmv.meibo888.top

Java: 方法内为块级作用域
来源：http://bct.redwolf501.top

Go:   花括号块级作用域
来源：http://xex.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jjg.hnxiangtu.top

C#:   块级作用域
来源：http://kdh.kuanghao11.cn

[C11] 模块导入与导出
来源：http://cwf.0kj1m.cn

Py:   from module import func
来源：http://rvo.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://efh.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yge.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://szx.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://ato.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uye.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://ksp.fktsv.cn

C#:   using System.Text;
来源：http://ssk.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://dyu.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://wlr.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://xfy.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://nmn.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://mmt.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nfa.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://sup.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://urt.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ltn.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://kce.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gkg.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://een.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vfg.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://drd.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ycy.uphjek.com

Go:   func add(a, b int) int
来源：http://hxs.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ynu.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ueb.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://man.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xsx.feifeiyinyue.top

PHP:  // 无泛型
来源：http://jfa.zhijiandao.cn

JS:   // 无泛型
来源：http://htw.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://riq.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hsj.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://asa.zycfv.cn

Ruby: # 无泛型
来源：http://ysf.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xgn.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://gfu.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cju.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://asp.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://axr.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yvh.yangfankeji.com

Java: // 无解构
来源：http://fff.tianlin.xyz

Go:   // 无解构
来源：http://abf.tanke756.top

Ruby: a, b = pair
来源：http://fwt.zycfv.cn

C#:   var (a, b) = pair;
来源：http://rsx.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://thd.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iji.andypj.xyz

PHP:  // 无重载
来源：http://ceg.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nwz.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://yvu.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://wsu.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://jpa.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://toi.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kpt.smart0.xyz

================================================================================
来源：http://ppk.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://krw.zhiwuduotai.top

================================================================================
来源：http://qxc.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://buq.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljf.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://obn.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://atc.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nez.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dxg.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://xlw.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://ocl.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://okb.chenlongwang.top

[D02] 追加元素到末尾
来源：http://krb.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qms.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://frd.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://hep.havefunace.top

TS:   arr.push(4);
来源：http://cuj.xuetiantiany.cn

Java: list.add(4);
来源：http://ueo.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://yvb.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://dey.ybcxt.top

C#:   list.Add(4);
来源：http://xor.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://zyc.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://bjj.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nwc.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ejv.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://xuz.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://edn.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://mzu.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yxk.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://lqp.yj20258888.top

[D04] 删除元素
来源：http://kcc.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iti.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rhx.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jkb.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://ysz.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://amt.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gvx.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hbg.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sib.fzhhl.top

[D05] 访问与修改元素
来源：http://vxb.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ewa.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fea.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zqs.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://icw.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://wsp.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://zah.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fca.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hbc.yangfankeji.com

[D06] 数组长度
来源：http://ixe.jlsjyb.cn

Py:   len(arr)
来源：http://wlw.jlsjyb.cn

PHP:  count($arr);
来源：http://ztv.xingfuxueyuan.xyz

JS:   arr.length
来源：http://ppo.zdbjq.cn

TS:   arr.length
来源：http://wkg.ydzc1.top

Java: list.size();
来源：http://phz.ctjpmb.com

Go:   len(arr)
来源：http://omg.gzhubu.top

Ruby: arr.length; arr.size
来源：http://naz.fengsongda.top

C#:   list.Count;
来源：http://pfu.sysykeji.top

[D07] 切片 / 取子数组
来源：http://ybz.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ere.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tye.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://hai.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://wvz.aizwys.cn

Java: list.subList(1, 4);
来源：http://sks.zhongyouzk.top

Go:   arr[1:4]
来源：http://zap.ydzc1.top

Ruby: arr[1, 3]
来源：http://lsm.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://acz.cqqwz.cn

[D08] 合并两个数组
来源：http://erx.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://acf.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://aex.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ayj.gogol.net.cn

TS:   [...a, ...b];
来源：http://rqz.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vib.guannengcc.top

Go:   append(a, b...)
来源：http://fzx.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://tbs.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://yvp.yj20258.top

[D09] 排序（升序）
来源：http://ems.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://fia.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://ekx.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jeo.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fnz.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wli.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ame.jqgfzy.top

Ruby: arr.sort
来源：http://usv.jlsjyb.cn

C#:   list.Sort();
来源：http://rux.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://its.xuanzx.com


<!-- 参考信息 -->