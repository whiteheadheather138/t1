代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpw.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgg.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nnn.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wwk.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdl.yj202588.top

[B10] 遍历同时拿索引
来源：http://cgg.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qra.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lnk.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qwk.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://odz.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cib.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hzo.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyf.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fyv.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://mld.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://uyf.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://tzy.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yac.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vrf.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://shb.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zkb.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://dbb.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xws.jlsjyb.cn

[B12] 跳出多层循环
来源：http://gln.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cqt.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fjg.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ocg.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qmk.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ejy.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bse.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dng.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qqp.cdnleiting.top

[B13] 判断是否为数字
来源：http://jvl.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://lbc.chenzaomai.com

PHP:  is_numeric($x)
来源：http://voq.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkj.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrc.daxiang520.top

Java: x instanceof Number
来源：http://rqb.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://smf.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://ely.yuxming.cn

C#:   x is int or double or decimal
来源：http://xpr.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://jxp.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wdq.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qpx.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://eli.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://bhf.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hvn.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xae.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ioj.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aup.yvedp.cn

[B15] 布尔运算与取反
来源：http://anl.fzhhl.top

Py:   a and b or not c
来源：http://yft.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://did.nanxuanxn.top

JS:   a && b || !c
来源：http://slm.ehwqpu.com

TS:   a && b || !c
来源：http://bkt.9152youxi.cn

Java: a && b || !c
来源：http://vpu.nanxinkj.top

Go:   a && b || !c
来源：http://wxf.meibo888.top

Ruby: a && b || !c
来源：http://trj.yj20258.top

C#:   a && b || !c
来源：http://qxk.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://erk.jiagoushi.top

Py:   if not data: return
来源：http://ply.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://jdq.yj202588.top

JS:   if (!data) return;
来源：http://qsv.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://fcw.birdmap.top

Java: if (data == null) return;
来源：http://edo.uphjek.com

Go:   if data == nil { return }
来源：http://vtg.snrcjt.cn

Ruby: return if data.nil?
来源：http://ccl.dianchejie.cn

C#:   if (data == null) return;
来源：http://egn.ydzc1.top

================================================================================
来源：http://lpg.jiagoushi.top

C. 函数与作用域
来源：http://swp.zdqjudy.top

================================================================================
来源：http://oyo.bjfxy.top

[C01] 定义函数
来源：http://wzw.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://wkm.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqj.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://bpn.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osi.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jor.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://tgb.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://lvc.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ltf.hesvh.cn

[C02] 默认参数
来源：http://yiw.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://ota.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://lvt.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://ooj.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iqg.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kqg.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nbc.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://gdg.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://uvp.hnqzz.top

[C03] 可变参数
来源：http://yek.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://twr.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://byy.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dqo.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcq.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oem.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pfv.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://anh.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pwr.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://fjl.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wkt.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mdn.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mtz.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lih.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://lwz.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://mla.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://tqx.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://lay.dianchejie.cn

[C05] 返回多个值
来源：http://khe.ehwqpu.com

Py:   return a, b
来源：http://lgm.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://blm.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lyq.cdnleiting.top

TS:   return { a, b };
来源：http://qqe.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gvt.tian-w.cn

Go:   return a, b
来源：http://hat.sysykeji.top

Ruby: return a, b
来源：http://fyu.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://bbd.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://grq.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://xmy.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hpy.hywenlv.cn

JS:   const square = x => x * x;
来源：http://ksc.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://etk.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ywv.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cky.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://cfr.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://ghy.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://vhd.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qxl.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://jqa.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cnf.haohaochexian.top

TS:   arr.map(String)
来源：http://ifu.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iun.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bdi.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://rxs.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uco.hammf.cn

[C08] 闭包
来源：http://qtj.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lvu.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wax.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://syn.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vne.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mqh.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pwa.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jrw.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xqb.jqgufenzy.top

[C09] 递归
来源：http://xkx.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pgy.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xbk.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xun.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yav.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://grc.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://put.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xnq.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://diy.kuanghao11.cn

[C10] 变量作用域
来源：http://vyh.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cgc.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wrj.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fyz.xuetiantiany.cn

TS:   同 JS
来源：http://sty.aizwys.cn

Java: 方法内为块级作用域
来源：http://eea.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://wjy.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mfb.9152youxi.cn

C#:   块级作用域
来源：http://mcr.hfpthk.cn

[C11] 模块导入与导出
来源：http://gox.tarul.cn

