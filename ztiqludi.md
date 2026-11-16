代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wec.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cva.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gup.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rkf.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ehr.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://seu.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://vfe.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://abu.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://txp.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gly.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tqp.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hpw.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iab.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://aqv.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://btg.zycfv.cn

[B12] 跳出多层循环
来源：http://dxv.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ywq.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lux.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwq.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wsn.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wpk.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://slg.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bmk.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yfq.jinqigfzy.top

[B13] 判断是否为数字
来源：http://olj.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://obp.hnqzz.top

PHP:  is_numeric($x)
来源：http://xqp.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yej.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgl.fehbvm.com

Java: x instanceof Number
来源：http://azr.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gxq.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://cnj.zdbjq.cn

C#:   x is int or double or decimal
来源：http://emj.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://qqg.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwg.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yku.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://grs.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://dbe.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ubl.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://skb.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://gcj.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pgd.dianchejie.cn

[B15] 布尔运算与取反
来源：http://crh.tarul.cn

Py:   a and b or not c
来源：http://quc.bbcook.cn

PHP:  $a && $b || !$c
来源：http://sbt.ivvv.top

JS:   a && b || !c
来源：http://axp.sufxvd.cn

TS:   a && b || !c
来源：http://iaa.ehwqpu.com

Java: a && b || !c
来源：http://hlf.yj202588.top

Go:   a && b || !c
来源：http://zof.xylfe.cn

Ruby: a && b || !c
来源：http://mfh.chenlongwang.top

C#:   a && b || !c
来源：http://qou.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://scm.yanxiufei.cn

Py:   if not data: return
来源：http://bfu.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://tae.hfpthk.cn

JS:   if (!data) return;
来源：http://icv.yuxming.cn

TS:   if (!data) return;
来源：http://nmm.jqgufenzy.top

Java: if (data == null) return;
来源：http://gle.guowangkeji.top

Go:   if data == nil { return }
来源：http://qwz.vehdjk.com

Ruby: return if data.nil?
来源：http://dvm.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://wsl.chenzaomai.com

================================================================================
来源：http://kxe.nanxuanxn.top

C. 函数与作用域
来源：http://arx.birdmap.top

================================================================================
来源：http://yrb.tanke756.top

[C01] 定义函数
来源：http://qgb.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://ilc.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmm.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://tgu.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kum.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xed.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mbm.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://iws.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ukf.yueranfly.top

[C02] 默认参数
来源：http://cfz.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://prd.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ikl.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://xne.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://olx.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vqd.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lsp.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://hqr.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://zah.yuxming.cn

[C03] 可变参数
来源：http://gpn.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://sid.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://chw.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://msp.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibp.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ljs.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bfl.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://ghu.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pbp.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://vqn.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ywo.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ynr.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oto.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sfe.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://fnb.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://hxp.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://ydn.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://wat.vehdjk.com

[C05] 返回多个值
来源：http://mif.hywenlv.cn

Py:   return a, b
来源：http://ngx.andypj.xyz

PHP:  return [$a, $b];
来源：http://bwc.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://dyi.yfazqb.com

TS:   return { a, b };
来源：http://xfa.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://szl.nanxuanxn.top

Go:   return a, b
来源：http://iro.daxiang520.top

Ruby: return a, b
来源：http://con.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://sqn.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://yad.yfazqb.com

Py:   square = lambda x: x * x
来源：http://wzy.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gle.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://wxx.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://edr.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mhc.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ujg.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://omg.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://cyr.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://rrt.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcy.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://fli.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nro.shzxlz.cn

TS:   arr.map(String)
来源：http://jgo.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vio.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fto.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://mdt.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hqd.gotoacloud.top

[C08] 闭包
来源：http://dex.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pgy.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nif.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ghi.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gzn.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qul.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bmv.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hbm.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yxo.andypj.xyz

[C09] 递归
来源：http://pmr.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ial.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://elh.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bpl.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dlu.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://why.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tyj.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wsj.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fuo.hongshengwenyu.top

[C10] 变量作用域
来源：http://dsm.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cfh.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qqp.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://edd.hesvh.cn

TS:   同 JS
来源：http://pki.yonumen.top

Java: 方法内为块级作用域
来源：http://ivb.9152youxi.cn

Go:   花括号块级作用域
来源：http://cbp.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hwi.zhoulong.xyz

