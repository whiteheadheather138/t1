代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kuk.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jsj.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rnm.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pmr.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oem.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wuw.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://pfu.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://dyu.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://ynl.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nlz.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kmn.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mrr.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://avn.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://uue.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpz.gogol.net.cn

[B12] 跳出多层循环
来源：http://htc.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwn.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://vne.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnu.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sbo.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kgu.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dhq.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kgk.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uzy.yueranfly.top

[B13] 判断是否为数字
来源：http://jau.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://tkh.bjfxy.top

PHP:  is_numeric($x)
来源：http://zci.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfy.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ovu.iojbl.cn

Java: x instanceof Number
来源：http://cza.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nlo.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://ocp.mhx1999.top

C#:   x is int or double or decimal
来源：http://zcy.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://rgp.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://smn.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pqp.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://cwl.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://fbz.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://ucc.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zfr.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vym.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ibn.hnqzz.top

[B15] 布尔运算与取反
来源：http://van.yongpay.top

Py:   a and b or not c
来源：http://nie.sweek.top

PHP:  $a && $b || !$c
来源：http://uwh.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://yra.daxiang520.top

TS:   a && b || !c
来源：http://bhl.ehwqpu.com

Java: a && b || !c
来源：http://oum.gogol.net.cn

Go:   a && b || !c
来源：http://atk.gzhubu.top

Ruby: a && b || !c
来源：http://pbn.zhongyouzk.top

C#:   a && b || !c
来源：http://hdk.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zsl.jqgfzy.top

Py:   if not data: return
来源：http://kcg.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://xlu.yj202588.top

JS:   if (!data) return;
来源：http://kqh.xylfe.cn

TS:   if (!data) return;
来源：http://atj.hongshengwenyu.top

Java: if (data == null) return;
来源：http://wfg.sxryk.cn

Go:   if data == nil { return }
来源：http://bkp.kuanghao11.cn

Ruby: return if data.nil?
来源：http://ern.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://vqf.tian-w.cn

================================================================================
来源：http://cil.ppjwa.cn

C. 函数与作用域
来源：http://fxs.hfpthk.cn

================================================================================
来源：http://ili.zhengqikj.top

[C01] 定义函数
来源：http://ucg.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://jhc.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fhj.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://www.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqm.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://tbl.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://tvn.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://agb.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ojr.vehdjk.com

[C02] 默认参数
来源：http://usv.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://ncz.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yar.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://ebd.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wsn.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rxl.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mzt.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://ggh.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://ngd.jinyuanbaomall.cn

[C03] 可变参数
来源：http://qga.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://mff.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xuv.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iel.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vji.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hvo.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hob.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://cxj.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uhn.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://wkq.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zpj.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tgb.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gmr.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xrh.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://qgd.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://slq.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://joe.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://ruc.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://yqw.gzhubu.top

Py:   return a, b
来源：http://yyi.tarul.cn

PHP:  return [$a, $b];
来源：http://bgm.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gzv.9152youxi.cn

TS:   return { a, b };
来源：http://blo.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sun.yongpay.top

Go:   return a, b
来源：http://zky.hysaishi.cn

Ruby: return a, b
来源：http://cua.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://jyi.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://ibp.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://msk.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jjp.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://cqs.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://rwy.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dqp.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://qfo.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://lzs.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://dwi.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://ylv.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dvs.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://ulz.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lfn.chenlongwang.top

TS:   arr.map(String)
来源：http://ekh.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://euv.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lcc.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://oej.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://cqi.fanxiaobao.xyz

[C08] 闭包
来源：http://rxj.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ami.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qrv.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ios.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fio.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hep.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tsz.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tze.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rfm.ybcxt.top

[C09] 递归
来源：http://znk.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xjc.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nyg.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqv.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://abe.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://myv.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxm.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gnk.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lfg.xziqi.cn

[C10] 变量作用域
来源：http://kwf.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mjx.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kbk.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aoj.feifeiyinyue.top

TS:   同 JS
来源：http://bvh.hfpthk.cn

Java: 方法内为块级作用域
来源：http://ufc.9152youxi.cn

Go:   花括号块级作用域
来源：http://bvu.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oxb.birdmap.top

C#:   块级作用域
来源：http://ztc.ppjwa.cn

[C11] 模块导入与导出
来源：http://uem.ctjpmb.com

Py:   from module import func
来源：http://mfz.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aza.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hdo.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://haa.yj202588.top

