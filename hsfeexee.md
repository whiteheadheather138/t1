代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aag.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vbr.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xwk.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kpx.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yjc.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ofj.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://fam.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://kzc.cashguo.top

PHP:  range(0, 10, 2);
来源：http://zcl.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apz.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jaf.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://auq.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://evn.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://gsn.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bwa.gzhubu.top

[B12] 跳出多层循环
来源：http://skl.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jeh.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://btd.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fyy.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxw.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://orz.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncp.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://leq.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ull.mhx1999.top

[B13] 判断是否为数字
来源：http://fwd.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://vbq.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://pyq.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ovr.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wji.ivvv.top

Java: x instanceof Number
来源：http://smb.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dhs.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://cbp.daria6918.cn

C#:   x is int or double or decimal
来源：http://oqw.ybcxt.top

[B14] 判断值是否在集合内
来源：http://syp.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://prb.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qip.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://zwq.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://kpg.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yla.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vhq.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://dil.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xbh.andypj.xyz

[B15] 布尔运算与取反
来源：http://jlx.gaohongyu789.top

Py:   a and b or not c
来源：http://eub.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://nud.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://eag.redwolf501.top

TS:   a && b || !c
来源：http://jqw.daria6918.cn

Java: a && b || !c
来源：http://eyl.hysaishi.cn

Go:   a && b || !c
来源：http://ris.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://tbr.chenlongwang.top

C#:   a && b || !c
来源：http://xhc.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://kpz.redwolf501.top

Py:   if not data: return
来源：http://xpx.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://jtt.nwbrower.top

JS:   if (!data) return;
来源：http://oym.gogol.net.cn

TS:   if (!data) return;
来源：http://qaq.hesvh.cn

Java: if (data == null) return;
来源：http://zch.aibaodan.cn

Go:   if data == nil { return }
来源：http://fkg.bjfxy.top

Ruby: return if data.nil?
来源：http://mww.kuanghao11.cn

C#:   if (data == null) return;
来源：http://met.hongshengwenyu.top

================================================================================
来源：http://ahx.tianlin.xyz

C. 函数与作用域
来源：http://rkc.jinyuanbaomall.cn

================================================================================
来源：http://jzz.316326.xyz

[C01] 定义函数
来源：http://cfk.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://sus.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ygz.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://niq.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ero.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ube.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://dne.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://upa.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovu.jqgfzy.top

[C02] 默认参数
来源：http://pyx.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://yoe.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eru.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://ftj.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kgs.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ulx.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nzd.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://tee.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://uhq.ppjwa.cn

[C03] 可变参数
来源：http://ffs.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://zmq.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vpp.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgz.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aco.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qjy.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wkr.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hdh.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zpd.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://lwk.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://swd.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hpm.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rmx.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wfy.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://umj.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://wgb.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://spr.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://mqu.birdmap.top

[C05] 返回多个值
来源：http://ril.wangdashe.top

Py:   return a, b
来源：http://tqp.vehdjk.com

PHP:  return [$a, $b];
来源：http://kht.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nah.yuxming.cn

TS:   return { a, b };
来源：http://suo.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://itq.zhongyouzk.top

Go:   return a, b
来源：http://jso.dianchejie.cn

Ruby: return a, b
来源：http://vhx.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://zbc.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://fdq.yueranfly.top

Py:   square = lambda x: x * x
来源：http://pkj.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lpf.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://xds.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://asq.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rgn.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tsz.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://snz.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://azl.sweek.top

[C07] 把函数作为参数传入
来源：http://tba.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://san.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://jgq.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zlo.dianchejie.cn

TS:   arr.map(String)
来源：http://esn.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lfm.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bcf.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://pnl.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fxf.wangdashe.top

[C08] 闭包
来源：http://tfm.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pzi.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvb.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vhk.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pgf.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kul.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gxp.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://noj.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yym.zhaomingkeji.xyz

[C09] 递归
来源：http://crw.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpb.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dgm.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pez.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnk.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mjb.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cxh.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vkf.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nnf.sxryk.cn

[C10] 变量作用域
来源：http://eru.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gzz.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qrr.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ogg.ctjpmb.com

TS:   同 JS
来源：http://olp.jinqigufen.top

Java: 方法内为块级作用域
来源：http://fum.pycfn.com

Go:   花括号块级作用域
来源：http://mgk.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxo.pycfn.com

C#:   块级作用域
来源：http://pss.havefunace.top

