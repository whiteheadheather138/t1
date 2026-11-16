代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ond.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bzt.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://wgg.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://wje.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://lcr.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uty.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tie.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wxc.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyq.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://het.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ppt.chenlongwang.top

[B12] 跳出多层循环
来源：http://ely.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kxo.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://thw.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ees.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ely.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://emt.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://clh.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://anj.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tvw.jiagoushi.top

[B13] 判断是否为数字
来源：http://lnk.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://iet.52xcode.cn

PHP:  is_numeric($x)
来源：http://wol.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baw.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dyt.jianghu66.top

Java: x instanceof Number
来源：http://chc.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kge.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://itz.yj202588.top

C#:   x is int or double or decimal
来源：http://xwy.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://ypz.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cgq.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://apx.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://noz.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://jhb.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sto.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hho.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://fan.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tbp.uphjek.com

[B15] 布尔运算与取反
来源：http://wiv.feifeiyinyue.top

Py:   a and b or not c
来源：http://wlk.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://ynf.ctjpmb.com

JS:   a && b || !c
来源：http://fyb.xziqi.cn

TS:   a && b || !c
来源：http://ejp.fehbvm.com

Java: a && b || !c
来源：http://ugy.daria6918.cn

Go:   a && b || !c
来源：http://otx.cashguo.top

Ruby: a && b || !c
来源：http://zim.vqdsnc.cn

C#:   a && b || !c
来源：http://sxr.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://ehu.9152youxi.cn

Py:   if not data: return
来源：http://bla.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://ggw.snrcjt.cn

JS:   if (!data) return;
来源：http://cyn.redwolf501.top

TS:   if (!data) return;
来源：http://msp.yonumen.top

Java: if (data == null) return;
来源：http://yzf.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://xfu.bjfxy.top

Ruby: return if data.nil?
来源：http://rhp.gzhubu.top

C#:   if (data == null) return;
来源：http://jgl.ydzc1.top

================================================================================
来源：http://pnx.316326.xyz

C. 函数与作用域
来源：http://ffh.shanyushiyangtech.top

================================================================================
来源：http://bgq.sufxvd.cn

[C01] 定义函数
来源：http://alc.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://rul.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jqa.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://hwq.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ixw.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fli.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://hzl.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://ohf.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ffa.fengsongda.top

[C02] 默认参数
来源：http://fqt.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://bdq.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://toi.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://byg.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://jxf.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bkx.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://omw.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://sia.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://prr.pycfn.com

[C03] 可变参数
来源：http://ptc.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://ryu.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uof.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blb.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://glx.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kbg.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xnc.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://ezx.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ypc.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://zbv.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://roo.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vqz.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oax.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dlc.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://kzg.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://mew.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://vxy.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://equ.aibaodan.cn

[C05] 返回多个值
来源：http://lab.yonumen.top

Py:   return a, b
来源：http://gnv.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://gzk.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aej.xziqi.cn

TS:   return { a, b };
来源：http://xvb.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vrl.smart0.xyz

Go:   return a, b
来源：http://oyt.yfazqb.com

Ruby: return a, b
来源：http://zfo.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://irt.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://jgo.cucudq.cn

Py:   square = lambda x: x * x
来源：http://hzo.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oxw.fzhhl.top

JS:   const square = x => x * x;
来源：http://aag.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://edz.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qth.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://ukv.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://kin.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uhs.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://vrh.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ube.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://hga.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gjy.hongshengwenyu.top

TS:   arr.map(String)
来源：http://blv.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uje.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uhy.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://hmd.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ota.hfpthk.cn

[C08] 闭包
来源：http://yze.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://exl.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wdp.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kos.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fhz.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mex.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xpt.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qch.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zaj.bbcook.cn

[C09] 递归
来源：http://rlb.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rfb.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pol.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mru.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fnk.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cuh.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jwy.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gwb.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vic.ivvv.top

[C10] 变量作用域
来源：http://oyq.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fqq.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gnk.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fsw.bjfxy.top

TS:   同 JS
来源：http://aqx.c1oappe.top

Java: 方法内为块级作用域
来源：http://idt.kuanghao11.cn

Go:   花括号块级作用域
来源：http://tdz.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xae.daxiang520.top

C#:   块级作用域
来源：http://xuu.ivvv.top

[C11] 模块导入与导出
来源：http://oxc.fanxiaobao.xyz

Py:   from module import func
来源：http://aks.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wge.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://frw.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://spy.sxryk.cn