Java: import java.util.List;
来源：http://zbr.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmm.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://rgb.nanxinkj.top

C#:   using System.Text;
来源：http://wmi.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://mnr.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://ric.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://ijm.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://ebj.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://kje.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xaw.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://mff.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://szm.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mfe.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://qnv.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ulh.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eht.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lbk.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://inz.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gev.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://xgf.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jbu.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ogw.yanxiufei.cn

[C14] 泛型函数
来源：http://jlp.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ntg.wangdashe.top

PHP:  // 无泛型
来源：http://pic.zhijiandao.cn

JS:   // 无泛型
来源：http://boo.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bfs.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mym.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://siu.yangfankeji.com

Ruby: # 无泛型
来源：http://oiu.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eop.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://iyo.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sks.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://qrx.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://buh.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iqi.birdmap.top

Java: // 无解构
来源：http://jrh.xinyue.icu

Go:   // 无解构
来源：http://lts.xinyue.icu

Ruby: a, b = pair
来源：http://ruy.c1oappe.top

C#:   var (a, b) = pair;
来源：http://cee.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://krg.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vcr.svipenyu.cn

PHP:  // 无重载
来源：http://bfz.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://twb.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://yht.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qgc.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://hku.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://wgm.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pge.gaohongyu789.top

================================================================================
来源：http://mxp.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://nnw.jqgfzy.top

================================================================================
来源：http://ozx.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://ydx.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dfq.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://prx.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ehq.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://efs.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cpr.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://bsf.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://gtw.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bxx.xylfe.cn

[D02] 追加元素到末尾
来源：http://mmo.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ywt.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fff.pengpengdd.cyou

JS:   arr.push(4);
来源：http://qhg.nanxinkj.top

TS:   arr.push(4);
来源：http://suv.aizwys.cn

Java: list.add(4);
来源：http://yya.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://rdy.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://gyq.bbcook.cn

C#:   list.Add(4);
来源：http://jgi.xinyue.icu

[D03] 在指定位置插入元素
来源：http://wdl.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://uek.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vxc.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://siq.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://bva.gaohongyu789.top

Java: list.add(0, 0);
来源：http://nkj.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://lqk.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntt.pycfn.com

C#:   list.Insert(0, 0);
来源：http://puq.zdbjq.cn

[D04] 删除元素
来源：http://kaa.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gmy.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qjo.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aoc.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://zci.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nvd.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wyy.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cem.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nrz.pycfn.com

[D05] 访问与修改元素
来源：http://svd.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpu.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uue.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qln.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://uop.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://njs.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://hux.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tog.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://unj.gzhubu.top

[D06] 数组长度
来源：http://qzi.jqgfzy.top

Py:   len(arr)
来源：http://zgn.uphjek.com

PHP:  count($arr);
来源：http://ebo.nanxinkj.top

JS:   arr.length
来源：http://xks.tarul.cn

TS:   arr.length
来源：http://and.andypj.xyz

Java: list.size();
来源：http://mwk.havefunace.top

Go:   len(arr)
来源：http://spf.bbcook.cn

Ruby: arr.length; arr.size
来源：http://oos.daria6918.cn

C#:   list.Count;
来源：http://fwo.jianghu66.top

[D07] 切片 / 取子数组
来源：http://uoo.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iea.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nhu.yj20258.top

JS:   arr.slice(1, 4);
来源：http://sde.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://wqg.aizwys.cn

Java: list.subList(1, 4);
来源：http://tlc.guannengcc.top

Go:   arr[1:4]
来源：http://erp.hfpthk.cn

Ruby: arr[1, 3]
来源：http://vfb.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://idp.vehdjk.com

[D08] 合并两个数组
来源：http://kxv.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://vvr.yongpay.top

PHP:  array_merge($a, $b);
来源：http://eqp.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nlq.yfazqb.com

TS:   [...a, ...b];
来源：http://kdz.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://emj.hysaishi.cn

Go:   append(a, b...)
来源：http://mii.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://vkv.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://kqh.tarul.cn

[D09] 排序（升序）
来源：http://pvb.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://gnw.pycfn.com

PHP:  sort($arr);
来源：http://vue.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfh.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://rxv.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ylf.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://atg.cashguo.top

Ruby: arr.sort
来源：http://chy.daria6918.cn

C#:   list.Sort();
来源：http://meg.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hwz.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zot.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uun.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uug.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ypg.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bxb.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aun.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zhi.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rfq.jianghu66.top


<!-- 参考信息 -->