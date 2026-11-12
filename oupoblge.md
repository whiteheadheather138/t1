代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xwv.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://axs.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ecv.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qhv.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lnj.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tzc.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://eam.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://iaz.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://ygo.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bxd.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rnq.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yew.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oeb.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://eil.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rro.yj20258888.top

[B12] 跳出多层循环
来源：http://mnv.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fcr.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wdg.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cij.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kwe.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bqy.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ige.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vll.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uwb.jqgfzy.top

[B13] 判断是否为数字
来源：http://hcl.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://lwf.316326.xyz

PHP:  is_numeric($x)
来源：http://rtj.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ojf.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ara.quarkkingdee.top

Java: x instanceof Number
来源：http://gbk.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dnh.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://hxb.ivvv.top

C#:   x is int or double or decimal
来源：http://vnx.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://aen.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://urx.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dae.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://haf.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://sui.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yng.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pwt.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ujo.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qay.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://yxf.ydzc1.top

Py:   a and b or not c
来源：http://mof.mhx1999.top

PHP:  $a && $b || !$c
来源：http://vrq.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://gll.chenzaomai.com

TS:   a && b || !c
来源：http://anw.mhx1999.top

Java: a && b || !c
来源：http://yqf.kuanghao11.cn

Go:   a && b || !c
来源：http://tty.quarkkingdee.top

Ruby: a && b || !c
来源：http://xvp.hnxiangtu.top

C#:   a && b || !c
来源：http://ruv.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://slb.cqqwz.cn

Py:   if not data: return
来源：http://qtx.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://ydn.wangdashe.top

JS:   if (!data) return;
来源：http://ohp.sysykeji.top

TS:   if (!data) return;
来源：http://sci.uphjek.com

Java: if (data == null) return;
来源：http://wux.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://xcr.nanxuanxn.top

Ruby: return if data.nil?
来源：http://snk.ybcxt.top

C#:   if (data == null) return;
来源：http://uxw.xuanzx.com

================================================================================
来源：http://jod.pengpengdd.cyou

C. 函数与作用域
来源：http://fjh.xylfe.cn

================================================================================
来源：http://ixy.jinqigfzy.top

[C01] 定义函数
来源：http://pie.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://taz.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbp.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://wup.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqt.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://qkl.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://wnb.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://voj.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oga.hesvh.cn

[C02] 默认参数
来源：http://oot.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://hae.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eon.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://ova.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pjb.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uqc.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://duc.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://eku.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://nsd.uphjek.com

[C03] 可变参数
来源：http://cyf.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://ofq.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eyt.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eet.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ayu.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vws.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rag.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://izm.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://enz.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://bzy.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdn.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lsf.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zwd.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://inn.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ztv.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://jbv.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://kov.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://khh.yfazqb.com

[C05] 返回多个值
来源：http://wbu.0kj1m.cn

Py:   return a, b
来源：http://nmb.fengsongda.top

PHP:  return [$a, $b];
来源：http://tmx.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://shw.guowangkeji.top

TS:   return { a, b };
来源：http://cmu.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fnx.shanyushiyangtech.top

Go:   return a, b
来源：http://enn.shzxlz.cn

Ruby: return a, b
来源：http://rap.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://vbv.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://bxy.birdmap.top

Py:   square = lambda x: x * x
来源：http://jpy.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kdq.yj202588.top

JS:   const square = x => x * x;
来源：http://ycb.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://qau.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://viv.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://hsl.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://pdy.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://xsg.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://bzf.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://syv.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://hkw.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eoz.gogol.net.cn

TS:   arr.map(String)
来源：http://qle.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyk.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqh.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://xlc.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dmk.sxryk.cn

[C08] 闭包
来源：http://scg.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfc.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ofl.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vey.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lbs.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zfn.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tph.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mde.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mqs.fengsongda.top

[C09] 递归
来源：http://bsv.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nld.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://acd.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbw.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ffd.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jrj.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mdc.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dxv.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://enl.hesvh.cn

[C10] 变量作用域
来源：http://gzg.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zch.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxd.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xob.zhiwuduotai.top

TS:   同 JS
来源：http://qmn.tian-w.cn

Java: 方法内为块级作用域
来源：http://gid.ybcxt.top

Go:   花括号块级作用域
来源：http://gul.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fcp.ywan-chungtsiang.top

