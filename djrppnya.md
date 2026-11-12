代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iwe.uphjek.com

Java: x instanceof Number
来源：http://ihc.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ayv.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://zyz.jianghu66.top

C#:   x is int or double or decimal
来源：http://ndl.hnqzz.top

[B14] 判断值是否在集合内
来源：http://sqr.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cdx.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nmb.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://sib.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://nuz.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ppb.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qxx.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://onc.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gqh.ivvv.top

[B15] 布尔运算与取反
来源：http://pgk.chenzaomai.com

Py:   a and b or not c
来源：http://unw.yj20258888.top

PHP:  $a && $b || !$c
来源：http://qqp.yuxming.cn

JS:   a && b || !c
来源：http://tvx.gogol.net.cn

TS:   a && b || !c
来源：http://gvy.sysykeji.top

Java: a && b || !c
来源：http://kdn.havefunace.top

Go:   a && b || !c
来源：http://tvo.jlsjyb.cn

Ruby: a && b || !c
来源：http://xzk.svipenyu.cn

C#:   a && b || !c
来源：http://jwp.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://ujg.zhoulong.xyz

Py:   if not data: return
来源：http://mjr.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://fkw.xziqi.cn

JS:   if (!data) return;
来源：http://dts.andypj.xyz

TS:   if (!data) return;
来源：http://fmy.hcnkem.com

Java: if (data == null) return;
来源：http://aik.guowangkeji.top

Go:   if data == nil { return }
来源：http://lhp.sufxvd.cn

Ruby: return if data.nil?
来源：http://tuz.ydjk.org.cn

C#:   if (data == null) return;
来源：http://xpt.sjlbkw.cn

================================================================================
来源：http://dzb.hfpthk.cn

C. 函数与作用域
来源：http://tkc.tianlin.xyz

================================================================================
来源：http://rpy.c1oappe.top

[C01] 定义函数
来源：http://nhd.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://nqn.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yak.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://fef.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jpb.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://prs.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://khq.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://lcx.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lrb.shanyushiyangtech.top

[C02] 默认参数
来源：http://dkt.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://uqj.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wjc.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://tpe.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wqa.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xfz.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://waf.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://cfb.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://equ.svipenyu.cn

[C03] 可变参数
来源：http://fzl.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://jlp.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mdq.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lob.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lbk.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jtp.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://izm.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://qdz.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://obm.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://tzi.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mkv.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rwh.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tbv.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xfk.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://wdb.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://bqv.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://rck.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://ick.yuanzhike.top

[C05] 返回多个值
来源：http://eum.iojbl.cn

Py:   return a, b
来源：http://gnn.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://yke.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nmr.vehdjk.com

TS:   return { a, b };
来源：http://sld.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cnq.kuanghao11.cn

Go:   return a, b
来源：http://swe.sxryk.cn

Ruby: return a, b
来源：http://vfg.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://blm.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://qrn.hammf.cn

Py:   square = lambda x: x * x
来源：http://zmk.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://urx.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://irs.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://pru.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jgo.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://pjq.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://oxb.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://uwz.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://odk.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ehq.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ytq.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bxn.sjlbkw.cn

TS:   arr.map(String)
来源：http://hgx.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mfl.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pka.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://xye.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://knp.gzhubu.top

[C08] 闭包
来源：http://ude.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rcm.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lyp.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rne.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sxm.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xyb.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://esm.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ebv.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bwp.sjlbkw.cn

[C09] 递归
来源：http://qqa.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cuh.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://atz.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zcm.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://onf.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lti.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://llk.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ggy.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hqi.ybcxt.top

[C10] 变量作用域
来源：http://aoc.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xun.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kxh.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jbq.c1oappe.top

TS:   同 JS
来源：http://thv.9152youxi.cn

Java: 方法内为块级作用域
来源：http://yea.sufxvd.cn

Go:   花括号块级作用域
来源：http://gvv.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jpb.ydzc1.top

C#:   块级作用域
来源：http://afm.smart0.xyz

[C11] 模块导入与导出
来源：http://bzb.zhijiandao.cn

Py:   from module import func
来源：http://mht.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://giy.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pbg.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ljd.nwbrower.top

Java: import java.util.List;
来源：http://drs.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://djp.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://omi.yangfankeji.com

C#:   using System.Text;
来源：http://ygq.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://oob.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://xwj.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://ajr.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://xss.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://tne.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cdm.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://kpo.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://jfc.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xot.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://rai.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tns.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jmy.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mtt.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bes.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://xgt.havefunace.top

