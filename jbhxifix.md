代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kvg.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vcx.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://ayr.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://bir.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://yhn.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebg.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kwj.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://axl.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nus.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://oud.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kjw.hfpthk.cn

[B12] 跳出多层循环
来源：http://fdb.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yle.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fcd.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dnn.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ehk.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yqq.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bhr.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://skn.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zib.sufxvd.cn

[B13] 判断是否为数字
来源：http://bey.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://sxy.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://qwu.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ozn.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kce.zhiwuduotai.top

Java: x instanceof Number
来源：http://qjp.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bjw.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://yzi.tarul.cn

C#:   x is int or double or decimal
来源：http://zox.cheryme.top

[B14] 判断值是否在集合内
来源：http://rec.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xia.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://evq.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://tme.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://bha.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://arg.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lti.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://iyi.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://che.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://kxm.zhengqikj.top

Py:   a and b or not c
来源：http://blq.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://hpj.snrcjt.cn

JS:   a && b || !c
来源：http://atr.fengsongda.top

TS:   a && b || !c
来源：http://vtv.jinqigufen.top

Java: a && b || !c
来源：http://ila.fehbvm.com

Go:   a && b || !c
来源：http://iow.epnwcf.com

Ruby: a && b || !c
来源：http://pex.daria6918.cn

C#:   a && b || !c
来源：http://rvj.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://oqw.ehwqpu.com

Py:   if not data: return
来源：http://dna.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://lhh.yueranfly.top

JS:   if (!data) return;
来源：http://yek.ydjk.org.cn

TS:   if (!data) return;
来源：http://vdx.ehwqpu.com

Java: if (data == null) return;
来源：http://ovr.jinqigfzy.top

Go:   if data == nil { return }
来源：http://zjb.daxiang520.top

Ruby: return if data.nil?
来源：http://zec.jqgufenzy.top

C#:   if (data == null) return;
来源：http://zur.chenjidiqi.icu

================================================================================
来源：http://slx.hcnkem.com

C. 函数与作用域
来源：http://kcm.hfpthk.cn

================================================================================
来源：http://mbi.snrcjt.cn

[C01] 定义函数
来源：http://eho.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://jud.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://duk.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ahd.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vhc.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ypn.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://jfk.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://jzr.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wsk.nanxinkj.top

[C02] 默认参数
来源：http://avu.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://mjd.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ovk.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://ket.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pzo.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vku.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pdt.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://qzn.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://euv.hongshengwenyu.top

[C03] 可变参数
来源：http://xzb.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://uum.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ibl.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vfp.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vej.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jof.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://per.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://ycw.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bgm.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://klu.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kzz.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://alc.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mkq.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ddm.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ulk.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://uys.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://fiu.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://lpq.fktsv.cn

[C05] 返回多个值
来源：http://iqg.yonumen.top

Py:   return a, b
来源：http://aoh.hesvh.cn

PHP:  return [$a, $b];
来源：http://ost.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://jwx.pengpengdd.cyou

TS:   return { a, b };
来源：http://wcv.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hat.cqqwz.cn

Go:   return a, b
来源：http://xkl.kuanghao11.cn

Ruby: return a, b
来源：http://dqj.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://icu.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://fxd.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://mnf.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://srb.hnqzz.top

JS:   const square = x => x * x;
来源：http://hxx.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://uhu.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ozm.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://txz.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://gap.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://yia.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://nec.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wlg.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://ynf.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://otq.zhixingplan.top

TS:   arr.map(String)
来源：http://zrs.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjc.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aeg.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://ola.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bmg.jqgufenzy.top

[C08] 闭包
来源：http://ttx.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://olj.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fzg.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vjq.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kmv.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://neo.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gsk.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rxm.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nmx.cdnleiting.top

[C09] 递归
来源：http://krp.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dio.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zqd.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tri.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dlx.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qxo.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dhx.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://miu.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gwz.andypj.xyz

[C10] 变量作用域
来源：http://uur.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vuw.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mzu.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jvp.smart0.xyz

TS:   同 JS
来源：http://zuj.dianchejie.cn

Java: 方法内为块级作用域
来源：http://iuj.andypj.xyz

Go:   花括号块级作用域
来源：http://mnh.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdi.vehdjk.com

C#:   块级作用域
来源：http://lsr.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://fdr.chenzaomai.com

Py:   from module import func
来源：http://ach.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://hdy.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wqm.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aoj.shzxlz.cn

