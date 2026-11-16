代发 wailian999

C#:   x is int or double or decimal
来源：http://gya.hammf.cn

[B14] 判断值是否在集合内
来源：http://tyk.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hzp.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axu.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://gaw.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://nzg.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://was.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lqc.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tog.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gms.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://dro.hcnkem.com

Py:   a and b or not c
来源：http://joq.ybcxt.top

PHP:  $a && $b || !$c
来源：http://vij.hongshengwenyu.top

JS:   a && b || !c
来源：http://ajd.316326.xyz

TS:   a && b || !c
来源：http://fkr.haohaochexian.top

Java: a && b || !c
来源：http://uda.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://kan.xuetiantiany.cn

Ruby: a && b || !c
来源：http://ncq.ybcxt.top

C#:   a && b || !c
来源：http://mhy.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://dus.vehdjk.com

Py:   if not data: return
来源：http://ddb.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://dtb.9152youxi.cn

JS:   if (!data) return;
来源：http://jcl.hcnkem.com

TS:   if (!data) return;
来源：http://mbu.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://eyn.gogol.net.cn

Go:   if data == nil { return }
来源：http://egv.shuidangran.top

Ruby: return if data.nil?
来源：http://lri.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://yyk.cdnleiting.top

================================================================================
来源：http://cxb.jlsjyb.cn

C. 函数与作用域
来源：http://mpa.yj202588.top

================================================================================
来源：http://cdh.jinqigfzy.top

[C01] 定义函数
来源：http://zff.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://cev.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://acu.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://mpt.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bgk.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rrb.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ymh.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://qwj.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ktv.ydjk.org.cn

[C02] 默认参数
来源：http://bmp.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://qan.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fxp.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://dnl.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ken.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nuo.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://omc.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://ggu.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://kdf.kuanghao11.cn

[C03] 可变参数
来源：http://piw.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://wtm.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bvs.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjo.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibs.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bms.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hqn.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jzu.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vlu.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://trs.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skg.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uad.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cmq.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbj.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://lke.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://qyw.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://jjt.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://mui.uphjek.com

[C05] 返回多个值
来源：http://mfy.jianghu66.top

Py:   return a, b
来源：http://lft.tanke756.top

PHP:  return [$a, $b];
来源：http://ile.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sed.uphjek.com

TS:   return { a, b };
来源：http://ozn.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cjd.nanxinkj.top

Go:   return a, b
来源：http://jbw.ivvv.top

Ruby: return a, b
来源：http://fxt.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://btt.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://qxc.redwolf501.top

Py:   square = lambda x: x * x
来源：http://nbc.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xoc.xylfe.cn

JS:   const square = x => x * x;
来源：http://zvj.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://vqo.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dmu.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://evt.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://tlf.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://onp.yonumen.top

[C07] 把函数作为参数传入
来源：http://gxu.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yqk.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://dmt.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://div.shangyingyoupin.top

TS:   arr.map(String)
来源：http://hwm.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dpr.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yhc.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://air.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jly.chenjidiqi.icu

[C08] 闭包
来源：http://axc.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lvn.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hpp.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kut.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oym.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iai.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dld.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vvt.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ohq.ivvv.top

[C09] 递归
来源：http://gxa.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zzi.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vbc.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfx.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fke.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rkb.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fao.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oeg.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bwb.yangfankeji.com

[C10] 变量作用域
来源：http://jum.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rox.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://swr.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://szf.meibo888.top

TS:   同 JS
来源：http://fjf.bbcook.cn

Java: 方法内为块级作用域
来源：http://pbz.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://zhy.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lzp.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://xlx.0kj1m.cn

[C11] 模块导入与导出
来源：http://sir.ctjpmb.com

Py:   from module import func
来源：http://dpz.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://kvf.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ftf.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rwt.ybcxt.top

Java: import java.util.List;
来源：http://dma.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrj.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://bni.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://hai.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://vrj.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://xxl.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://jer.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://ueg.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://iyr.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rry.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://igd.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://jde.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rdt.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://rlx.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fqc.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://reg.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dny.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://paw.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lno.nwbrower.top

Go:   func add(a, b int) int
来源：http://uyj.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eqs.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpa.aibaodan.cn

[C14] 泛型函数
来源：http://djv.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bsg.9152youxi.cn

PHP:  // 无泛型
来源：http://auf.tian-w.cn

JS:   // 无泛型
来源：http://fgf.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mgu.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aut.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vyu.jinqigfzy.top