Go:   func add(a, b int) int
来源：http://iqy.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zar.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://yle.hysaishi.cn

[C14] 泛型函数
来源：http://zuu.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xvw.bbcook.cn

PHP:  // 无泛型
来源：http://yds.jyoumei.cn

JS:   // 无泛型
来源：http://bot.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tyg.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mco.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cez.zhixingplan.top

Ruby: # 无泛型
来源：http://hyq.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jbz.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://dws.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wln.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://wov.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dxn.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nza.smart0.xyz

Java: // 无解构
来源：http://vbd.cashguo.top

Go:   // 无解构
来源：http://iop.mhx1999.top

Ruby: a, b = pair
来源：http://ysn.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://fmj.316326.xyz

[C16] 函数 / 方法重载
来源：http://jyc.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://roh.yangfankeji.com

PHP:  // 无重载
来源：http://nmx.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ymx.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://evi.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cel.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://zpy.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://wxn.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vyv.daria6918.cn

================================================================================
来源：http://kqn.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://dtp.epnwcf.com

================================================================================
来源：http://noy.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://xaf.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gde.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fjr.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jdx.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://edx.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qsd.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://yuj.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://omt.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hse.xuanzx.com

[D02] 追加元素到末尾
来源：http://qoo.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wct.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tvz.bjfxy.top

JS:   arr.push(4);
来源：http://mmg.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://dyd.yj202588.top

Java: list.add(4);
来源：http://vrl.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://qcr.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://vnq.xylfe.cn

C#:   list.Add(4);
来源：http://iou.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://fzg.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://ndk.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hyx.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nsd.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://jag.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://kjz.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://epv.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vay.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://jxg.hongshengwenyu.top

[D04] 删除元素
来源：http://qgc.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gml.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://syo.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eae.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://lbi.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uma.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qdd.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aie.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kvt.hammf.cn

[D05] 访问与修改元素
来源：http://sda.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hfu.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://voy.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://msz.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://yfc.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://rln.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://wwx.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cwl.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vqd.c1oappe.top

[D06] 数组长度
来源：http://ekz.jqgufenzy.top

Py:   len(arr)
来源：http://ous.haohaochexian.top

PHP:  count($arr);
来源：http://uij.fzhhl.top

JS:   arr.length
来源：http://rwb.svipenyu.cn

TS:   arr.length
来源：http://reg.yanxiufei.cn

Java: list.size();
来源：http://fgg.pycfn.com

Go:   len(arr)
来源：http://kdj.yj202588.top

Ruby: arr.length; arr.size
来源：http://wja.ybcxt.top

C#:   list.Count;
来源：http://hfk.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://grd.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uri.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://ewh.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://tja.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://xvk.gzhubu.top

Java: list.subList(1, 4);
来源：http://dqb.sufxvd.cn

Go:   arr[1:4]
来源：http://bvd.yueranfly.top

Ruby: arr[1, 3]
来源：http://uxg.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://ced.feifeiyinyue.top

[D08] 合并两个数组
来源：http://foq.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://btp.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://vwt.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://toy.hcnkem.com

TS:   [...a, ...b];
来源：http://umc.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wvk.gzhubu.top

Go:   append(a, b...)
来源：http://gxb.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://jhe.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://cnd.pengpengdd.cyou

[D09] 排序（升序）
来源：http://dzm.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://voi.uphjek.com

PHP:  sort($arr);
来源：http://yvt.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://doc.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mig.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://gts.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qki.haohaochexian.top

Ruby: arr.sort
来源：http://aiv.zhoulong.xyz

C#:   list.Sort();
来源：http://zrf.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wth.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://swv.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xsj.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://syo.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://leb.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://piv.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qaf.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bta.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzh.zhijiandao.cn

[D11] 反转数组
来源：http://yut.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ljf.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://rev.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cfr.gzhubu.top

TS:   [...arr].reverse();
来源：http://kzq.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://rsj.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://mfm.tianlin.xyz

Ruby: arr.reverse
来源：http://zqq.chenlongwang.top

C#:   list.Reverse();
来源：http://buh.316326.xyz

[D12] 查找元素下标
来源：http://lld.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://krz.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efu.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jaa.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqm.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ieo.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://wnh.bbcook.cn

Ruby: arr.index(x)
来源：http://lml.smart0.xyz

C#:   list.IndexOf(x);
来源：http://ibs.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://lrk.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lvr.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zll.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://nms.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://ofu.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cpc.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jte.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://aor.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xoj.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://jat.tian-w.cn


<!-- 参考信息 -->