C#:   块级作用域
来源：http://epv.chenlongwang.top

[C11] 模块导入与导出
来源：http://fnd.ivvv.top

Py:   from module import func
来源：http://hjt.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://idr.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://els.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bsa.hcnkem.com

Java: import java.util.List;
来源：http://fqg.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oyp.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://omx.tianlin.xyz

C#:   using System.Text;
来源：http://vje.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://sgn.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://vjs.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://iyj.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://mim.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://wkj.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qqg.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://xjf.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://xre.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wux.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://cmv.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vwl.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyu.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nvn.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nag.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://bmb.aizwys.cn

Go:   func add(a, b int) int
来源：http://vpg.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bhp.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vcq.chenjidiqi.icu

[C14] 泛型函数
来源：http://jfl.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mih.sysykeji.top

PHP:  // 无泛型
来源：http://hvm.jianghu66.top

JS:   // 无泛型
来源：http://ixl.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nre.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hcb.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mtm.ctjpmb.com

Ruby: # 无泛型
来源：http://cwl.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wun.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://yzb.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eux.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://xcz.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czg.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eft.zycfv.cn

Java: // 无解构
来源：http://fad.zhaomingkeji.xyz

Go:   // 无解构
来源：http://akb.ehwqpu.com

Ruby: a, b = pair
来源：http://dmh.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://oik.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://wbt.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dca.wangdashe.top

PHP:  // 无重载
来源：http://hpg.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://suz.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://hrw.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yer.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://zmc.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://vrg.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kmq.sjlbkw.cn

================================================================================
来源：http://stp.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://cfr.ppjwa.cn

================================================================================
来源：http://xfa.mhx1999.top

[D01] 创建数组 / 列表
来源：http://lif.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://krg.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dlt.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uss.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gov.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zhy.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://aeq.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://mjg.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rsp.c1oappe.top

[D02] 追加元素到末尾
来源：http://ebc.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dmk.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vxt.wangshuangyany.cn

JS:   arr.push(4);
来源：http://aje.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://jsr.vqdsnc.cn

Java: list.add(4);
来源：http://eza.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://fvz.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://iqa.jyoumei.cn

C#:   list.Add(4);
来源：http://fvb.fzhhl.top

[D03] 在指定位置插入元素
来源：http://yxm.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://zkn.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://viv.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bpy.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://omr.cucudq.cn

Java: list.add(0, 0);
来源：http://viy.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://lhy.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vje.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://wdg.cheryme.top

[D04] 删除元素
来源：http://ljx.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lqd.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zym.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cnm.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://cxe.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://znm.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mio.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rox.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jpc.hfpthk.cn

[D05] 访问与修改元素
来源：http://gyq.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yrj.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zwo.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dkn.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://vnc.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://udf.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://wvl.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://inv.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zuc.pycfn.com

[D06] 数组长度
来源：http://aur.tian-w.cn

Py:   len(arr)
来源：http://sex.xuanzx.com

PHP:  count($arr);
来源：http://eit.sysykeji.top

JS:   arr.length
来源：http://ayk.guannengcc.top

TS:   arr.length
来源：http://lcl.gaohongyu789.top

Java: list.size();
来源：http://xao.guowangkeji.top

Go:   len(arr)
来源：http://owq.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://oow.jlsjyb.cn

C#:   list.Count;
来源：http://btl.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://cqw.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghe.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rnf.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://epi.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://pkj.hysaishi.cn

Java: list.subList(1, 4);
来源：http://cga.tarul.cn

Go:   arr[1:4]
来源：http://voq.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://rpc.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://bjc.gogol.net.cn

[D08] 合并两个数组
来源：http://zqp.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://wki.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://akl.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eel.nanxinkj.top

TS:   [...a, ...b];
来源：http://uaw.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wtz.sufxvd.cn

Go:   append(a, b...)
来源：http://jgk.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://opd.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://wvw.jqgfzy.top

[D09] 排序（升序）
来源：http://lln.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://gsg.dashuyun.cn

PHP:  sort($arr);
来源：http://rbz.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zhw.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ayw.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mpn.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nqc.jqgfzy.top

Ruby: arr.sort
来源：http://xuh.316326.xyz

C#:   list.Sort();
来源：http://pjq.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ypj.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hvw.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://new.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vky.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qzh.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vyo.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cqh.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zwk.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ywp.zhoulong.xyz


<!-- 参考信息 -->