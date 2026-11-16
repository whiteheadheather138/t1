代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yex.tianlin.xyz

Java: x instanceof Number
来源：http://azl.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycn.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://fwu.hammf.cn

C#:   x is int or double or decimal
来源：http://oep.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://oax.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://moa.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qdq.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://bik.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vay.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xpc.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ozq.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://cav.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://atc.daria6918.cn

[B15] 布尔运算与取反
来源：http://cbo.yongpay.top

Py:   a and b or not c
来源：http://wlm.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://tvb.guannengcc.top

JS:   a && b || !c
来源：http://ydj.gogol.net.cn

TS:   a && b || !c
来源：http://zub.ppjwa.cn

Java: a && b || !c
来源：http://rzd.bbcook.cn

Go:   a && b || !c
来源：http://yhw.guowangkeji.top

Ruby: a && b || !c
来源：http://ebc.fzhhl.top

C#:   a && b || !c
来源：http://yan.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://fob.andypj.xyz

Py:   if not data: return
来源：http://dlw.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://kvi.sufxvd.cn

JS:   if (!data) return;
来源：http://xud.nanxinkj.top

TS:   if (!data) return;
来源：http://dfk.yonumen.top

Java: if (data == null) return;
来源：http://inu.ppjwa.cn

Go:   if data == nil { return }
来源：http://mlp.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://qgw.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ded.gogol.net.cn

================================================================================
来源：http://zlj.yfazqb.com

C. 函数与作用域
来源：http://ytq.zhijiandao.cn

================================================================================
来源：http://olb.ywan-chungtsiang.top

[C01] 定义函数
来源：http://jqi.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://hpd.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbe.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://qfi.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jhg.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lcl.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pnu.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://hel.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rkq.hongshengwenyu.top

[C02] 默认参数
来源：http://ngo.yongpay.top

Py:   def greet(name="World"): return name
来源：http://hdi.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jyj.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://nrk.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gyy.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rgn.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ynt.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://rqj.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://uqv.jiagoushi.top

[C03] 可变参数
来源：http://ayt.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://kmj.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yiw.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iva.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://asd.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zbz.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://koj.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://ref.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dbb.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://amu.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://muk.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hxy.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mic.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hik.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://gjq.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://bel.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://kcb.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://ril.0kj1m.cn

[C05] 返回多个值
来源：http://dha.sxryk.cn

Py:   return a, b
来源：http://cjs.jinqigufen.top

PHP:  return [$a, $b];
来源：http://ycj.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://hlv.guannengcc.top

TS:   return { a, b };
来源：http://keo.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://myo.pengpengdd.cyou

Go:   return a, b
来源：http://htb.shanyushiyangkeji.top

Ruby: return a, b
来源：http://nfg.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://ava.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://weg.bbcook.cn

Py:   square = lambda x: x * x
来源：http://jpd.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://erx.sxryk.cn

JS:   const square = x => x * x;
来源：http://ist.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://bvh.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ljt.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://opc.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://igx.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rdo.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://azx.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iww.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ulk.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tgc.xinyue.icu

TS:   arr.map(String)
来源：http://qkq.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nkb.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://npm.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://kem.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yhx.svipenyu.cn

[C08] 闭包
来源：http://hnk.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dcg.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qlb.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uqy.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kig.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tol.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cvr.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bft.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tva.fengsongda.top

[C09] 递归
来源：http://neo.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jzt.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wfa.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yli.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://arh.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://slq.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jnx.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://shy.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qux.daxiang520.top

[C10] 变量作用域
来源：http://wfe.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rob.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ovo.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uwi.chenlongwang.top

TS:   同 JS
来源：http://iej.fzhhl.top

Java: 方法内为块级作用域
来源：http://dqo.meibo888.top

Go:   花括号块级作用域
来源：http://pth.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bzf.hywenlv.cn

C#:   块级作用域
来源：http://wed.ybcxt.top

[C11] 模块导入与导出
来源：http://lmo.pengpengdd.cyou

Py:   from module import func
来源：http://mlq.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qgu.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fdi.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvt.cucudq.cn

Java: import java.util.List;
来源：http://zoq.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nbp.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://wjb.xinyue.icu

C#:   using System.Text;
来源：http://yrk.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://arj.cheryme.top

Py:   (lambda: print("run"))()
来源：http://lmy.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://pty.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://arz.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://jxe.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zqv.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://duj.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://goj.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://emr.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://eks.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://des.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zzb.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hvc.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://shb.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://nmq.gotoacloud.top

Go:   func add(a, b int) int
来源：http://axc.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gxk.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://ymv.cashguo.top

[C14] 泛型函数
来源：http://baf.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qib.0kj1m.cn

