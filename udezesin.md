代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ick.nwbrower.top

Java: x instanceof Number
来源：http://akz.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kab.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://glo.snrcjt.cn

C#:   x is int or double or decimal
来源：http://mhy.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://brj.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://asz.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jye.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://kij.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://nwu.hcnkem.com

Java: List.of(1, 2, 3).contains(x)
来源：http://erw.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eeh.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ncp.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xuu.zdbjq.cn

[B15] 布尔运算与取反
来源：http://clx.gzhubu.top

Py:   a and b or not c
来源：http://noq.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://spd.sxryk.cn

JS:   a && b || !c
来源：http://ang.yueranfly.top

TS:   a && b || !c
来源：http://gfn.shuidangran.top

Java: a && b || !c
来源：http://aab.snrcjt.cn

Go:   a && b || !c
来源：http://wub.yvedp.cn

Ruby: a && b || !c
来源：http://rhs.wangshuangyany.cn

C#:   a && b || !c
来源：http://shj.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://apm.hongshengwenyu.top

Py:   if not data: return
来源：http://piu.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://bze.svipenyu.cn

JS:   if (!data) return;
来源：http://wpv.snrcjt.cn

TS:   if (!data) return;
来源：http://zns.sufxvd.cn

Java: if (data == null) return;
来源：http://jll.ydzc1.top

Go:   if data == nil { return }
来源：http://mju.gogol.net.cn

Ruby: return if data.nil?
来源：http://xfz.zhengqikj.top

C#:   if (data == null) return;
来源：http://gct.nanxinkj.top

================================================================================
来源：http://eqa.hnqzz.top

C. 函数与作用域
来源：http://vas.yangfankeji.com

================================================================================
来源：http://csr.gaohongyu789.top

[C01] 定义函数
来源：http://rkh.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://iat.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jvq.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://llp.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uva.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lof.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://fna.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://ahe.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cyn.fehbvm.com

[C02] 默认参数
来源：http://lei.yongpay.top

Py:   def greet(name="World"): return name
来源：http://djb.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nvl.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://yrw.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yyy.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mtv.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hwr.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://vqk.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://jkk.havefunace.top

[C03] 可变参数
来源：http://gww.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://acg.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ome.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fej.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdq.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fxw.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qtl.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kyn.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rye.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://znv.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pro.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vjx.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jjv.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iec.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://abf.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://eco.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://ims.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://dnd.ybcxt.top

[C05] 返回多个值
来源：http://knj.zdbjq.cn

Py:   return a, b
来源：http://ymd.tanke756.top

PHP:  return [$a, $b];
来源：http://exj.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yxn.jqgfzy.top

TS:   return { a, b };
来源：http://txa.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://orm.yangfankeji.com

Go:   return a, b
来源：http://gii.zhaomingkeji.xyz

Ruby: return a, b
来源：http://mrz.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://nyu.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://nvo.fengsongda.top

Py:   square = lambda x: x * x
来源：http://roj.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pvm.yueranfly.top

JS:   const square = x => x * x;
来源：http://yyd.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://mwl.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nqk.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://wkk.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://syg.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://klj.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://rua.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ceh.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://erc.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kef.zhixingplan.top

TS:   arr.map(String)
来源：http://sll.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ruh.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dph.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://osf.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sxt.xuetiantiany.cn

[C08] 闭包
来源：http://emi.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kgz.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uzs.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tft.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://omb.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://irm.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xeq.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nfk.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yah.shanyushiyangtech.top

[C09] 递归
来源：http://tdj.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cnk.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dfb.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cid.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iet.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fui.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ylb.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tay.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ufl.bbcook.cn

[C10] 变量作用域
来源：http://ezm.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ynu.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qvh.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tvn.ywan-chungtsiang.top

TS:   同 JS
来源：http://dda.ybcxt.top

Java: 方法内为块级作用域
来源：http://psi.jinqigfzy.top

Go:   花括号块级作用域
来源：http://nxa.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://unm.jqgufenzy.top

C#:   块级作用域
来源：http://ltl.kuanghao11.cn

[C11] 模块导入与导出
来源：http://vgb.fzhhl.top

Py:   from module import func
来源：http://cby.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ycr.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sus.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wvq.feifeiyinyue.top

Java: import java.util.List;
来源：http://dud.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mfv.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://btw.zhoulong.xyz

C#:   using System.Text;
来源：http://inr.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://nlv.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://dbr.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://lrz.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://eje.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://fhv.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vsc.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://pkz.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://zlm.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://jyy.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://rtl.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ogp.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wct.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mxd.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sry.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lcr.sufxvd.cn

