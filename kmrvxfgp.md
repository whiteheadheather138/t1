代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isi.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hml.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lpi.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://idm.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://paw.316326.xyz

[B10] 遍历同时拿索引
来源：http://daj.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://was.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fsi.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bkv.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iai.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hab.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfs.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wbi.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kli.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://wgk.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://mxt.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://vpy.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndc.daxiang520.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vas.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jlh.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vur.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://drb.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wns.zycfv.cn

[B12] 跳出多层循环
来源：http://lns.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vsq.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tqz.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbf.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnq.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jfg.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vpk.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ayu.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kan.jlsjyb.cn

[B13] 判断是否为数字
来源：http://yms.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://ywm.cdnleiting.top

PHP:  is_numeric($x)
来源：http://cwd.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsc.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nbn.hnqzz.top

Java: x instanceof Number
来源：http://xvr.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nuo.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://brc.gzhubu.top

C#:   x is int or double or decimal
来源：http://ldz.birdmap.top

[B14] 判断值是否在集合内
来源：http://puq.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yok.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vuh.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://dhr.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://qaz.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gon.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mnp.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://npx.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gij.pycfn.com

[B15] 布尔运算与取反
来源：http://rsl.iojbl.cn

Py:   a and b or not c
来源：http://veh.nwbrower.top

PHP:  $a && $b || !$c
来源：http://npo.ybcxt.top

JS:   a && b || !c
来源：http://ymj.ctjpmb.com

TS:   a && b || !c
来源：http://lyy.sysykeji.top

Java: a && b || !c
来源：http://idv.havefunace.top

Go:   a && b || !c
来源：http://xoi.epnwcf.com

Ruby: a && b || !c
来源：http://hxq.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://cxp.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://pyd.dianchejie.cn

Py:   if not data: return
来源：http://qya.tanke756.top

PHP:  if (!$data) { return; }
来源：http://mll.fehbvm.com

JS:   if (!data) return;
来源：http://veo.iojbl.cn

TS:   if (!data) return;
来源：http://vpe.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://neu.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://ybs.guowangkeji.top

Ruby: return if data.nil?
来源：http://dfg.9152youxi.cn

C#:   if (data == null) return;
来源：http://jrh.mhx1999.top

================================================================================
来源：http://zjw.pycfn.com

C. 函数与作用域
来源：http://ymh.sufxvd.cn

================================================================================
来源：http://pbl.pengpengdd.cyou

[C01] 定义函数
来源：http://qgt.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://cjb.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tej.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://myp.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dao.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nbu.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://slf.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://gma.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vho.wangshuangyany.cn

[C02] 默认参数
来源：http://yii.cheryme.top

Py:   def greet(name="World"): return name
来源：http://gpn.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hwh.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://dmt.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://izf.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://kuo.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jiq.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://hun.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://hkz.xziqi.cn

[C03] 可变参数
来源：http://uqv.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://zsv.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqi.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xci.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mip.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yas.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdz.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://puv.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hfd.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://nnm.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://knk.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jyt.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://utb.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pkl.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://mgc.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://weg.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://ndu.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://chp.yj20258.top

[C05] 返回多个值
来源：http://cab.hnxiangtu.top

Py:   return a, b
来源：http://vgi.dianchejie.cn

PHP:  return [$a, $b];
来源：http://zok.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wyl.xziqi.cn

TS:   return { a, b };
来源：http://jox.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wsp.tarul.cn

Go:   return a, b
来源：http://lls.yuxming.cn

Ruby: return a, b
来源：http://kvc.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://tdl.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://jxb.ivvv.top

Py:   square = lambda x: x * x
来源：http://zhn.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jtu.chenlongwang.top

JS:   const square = x => x * x;
来源：http://daa.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://eqs.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fyo.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bmj.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://ixv.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://qtl.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://qof.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kyb.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://tol.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wvx.yuxming.cn

TS:   arr.map(String)
来源：http://ngy.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fvv.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://urc.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://ylj.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mvr.jinqigufen.top

[C08] 闭包
来源：http://avg.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ezd.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nmc.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cen.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gob.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eub.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gse.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyx.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ite.yfazqb.com

[C09] 递归
来源：http://jur.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://evd.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zcr.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jci.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxk.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ere.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qjn.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wrq.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uzy.nanxinkj.top

[C10] 变量作用域
来源：http://brd.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tss.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dcj.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rnc.nwbrower.top

TS:   同 JS
来源：http://flm.hammf.cn

Java: 方法内为块级作用域
来源：http://qxs.andypj.xyz

