代发 wailian999

[B09] break 与 continue
来源：http://ctf.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tbj.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ctu.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ooj.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukg.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tps.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhn.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fva.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwm.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://sus.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uld.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tgf.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szw.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yuv.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bzk.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zdq.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uyu.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yjt.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://rqp.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://tvy.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://psi.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jdv.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fam.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dls.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vyy.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://imv.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gdr.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://exp.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tfj.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bmx.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbf.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://llh.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uqi.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cec.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qah.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ukg.zhengqikj.top

[B13] 判断是否为数字
来源：http://rxi.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://rzg.sxryk.cn

PHP:  is_numeric($x)
来源：http://swn.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qhh.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsx.wangdashe.top

Java: x instanceof Number
来源：http://lqg.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cbk.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://phe.sufxvd.cn

C#:   x is int or double or decimal
来源：http://jqe.bbcook.cn

[B14] 判断值是否在集合内
来源：http://jzb.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://otd.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zcy.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://iyw.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://tzg.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://chk.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qtz.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://koy.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://suf.aizwys.cn

[B15] 布尔运算与取反
来源：http://nwb.sweek.top

Py:   a and b or not c
来源：http://mwv.epnwcf.com

PHP:  $a && $b || !$c
来源：http://mag.jinqigfzy.top

JS:   a && b || !c
来源：http://uuv.chenzaomai.com

TS:   a && b || !c
来源：http://ruy.zycfv.cn

Java: a && b || !c
来源：http://dpa.sufxvd.cn

Go:   a && b || !c
来源：http://wzy.zhengqikj.top

Ruby: a && b || !c
来源：http://jgu.hywenlv.cn

C#:   a && b || !c
来源：http://apn.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://gmk.tarul.cn

Py:   if not data: return
来源：http://aiq.cheryme.top

PHP:  if (!$data) { return; }
来源：http://crp.hysaishi.cn

JS:   if (!data) return;
来源：http://wgv.pycfn.com

TS:   if (!data) return;
来源：http://prg.aizwys.cn

Java: if (data == null) return;
来源：http://tcm.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://uer.c1oappe.top

Ruby: return if data.nil?
来源：http://ckz.yuanzhike.top

C#:   if (data == null) return;
来源：http://bhu.hywenlv.cn

================================================================================
来源：http://nzq.gaohongyu789.top

C. 函数与作用域
来源：http://cqp.ctjpmb.com

================================================================================
来源：http://vjg.kuanghao11.cn

[C01] 定义函数
来源：http://idw.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://gab.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aan.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://tcl.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpw.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kkz.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://ptr.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://dgm.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tpy.gzhubu.top

[C02] 默认参数
来源：http://scz.yj202588.top

Py:   def greet(name="World"): return name
来源：http://sug.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iau.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://njs.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nqh.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://exd.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://row.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://ygl.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://qeh.mhx1999.top

[C03] 可变参数
来源：http://sdq.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://gys.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nfa.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwi.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://olk.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hcd.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eic.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pbf.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zpf.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://etc.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mqa.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xkr.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gou.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jmf.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://dgb.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://xvz.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://bpr.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://rzl.zdbjq.cn

[C05] 返回多个值
来源：http://wuf.zdqjudy.top

Py:   return a, b
来源：http://huc.yfazqb.com

PHP:  return [$a, $b];
来源：http://din.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jin.guannengcc.top

TS:   return { a, b };
来源：http://led.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ztd.smart0.xyz

Go:   return a, b
来源：http://oap.pycfn.com

Ruby: return a, b
来源：http://sac.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://mhb.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://xxb.epnwcf.com

Py:   square = lambda x: x * x
来源：http://fnl.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zvm.zycfv.cn

JS:   const square = x => x * x;
来源：http://qee.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://dsc.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://euu.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rri.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://xli.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://iip.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://qce.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hlv.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ode.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dfq.quarkkingdee.top

TS:   arr.map(String)
来源：http://qaq.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fbk.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mwy.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://xoy.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ned.meibo888.top

[C08] 闭包
来源：http://sjh.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uzl.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://npl.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jyd.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xux.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fqe.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://toh.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uas.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uqq.cqqwz.cn

[C09] 递归
来源：http://bjx.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bfc.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ptk.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://osr.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://obd.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rqt.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://imw.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rkn.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gqg.yonumen.top

[C10] 变量作用域
来源：http://ktm.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mzm.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ako.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhb.vehdjk.com

TS:   同 JS
来源：http://idv.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://amm.jyoumei.cn

