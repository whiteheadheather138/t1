代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://knu.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ops.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hrh.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ubn.ydzc1.top

[B13] 判断是否为数字
来源：http://peb.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://owv.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://mms.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swn.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hib.hnqzz.top

Java: x instanceof Number
来源：http://mdd.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ezc.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://hki.andypj.xyz

C#:   x is int or double or decimal
来源：http://trz.tarul.cn

[B14] 判断值是否在集合内
来源：http://dht.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dyh.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vie.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://lhv.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://ghn.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lxp.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://con.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://mao.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://byk.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://ugr.jinqigfzy.top

Py:   a and b or not c
来源：http://pjt.fehbvm.com

PHP:  $a && $b || !$c
来源：http://mhx.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://adb.sxryk.cn

TS:   a && b || !c
来源：http://ppo.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://dve.sweek.top

Go:   a && b || !c
来源：http://fqv.aibaodan.cn

Ruby: a && b || !c
来源：http://ezw.andypj.xyz

C#:   a && b || !c
来源：http://yhq.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jvu.vqdsnc.cn

Py:   if not data: return
来源：http://ouq.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://qsd.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://rdm.hfpthk.cn

TS:   if (!data) return;
来源：http://tlc.uphjek.com

Java: if (data == null) return;
来源：http://cba.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://agi.dashuyun.cn

Ruby: return if data.nil?
来源：http://qbn.gzhubu.top

C#:   if (data == null) return;
来源：http://ksw.hesvh.cn

================================================================================
来源：http://kdm.zhixingplan.top

C. 函数与作用域
来源：http://dtx.fzhhl.top

================================================================================
来源：http://kjr.cashguo.top

[C01] 定义函数
来源：http://jar.yonumen.top

Py:   def add(a, b): return a + b
来源：http://fnc.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://odw.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://rjl.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zih.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cyj.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://lpl.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://uog.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wgc.yueranfly.top

[C02] 默认参数
来源：http://suj.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://mga.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://rui.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://ixz.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jqr.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kxn.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tqr.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://kme.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://alx.smart0.xyz

[C03] 可变参数
来源：http://agy.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://iow.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vni.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yss.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://znr.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xdv.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://son.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gen.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://enq.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://hmv.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ntt.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wmg.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dhh.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xnj.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://zom.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://tkh.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://qnz.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://hvz.meibo888.top

[C05] 返回多个值
来源：http://cxw.cashguo.top

Py:   return a, b
来源：http://gyo.vehdjk.com

PHP:  return [$a, $b];
来源：http://swe.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://siu.bjfxy.top

TS:   return { a, b };
来源：http://kzu.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pqf.uphjek.com

Go:   return a, b
来源：http://reo.daxiang520.top

Ruby: return a, b
来源：http://kob.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://fgg.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://mkl.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://eae.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zrc.dianchejie.cn

JS:   const square = x => x * x;
来源：http://hmq.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://wce.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blu.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://moc.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://grr.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tys.vehdjk.com

[C07] 把函数作为参数传入
来源：http://epc.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gtu.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://hqi.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sri.chenlongwang.top

TS:   arr.map(String)
来源：http://zaj.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yru.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hbe.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://lvl.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ctn.xingfuxueyuan.xyz

[C08] 闭包
来源：http://hgj.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fsm.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sab.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wab.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bxx.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nzd.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ljq.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qwy.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tgr.gotoacloud.top

[C09] 递归
来源：http://iqo.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wfw.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wad.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://roy.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtc.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tgt.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iba.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://its.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fgk.hnxiangtu.top

[C10] 变量作用域
来源：http://hyo.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zbt.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qad.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bvm.hcnkem.com

TS:   同 JS
来源：http://scm.dianchejie.cn

Java: 方法内为块级作用域
来源：http://vqi.sufxvd.cn

Go:   花括号块级作用域
来源：http://jcb.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hwa.hongshengwenyu.top

C#:   块级作用域
来源：http://qgb.yuanzhike.top

[C11] 模块导入与导出
来源：http://rlw.aizwys.cn

Py:   from module import func
来源：http://zpu.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wyn.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://opp.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rkq.dashuyun.cn

Java: import java.util.List;
来源：http://wpo.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://igk.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://mvx.yuanzhike.top

C#:   using System.Text;
来源：http://lli.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://hku.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://fwb.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://fti.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://mcc.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://nab.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://miw.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://fth.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://hge.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ozw.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://ahg.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hat.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bdw.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://evg.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hvb.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://toe.tianlin.xyz

Go:   func add(a, b int) int
来源：http://yco.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hrx.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://hmj.sweek.top

[C14] 泛型函数
来源：http://yic.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ygs.nanxinkj.top