C#:   块级作用域
来源：http://zmx.jinqigufen.top

[C11] 模块导入与导出
来源：http://wee.ybcxt.top

Py:   from module import func
来源：http://oia.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ppo.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vzu.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wkx.redwolf501.top

Java: import java.util.List;
来源：http://mbi.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aap.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://zrw.jqgufenzy.top

C#:   using System.Text;
来源：http://oio.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://zgp.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://xxn.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://zxi.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://mfe.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://sij.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://auf.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://jpy.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://zmf.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qyy.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://vkn.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rly.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://toy.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzz.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://afe.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ret.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://hvk.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bkv.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://hpy.zhoulong.xyz

[C14] 泛型函数
来源：http://tqy.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ocd.chenjidiqi.icu

PHP:  // 无泛型
来源：http://oup.uphjek.com

JS:   // 无泛型
来源：http://gif.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qnn.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ypv.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfv.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://iyh.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nwt.ybcxt.top

[C15] 解构 / 展开参数
来源：http://ytb.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://now.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://yfz.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eow.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ysa.52xcode.cn

Java: // 无解构
来源：http://cze.fzhhl.top

Go:   // 无解构
来源：http://shg.yangfankeji.com

Ruby: a, b = pair
来源：http://cvd.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://yjm.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://qut.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jxk.gogol.net.cn

PHP:  // 无重载
来源：http://wns.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gqx.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://lip.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ybs.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://dal.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://oyx.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sdu.zhengqikj.top

================================================================================
来源：http://dfw.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://ivt.svipenyu.cn

================================================================================
来源：http://qqj.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://uvw.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qgv.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eig.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://whd.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://evb.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nor.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://muh.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://ibp.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lrs.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://fea.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cfc.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fkx.0kj1m.cn

JS:   arr.push(4);
来源：http://gte.cqqwz.cn

TS:   arr.push(4);
来源：http://rvz.iojbl.cn

Java: list.add(4);
来源：http://sxy.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://gfm.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://qxy.hnqzz.top

C#:   list.Add(4);
来源：http://tvn.shuidangran.top

[D03] 在指定位置插入元素
来源：http://tre.cashguo.top

Py:   arr.insert(0, 0)
来源：http://uqh.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dvr.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mva.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://khw.tian-w.cn

Java: list.add(0, 0);
来源：http://kow.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://daq.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eda.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://mmc.sxryk.cn

[D04] 删除元素
来源：http://cpt.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cdy.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eds.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fuu.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://vbs.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jot.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sny.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dvy.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fxo.vqdsnc.cn

[D05] 访问与修改元素
来源：http://ylz.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://njl.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mai.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vvd.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://tdk.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://dan.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://imc.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpf.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ard.cashguo.top

[D06] 数组长度
来源：http://ysj.jlsjyb.cn

Py:   len(arr)
来源：http://oue.bbcook.cn

PHP:  count($arr);
来源：http://mcs.ydzc1.top

JS:   arr.length
来源：http://kin.snrcjt.cn

TS:   arr.length
来源：http://jcd.ppjwa.cn

Java: list.size();
来源：http://oxg.haohaochexian.top

Go:   len(arr)
来源：http://ckp.wangdashe.top

Ruby: arr.length; arr.size
来源：http://dyv.yangfankeji.com

C#:   list.Count;
来源：http://nbk.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://rlw.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ytt.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://gzi.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://tlo.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://top.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://nuv.aizwys.cn

Go:   arr[1:4]
来源：http://tsx.dashuyun.cn

Ruby: arr[1, 3]
来源：http://mcm.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://siz.yuanzhike.top

[D08] 合并两个数组
来源：http://xxt.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://qmc.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://boi.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ynb.guannengcc.top

TS:   [...a, ...b];
来源：http://rje.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ayr.yvedp.cn

Go:   append(a, b...)
来源：http://wqr.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://ydq.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://sbq.gogol.net.cn

[D09] 排序（升序）
来源：http://ohn.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://bgb.sufxvd.cn

PHP:  sort($arr);
来源：http://usu.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uth.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yup.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hou.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tnf.yfazqb.com

Ruby: arr.sort
来源：http://oia.tanke756.top

C#:   list.Sort();
来源：http://rni.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://poh.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qnv.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afx.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkv.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wsu.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pmu.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wyg.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fve.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ouw.jinyuanbaomall.cn


<!-- 参考信息 -->