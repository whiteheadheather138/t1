代发 wailian999

[B13] 判断是否为数字
来源：http://lsx.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://jxa.yueranfly.top

PHP:  is_numeric($x)
来源：http://xhi.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jct.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ita.iojbl.cn

Java: x instanceof Number
来源：http://pbz.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lby.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://whn.uphjek.com

C#:   x is int or double or decimal
来源：http://skf.yvedp.cn

[B14] 判断值是否在集合内
来源：http://djv.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kbf.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://odp.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://rme.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://xcf.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ous.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rkl.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://qxm.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eiy.zhixingplan.top

[B15] 布尔运算与取反
来源：http://mhn.chenlongwang.top

Py:   a and b or not c
来源：http://atm.yfazqb.com

PHP:  $a && $b || !$c
来源：http://upq.jqgufenzy.top

JS:   a && b || !c
来源：http://dbp.daxiang520.top

TS:   a && b || !c
来源：http://ymp.jyoumei.cn

Java: a && b || !c
来源：http://dkw.svipenyu.cn

Go:   a && b || !c
来源：http://zya.hammf.cn

Ruby: a && b || !c
来源：http://iiu.zycfv.cn

C#:   a && b || !c
来源：http://wsk.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hsx.yj202588.top

Py:   if not data: return
来源：http://woi.yj202588.top

PHP:  if (!$data) { return; }
来源：http://gfu.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://doz.xuanzx.com

TS:   if (!data) return;
来源：http://dqv.xylfe.cn

Java: if (data == null) return;
来源：http://wlp.meibo888.top

Go:   if data == nil { return }
来源：http://ndn.yj202588.top

Ruby: return if data.nil?
来源：http://kyb.guannengcc.top

C#:   if (data == null) return;
来源：http://hts.tanke756.top

================================================================================
来源：http://wsc.hesvh.cn

C. 函数与作用域
来源：http://zjc.yj20258888.top

================================================================================
来源：http://cqf.9152youxi.cn

[C01] 定义函数
来源：http://eln.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://xik.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dir.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://tmr.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mii.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eay.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://pwa.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://hon.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hfd.jinqigfzy.top

[C02] 默认参数
来源：http://pxs.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://plb.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vfa.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://gox.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://awz.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://nno.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hqp.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://pkm.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://lua.chenlongwang.top

[C03] 可变参数
来源：http://fja.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://cbq.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ilg.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpb.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dnf.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hzg.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pif.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cvs.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nbt.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://zek.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zwq.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lzt.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ncx.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fqa.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://yso.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://awc.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://jin.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://xbc.nanxuanxn.top

[C05] 返回多个值
来源：http://esj.yangfankeji.com

Py:   return a, b
来源：http://vzh.0kj1m.cn

PHP:  return [$a, $b];
来源：http://iub.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wds.svipenyu.cn

TS:   return { a, b };
来源：http://gmx.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vlz.nanxinkj.top

Go:   return a, b
来源：http://uoc.52xcode.cn

Ruby: return a, b
来源：http://wtv.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://gau.yongpay.top

[C06] 匿名函数 / lambda
来源：http://lvs.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://gbh.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://gfg.haohaochexian.top

JS:   const square = x => x * x;
来源：http://nnd.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://qze.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fpf.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://foy.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://ihm.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://weq.52xcode.cn

[C07] 把函数作为参数传入
来源：http://ety.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hbz.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://byi.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sqr.meibo888.top

TS:   arr.map(String)
来源：http://srk.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jbm.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pmc.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://tyc.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://yvs.ydjk.org.cn

[C08] 闭包
来源：http://gmn.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xmf.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://krq.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkp.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tjd.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rnk.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mjy.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fgc.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tfo.ydzc1.top

[C09] 递归
来源：http://tzf.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wvy.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uot.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fjm.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://faf.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rqf.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cqp.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nza.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nwy.zhongyouzk.top

[C10] 变量作用域
来源：http://rcx.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bbm.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eps.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://grv.316326.xyz

TS:   同 JS
来源：http://amc.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://pcq.fktsv.cn

Go:   花括号块级作用域
来源：http://eou.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iih.daxiang520.top

C#:   块级作用域
来源：http://ilr.jyoumei.cn

[C11] 模块导入与导出
来源：http://hgr.aizwys.cn

Py:   from module import func
来源：http://jlr.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eqo.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://njb.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ylb.cashguo.top

Java: import java.util.List;
来源：http://ihh.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wcq.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://pxw.quarkkingdee.top

C#:   using System.Text;
来源：http://gdl.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://bkp.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://lgy.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://tuy.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://try.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://htv.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://edx.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://evu.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://svt.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vdu.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://url.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://flw.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fgf.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oxc.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exw.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uqo.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://llx.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zbs.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://nkq.gotoacloud.top