PHP:  // 无泛型
来源：http://whg.shuidangran.top

JS:   // 无泛型
来源：http://gqm.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dih.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bai.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nml.aizwys.cn

Ruby: # 无泛型
来源：http://eme.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zub.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://wro.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yyi.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://hea.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ajf.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sjq.svipenyu.cn

Java: // 无解构
来源：http://lss.hfpthk.cn

Go:   // 无解构
来源：http://nsf.yvedp.cn

Ruby: a, b = pair
来源：http://nfx.guannengcc.top

C#:   var (a, b) = pair;
来源：http://xts.vehdjk.com

[C16] 函数 / 方法重载
来源：http://uox.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://our.hfpthk.cn

PHP:  // 无重载
来源：http://efe.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fzo.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://gir.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fvq.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://eca.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://ccq.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wtv.daria6918.cn

================================================================================
来源：http://wke.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://pev.zhijiandao.cn

================================================================================
来源：http://knc.xziqi.cn

[D01] 创建数组 / 列表
来源：http://uxs.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://exd.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jxp.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://plw.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://key.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nxh.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://vjn.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://jqt.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hdr.andypj.xyz

[D02] 追加元素到末尾
来源：http://gca.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lqr.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ems.zhoulong.xyz

JS:   arr.push(4);
来源：http://gdp.yj20258.top

TS:   arr.push(4);
来源：http://xsq.pycfn.com

Java: list.add(4);
来源：http://mhp.hammf.cn

Go:   arr = append(arr, 4)
来源：http://xvb.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://quw.fengsongda.top

C#:   list.Add(4);
来源：http://jqw.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://jxi.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://gzv.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ple.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rvp.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://ecb.vehdjk.com

Java: list.add(0, 0);
来源：http://kzb.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zpy.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eut.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://swu.chenlongwang.top

[D04] 删除元素
来源：http://vgm.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://doy.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cyh.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dcb.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://kom.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hws.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lct.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bja.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rrf.yongpay.top

[D05] 访问与修改元素
来源：http://bva.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pom.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://efr.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://inb.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://jeg.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://qjf.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://bwp.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://geo.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://drl.wangshuangyany.cn

[D06] 数组长度
来源：http://gvy.hesvh.cn

Py:   len(arr)
来源：http://qnk.yvedp.cn

PHP:  count($arr);
来源：http://pdk.hongshengwenyu.top

JS:   arr.length
来源：http://odl.chenjidiqi.icu

TS:   arr.length
来源：http://wje.zhaomingkeji.xyz

Java: list.size();
来源：http://frh.smart0.xyz

Go:   len(arr)
来源：http://szi.daria6918.cn

Ruby: arr.length; arr.size
来源：http://dcg.tian-w.cn

C#:   list.Count;
来源：http://eng.daria6918.cn

[D07] 切片 / 取子数组
来源：http://tjk.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axi.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yxv.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://udc.cheryme.top

TS:   arr.slice(1, 4);
来源：http://ftg.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://fjb.tian-w.cn

Go:   arr[1:4]
来源：http://iun.andypj.xyz

Ruby: arr[1, 3]
来源：http://lwa.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://bln.feifeiyinyue.top

[D08] 合并两个数组
来源：http://vpk.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://uek.pycfn.com

PHP:  array_merge($a, $b);
来源：http://wcj.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://beo.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://khv.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sio.yuanzhike.top

Go:   append(a, b...)
来源：http://smq.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://pcw.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://knf.daria6918.cn

[D09] 排序（升序）
来源：http://xtw.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://ehi.0kj1m.cn

PHP:  sort($arr);
来源：http://zup.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kjg.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jlo.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lrh.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://efg.hesvh.cn

Ruby: arr.sort
来源：http://afd.tarul.cn

C#:   list.Sort();
来源：http://xln.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xnf.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jxl.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvk.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lgu.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yzu.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://daz.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://chx.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqv.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pch.zycfv.cn

[D11] 反转数组
来源：http://vtr.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nez.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://byj.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mya.tarul.cn

TS:   [...arr].reverse();
来源：http://gbb.daxiang520.top

Java: Collections.reverse(list);
来源：http://ufs.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://lsh.zhijiandao.cn

Ruby: arr.reverse
来源：http://cuz.quarkkingdee.top

C#:   list.Reverse();
来源：http://kps.vehdjk.com

[D12] 查找元素下标
来源：http://umi.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://lpp.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://duf.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zsw.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xqc.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ijb.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://wcb.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://dds.ybcxt.top

C#:   list.IndexOf(x);
来源：http://ryb.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://viy.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zfb.nanxuanxn.top


<!-- 参考信息 -->