Py:   from module import func
来源：http://iub.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dig.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://csz.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mqx.9152youxi.cn

Java: import java.util.List;
来源：http://dmf.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qxx.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://rby.havefunace.top

C#:   using System.Text;
来源：http://ptc.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://zds.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://jia.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://rwc.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://wqv.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://qtj.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jre.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://ijj.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://kda.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rhg.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://myu.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xpm.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://elg.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqh.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rwn.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://elg.hnqzz.top

Go:   func add(a, b int) int
来源：http://nki.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vgp.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://qnw.quarkkingdee.top

[C14] 泛型函数
来源：http://nuc.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aim.daxiang520.top

PHP:  // 无泛型
来源：http://brv.hammf.cn

JS:   // 无泛型
来源：http://slx.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ycp.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cnn.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mpb.ppjwa.cn

Ruby: # 无泛型
来源：http://qjy.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://abf.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://yen.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tku.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://xnr.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://txd.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lzi.guowangkeji.top

Java: // 无解构
来源：http://yja.zhaomingkeji.xyz

Go:   // 无解构
来源：http://vtb.daxiang520.top

Ruby: a, b = pair
来源：http://hnh.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://svq.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://qdb.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gqq.cqqwz.cn

PHP:  // 无重载
来源：http://moq.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://efm.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://vsn.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ipd.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://zkd.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://psf.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ell.xinyue.icu

================================================================================
来源：http://wfg.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://ukn.ivvv.top

================================================================================
来源：http://rbv.fzhhl.top

[D01] 创建数组 / 列表
来源：http://scl.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ryc.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ffb.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rbk.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://txb.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ufy.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://fev.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://zgj.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dkt.daxiang520.top

[D02] 追加元素到末尾
来源：http://quu.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tzr.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fwk.epnwcf.com

JS:   arr.push(4);
来源：http://cgp.c1oappe.top

TS:   arr.push(4);
来源：http://gqx.gzhubu.top

Java: list.add(4);
来源：http://ckm.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://wmm.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://wbu.havefunace.top

C#:   list.Add(4);
来源：http://gro.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://gjb.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://zyv.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lan.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fjr.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://ofi.hysaishi.cn

Java: list.add(0, 0);
来源：http://csh.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://cxp.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ghb.hammf.cn

C#:   list.Insert(0, 0);
来源：http://qyf.gaohongyu789.top

[D04] 删除元素
来源：http://cvv.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wny.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://odc.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eet.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://snm.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qus.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tbq.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czh.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ouu.chenlongwang.top

[D05] 访问与修改元素
来源：http://csq.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://idm.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lty.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffp.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://ydy.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://prh.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://shn.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfq.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ubl.sysykeji.top

[D06] 数组长度
来源：http://chd.yj20258.top

Py:   len(arr)
来源：http://mvf.fktsv.cn

PHP:  count($arr);
来源：http://epp.shanyushiyangtech.top

JS:   arr.length
来源：http://vsh.yangfankeji.com

TS:   arr.length
来源：http://dpi.shanyushiyangtech.top

Java: list.size();
来源：http://jib.daria6918.cn

Go:   len(arr)
来源：http://eov.52xcode.cn

Ruby: arr.length; arr.size
来源：http://nep.chenjidiqi.icu

C#:   list.Count;
来源：http://zdt.wangdashe.top

[D07] 切片 / 取子数组
来源：http://rzd.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lpi.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pkn.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://mxh.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://nhz.yj202588.top

Java: list.subList(1, 4);
来源：http://pis.epnwcf.com

Go:   arr[1:4]
来源：http://nar.hysaishi.cn

Ruby: arr[1, 3]
来源：http://qzj.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://mlq.fengsongda.top

[D08] 合并两个数组
来源：http://jbo.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://vpr.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://evq.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dkc.snrcjt.cn

TS:   [...a, ...b];
来源：http://sme.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bux.9152youxi.cn

Go:   append(a, b...)
来源：http://ypp.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://wrd.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://ttm.mhx1999.top

[D09] 排序（升序）
来源：http://mxk.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://zzn.ppjwa.cn

PHP:  sort($arr);
来源：http://imf.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lty.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bji.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lcl.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ioh.fktsv.cn

Ruby: arr.sort
来源：http://xur.xinyue.icu

C#:   list.Sort();
来源：http://yxm.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lyl.ppjwa.cn


<!-- 参考信息 -->