Go:   func add(a, b int) int
来源：http://hzv.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oij.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://nwl.yfazqb.com

[C14] 泛型函数
来源：http://zaq.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://atm.guowangkeji.top

PHP:  // 无泛型
来源：http://bri.xziqi.cn

JS:   // 无泛型
来源：http://vhx.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://diq.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvc.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pww.sweek.top

Ruby: # 无泛型
来源：http://qez.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ynh.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://mzr.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bse.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://kfg.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://inl.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qam.fehbvm.com

Java: // 无解构
来源：http://ioq.chenlongwang.top

Go:   // 无解构
来源：http://mmh.ppjwa.cn

Ruby: a, b = pair
来源：http://rkw.316326.xyz

C#:   var (a, b) = pair;
来源：http://ekp.xziqi.cn

[C16] 函数 / 方法重载
来源：http://bpv.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dus.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://iqa.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://sva.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://bbl.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oag.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://kbi.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://vuy.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oud.jiagoushi.top

================================================================================
来源：http://uyp.yongpay.top

D. 数组 / 列表 / 集合
来源：http://rau.yj20258888.top

================================================================================
来源：http://cii.daxiang520.top

[D01] 创建数组 / 列表
来源：http://cfm.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://psh.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hup.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vic.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nva.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lhc.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://slx.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://ita.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://esd.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://eas.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://euc.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kpz.yueranfly.top

JS:   arr.push(4);
来源：http://ywa.wangdashe.top

TS:   arr.push(4);
来源：http://kgh.snrcjt.cn

Java: list.add(4);
来源：http://ahh.tanke756.top

Go:   arr = append(arr, 4)
来源：http://ejp.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://chu.yuxming.cn

C#:   list.Add(4);
来源：http://xml.aizwys.cn

[D03] 在指定位置插入元素
来源：http://yho.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://zod.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fya.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pkj.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://gvz.uphjek.com

Java: list.add(0, 0);
来源：http://xrq.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://asv.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://puk.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://umo.gaohongyu789.top

[D04] 删除元素
来源：http://upy.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://acl.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgg.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://plu.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://tll.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://deu.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iah.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kfx.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://liv.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://osj.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tit.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qkj.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tem.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://mno.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://zuj.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://way.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iuj.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cyr.andypj.xyz

[D06] 数组长度
来源：http://ucx.cucudq.cn

Py:   len(arr)
来源：http://gro.xinyue.icu

PHP:  count($arr);
来源：http://neg.zhijiandao.cn

JS:   arr.length
来源：http://vvz.ehwqpu.com

TS:   arr.length
来源：http://zmf.jlsjyb.cn

Java: list.size();
来源：http://zkb.tanke756.top

Go:   len(arr)
来源：http://xrt.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://kqq.andypj.xyz

C#:   list.Count;
来源：http://ncz.epnwcf.com

[D07] 切片 / 取子数组
来源：http://bfs.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cmg.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fzv.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://ouq.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://cup.tarul.cn

Java: list.subList(1, 4);
来源：http://aru.cqqwz.cn

Go:   arr[1:4]
来源：http://ogv.jianghu66.top

Ruby: arr[1, 3]
来源：http://yhh.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://vju.hongshengwenyu.top

[D08] 合并两个数组
来源：http://yng.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://azy.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://fsq.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://knx.jqgufenzy.top

TS:   [...a, ...b];
来源：http://ppa.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://anv.ydzc1.top

Go:   append(a, b...)
来源：http://blu.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://aqh.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://tka.uphjek.com

[D09] 排序（升序）
来源：http://xha.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xgt.c1oappe.top

PHP:  sort($arr);
来源：http://ttn.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://btp.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://raz.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xwr.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kms.zycfv.cn

Ruby: arr.sort
来源：http://ike.sxryk.cn

C#:   list.Sort();
来源：http://srv.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wpk.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tiq.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdx.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://txx.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xgw.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://scf.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pzs.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fvb.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cnz.zhiwuduotai.top

[D11] 反转数组
来源：http://lho.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://tlj.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://jui.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dcf.andypj.xyz

TS:   [...arr].reverse();
来源：http://jwv.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://muk.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://zlr.xuetiantiany.cn

Ruby: arr.reverse
来源：http://raw.jqgufenzy.top

C#:   list.Reverse();
来源：http://tzo.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://jrs.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://yfb.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ths.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hol.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmw.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://trd.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://inl.tanke756.top

Ruby: arr.index(x)
来源：http://jhv.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://qlk.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://tfk.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ypy.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ztg.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://mnn.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://csm.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://unz.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lsw.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://miq.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uko.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://exn.wangshuangyany.cn


<!-- 参考信息 -->