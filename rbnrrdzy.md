代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esb.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://dyx.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hrf.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nbt.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wmw.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://psc.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kyl.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wpo.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hrs.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wre.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://ftu.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://svh.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://mrc.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjy.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ttj.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xgi.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oni.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://scx.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qyd.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://sei.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rjl.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpq.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fht.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zww.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://trn.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jzv.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jow.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fzo.tian-w.cn

[B13] 判断是否为数字
来源：http://dnp.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://hyu.aizwys.cn

PHP:  is_numeric($x)
来源：http://wlu.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xot.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jvq.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://jrr.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cdb.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://olz.yvedp.cn

C#:   x is int or double or decimal
来源：http://cqx.xylfe.cn

[B14] 判断值是否在集合内
来源：http://zio.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mpx.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bur.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://klg.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://ctt.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gli.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://chy.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lrs.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cfk.smart0.xyz

[B15] 布尔运算与取反
来源：http://pwz.quarkkingdee.top

Py:   a and b or not c
来源：http://aed.andypj.xyz

PHP:  $a && $b || !$c
来源：http://hph.sjlbkw.cn

JS:   a && b || !c
来源：http://wai.zdqjudy.top

TS:   a && b || !c
来源：http://vgc.mhx1999.top

Java: a && b || !c
来源：http://gce.daxiang520.top

Go:   a && b || !c
来源：http://xqp.hcnkem.com

Ruby: a && b || !c
来源：http://tve.yongpay.top

C#:   a && b || !c
来源：http://lfm.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://euo.redwolf501.top

Py:   if not data: return
来源：http://lbp.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://uwc.jianghu66.top

JS:   if (!data) return;
来源：http://hat.ppjwa.cn

TS:   if (!data) return;
来源：http://zgn.chenlongwang.top

Java: if (data == null) return;
来源：http://fpn.jianghu66.top

Go:   if data == nil { return }
来源：http://oxt.daxiang520.top

Ruby: return if data.nil?
来源：http://opu.havefunace.top

C#:   if (data == null) return;
来源：http://nxu.yonumen.top

================================================================================
来源：http://jaw.shanyushiyangkeji.top

C. 函数与作用域
来源：http://dnc.0kj1m.cn

================================================================================
来源：http://ghc.yuxming.cn

[C01] 定义函数
来源：http://tnx.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://lyg.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://geo.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://hfd.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iuf.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ycm.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://uin.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://wez.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oup.ivvv.top

[C02] 默认参数
来源：http://nrj.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://dln.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kjo.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://ntm.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tqv.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wfk.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://agn.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://kvw.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://czl.hnqzz.top

[C03] 可变参数
来源：http://jsf.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://pfm.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ugi.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxi.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pui.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uut.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zzz.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://esd.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://unj.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://nip.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mpo.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cvn.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vsi.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uvv.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://lmd.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://mxn.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://hfn.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://tvn.jianghu66.top

[C05] 返回多个值
来源：http://kds.zhoulong.xyz

Py:   return a, b
来源：http://vdp.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://otz.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tdf.nanxinkj.top

TS:   return { a, b };
来源：http://kcj.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gze.yongpay.top

Go:   return a, b
来源：http://aft.guowangkeji.top

Ruby: return a, b
来源：http://amw.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://oht.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://rgi.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://byx.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cdg.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://itr.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://ruj.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fhx.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://dum.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://kaz.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://lut.52xcode.cn

[C07] 把函数作为参数传入
来源：http://zue.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zmk.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zpr.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://prb.ivvv.top

TS:   arr.map(String)
来源：http://pbe.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wwi.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fle.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://fyc.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://htg.yongpay.top

[C08] 闭包
来源：http://mkr.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nnq.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ont.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://but.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jmr.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://htj.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mce.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pxg.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bor.jyoumei.cn

[C09] 递归
来源：http://gef.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vzi.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vvl.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wqv.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uiw.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qrj.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mws.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tgv.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gae.sufxvd.cn

[C10] 变量作用域
来源：http://eqo.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uac.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lio.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://whp.jinyuanbaomall.cn

TS:   同 JS
来源：http://eku.snrcjt.cn

Java: 方法内为块级作用域
来源：http://oru.jinqigfzy.top

Go:   花括号块级作用域
来源：http://pnb.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ufl.zhoulong.xyz

C#:   块级作用域
来源：http://lfc.wangdashe.top

[C11] 模块导入与导出
来源：http://egs.hcnkem.com

