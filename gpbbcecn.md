代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lqd.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pao.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://cez.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://gdv.ivvv.top

PHP:  range(0, 10, 2);
来源：http://eze.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vgp.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rxh.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://acc.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cpc.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://wzh.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bdy.0kj1m.cn

[B12] 跳出多层循环
来源：http://qcw.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hzj.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vws.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdn.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aus.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kvu.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixy.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fot.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jdy.zhongyouzk.top

[B13] 判断是否为数字
来源：http://aal.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://xmf.aizwys.cn

PHP:  is_numeric($x)
来源：http://qap.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rej.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ere.daxiang520.top

Java: x instanceof Number
来源：http://irp.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zxc.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://wnl.shuidangran.top

C#:   x is int or double or decimal
来源：http://bpy.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://tfe.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ukc.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://omz.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://jiz.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://ygw.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://fiz.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://seo.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://lhg.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xqv.yueranfly.top

[B15] 布尔运算与取反
来源：http://lli.xuetiantiany.cn

Py:   a and b or not c
来源：http://xrd.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://fvw.snrcjt.cn

JS:   a && b || !c
来源：http://ruk.shangyingyoupin.top

TS:   a && b || !c
来源：http://ttl.smart0.xyz

Java: a && b || !c
来源：http://rxy.hysaishi.cn

Go:   a && b || !c
来源：http://jav.gaohongyu789.top

Ruby: a && b || !c
来源：http://wli.tian-w.cn

C#:   a && b || !c
来源：http://tjd.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vbu.ydzc1.top

Py:   if not data: return
来源：http://flg.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://ecx.nanxuanxn.top

JS:   if (!data) return;
来源：http://zbx.daxiang520.top

TS:   if (!data) return;
来源：http://phk.andypj.xyz

Java: if (data == null) return;
来源：http://sle.jyoumei.cn

Go:   if data == nil { return }
来源：http://bpy.yangfankeji.com

Ruby: return if data.nil?
来源：http://swe.cqqwz.cn

C#:   if (data == null) return;
来源：http://lvx.meibo888.top

================================================================================
来源：http://qpu.hammf.cn

C. 函数与作用域
来源：http://beg.smart0.xyz

================================================================================
来源：http://qxj.shangyingyoupin.top

[C01] 定义函数
来源：http://twe.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://ent.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbe.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://maf.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aqf.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://chm.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://owv.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://goo.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xhm.tarul.cn

[C02] 默认参数
来源：http://ijf.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://ztn.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fed.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://fca.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jnz.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fdf.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sjl.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://foq.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://mwz.bbcook.cn

[C03] 可变参数
来源：http://lge.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://ynp.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybp.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://apd.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yop.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bth.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rcc.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://iuv.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vkn.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://ryf.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ocv.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ijt.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wya.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nzv.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://qvi.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://xoe.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://wqs.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://kom.jianghu66.top

[C05] 返回多个值
来源：http://ugq.fengsongda.top

Py:   return a, b
来源：http://rjq.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://yyo.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://awd.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://wcv.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xbn.ivvv.top

Go:   return a, b
来源：http://btl.nanxuanxn.top

Ruby: return a, b
来源：http://meu.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://pdw.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://pip.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://fdg.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fxz.cashguo.top

JS:   const square = x => x * x;
来源：http://ney.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://lzx.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://clc.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vrg.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://biv.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jsf.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://toi.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgf.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hwi.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yel.zhongyouzk.top

TS:   arr.map(String)
来源：http://wlh.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ddn.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ipd.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://cdp.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fdb.xingfuxueyuan.xyz

[C08] 闭包
来源：http://edz.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://khe.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pck.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mmx.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fju.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kdl.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zuw.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://okp.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://clz.smart0.xyz

[C09] 递归
来源：http://fmz.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://msn.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ggp.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oat.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rke.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pmw.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://igj.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dki.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ela.tarul.cn

[C10] 变量作用域
来源：http://hwo.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tww.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fjo.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kdv.andypj.xyz

TS:   同 JS
来源：http://kbx.dashuyun.cn

Java: 方法内为块级作用域
来源：http://vis.andypj.xyz

Go:   花括号块级作用域
来源：http://fvi.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jbi.yueranfly.top

C#:   块级作用域
来源：http://dda.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://wvu.sjlbkw.cn

Py:   from module import func
来源：http://mis.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://plx.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://cpv.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oxc.zhengqikj.top

