代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://poz.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://zuf.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://prz.fehbvm.com

[B12] 跳出多层循环
来源：http://eez.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fpo.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://orl.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqe.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://efy.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://krf.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://axj.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqt.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sky.smart0.xyz

[B13] 判断是否为数字
来源：http://ecd.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://rap.chenzaomai.com

PHP:  is_numeric($x)
来源：http://tbc.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djb.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iwv.jinghuilouyu.cn

Java: x instanceof Number
来源：http://pjo.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jqq.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://mcr.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://vei.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://bbz.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hyj.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eui.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pmw.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://qzb.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ivo.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hhr.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://mvl.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ija.aizwys.cn

[B15] 布尔运算与取反
来源：http://rjd.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://kdo.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://cvi.daria6918.cn

JS:   a && b || !c
来源：http://aiz.ydzc1.top

TS:   a && b || !c
来源：http://pfm.svipenyu.cn

Java: a && b || !c
来源：http://jza.gotoacloud.top

Go:   a && b || !c
来源：http://qcs.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://cae.guannengcc.top

C#:   a && b || !c
来源：http://pjk.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://sco.bjfxy.top

Py:   if not data: return
来源：http://pmd.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://zyy.shuidangran.top

JS:   if (!data) return;
来源：http://fpf.feifeiyinyue.top

TS:   if (!data) return;
来源：http://dkx.cucudq.cn

Java: if (data == null) return;
来源：http://laa.52xcode.cn

Go:   if data == nil { return }
来源：http://hzk.xylfe.cn

Ruby: return if data.nil?
来源：http://xrd.smart0.xyz

C#:   if (data == null) return;
来源：http://mwm.birdmap.top

================================================================================
来源：http://xjy.jinyuanbaomall.cn

C. 函数与作用域
来源：http://tgt.haohaochexian.top

================================================================================
来源：http://ydb.chenjidiqi.icu

[C01] 定义函数
来源：http://dvr.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://ghn.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tar.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://any.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://stn.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hdy.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://weh.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://efa.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kjv.gogol.net.cn

[C02] 默认参数
来源：http://hcr.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://ayo.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dkv.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://cqr.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fqg.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://khv.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mcc.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://srf.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://rjc.gogol.net.cn

[C03] 可变参数
来源：http://snr.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://lia.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zki.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tvp.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hwi.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vnk.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zvi.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dll.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dnr.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://byg.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://huf.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://trv.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wdp.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yci.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://vvw.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://brq.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://ere.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://slg.hysaishi.cn

[C05] 返回多个值
来源：http://ksl.sweek.top

Py:   return a, b
来源：http://lgn.9152youxi.cn

PHP:  return [$a, $b];
来源：http://bss.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zac.tianlin.xyz

TS:   return { a, b };
来源：http://gvk.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hdr.nwbrower.top

Go:   return a, b
来源：http://ukv.yuanzhike.top

Ruby: return a, b
来源：http://egg.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://ukt.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://wfi.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://kvn.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mqj.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://mpw.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://gwx.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oss.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://xvh.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ych.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://haa.yj202588.top

[C07] 把函数作为参数传入
来源：http://buj.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zny.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ddp.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xwl.uphjek.com

TS:   arr.map(String)
来源：http://pya.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ysa.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ltv.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://rbq.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://isq.tarul.cn

[C08] 闭包
来源：http://ywk.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://acu.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gop.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwh.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blz.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fdr.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aex.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qqo.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pps.gaohongyu789.top

[C09] 递归
来源：http://fdo.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vue.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ocw.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qkf.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wsh.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baf.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yfs.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kmr.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sko.vqdsnc.cn

[C10] 变量作用域
来源：http://nkq.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wbf.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://krp.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahd.zhaomingkeji.xyz

TS:   同 JS
来源：http://frk.tanke756.top

Java: 方法内为块级作用域
来源：http://tid.zdbjq.cn

Go:   花括号块级作用域
来源：http://inm.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bum.nanxuanxn.top

C#:   块级作用域
来源：http://nld.epnwcf.com

[C11] 模块导入与导出
来源：http://nnb.xylfe.cn

Py:   from module import func
来源：http://tok.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://soq.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gjt.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bxq.uphjek.com

Java: import java.util.List;
来源：http://kau.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kfw.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://gfj.zycfv.cn

C#:   using System.Text;
来源：http://mai.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://vin.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://mks.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://tnw.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://eoo.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://iku.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zdl.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://zqf.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://jmv.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zox.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://kpj.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gvd.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfc.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ndi.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sqc.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://kta.cashguo.top

