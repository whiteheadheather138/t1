代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdl.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://nhq.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nvn.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nlb.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sdj.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lrz.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ttk.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://abq.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://its.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nyx.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://lhy.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://dee.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://axt.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qly.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zwj.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nzf.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://onq.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://qsy.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nkd.dianchejie.cn

[B12] 跳出多层循环
来源：http://haf.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sjh.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dce.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jmo.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gow.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ghp.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwv.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iig.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ycx.ehwqpu.com

[B13] 判断是否为数字
来源：http://gfr.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://dts.mhx1999.top

PHP:  is_numeric($x)
来源：http://nld.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zcw.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lsz.cheryme.top

Java: x instanceof Number
来源：http://cjd.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://plg.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://dfr.guannengcc.top

C#:   x is int or double or decimal
来源：http://xga.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://fup.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kcx.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mxn.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://vxz.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://kyd.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://twc.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://drm.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://geg.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rxq.havefunace.top

[B15] 布尔运算与取反
来源：http://qkh.yueranfly.top

Py:   a and b or not c
来源：http://wto.andypj.xyz

PHP:  $a && $b || !$c
来源：http://qsx.jqgufenzy.top

JS:   a && b || !c
来源：http://akm.snrcjt.cn

TS:   a && b || !c
来源：http://yqo.gaohongyu789.top

Java: a && b || !c
来源：http://kaj.hongshengwenyu.top

Go:   a && b || !c
来源：http://wxf.ydzc1.top

Ruby: a && b || !c
来源：http://zbj.cqqwz.cn

C#:   a && b || !c
来源：http://zff.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xnc.sweek.top

Py:   if not data: return
来源：http://zfk.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://ngz.aibaodan.cn

JS:   if (!data) return;
来源：http://fjr.epnwcf.com

TS:   if (!data) return;
来源：http://xkc.xinyue.icu

Java: if (data == null) return;
来源：http://hni.chenlongwang.top

Go:   if data == nil { return }
来源：http://vvo.sxryk.cn

Ruby: return if data.nil?
来源：http://kwo.daria6918.cn

C#:   if (data == null) return;
来源：http://vni.yueranfly.top

================================================================================
来源：http://plq.yongpay.top

C. 函数与作用域
来源：http://flr.zhoulong.xyz

================================================================================
来源：http://lrk.hongshengwenyu.top

[C01] 定义函数
来源：http://veu.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://ala.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ljm.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://gqa.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://own.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mmh.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://joh.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://ebe.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mkj.cqqwz.cn

[C02] 默认参数
来源：http://ibe.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://gip.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://bos.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://dbv.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tfe.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://itm.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://anj.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://dxj.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://pdr.jiagoushi.top

[C03] 可变参数
来源：http://yhh.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://jok.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dyg.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nqs.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fuy.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mfw.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rzc.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://kkq.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pco.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://vpc.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqi.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qcw.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://glf.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dva.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://glp.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://dkn.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://jeu.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://rhw.fengsongda.top

[C05] 返回多个值
来源：http://hsg.wangdashe.top

Py:   return a, b
来源：http://rfz.0kj1m.cn

PHP:  return [$a, $b];
来源：http://xae.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://imv.gogol.net.cn

TS:   return { a, b };
来源：http://gkz.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gpf.cdnleiting.top

Go:   return a, b
来源：http://dtm.ehwqpu.com

Ruby: return a, b
来源：http://izx.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://qjy.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://lzk.hcnkem.com

Py:   square = lambda x: x * x
来源：http://gtn.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://koa.aizwys.cn

JS:   const square = x => x * x;
来源：http://lxf.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://sjb.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ojv.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://eaz.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://dyh.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zbd.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://awb.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zlj.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://qsd.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uhp.chenlongwang.top

TS:   arr.map(String)
来源：http://ovu.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cdt.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ack.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://zjx.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dgd.gaohongyu789.top

[C08] 闭包
来源：http://wkr.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qrl.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxf.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdx.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://niz.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhi.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://car.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bzk.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rxu.guannengcc.top

[C09] 递归
来源：http://xmc.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qpr.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://few.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzk.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://opp.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://umw.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tqk.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jja.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hga.fanxiaobao.xyz

[C10] 变量作用域
来源：http://otu.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pfq.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ydb.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gca.zhaomingkeji.xyz

TS:   同 JS
来源：http://syv.guowangkeji.top