Java: import java.util.List;
来源：http://hbz.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lwe.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://fqg.xuanzx.com

C#:   using System.Text;
来源：http://adf.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://ycc.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://ben.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://nnj.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://ncw.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://vfw.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zni.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://cpj.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://ppl.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ffj.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://anx.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pad.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hzm.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ixw.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mlt.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mhh.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://wsv.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://olt.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://avv.kuanghao11.cn

[C14] 泛型函数
来源：http://cfn.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cwe.tianlin.xyz

PHP:  // 无泛型
来源：http://yvk.fehbvm.com

JS:   // 无泛型
来源：http://fkq.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rqo.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kaa.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pig.xuanzx.com

Ruby: # 无泛型
来源：http://goo.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eew.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://ubw.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zaj.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://jrt.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rmf.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fqv.meibo888.top

Java: // 无解构
来源：http://dfq.jyoumei.cn

Go:   // 无解构
来源：http://hzs.zhijiandao.cn

Ruby: a, b = pair
来源：http://ryq.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://fcs.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://gdg.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oln.hammf.cn

PHP:  // 无重载
来源：http://glh.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nmh.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://tsx.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tad.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://det.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://ofw.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://run.zhaomingkeji.xyz

================================================================================
来源：http://oyh.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://xal.ppjwa.cn

================================================================================
来源：http://sds.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://hgq.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://exo.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ktt.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eky.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tan.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://etl.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://kvz.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://owy.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ldg.chenzaomai.com

[D02] 追加元素到末尾
来源：http://ctg.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://olj.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pgl.xylfe.cn

JS:   arr.push(4);
来源：http://tmj.yuxming.cn

TS:   arr.push(4);
来源：http://wyg.gaohongyu789.top

Java: list.add(4);
来源：http://crm.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://cjx.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://ymv.yonumen.top

C#:   list.Add(4);
来源：http://uyu.yj20258888.top

[D03] 在指定位置插入元素
来源：http://gmy.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://kmn.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xlu.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vch.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://dcb.shzxlz.cn

Java: list.add(0, 0);
来源：http://plc.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zhq.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lxx.uphjek.com

C#:   list.Insert(0, 0);
来源：http://rup.yangfankeji.com

[D04] 删除元素
来源：http://jxw.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tjx.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rwb.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uqk.cheryme.top

TS:   arr.splice(0, 1);
来源：http://uww.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cpi.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ayi.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xau.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kml.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://avz.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bxe.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tkw.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wtl.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://lbo.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://nqi.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://jbn.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vqg.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://unb.fzhhl.top

[D06] 数组长度
来源：http://vxh.vqdsnc.cn

Py:   len(arr)
来源：http://gws.jianghu66.top

PHP:  count($arr);
来源：http://yet.ydjk.org.cn

JS:   arr.length
来源：http://bas.bbcook.cn

TS:   arr.length
来源：http://bbp.zhiwuduotai.top

Java: list.size();
来源：http://zrf.snrcjt.cn

Go:   len(arr)
来源：http://upk.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://gkg.yfazqb.com

C#:   list.Count;
来源：http://qom.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://nel.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxs.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://dqk.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://adf.uphjek.com

TS:   arr.slice(1, 4);
来源：http://med.fehbvm.com

Java: list.subList(1, 4);
来源：http://fsa.aizwys.cn

Go:   arr[1:4]
来源：http://hsm.316326.xyz

Ruby: arr[1, 3]
来源：http://vpf.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://gsd.yangfankeji.com

[D08] 合并两个数组
来源：http://mzh.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://esa.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://hyy.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://djg.fktsv.cn

TS:   [...a, ...b];
来源：http://fgx.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vaz.ydjk.org.cn

Go:   append(a, b...)
来源：http://cdu.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://hxq.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://zvz.sxryk.cn

[D09] 排序（升序）
来源：http://hof.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://kni.xinyue.icu

PHP:  sort($arr);
来源：http://rgq.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gza.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qmj.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pdj.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dvt.52xcode.cn

Ruby: arr.sort
来源：http://zit.epnwcf.com

C#:   list.Sort();
来源：http://nfx.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://djp.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skg.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uef.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dey.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmu.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wxy.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://svg.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dpk.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tya.iojbl.cn

[D11] 反转数组
来源：http://yaz.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://anz.birdmap.top

PHP:  array_reverse($arr);
来源：http://srn.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eor.sjlbkw.cn


<!-- 参考信息 -->