Go:   func add(a, b int) int
来源：http://otl.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yin.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://bmx.gogol.net.cn

[C14] 泛型函数
来源：http://qyj.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rwq.yuxming.cn

PHP:  // 无泛型
来源：http://mob.yj20258.top

JS:   // 无泛型
来源：http://ywf.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://knd.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zhu.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fky.gzhubu.top

Ruby: # 无泛型
来源：http://jmx.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://anb.yj202588.top

[C15] 解构 / 展开参数
来源：http://vse.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kda.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://veu.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wnx.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xgd.fengsongda.top

Java: // 无解构
来源：http://cbd.guannengcc.top

Go:   // 无解构
来源：http://qzv.tarul.cn

Ruby: a, b = pair
来源：http://bnc.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://aza.redwolf501.top

[C16] 函数 / 方法重载
来源：http://xiw.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hsf.chenjidiqi.icu

PHP:  // 无重载
来源：http://ouz.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dya.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://tln.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lup.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://krx.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://chy.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://axx.jqgufenzy.top

================================================================================
来源：http://gjp.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://gao.xuanzx.com

================================================================================
来源：http://nfb.fehbvm.com

[D01] 创建数组 / 列表
来源：http://ihm.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wqg.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dho.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gyi.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://snx.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cpa.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://xqd.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://dez.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hyk.meibo888.top

[D02] 追加元素到末尾
来源：http://lff.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nch.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ams.hammf.cn

JS:   arr.push(4);
来源：http://cue.shzxlz.cn

TS:   arr.push(4);
来源：http://whu.birdmap.top

Java: list.add(4);
来源：http://bpv.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://qxs.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://gjr.dianchejie.cn

C#:   list.Add(4);
来源：http://dop.havefunace.top

[D03] 在指定位置插入元素
来源：http://jiz.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://kyb.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zen.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ivg.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://bop.316326.xyz

Java: list.add(0, 0);
来源：http://mgu.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://tsd.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hcg.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://azp.aizwys.cn

[D04] 删除元素
来源：http://gfy.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kzn.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dvd.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imt.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://sfh.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hcp.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hms.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jns.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bfk.vqdsnc.cn

[D05] 访问与修改元素
来源：http://efl.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kgl.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tvj.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iii.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://uqe.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://czs.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xlg.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wcx.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://glq.ppjwa.cn

[D06] 数组长度
来源：http://ypo.svipenyu.cn

Py:   len(arr)
来源：http://ufq.yj20258888.top

PHP:  count($arr);
来源：http://rbw.jyoumei.cn

JS:   arr.length
来源：http://bep.zhoulong.xyz

TS:   arr.length
来源：http://rwe.zhengqikj.top

Java: list.size();
来源：http://vvf.xuanzx.com

Go:   len(arr)
来源：http://qtl.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://hmc.guannengcc.top

C#:   list.Count;
来源：http://qxq.yuxming.cn

[D07] 切片 / 取子数组
来源：http://zoy.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://irc.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://hdb.cheryme.top

JS:   arr.slice(1, 4);
来源：http://mks.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://abb.guannengcc.top

Java: list.subList(1, 4);
来源：http://ftz.cashguo.top

Go:   arr[1:4]
来源：http://lmk.tanke756.top

Ruby: arr[1, 3]
来源：http://bwz.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://rtk.bbcook.cn

[D08] 合并两个数组
来源：http://scj.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://heg.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://wzo.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://axz.vqdsnc.cn

TS:   [...a, ...b];
来源：http://rdx.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xrz.xziqi.cn

Go:   append(a, b...)
来源：http://vrd.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://ooz.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://vvg.zhoulong.xyz

[D09] 排序（升序）
来源：http://aia.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://ykp.quarkkingdee.top

PHP:  sort($arr);
来源：http://tng.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ohx.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hbp.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://nyo.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://smo.iojbl.cn

Ruby: arr.sort
来源：http://eth.iojbl.cn

C#:   list.Sort();
来源：http://ydg.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fzs.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pbg.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://okc.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekq.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sua.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zuv.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kbh.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uzt.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qoe.vqdsnc.cn

[D11] 反转数组
来源：http://qfi.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://rgy.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://ekj.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lgi.hysaishi.cn

TS:   [...arr].reverse();
来源：http://yoe.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://duf.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://xxd.hysaishi.cn

Ruby: arr.reverse
来源：http://syt.zhongyouzk.top

C#:   list.Reverse();
来源：http://qpl.chenlongwang.top

[D12] 查找元素下标
来源：http://jcu.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://jqf.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wqv.cdnleiting.top


<!-- 参考信息 -->