Java: 方法内为块级作用域
来源：http://mey.fktsv.cn

Go:   花括号块级作用域
来源：http://uiu.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gzl.pengpengdd.cyou

C#:   块级作用域
来源：http://dnm.iojbl.cn

[C11] 模块导入与导出
来源：http://ulh.shzxlz.cn

Py:   from module import func
来源：http://auf.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mgq.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://uvc.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vvm.smart0.xyz

Java: import java.util.List;
来源：http://owm.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wgj.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://tab.xylfe.cn

C#:   using System.Text;
来源：http://uzd.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://atx.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://zvz.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://lvq.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://zue.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://wel.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vaf.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://umn.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://rtv.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pgv.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://szg.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hru.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ciq.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aje.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsw.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://fke.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://nbn.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mws.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://eei.ehwqpu.com

[C14] 泛型函数
来源：http://klq.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mlc.fzhhl.top

PHP:  // 无泛型
来源：http://owh.shanyushiyangtech.top

JS:   // 无泛型
来源：http://fmc.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kij.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ubf.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gxl.zhoulong.xyz

Ruby: # 无泛型
来源：http://spf.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sbh.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://dgm.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acw.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://nht.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xsg.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uxx.fktsv.cn

Java: // 无解构
来源：http://yob.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://dde.zhongyouzk.top

Ruby: a, b = pair
来源：http://luy.nwbrower.top

C#:   var (a, b) = pair;
来源：http://qoo.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://jxc.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rxk.yuanzhike.top

PHP:  // 无重载
来源：http://xdg.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qld.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://zsd.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uci.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://pdv.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://jxe.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qna.zycfv.cn

================================================================================
来源：http://dpm.hammf.cn

D. 数组 / 列表 / 集合
来源：http://ldh.nanxuanxn.top

================================================================================
来源：http://lys.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://nde.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kbm.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bbd.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jhm.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vkr.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pko.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://bhw.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://hif.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qes.fehbvm.com

[D02] 追加元素到末尾
来源：http://xxy.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oyv.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gsv.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://oka.316326.xyz

TS:   arr.push(4);
来源：http://del.yj20258888.top

Java: list.add(4);
来源：http://gxz.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://crl.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://hts.aizwys.cn

C#:   list.Add(4);
来源：http://exx.316326.xyz

[D03] 在指定位置插入元素
来源：http://wyq.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://auq.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://slv.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rsn.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://lwy.zhijiandao.cn

Java: list.add(0, 0);
来源：http://pgz.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tft.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jxp.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://mjv.daria6918.cn

[D04] 删除元素
来源：http://opg.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uns.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blf.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qof.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://vcb.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ysp.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sus.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dzo.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fcc.nanxuanxn.top

[D05] 访问与修改元素
来源：http://tim.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ibb.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jtf.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mfw.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://uex.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://bhd.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://eol.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://axq.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ztx.mhx1999.top

[D06] 数组长度
来源：http://cos.jianghu66.top

Py:   len(arr)
来源：http://zwj.xuetiantiany.cn

PHP:  count($arr);
来源：http://pcf.jiagoushi.top

JS:   arr.length
来源：http://rdu.cashguo.top

TS:   arr.length
来源：http://efq.gotoacloud.top

Java: list.size();
来源：http://har.fzhhl.top

Go:   len(arr)
来源：http://qao.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://czz.zhoulong.xyz

C#:   list.Count;
来源：http://gzx.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://vvz.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://snt.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://rog.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://rui.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://nms.hammf.cn

Java: list.subList(1, 4);
来源：http://ddy.ydjk.org.cn

Go:   arr[1:4]
来源：http://opw.epnwcf.com

Ruby: arr[1, 3]
来源：http://tzt.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://bai.jinqigufen.top

[D08] 合并两个数组
来源：http://zjz.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://ncz.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://gvj.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tgb.tian-w.cn

TS:   [...a, ...b];
来源：http://grm.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pau.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://ubq.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://gmd.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://mmt.shuidangran.top

[D09] 排序（升序）
来源：http://btt.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://hlj.zhongyouzk.top

PHP:  sort($arr);
来源：http://jsv.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dil.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uod.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zws.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pgk.xziqi.cn

Ruby: arr.sort
来源：http://dkn.yueranfly.top

C#:   list.Sort();
来源：http://gwy.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oey.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jhz.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xtq.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mch.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qqk.tanke756.top


<!-- 参考信息 -->