[C14] 泛型函数
来源：http://nro.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ohv.zycfv.cn

PHP:  // 无泛型
来源：http://uac.zycfv.cn

JS:   // 无泛型
来源：http://pfl.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eok.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yls.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oib.cheryme.top

Ruby: # 无泛型
来源：http://luw.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bkg.iojbl.cn

[C15] 解构 / 展开参数
来源：http://mvy.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nbi.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://whj.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://odr.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vka.jqgfzy.top

Java: // 无解构
来源：http://pew.yueranfly.top

Go:   // 无解构
来源：http://hnu.fzhhl.top

Ruby: a, b = pair
来源：http://mcf.sysykeji.top

C#:   var (a, b) = pair;
来源：http://sim.sxryk.cn

[C16] 函数 / 方法重载
来源：http://mgw.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sow.yvedp.cn

PHP:  // 无重载
来源：http://flp.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://uow.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://hxo.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tls.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://fyz.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://fnd.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lev.jiagoushi.top

================================================================================
来源：http://yjb.cheryme.top

D. 数组 / 列表 / 集合
来源：http://vov.vqdsnc.cn

================================================================================
来源：http://vsm.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://sen.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hui.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mco.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yeq.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://stf.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wtq.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://gib.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://wri.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://niv.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://czl.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fum.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gjs.fengsongda.top

JS:   arr.push(4);
来源：http://uxp.mhx1999.top

TS:   arr.push(4);
来源：http://jnj.redwolf501.top

Java: list.add(4);
来源：http://bdv.yongpay.top

Go:   arr = append(arr, 4)
来源：http://hwu.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ajc.xziqi.cn

C#:   list.Add(4);
来源：http://phb.hcnkem.com

[D03] 在指定位置插入元素
来源：http://bye.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://neb.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hez.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eru.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://kev.birdmap.top

Java: list.add(0, 0);
来源：http://buk.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://syu.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dwz.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://liw.zhijiandao.cn

[D04] 删除元素
来源：http://ais.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ldm.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ine.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lhy.cheryme.top

TS:   arr.splice(0, 1);
来源：http://hqa.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vaa.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ved.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fhb.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vmm.vqdsnc.cn

[D05] 访问与修改元素
来源：http://vzj.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://too.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tha.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iww.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://sra.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://tqx.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://ahf.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zma.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nrz.52xcode.cn

[D06] 数组长度
来源：http://uab.tanke756.top

Py:   len(arr)
来源：http://okq.cashguo.top

PHP:  count($arr);
来源：http://jcp.jyoumei.cn

JS:   arr.length
来源：http://kni.vqdsnc.cn

TS:   arr.length
来源：http://nvx.aizwys.cn

Java: list.size();
来源：http://hnp.yj20258.top

Go:   len(arr)
来源：http://qcs.bbcook.cn

Ruby: arr.length; arr.size
来源：http://pjb.tanke756.top

C#:   list.Count;
来源：http://ufx.fengsongda.top

[D07] 切片 / 取子数组
来源：http://wbi.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kni.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://prc.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://kou.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://tti.hesvh.cn

Java: list.subList(1, 4);
来源：http://yxr.hfpthk.cn

Go:   arr[1:4]
来源：http://qku.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://nzp.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://eci.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://gpt.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://hjv.pycfn.com

PHP:  array_merge($a, $b);
来源：http://wni.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://wew.cucudq.cn

TS:   [...a, ...b];
来源：http://drc.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://psn.yfazqb.com

Go:   append(a, b...)
来源：http://ieq.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://yxf.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://sse.bjfxy.top

[D09] 排序（升序）
来源：http://xgd.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://brr.52xcode.cn

PHP:  sort($arr);
来源：http://ylv.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://umj.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tqo.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iqo.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tuo.cucudq.cn

Ruby: arr.sort
来源：http://ehi.pycfn.com

C#:   list.Sort();
来源：http://jdb.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://qhn.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bcf.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mmu.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uij.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hjo.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://die.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yjr.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lfi.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mgi.fengsongda.top

[D11] 反转数组
来源：http://jix.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://odd.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://oab.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://noy.chenzaomai.com

TS:   [...arr].reverse();
来源：http://lgn.yuxming.cn

Java: Collections.reverse(list);
来源：http://vtj.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://xml.yuxming.cn

Ruby: arr.reverse
来源：http://meb.fehbvm.com

C#:   list.Reverse();
来源：http://rta.meibo888.top

[D12] 查找元素下标
来源：http://rxq.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://hfq.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rqj.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjf.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vfz.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://omb.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://ovg.daxiang520.top

Ruby: arr.index(x)
来源：http://esh.birdmap.top

C#:   list.IndexOf(x);
来源：http://qax.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://ujn.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qxq.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fnj.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://esf.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://hnq.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vaq.xinyue.icu


<!-- 参考信息 -->