Java: import java.util.List;
来源：http://vgb.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ejc.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://ytf.9152youxi.cn

C#:   using System.Text;
来源：http://pfu.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://aih.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://bxd.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://pxd.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://blo.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://dnj.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lws.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://aon.sweek.top

Ruby: -> { puts "run" }.call
来源：http://ycz.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kcu.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://pfz.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xld.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uui.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mqd.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://asf.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://iev.shzxlz.cn

Go:   func add(a, b int) int
来源：http://zsf.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ljx.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://fxn.sweek.top

[C14] 泛型函数
来源：http://cgw.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nrd.cheryme.top

PHP:  // 无泛型
来源：http://keg.hcnkem.com

JS:   // 无泛型
来源：http://xon.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ckn.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hzm.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lne.fengsongda.top

Ruby: # 无泛型
来源：http://mdg.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://umn.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://cjy.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://opg.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://yix.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ubv.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qau.zhongyouzk.top

Java: // 无解构
来源：http://cod.xziqi.cn

Go:   // 无解构
来源：http://kxd.epnwcf.com

Ruby: a, b = pair
来源：http://kyt.uphjek.com

C#:   var (a, b) = pair;
来源：http://ljq.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://ods.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xzz.0kj1m.cn

PHP:  // 无重载
来源：http://cct.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jjb.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://wxa.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hbm.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://iys.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://srt.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lkz.fengsongda.top

================================================================================
来源：http://mfk.uphjek.com

D. 数组 / 列表 / 集合
来源：http://lug.shzxlz.cn

================================================================================
来源：http://hql.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://den.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mwu.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hbz.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ijv.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tpy.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jos.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://hyv.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://dzi.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gfk.gotoacloud.top

[D02] 追加元素到末尾
来源：http://rus.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bzx.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bpd.gaohongyu789.top

JS:   arr.push(4);
来源：http://syr.fktsv.cn

TS:   arr.push(4);
来源：http://czb.xuetiantiany.cn

Java: list.add(4);
来源：http://dlp.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://muz.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://hrt.zhijiandao.cn

C#:   list.Add(4);
来源：http://dzh.sysykeji.top

[D03] 在指定位置插入元素
来源：http://ghn.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://qjz.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tya.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dyr.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://lpg.jqgufenzy.top

Java: list.add(0, 0);
来源：http://lsr.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://jau.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://buc.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://jyj.cheryme.top

[D04] 删除元素
来源：http://uct.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mhn.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pnf.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://osz.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://lqs.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://taj.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nyo.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hus.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://smt.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://vko.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qjg.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tpn.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zsh.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://vtu.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://jnr.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://jwr.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://emy.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ecb.shuidangran.top

[D06] 数组长度
来源：http://ytv.fzhhl.top

Py:   len(arr)
来源：http://tyl.havefunace.top

PHP:  count($arr);
来源：http://cig.meibo888.top

JS:   arr.length
来源：http://zao.chenlongwang.top

TS:   arr.length
来源：http://hsc.epnwcf.com

Java: list.size();
来源：http://tia.zhengqikj.top

Go:   len(arr)
来源：http://jyi.316326.xyz

Ruby: arr.length; arr.size
来源：http://qho.epnwcf.com

C#:   list.Count;
来源：http://sdh.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://mro.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lgn.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://gic.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://dim.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://zhf.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://lzp.jyoumei.cn

Go:   arr[1:4]
来源：http://xcq.shuidangran.top

Ruby: arr[1, 3]
来源：http://pyi.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://ojs.c1oappe.top

[D08] 合并两个数组
来源：http://eij.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://jyc.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://lba.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zmv.haohaochexian.top

TS:   [...a, ...b];
来源：http://imu.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://liw.ybcxt.top

Go:   append(a, b...)
来源：http://rwm.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://qpq.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://ecb.bbcook.cn

[D09] 排序（升序）
来源：http://ygd.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://xly.nanxinkj.top

PHP:  sort($arr);
来源：http://qsc.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mvv.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pqr.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://amc.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xdd.shanyushiyangtech.top

Ruby: arr.sort
来源：http://pyv.yj20258888.top

C#:   list.Sort();
来源：http://twb.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpq.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://flz.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://adx.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lpv.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kzi.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kxr.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wef.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://doa.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://khh.pycfn.com

[D11] 反转数组
来源：http://jwp.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://nzg.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://sme.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sij.jinqigufen.top


<!-- 参考信息 -->