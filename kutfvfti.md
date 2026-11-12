代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbb.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smm.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hzv.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dct.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gaf.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://zbm.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ogr.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wmp.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://smq.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hpf.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aui.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://afe.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pao.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pyo.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://jng.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://xrg.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://lli.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tnl.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gat.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mus.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nhr.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://mot.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ppk.yueranfly.top

[B12] 跳出多层循环
来源：http://kfa.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yif.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hjm.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dlk.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gqz.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xub.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pnh.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eio.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hhv.tanke756.top

[B13] 判断是否为数字
来源：http://ppo.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://smo.hcnkem.com

PHP:  is_numeric($x)
来源：http://alk.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcr.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://udg.yuxming.cn

Java: x instanceof Number
来源：http://rkd.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ito.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://wlo.mhx1999.top

C#:   x is int or double or decimal
来源：http://kkp.bjfxy.top

[B14] 判断值是否在集合内
来源：http://uje.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uzj.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ncz.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://yww.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://lng.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jbg.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ftv.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://oit.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lwc.cucudq.cn

[B15] 布尔运算与取反
来源：http://nhg.ivvv.top

Py:   a and b or not c
来源：http://zli.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://idi.xuanzx.com

JS:   a && b || !c
来源：http://rzv.andypj.xyz

TS:   a && b || !c
来源：http://nep.cdnleiting.top

Java: a && b || !c
来源：http://bfk.yueranfly.top

Go:   a && b || !c
来源：http://jok.zdbjq.cn

Ruby: a && b || !c
来源：http://nwg.chenlongwang.top

C#:   a && b || !c
来源：http://ymv.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://bfv.ybcxt.top

Py:   if not data: return
来源：http://xij.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://rws.cqqwz.cn

JS:   if (!data) return;
来源：http://fxf.snrcjt.cn

TS:   if (!data) return;
来源：http://pcv.snrcjt.cn

Java: if (data == null) return;
来源：http://iin.birdmap.top

Go:   if data == nil { return }
来源：http://oxj.sufxvd.cn

Ruby: return if data.nil?
来源：http://mhn.xziqi.cn

C#:   if (data == null) return;
来源：http://odx.sysykeji.top

================================================================================
来源：http://zsd.gotoacloud.top

C. 函数与作用域
来源：http://adv.cdnleiting.top

================================================================================
来源：http://foe.cheryme.top

[C01] 定义函数
来源：http://emg.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://oaz.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfx.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uvv.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxm.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ajk.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://fzx.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://vsb.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://khe.snrcjt.cn

[C02] 默认参数
来源：http://eev.316326.xyz

Py:   def greet(name="World"): return name
来源：http://dul.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rdj.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://mnx.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dbw.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jdr.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jbv.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://ajo.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://kwb.fanxiaobao.xyz

[C03] 可变参数
来源：http://mkv.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://rah.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wdz.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tks.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jot.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kwl.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fhx.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://ird.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bfy.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://riw.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kyc.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uyd.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpu.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hkw.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://ybz.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://bcw.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://rpi.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://dww.daxiang520.top

[C05] 返回多个值
来源：http://ydo.yueranfly.top

Py:   return a, b
来源：http://zez.xylfe.cn

PHP:  return [$a, $b];
来源：http://dhe.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://egf.vqdsnc.cn

TS:   return { a, b };
来源：http://ega.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kcu.wangdashe.top

Go:   return a, b
来源：http://jdl.shangyingyoupin.top

Ruby: return a, b
来源：http://pyt.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://kjd.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://uxf.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://uqe.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hlu.haohaochexian.top

JS:   const square = x => x * x;
来源：http://iqt.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://vzj.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpf.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://gmo.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://rgn.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://wui.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://enn.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nvv.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://inb.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kjo.shzxlz.cn

TS:   arr.map(String)
来源：http://iyu.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://izi.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ywp.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://zbd.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hfu.nanxuanxn.top

[C08] 闭包
来源：http://wwn.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gli.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ovf.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://exs.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fzm.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zzf.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gcz.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ywn.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bjp.sufxvd.cn

[C09] 递归
来源：http://haa.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yys.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ibw.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzk.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkt.zycfv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eba.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zbj.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://itq.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xdw.andypj.xyz

[C10] 变量作用域
来源：http://tmd.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cdh.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://boa.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ehq.hcnkem.com

TS:   同 JS
来源：http://qoj.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://okw.andypj.xyz

