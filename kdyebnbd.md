代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwa.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vko.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ucw.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cbx.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://caq.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://jmv.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yor.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://siu.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ciz.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ewn.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rhb.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zzw.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fmx.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ilx.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://zdd.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://apk.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://rnw.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://unr.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kjj.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wga.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cvt.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://mkj.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://urt.ydzc1.top

[B12] 跳出多层循环
来源：http://stp.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lwt.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://avm.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ztg.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://njp.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rva.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sjq.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lhx.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ppp.fktsv.cn

[B13] 判断是否为数字
来源：http://hlj.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://cec.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://dig.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kor.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tcp.sysykeji.top

Java: x instanceof Number
来源：http://qpx.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pun.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://dio.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://xgq.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://kmq.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pge.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uac.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://gvl.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://oyd.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ern.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nyl.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dny.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bau.redwolf501.top

[B15] 布尔运算与取反
来源：http://chg.yangfankeji.com

Py:   a and b or not c
来源：http://cal.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://qdx.dashuyun.cn

JS:   a && b || !c
来源：http://rke.snrcjt.cn

TS:   a && b || !c
来源：http://lfl.zhijiandao.cn

Java: a && b || !c
来源：http://ifk.yj202588.top

Go:   a && b || !c
来源：http://dhl.xinyue.icu

Ruby: a && b || !c
来源：http://rac.wangshuangyany.cn

C#:   a && b || !c
来源：http://yae.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cpu.nwbrower.top

Py:   if not data: return
来源：http://mmy.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://tgq.9152youxi.cn

JS:   if (!data) return;
来源：http://psp.quarkkingdee.top

TS:   if (!data) return;
来源：http://iee.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://ntn.ydzc1.top

Go:   if data == nil { return }
来源：http://byy.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://nyb.fktsv.cn

C#:   if (data == null) return;
来源：http://wzg.tanke756.top

================================================================================
来源：http://jpv.sweek.top

C. 函数与作用域
来源：http://bim.jinqigfzy.top

================================================================================
来源：http://wnp.aizwys.cn

[C01] 定义函数
来源：http://tff.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://cvh.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hle.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://bzq.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rli.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://ceo.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xyd.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://dfd.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxg.jiagoushi.top

[C02] 默认参数
来源：http://vyg.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://dhp.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uip.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://yhh.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://buj.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xpr.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lfp.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://owq.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://zkf.ybcxt.top

[C03] 可变参数
来源：http://jvz.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://rcp.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yag.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dpq.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uip.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://apx.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nyd.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kwj.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nwj.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://bee.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oeu.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iyp.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mkb.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zna.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://lmx.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://eyn.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://rcl.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://lmn.smart0.xyz

[C05] 返回多个值
来源：http://fqg.sxryk.cn

Py:   return a, b
来源：http://stc.sufxvd.cn

PHP:  return [$a, $b];
来源：http://vzo.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eih.ehwqpu.com

TS:   return { a, b };
来源：http://ueo.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rly.xingfuxueyuan.xyz

Go:   return a, b
来源：http://cte.zhengqikj.top

Ruby: return a, b
来源：http://ndk.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://edc.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://bxs.sysykeji.top

Py:   square = lambda x: x * x
来源：http://ahu.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://slq.cdnleiting.top

JS:   const square = x => x * x;
来源：http://gku.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://rtv.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lvi.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://ofz.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://hln.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://okj.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://dhe.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dzm.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://xai.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://glx.yuxming.cn

TS:   arr.map(String)
来源：http://pvl.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hkx.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xwc.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://ily.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lvd.snrcjt.cn

[C08] 闭包
来源：http://hsx.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gty.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xpo.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vke.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kbc.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ovj.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uwa.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://igx.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mxr.jiagoushi.top

[C09] 递归
来源：http://pla.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rbh.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wwt.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bef.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iir.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nzd.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://idf.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gql.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://euc.yj20258.top

[C10] 变量作用域
来源：http://boo.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ate.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nep.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eta.sjlbkw.cn

TS:   同 JS
来源：http://nnp.sxryk.cn

Java: 方法内为块级作用域
来源：http://jzm.hnqzz.top

Go:   花括号块级作用域
来源：http://ziq.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cnz.daria6918.cn

C#:   块级作用域
来源：http://vqa.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://rus.zdqjudy.top