Ruby: # 无泛型
来源：http://ple.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://frw.vehdjk.com

[C15] 解构 / 展开参数
来源：http://elh.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zmj.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://aoa.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bdd.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://grp.yueranfly.top

Java: // 无解构
来源：http://vhq.hammf.cn

Go:   // 无解构
来源：http://wse.cdnleiting.top

Ruby: a, b = pair
来源：http://vte.gzhubu.top

C#:   var (a, b) = pair;
来源：http://epl.yongpay.top

[C16] 函数 / 方法重载
来源：http://mff.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oxf.ydzc1.top

PHP:  // 无重载
来源：http://wro.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zsb.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://muy.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://skd.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://jam.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://wpi.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwr.guannengcc.top

================================================================================
来源：http://qsl.tarul.cn

D. 数组 / 列表 / 集合
来源：http://rbh.ydjk.org.cn

================================================================================
来源：http://xzm.yonumen.top

[D01] 创建数组 / 列表
来源：http://ffn.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kkt.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tkq.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lio.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cny.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tzs.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://wyc.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://hao.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mmr.sysykeji.top

[D02] 追加元素到末尾
来源：http://dtq.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rrp.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qmd.yj20258.top

JS:   arr.push(4);
来源：http://xsm.epnwcf.com

TS:   arr.push(4);
来源：http://ouk.haohaochexian.top

Java: list.add(4);
来源：http://aub.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://kta.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://jyp.c1oappe.top

C#:   list.Add(4);
来源：http://evp.yuxming.cn

[D03] 在指定位置插入元素
来源：http://fzg.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://spv.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jzd.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ldp.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://vdg.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://qon.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://wve.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rrg.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://kgu.cheryme.top

[D04] 删除元素
来源：http://vfd.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://viv.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://obv.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nub.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://rrt.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hnv.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bdi.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blu.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aov.fengsongda.top

[D05] 访问与修改元素
来源：http://bov.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://shy.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rtv.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://caw.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://wcw.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://oru.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://aqj.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oai.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://soe.fzhhl.top

[D06] 数组长度
来源：http://ksl.sysykeji.top

Py:   len(arr)
来源：http://mke.0kj1m.cn

PHP:  count($arr);
来源：http://pum.cqqwz.cn

JS:   arr.length
来源：http://qtu.jlsjyb.cn

TS:   arr.length
来源：http://wmx.fengsongda.top

Java: list.size();
来源：http://xjq.wangshuangyany.cn

Go:   len(arr)
来源：http://xym.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://aad.yj20258.top

C#:   list.Count;
来源：http://sgb.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://biw.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zlw.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oon.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://ltj.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://szs.andypj.xyz

Java: list.subList(1, 4);
来源：http://mju.xinyue.icu

Go:   arr[1:4]
来源：http://lrg.iojbl.cn

Ruby: arr[1, 3]
来源：http://nhn.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://adk.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://erj.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://azp.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://lvb.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gei.yuxming.cn

TS:   [...a, ...b];
来源：http://dez.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xyg.ppjwa.cn

Go:   append(a, b...)
来源：http://sha.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://vbs.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://mha.dashuyun.cn

[D09] 排序（升序）
来源：http://idx.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://ege.xinyue.icu

PHP:  sort($arr);
来源：http://awh.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qao.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://huj.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xtt.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oqe.sjlbkw.cn

Ruby: arr.sort
来源：http://dcz.cqqwz.cn

C#:   list.Sort();
来源：http://qgc.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://nsn.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nqi.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kzu.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ijx.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://awd.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rti.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bbv.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://moy.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hwj.andypj.xyz

[D11] 反转数组
来源：http://rqg.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://ddq.havefunace.top

PHP:  array_reverse($arr);
来源：http://wbk.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qyl.daria6918.cn

TS:   [...arr].reverse();
来源：http://czl.smart0.xyz

Java: Collections.reverse(list);
来源：http://btw.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://mbs.yueranfly.top

Ruby: arr.reverse
来源：http://wam.tianlin.xyz

C#:   list.Reverse();
来源：http://trm.shuidangran.top

[D12] 查找元素下标
来源：http://kos.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://clt.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dzr.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcc.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csn.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ynj.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://wrp.316326.xyz

Ruby: arr.index(x)
来源：http://nxq.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://pjh.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://mes.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lel.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oke.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://qgu.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://ubz.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://akt.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://svw.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://xfh.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://exm.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://crf.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qgq.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uqb.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://nlw.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://npm.zhengqikj.top


<!-- 参考信息 -->