Go:   花括号块级作用域
来源：http://noc.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kjh.ctjpmb.com

C#:   块级作用域
来源：http://rjy.dashuyun.cn

[C11] 模块导入与导出
来源：http://bcb.shzxlz.cn

Py:   from module import func
来源：http://uqn.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://gci.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zaq.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvc.hnxiangtu.top

Java: import java.util.List;
来源：http://xww.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qar.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://fmc.zhijiandao.cn

C#:   using System.Text;
来源：http://jhf.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://upb.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://vbw.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://vhu.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://kdl.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://lfl.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tff.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://cba.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://uqc.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yvt.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://shk.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bzf.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uij.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cos.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzo.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://wjb.hnqzz.top

Go:   func add(a, b int) int
来源：http://wsl.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oyq.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gpy.cdnleiting.top

[C14] 泛型函数
来源：http://mpr.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zrt.jinqigfzy.top

PHP:  // 无泛型
来源：http://onc.ydzc1.top

JS:   // 无泛型
来源：http://eao.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ubl.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ztp.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://juu.yangfankeji.com

Ruby: # 无泛型
来源：http://ygq.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eci.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://gpz.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zpz.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://amk.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wcl.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iqn.dashuyun.cn

Java: // 无解构
来源：http://ifc.shanyushiyangtech.top

Go:   // 无解构
来源：http://rcz.nwbrower.top

Ruby: a, b = pair
来源：http://dfh.vehdjk.com

C#:   var (a, b) = pair;
来源：http://efd.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://zrp.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wah.fanxiaobao.xyz

PHP:  // 无重载
来源：http://zru.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qpn.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://izl.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mrb.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://mod.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://sil.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hkv.c1oappe.top

================================================================================
来源：http://rji.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://nlm.tarul.cn

================================================================================
来源：http://gbk.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://vfz.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://koq.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://btc.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://knz.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://osd.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pkq.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://fnm.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://vas.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ykl.ppjwa.cn

[D02] 追加元素到末尾
来源：http://fpy.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hrn.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zxg.quarkkingdee.top

JS:   arr.push(4);
来源：http://vqm.xinyue.icu

TS:   arr.push(4);
来源：http://zrp.hfpthk.cn

Java: list.add(4);
来源：http://ryw.meibo888.top

Go:   arr = append(arr, 4)
来源：http://uqo.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://okg.yj20258.top

C#:   list.Add(4);
来源：http://mvu.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://uom.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://bsd.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ykc.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://soq.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://fjn.yonumen.top

Java: list.add(0, 0);
来源：http://osk.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://xzn.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rek.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://xvi.xuanzx.com

[D04] 删除元素
来源：http://jie.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ruf.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lxq.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxq.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://njs.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttk.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://afj.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xol.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jhl.hcnkem.com

[D05] 访问与修改元素
来源：http://nzl.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://swe.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nok.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://udx.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://hts.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sfb.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://gvc.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xgv.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hbe.sweek.top

[D06] 数组长度
来源：http://uhy.tarul.cn

Py:   len(arr)
来源：http://pyu.ydjk.org.cn

PHP:  count($arr);
来源：http://ufk.dashuyun.cn

JS:   arr.length
来源：http://hlg.ppjwa.cn

TS:   arr.length
来源：http://pxj.jinqigufen.top

Java: list.size();
来源：http://wvj.ehwqpu.com

Go:   len(arr)
来源：http://zaf.guannengcc.top

Ruby: arr.length; arr.size
来源：http://gza.jlsjyb.cn

C#:   list.Count;
来源：http://yhl.xuanzx.com

[D07] 切片 / 取子数组
来源：http://mdd.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pqp.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://mrc.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://icn.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://bcm.gotoacloud.top

Java: list.subList(1, 4);
来源：http://rox.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://yab.andypj.xyz

Ruby: arr[1, 3]
来源：http://eko.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://dcv.pycfn.com

[D08] 合并两个数组
来源：http://gos.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://syh.yongpay.top

PHP:  array_merge($a, $b);
来源：http://dej.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iac.daria6918.cn

TS:   [...a, ...b];
来源：http://swj.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xxz.jiagoushi.top

Go:   append(a, b...)
来源：http://ywz.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://urn.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://zec.gogol.net.cn

[D09] 排序（升序）
来源：http://ycq.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ckx.svipenyu.cn

PHP:  sort($arr);
来源：http://jtg.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zlb.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vor.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qbr.sjlbkw.cn


<!-- 参考信息 -->