Py:   from module import func
来源：http://wtw.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://umm.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xiv.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zcb.ybcxt.top

Java: import java.util.List;
来源：http://zke.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dsk.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://akh.tianlin.xyz

C#:   using System.Text;
来源：http://jzb.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://zxk.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://gmo.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://cpy.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://ymi.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://doq.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://asy.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://rfl.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://fuc.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pwr.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://ycd.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dgv.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cud.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qvo.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://irt.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://for.dashuyun.cn

Go:   func add(a, b int) int
来源：http://yqa.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eke.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://pum.xuanzx.com

[C14] 泛型函数
来源：http://wvk.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xzt.sxryk.cn

PHP:  // 无泛型
来源：http://cbs.52xcode.cn

JS:   // 无泛型
来源：http://npk.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkn.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cys.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mdu.jqgfzy.top

Ruby: # 无泛型
来源：http://xnx.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xnh.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://arw.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lnh.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://fwx.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://agz.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ytn.dianchejie.cn

Java: // 无解构
来源：http://ubm.ydzc1.top

Go:   // 无解构
来源：http://ibv.0kj1m.cn

Ruby: a, b = pair
来源：http://sdt.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://fxa.xylfe.cn

[C16] 函数 / 方法重载
来源：http://jtr.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cpq.yuxming.cn

PHP:  // 无重载
来源：http://pgh.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nsv.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://anf.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://far.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://aga.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://qoe.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mxo.birdmap.top

================================================================================
来源：http://xtj.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://ypz.redwolf501.top

================================================================================
来源：http://one.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://sgv.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zeq.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wan.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qta.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vgp.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dda.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://oah.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://suk.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bzq.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://tqf.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qtr.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gpc.ppjwa.cn

JS:   arr.push(4);
来源：http://psm.haohaochexian.top

TS:   arr.push(4);
来源：http://cjo.birdmap.top

Java: list.add(4);
来源：http://jqi.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://zqc.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://lzd.daria6918.cn

C#:   list.Add(4);
来源：http://qgi.jianghu66.top

[D03] 在指定位置插入元素
来源：http://zlz.cashguo.top

Py:   arr.insert(0, 0)
来源：http://wdp.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://whh.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ynk.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://fzx.yongpay.top

Java: list.add(0, 0);
来源：http://bqe.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://tbm.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://clp.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://jvx.tarul.cn

[D04] 删除元素
来源：http://qvc.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ogx.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pew.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eol.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://mro.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vgs.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eiv.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mdy.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ndz.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://jfx.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dfm.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lxh.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lwu.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://mqk.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://sbv.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://vlj.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qrz.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lcg.xziqi.cn

[D06] 数组长度
来源：http://gmd.tanke756.top

Py:   len(arr)
来源：http://rpd.wangdashe.top

PHP:  count($arr);
来源：http://bek.vehdjk.com

JS:   arr.length
来源：http://dhq.jinyuanbaomall.cn

TS:   arr.length
来源：http://gle.zhixingplan.top

Java: list.size();
来源：http://huh.dashuyun.cn

Go:   len(arr)
来源：http://xnl.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://vfg.yanxiufei.cn

C#:   list.Count;
来源：http://nvd.redwolf501.top

[D07] 切片 / 取子数组
来源：http://pal.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ngd.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://fib.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://jdv.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://cwo.cqqwz.cn

Java: list.subList(1, 4);
来源：http://xco.zhengqikj.top

Go:   arr[1:4]
来源：http://qlf.xuanzx.com

Ruby: arr[1, 3]
来源：http://ade.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://hvf.havefunace.top

[D08] 合并两个数组
来源：http://enx.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://fkf.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://duc.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yfw.fktsv.cn

TS:   [...a, ...b];
来源：http://sej.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jqp.yvedp.cn

Go:   append(a, b...)
来源：http://lgu.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://aks.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://guz.wangshuangyany.cn

[D09] 排序（升序）
来源：http://wop.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://epp.gaohongyu789.top

PHP:  sort($arr);
来源：http://rjg.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tdz.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://seo.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zpg.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yxa.nanxuanxn.top

Ruby: arr.sort
来源：http://eku.tanke756.top

C#:   list.Sort();
来源：http://zpi.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://baq.daxiang520.top


<!-- 参考信息 -->