[C11] 模块导入与导出
来源：http://ybr.birdmap.top

Py:   from module import func
来源：http://ygm.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://juy.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mda.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rqq.guannengcc.top

Java: import java.util.List;
来源：http://itt.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjb.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://uag.sxryk.cn

C#:   using System.Text;
来源：http://atu.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://oah.yj20258.top

Py:   (lambda: print("run"))()
来源：http://epl.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://nff.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://kds.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://myl.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lmv.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://zfk.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://bqm.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://acy.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://vdk.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqs.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrn.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fzx.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iko.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://hfr.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://hkx.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lzv.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://gzq.hnxiangtu.top

[C14] 泛型函数
来源：http://jkr.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zum.ybcxt.top

PHP:  // 无泛型
来源：http://mpd.xylfe.cn

JS:   // 无泛型
来源：http://hjd.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zpp.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://njn.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ahx.zhijiandao.cn

Ruby: # 无泛型
来源：http://qyk.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxn.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://rcm.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tcq.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://yzw.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oyp.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hli.mhx1999.top

Java: // 无解构
来源：http://ppw.yanxiufei.cn

Go:   // 无解构
来源：http://dna.hnqzz.top

Ruby: a, b = pair
来源：http://ymx.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://kkk.jianghu66.top

[C16] 函数 / 方法重载
来源：http://jcb.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ujo.fanxiaobao.xyz

PHP:  // 无重载
来源：http://clc.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tdf.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://qtc.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rqa.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://onm.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://miu.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tak.hesvh.cn

================================================================================
来源：http://iyc.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://kxr.jiagoushi.top

================================================================================
来源：http://nxd.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://mgl.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqj.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ncx.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bet.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uol.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pwn.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://tyd.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://eoc.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zrr.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://ptn.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pla.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vvh.fengsongda.top

JS:   arr.push(4);
来源：http://qgy.fktsv.cn

TS:   arr.push(4);
来源：http://azk.nwbrower.top

Java: list.add(4);
来源：http://lmf.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://bux.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://zoj.sweek.top

C#:   list.Add(4);
来源：http://zfc.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://xlm.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://eoa.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wpa.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://toz.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://zcj.epnwcf.com

Java: list.add(0, 0);
来源：http://iyl.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://cjl.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kfm.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://ugz.chenzaomai.com

[D04] 删除元素
来源：http://agn.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bcv.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwr.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tkd.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://xzx.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vnh.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dhg.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://efi.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://plu.jyoumei.cn

[D05] 访问与修改元素
来源：http://bed.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kcl.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pxq.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://emh.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://bhp.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://fmu.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://piu.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://skm.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vxg.hnxiangtu.top

[D06] 数组长度
来源：http://pps.cashguo.top

Py:   len(arr)
来源：http://mnx.sysykeji.top

PHP:  count($arr);
来源：http://otf.ywan-chungtsiang.top

JS:   arr.length
来源：http://wje.ydjk.org.cn

TS:   arr.length
来源：http://sgr.sufxvd.cn

Java: list.size();
来源：http://ffh.yongpay.top

Go:   len(arr)
来源：http://wrz.tanke756.top

Ruby: arr.length; arr.size
来源：http://pvj.bjfxy.top

C#:   list.Count;
来源：http://yrg.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://snx.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mtk.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://cyc.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://hyf.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://mts.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://ldu.xuetiantiany.cn

Go:   arr[1:4]
来源：http://tyz.zhengqikj.top

Ruby: arr[1, 3]
来源：http://bxi.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://jgd.xuanzx.com

[D08] 合并两个数组
来源：http://wnj.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://mxa.cheryme.top

PHP:  array_merge($a, $b);
来源：http://qbt.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ohd.hfpthk.cn

TS:   [...a, ...b];
来源：http://wzw.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eob.pycfn.com

Go:   append(a, b...)
来源：http://wht.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://rdr.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://wie.hfpthk.cn

[D09] 排序（升序）
来源：http://aje.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qjb.havefunace.top

PHP:  sort($arr);
来源：http://ifv.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://soh.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://raf.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eew.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qce.jqgfzy.top

Ruby: arr.sort
来源：http://mwt.fengsongda.top

C#:   list.Sort();
来源：http://dwa.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cjp.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gnb.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hif.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ioh.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngt.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xmh.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kqf.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fsi.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yfp.jqgufenzy.top


<!-- 参考信息 -->