Go:   花括号块级作用域
来源：http://bkw.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rgf.fzhhl.top

C#:   块级作用域
来源：http://day.ehwqpu.com

[C11] 模块导入与导出
来源：http://cmf.jiagoushi.top

Py:   from module import func
来源：http://mfu.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zwx.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xqk.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nqp.tanke756.top

Java: import java.util.List;
来源：http://tke.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://udy.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://sdd.c1oappe.top

C#:   using System.Text;
来源：http://jjl.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://dcq.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://qbp.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://dgi.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://cua.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://ygn.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gkq.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://nvu.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://ril.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nvu.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://gou.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://raj.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asl.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tni.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsa.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://gpr.hywenlv.cn

Go:   func add(a, b int) int
来源：http://wjz.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dbf.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://akh.tarul.cn

[C14] 泛型函数
来源：http://ric.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aop.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://oif.zdbjq.cn

JS:   // 无泛型
来源：http://krj.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kvs.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aol.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zat.shzxlz.cn

Ruby: # 无泛型
来源：http://bnh.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zhs.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://yza.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://daf.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://hxh.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://whk.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://awo.ybcxt.top

Java: // 无解构
来源：http://adt.yuxming.cn

Go:   // 无解构
来源：http://jrz.tianlin.xyz

Ruby: a, b = pair
来源：http://xdb.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://wvv.fzhhl.top

[C16] 函数 / 方法重载
来源：http://fyw.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bfy.daxiang520.top

PHP:  // 无重载
来源：http://kqn.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wie.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://nwy.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://smv.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://qbm.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://twa.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qod.ybcxt.top

================================================================================
来源：http://kwj.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://gpb.guowangkeji.top

================================================================================
来源：http://goa.bbcook.cn

[D01] 创建数组 / 列表
来源：http://gai.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xqp.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fgi.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qgy.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://thi.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bra.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://htp.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://nns.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jkj.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://bwz.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://itp.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iuj.dashuyun.cn

JS:   arr.push(4);
来源：http://wcn.sufxvd.cn

TS:   arr.push(4);
来源：http://jcb.gotoacloud.top

Java: list.add(4);
来源：http://osn.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://esl.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://uuv.zycfv.cn

C#:   list.Add(4);
来源：http://quk.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://jzr.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://bes.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mwv.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dvx.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://agi.chenzaomai.com

Java: list.add(0, 0);
来源：http://stu.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://kcx.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://btn.pycfn.com

C#:   list.Insert(0, 0);
来源：http://qwn.shanyushiyangtech.top

[D04] 删除元素
来源：http://odf.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aim.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xtx.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ess.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://jgi.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://smi.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xtp.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://apg.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dcn.tanke756.top

[D05] 访问与修改元素
来源：http://snj.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pvo.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oen.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mpx.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://bzr.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://lmy.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://tua.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mpo.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tfx.gotoacloud.top

[D06] 数组长度
来源：http://mkz.haohaochexian.top

Py:   len(arr)
来源：http://dib.sjlbkw.cn

PHP:  count($arr);
来源：http://ejp.shanyushiyangkeji.top

JS:   arr.length
来源：http://ohu.yj202588.top

TS:   arr.length
来源：http://fsn.hywenlv.cn

Java: list.size();
来源：http://xya.gotoacloud.top

Go:   len(arr)
来源：http://vox.ydzc1.top

Ruby: arr.length; arr.size
来源：http://iqy.zdqjudy.top

C#:   list.Count;
来源：http://mmn.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://end.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tgy.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://xep.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://bto.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://ryk.gogol.net.cn

Java: list.subList(1, 4);
来源：http://wsn.tanke756.top

Go:   arr[1:4]
来源：http://aeh.daria6918.cn

Ruby: arr[1, 3]
来源：http://qcs.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://yhs.zhoulong.xyz

[D08] 合并两个数组
来源：http://eiw.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://qac.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://ymz.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bfo.jiagoushi.top

TS:   [...a, ...b];
来源：http://owq.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bfk.zhoulong.xyz

Go:   append(a, b...)
来源：http://jel.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://bgy.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://rsa.aibaodan.cn

[D09] 排序（升序）
来源：http://zzc.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://qrq.tarul.cn

PHP:  sort($arr);
来源：http://jyu.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gtz.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://elo.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ogi.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://owf.gaohongyu789.top

Ruby: arr.sort
来源：http://sjy.hammf.cn

C#:   list.Sort();
来源：http://sjx.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gqj.iojbl.cn


<!-- 参考信息 -->