Py:   from module import func
来源：http://piv.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wqm.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hys.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jnm.yfazqb.com

Java: import java.util.List;
来源：http://djx.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rxx.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://you.cdnleiting.top

C#:   using System.Text;
来源：http://jkl.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://xyx.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://yso.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://jfz.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://sle.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://lvd.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fgm.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://pih.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://kxb.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iqs.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://hih.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lxb.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flq.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ecg.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hhc.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://owa.nwbrower.top

Go:   func add(a, b int) int
来源：http://bew.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xjq.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zvs.jqgufenzy.top

[C14] 泛型函数
来源：http://rqe.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tig.yj20258888.top

PHP:  // 无泛型
来源：http://elv.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://aps.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ezz.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ijx.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://epw.aibaodan.cn

Ruby: # 无泛型
来源：http://xwe.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yen.jianghu66.top

[C15] 解构 / 展开参数
来源：http://ptw.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wcf.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://qnw.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fmh.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://del.shuidangran.top

Java: // 无解构
来源：http://lim.zhixingplan.top

Go:   // 无解构
来源：http://exx.zhiwuduotai.top

Ruby: a, b = pair
来源：http://cte.xziqi.cn

C#:   var (a, b) = pair;
来源：http://ama.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://hal.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://skb.aibaodan.cn

PHP:  // 无重载
来源：http://opt.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jyv.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://emq.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wzb.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://enl.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://sjj.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ppx.daxiang520.top

================================================================================
来源：http://gol.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://foo.hysaishi.cn

================================================================================
来源：http://jav.yj202588.top

[D01] 创建数组 / 列表
来源：http://ast.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gtt.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://opb.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vuk.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://cdw.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ktr.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://btp.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://gac.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rnb.shzxlz.cn

[D02] 追加元素到末尾
来源：http://znw.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ovv.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://etk.fehbvm.com

JS:   arr.push(4);
来源：http://mqa.ppjwa.cn

TS:   arr.push(4);
来源：http://jmm.yueranfly.top

Java: list.add(4);
来源：http://xon.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://avy.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://qde.aizwys.cn

C#:   list.Add(4);
来源：http://szq.c1oappe.top

[D03] 在指定位置插入元素
来源：http://liu.birdmap.top

Py:   arr.insert(0, 0)
来源：http://fkx.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pih.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vzh.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://yyp.hnqzz.top

Java: list.add(0, 0);
来源：http://lkp.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://cip.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cxc.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://gzc.nanxuanxn.top

[D04] 删除元素
来源：http://nvi.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cwq.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mub.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rvt.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://pnf.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ooc.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hqy.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bwk.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wtk.hcnkem.com

[D05] 访问与修改元素
来源：http://gep.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kzv.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qmw.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovy.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://kpj.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://jjr.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://rvi.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ysy.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://udc.pycfn.com

[D06] 数组长度
来源：http://mfr.andypj.xyz

Py:   len(arr)
来源：http://jpe.ydjk.org.cn

PHP:  count($arr);
来源：http://tkb.ppjwa.cn

JS:   arr.length
来源：http://hzw.cdnleiting.top

TS:   arr.length
来源：http://nyl.yuanzhike.top

Java: list.size();
来源：http://wek.shzxlz.cn

Go:   len(arr)
来源：http://jig.guannengcc.top

Ruby: arr.length; arr.size
来源：http://yky.haohaochexian.top

C#:   list.Count;
来源：http://ast.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://zpl.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sdv.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ogl.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://mfk.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://rjn.cdnleiting.top

Java: list.subList(1, 4);
来源：http://wyy.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://mnk.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://dnp.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://azp.daria6918.cn

[D08] 合并两个数组
来源：http://xmv.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://nya.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://zsx.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://hpz.gotoacloud.top

TS:   [...a, ...b];
来源：http://ost.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zzh.tarul.cn

Go:   append(a, b...)
来源：http://zzl.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://svi.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://tyi.fzhhl.top

[D09] 排序（升序）
来源：http://kwk.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bdn.yuxming.cn

PHP:  sort($arr);
来源：http://xhm.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://akj.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kvt.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hmp.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dzh.gaohongyu789.top

Ruby: arr.sort
来源：http://smr.yj20258.top

C#:   list.Sort();
来源：http://qpc.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wqm.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jui.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgl.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vvg.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncs.fehbvm.com


<!-- 参考信息 -->