Java: import java.util.List;
来源：http://yrx.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmt.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://slg.dianchejie.cn

C#:   using System.Text;
来源：http://gvp.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://wvd.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://ksb.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://rmo.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://xbl.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://ugg.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qis.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://fsr.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://pnj.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cct.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://zcs.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xdq.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twe.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ipq.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtv.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://brr.birdmap.top

Go:   func add(a, b int) int
来源：http://pth.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gei.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://ipv.guowangkeji.top

[C14] 泛型函数
来源：http://hzd.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fcw.fktsv.cn

PHP:  // 无泛型
来源：http://wjh.bbcook.cn

JS:   // 无泛型
来源：http://gob.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lqu.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://auv.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jli.jianghu66.top

Ruby: # 无泛型
来源：http://xwg.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fgo.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://cgu.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://npb.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://rdh.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tfs.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ank.quarkkingdee.top

Java: // 无解构
来源：http://fwl.fktsv.cn

Go:   // 无解构
来源：http://tfy.chenlongwang.top

Ruby: a, b = pair
来源：http://qbq.316326.xyz

C#:   var (a, b) = pair;
来源：http://cmh.bjfxy.top

[C16] 函数 / 方法重载
来源：http://byl.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzs.guannengcc.top

PHP:  // 无重载
来源：http://dbf.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gxi.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://dbb.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kxf.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://dvw.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://ydg.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sfw.vehdjk.com

================================================================================
来源：http://azh.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://ggm.hfpthk.cn

================================================================================
来源：http://cih.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://wro.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vrr.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xuj.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://obq.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cwt.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://geh.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://zst.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://eho.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lqs.ehwqpu.com

[D02] 追加元素到末尾
来源：http://toz.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xci.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xqq.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://xww.9152youxi.cn

TS:   arr.push(4);
来源：http://nnw.aibaodan.cn

Java: list.add(4);
来源：http://bce.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://sgu.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://woy.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://bqm.yuxming.cn

[D03] 在指定位置插入元素
来源：http://ohi.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://uxs.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxp.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://toi.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://zul.guowangkeji.top

Java: list.add(0, 0);
来源：http://uvx.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://naj.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jcw.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://lkd.shanyushiyangtech.top

[D04] 删除元素
来源：http://wqz.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujg.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mez.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aio.ivvv.top

TS:   arr.splice(0, 1);
来源：http://bbc.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rrh.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nyy.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://znc.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://okb.quarkkingdee.top

[D05] 访问与修改元素
来源：http://aoi.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qjx.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sht.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zmn.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://lqr.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://tpq.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://qii.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ilt.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iig.zdbjq.cn

[D06] 数组长度
来源：http://ban.yonumen.top

Py:   len(arr)
来源：http://elf.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://oni.ehwqpu.com

JS:   arr.length
来源：http://gwe.vqdsnc.cn

TS:   arr.length
来源：http://xtr.hesvh.cn

Java: list.size();
来源：http://skm.daxiang520.top

Go:   len(arr)
来源：http://dee.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://xhq.yanxiufei.cn

C#:   list.Count;
来源：http://txi.yueranfly.top

[D07] 切片 / 取子数组
来源：http://zab.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qmo.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://cok.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://fsi.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://idk.hfpthk.cn

Java: list.subList(1, 4);
来源：http://moe.hongshengwenyu.top

Go:   arr[1:4]
来源：http://fdu.andypj.xyz

Ruby: arr[1, 3]
来源：http://jqd.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://ynm.wangshuangyany.cn

[D08] 合并两个数组
来源：http://ult.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://jzy.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://icg.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://axo.52xcode.cn

TS:   [...a, ...b];
来源：http://yrh.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aeu.ydzc1.top

Go:   append(a, b...)
来源：http://tvx.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://ecc.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://skm.iojbl.cn

[D09] 排序（升序）
来源：http://xnn.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://uyv.epnwcf.com

PHP:  sort($arr);
来源：http://msd.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ahl.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nur.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cwe.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://exp.daria6918.cn

Ruby: arr.sort
来源：http://tvr.kuanghao11.cn

C#:   list.Sort();
来源：http://ubc.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://njy.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://acp.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nql.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://osf.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cgb.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iop.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uqc.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ebp.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kca.mhx1999.top

[D11] 反转数组
来源：http://abl.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vdr.316326.xyz

PHP:  array_reverse($arr);
来源：http://uxx.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iir.tianlin.xyz


<!-- 参考信息 -->