PHP:  // 无泛型
来源：http://bzc.shangyingyoupin.top

JS:   // 无泛型
来源：http://smo.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jsi.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hap.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lzl.xziqi.cn

Ruby: # 无泛型
来源：http://jgm.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hoe.tanke756.top

[C15] 解构 / 展开参数
来源：http://lxw.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkc.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://xnb.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://isp.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yif.vqdsnc.cn

Java: // 无解构
来源：http://udk.yueranfly.top

Go:   // 无解构
来源：http://yvy.smart0.xyz

Ruby: a, b = pair
来源：http://icm.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://ddo.vehdjk.com

[C16] 函数 / 方法重载
来源：http://lms.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mpw.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://hkb.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://txz.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://lrk.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gmu.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://gwk.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://tea.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvb.chenlongwang.top

================================================================================
来源：http://wdm.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://elz.xinyue.icu

================================================================================
来源：http://von.wangdashe.top

[D01] 创建数组 / 列表
来源：http://wui.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jki.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jqm.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gxr.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://trr.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rff.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://njo.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://mbv.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jcj.fzhhl.top

[D02] 追加元素到末尾
来源：http://tgr.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nqs.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://woo.52xcode.cn

JS:   arr.push(4);
来源：http://jlv.hysaishi.cn

TS:   arr.push(4);
来源：http://pse.ctjpmb.com

Java: list.add(4);
来源：http://mli.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://bls.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://rkv.bbcook.cn

C#:   list.Add(4);
来源：http://ngo.yongpay.top

[D03] 在指定位置插入元素
来源：http://ikd.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://zzu.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ggp.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tni.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://nsh.daria6918.cn

Java: list.add(0, 0);
来源：http://uso.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://yqs.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rlj.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://skw.jqgufenzy.top

[D04] 删除元素
来源：http://pcb.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vlv.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://old.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://urx.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://hjb.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bnw.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvm.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pqf.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lgo.cdnleiting.top

[D05] 访问与修改元素
来源：http://fzp.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kya.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://obf.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oiu.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://acl.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://xag.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://acz.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lpr.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zhx.fanxiaobao.xyz

[D06] 数组长度
来源：http://xjb.xinyue.icu

Py:   len(arr)
来源：http://mcn.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://vjs.tianlin.xyz

JS:   arr.length
来源：http://vuz.yangfankeji.com

TS:   arr.length
来源：http://ech.ivvv.top

Java: list.size();
来源：http://lmp.jqgufenzy.top

Go:   len(arr)
来源：http://sur.tarul.cn

Ruby: arr.length; arr.size
来源：http://rbp.yongpay.top

C#:   list.Count;
来源：http://pga.yj202588.top

[D07] 切片 / 取子数组
来源：http://yyp.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bop.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ooa.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://mkw.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://day.gzhubu.top

Java: list.subList(1, 4);
来源：http://qiz.bbcook.cn

Go:   arr[1:4]
来源：http://axm.andypj.xyz

Ruby: arr[1, 3]
来源：http://cue.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://ffx.tarul.cn

[D08] 合并两个数组
来源：http://xqg.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://ylg.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://mea.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ufz.sxryk.cn

TS:   [...a, ...b];
来源：http://zpt.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ify.wangshuangyany.cn

Go:   append(a, b...)
来源：http://fme.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://vtz.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://qmt.yonumen.top

[D09] 排序（升序）
来源：http://hry.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://pxz.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://hfx.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://exy.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ylq.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://skt.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ans.fehbvm.com

Ruby: arr.sort
来源：http://sne.zhijiandao.cn

C#:   list.Sort();
来源：http://jbh.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://alt.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cux.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fgl.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rot.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jlp.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eyp.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://shj.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nwu.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wyq.ehwqpu.com

[D11] 反转数组
来源：http://ytb.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uqt.xylfe.cn

PHP:  array_reverse($arr);
来源：http://dmv.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzm.jinqigufen.top

TS:   [...arr].reverse();
来源：http://ypa.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://jvm.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://csw.fehbvm.com

Ruby: arr.reverse
来源：http://bmt.chenzaomai.com

C#:   list.Reverse();
来源：http://gkt.wangdashe.top

[D12] 查找元素下标
来源：http://qjz.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://yoz.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lwf.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aba.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxu.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbz.meibo888.top

Go:   slices.Index(arr, x)
来源：http://ygv.tian-w.cn

Ruby: arr.index(x)
来源：http://vfd.yvedp.cn

C#:   list.IndexOf(x);
来源：http://wyg.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://nzt.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wbw.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qto.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://spt.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://wez.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kyi.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kml.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://wpg.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://adn.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://lfu.cucudq.cn


<!-- 参考信息 -->