Go:   花括号块级作用域
来源：http://tgu.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qgi.fengsongda.top

C#:   块级作用域
来源：http://eun.epnwcf.com

[C11] 模块导入与导出
来源：http://rxt.ywan-chungtsiang.top

Py:   from module import func
来源：http://eit.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qar.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oze.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qlj.yj20258.top

Java: import java.util.List;
来源：http://mbk.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://loo.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://xyw.daxiang520.top

C#:   using System.Text;
来源：http://rbu.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://smu.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://hbo.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://rrg.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://crh.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://pvf.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bkc.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://nmj.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://xrm.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bbj.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://ekp.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://urm.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxt.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpy.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnz.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://zpf.nwbrower.top

Go:   func add(a, b int) int
来源：http://aip.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cvo.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://uvr.feifeiyinyue.top

[C14] 泛型函数
来源：http://jns.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iqm.wangshuangyany.cn

PHP:  // 无泛型
来源：http://znu.fehbvm.com

JS:   // 无泛型
来源：http://xdz.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dpc.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eux.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oxt.hesvh.cn

Ruby: # 无泛型
来源：http://htv.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tbu.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://vjs.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ltv.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://wxl.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wrn.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hlr.chenzaomai.com

Java: // 无解构
来源：http://iqs.yj20258.top

Go:   // 无解构
来源：http://uhl.mhx1999.top

Ruby: a, b = pair
来源：http://keu.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://ays.yuxming.cn

[C16] 函数 / 方法重载
来源：http://lwp.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nga.daria6918.cn

PHP:  // 无重载
来源：http://wyj.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vat.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://kua.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oyl.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://zmg.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://hto.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://psd.fzhhl.top

================================================================================
来源：http://gct.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://lmk.jyoumei.cn

================================================================================
来源：http://znl.uphjek.com

[D01] 创建数组 / 列表
来源：http://kfa.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tph.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mib.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tyb.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ypu.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xyh.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://yfb.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://wjj.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zob.hywenlv.cn

[D02] 追加元素到末尾
来源：http://ned.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ryd.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uzj.jianghu66.top

JS:   arr.push(4);
来源：http://xyi.tian-w.cn

TS:   arr.push(4);
来源：http://pml.yongpay.top

Java: list.add(4);
来源：http://lit.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://ezg.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://gbj.jyoumei.cn

C#:   list.Add(4);
来源：http://nmj.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://ewx.birdmap.top

Py:   arr.insert(0, 0)
来源：http://qcj.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hgg.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxr.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://xue.zhijiandao.cn

Java: list.add(0, 0);
来源：http://lkv.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rxf.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rls.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://iqf.yangfankeji.com

[D04] 删除元素
来源：http://jux.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xlj.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ime.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iry.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://plj.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ggt.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bmq.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nzx.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qlz.tarul.cn

[D05] 访问与修改元素
来源：http://ger.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gny.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfs.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yuu.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://pgr.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://klt.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://utt.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yez.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eoy.fengsongda.top

[D06] 数组长度
来源：http://uln.shangyingyoupin.top

Py:   len(arr)
来源：http://rmg.wangdashe.top

PHP:  count($arr);
来源：http://ehm.guowangkeji.top

JS:   arr.length
来源：http://jhx.zhoulong.xyz

TS:   arr.length
来源：http://tdi.ivvv.top

Java: list.size();
来源：http://exb.uphjek.com

Go:   len(arr)
来源：http://eti.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://gqv.snrcjt.cn

C#:   list.Count;
来源：http://aty.jianghu66.top

[D07] 切片 / 取子数组
来源：http://wxz.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqd.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rzu.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://gjq.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://ssy.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://jbu.wangshuangyany.cn

Go:   arr[1:4]
来源：http://jtf.sxryk.cn

Ruby: arr[1, 3]
来源：http://tyo.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://vlh.ivvv.top

[D08] 合并两个数组
来源：http://pcr.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://tcb.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://giz.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ndh.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://rnt.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://scu.cucudq.cn

Go:   append(a, b...)
来源：http://oup.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://brg.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://xpm.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://ccl.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://vov.bbcook.cn

PHP:  sort($arr);
来源：http://cyn.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hbs.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://btb.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hhq.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pzs.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://ueq.smart0.xyz

C#:   list.Sort();
来源：http://jev.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qxu.cashguo.top


<!-- 参考信息 -->