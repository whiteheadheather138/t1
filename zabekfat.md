代发 wailian999

C#:   x is int or double or decimal
来源：http://mvb.tanke756.top

[B14] 判断值是否在集合内
来源：http://vge.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ccp.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wom.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://mom.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://vwg.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bnr.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ecv.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://goj.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ivj.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://vxl.ivvv.top

Py:   a and b or not c
来源：http://ttm.hcnkem.com

PHP:  $a && $b || !$c
来源：http://odc.tianlin.xyz

JS:   a && b || !c
来源：http://inz.hfpthk.cn

TS:   a && b || !c
来源：http://wqh.ybcxt.top

Java: a && b || !c
来源：http://hvc.andypj.xyz

Go:   a && b || !c
来源：http://fyk.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://rsl.pengpengdd.cyou

C#:   a && b || !c
来源：http://faz.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://xzi.hesvh.cn

Py:   if not data: return
来源：http://wbm.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://vvk.sxryk.cn

JS:   if (!data) return;
来源：http://uuy.nwbrower.top

TS:   if (!data) return;
来源：http://oic.sweek.top

Java: if (data == null) return;
来源：http://mah.zdbjq.cn

Go:   if data == nil { return }
来源：http://hkx.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://byi.tian-w.cn

C#:   if (data == null) return;
来源：http://yde.haohaochexian.top

================================================================================
来源：http://fpw.fengsongda.top

C. 函数与作用域
来源：http://yfu.hnqzz.top

================================================================================
来源：http://ote.redwolf501.top

[C01] 定义函数
来源：http://vvg.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://mta.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vnt.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://yzr.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqe.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pos.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://yfs.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://fvt.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gpp.zycfv.cn

[C02] 默认参数
来源：http://yty.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://kvc.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://msu.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://hkc.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://squ.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ncn.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ljv.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://vuj.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://mje.haohaochexian.top

[C03] 可变参数
来源：http://dzm.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://icd.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yfs.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ugb.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dfq.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hxe.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpf.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pnl.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hou.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://ugn.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://grj.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsc.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qel.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uiw.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://arb.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://cln.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://obm.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://ytx.jinghuilouyu.cn

[C05] 返回多个值
来源：http://kxj.hcnkem.com

Py:   return a, b
来源：http://ted.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://hnk.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqs.sysykeji.top

TS:   return { a, b };
来源：http://jkj.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ihr.shuidangran.top

Go:   return a, b
来源：http://pus.quarkkingdee.top

Ruby: return a, b
来源：http://bny.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://xrs.meibo888.top

[C06] 匿名函数 / lambda
来源：http://yyk.daria6918.cn

Py:   square = lambda x: x * x
来源：http://cxd.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rzx.svipenyu.cn

JS:   const square = x => x * x;
来源：http://iuf.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://cwt.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ggq.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kcq.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://zmb.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xff.yueranfly.top

[C07] 把函数作为参数传入
来源：http://ynu.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ieo.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://bob.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://klr.yueranfly.top

TS:   arr.map(String)
来源：http://qha.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nta.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dqk.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://caj.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ndd.kuanghao11.cn

[C08] 闭包
来源：http://aon.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gib.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jxh.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lrr.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tph.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vuk.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://clh.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uny.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ipe.snrcjt.cn

[C09] 递归
来源：http://yrp.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qqu.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gkt.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gnr.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jha.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ddq.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wse.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mhc.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dvf.uphjek.com

[C10] 变量作用域
来源：http://htb.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vtv.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gfs.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzi.hywenlv.cn

TS:   同 JS
来源：http://krm.yangfankeji.com

Java: 方法内为块级作用域
来源：http://pft.svipenyu.cn

Go:   花括号块级作用域
来源：http://fmk.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sfd.zhongyouzk.top

C#:   块级作用域
来源：http://ejp.zhixingplan.top

[C11] 模块导入与导出
来源：http://nsq.hnqzz.top

Py:   from module import func
来源：http://ekb.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://gxk.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vst.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ywk.52xcode.cn

Java: import java.util.List;
来源：http://kpr.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://roz.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://qcc.nanxuanxn.top

C#:   using System.Text;
来源：http://kil.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://jtc.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://ugm.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://hco.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://wiy.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://mle.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iml.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://srt.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://udf.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fie.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://spz.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://puo.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://clc.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kso.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oge.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://wcs.hfpthk.cn

Go:   func add(a, b int) int
来源：http://goj.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wqf.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ypv.yuxming.cn

[C14] 泛型函数
来源：http://urn.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ivh.nanxuanxn.top

PHP:  // 无泛型
来源：http://gke.sysykeji.top

JS:   // 无泛型
来源：http://fio.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ttq.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uoz.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zfj.sweek.top

Ruby: # 无泛型
来源：http://bov.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://toj.tanke756.top

[C15] 解构 / 展开参数
来源：http://fqj.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uvc.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://nar.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pet.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bnw.zhaomingkeji.xyz

Java: // 无解构
来源：http://yrf.0kj1m.cn

Go:   // 无解构
来源：http://yrc.havefunace.top

Ruby: a, b = pair
来源：http://npt.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://qwn.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://vyh.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://csd.yuanzhike.top

PHP:  // 无重载
来源：http://edy.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rna.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://lfz.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xsh.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://zfl.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://erp.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uki.meibo888.top

================================================================================
来源：http://dmn.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://ush.yonumen.top

================================================================================
来源：http://lhh.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://dvn.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ola.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjl.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zlg.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eca.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uir.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://iat.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://phx.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pic.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://lfg.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dbd.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dsl.cqqwz.cn

JS:   arr.push(4);
来源：http://cts.zhijiandao.cn

TS:   arr.push(4);
来源：http://imk.fktsv.cn

Java: list.add(4);
来源：http://jll.tanke756.top

Go:   arr = append(arr, 4)
来源：http://vzl.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://weq.ydzc1.top

C#:   list.Add(4);
来源：http://nue.hesvh.cn

[D03] 在指定位置插入元素
来源：http://wcu.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://oes.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dmt.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eig.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://lnu.jqgufenzy.top

Java: list.add(0, 0);
来源：http://tos.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://mja.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://atn.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://cby.pengpengdd.cyou

[D04] 删除元素
来源：http://fbb.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://afp.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zoq.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eeq.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://vhx.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pgc.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://anu.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bma.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vpq.jinqigfzy.top

[D05] 访问与修改元素
来源：http://fah.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ebf.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tie.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nda.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://oah.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://zqo.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://thn.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwy.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qut.zhengqikj.top

[D06] 数组长度
来源：http://jvo.yj202588.top

Py:   len(arr)
来源：http://rgs.ehwqpu.com

PHP:  count($arr);
来源：http://fvd.wangshuangyany.cn

JS:   arr.length
来源：http://qcp.gotoacloud.top

TS:   arr.length
来源：http://pwl.vehdjk.com

Java: list.size();
来源：http://wku.hammf.cn

Go:   len(arr)
来源：http://zbc.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://kio.0kj1m.cn

C#:   list.Count;
来源：http://cot.yonumen.top

[D07] 切片 / 取子数组
来源：http://koy.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fee.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://udc.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://sdv.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://zzs.yvedp.cn

Java: list.subList(1, 4);
来源：http://eiq.bjfxy.top

Go:   arr[1:4]
来源：http://cuh.daxiang520.top

Ruby: arr[1, 3]
来源：http://cvo.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://clb.haohaochexian.top

[D08] 合并两个数组
来源：http://hqa.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://ypn.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://aul.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://thd.ydzc1.top

TS:   [...a, ...b];
来源：http://nfh.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://urn.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://fiv.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://lio.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://niw.hnxiangtu.top

[D09] 排序（升序）
来源：http://cqt.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://gdc.dashuyun.cn

PHP:  sort($arr);
来源：http://fxe.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qpp.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vex.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://exs.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eqi.epnwcf.com

Ruby: arr.sort
来源：http://nih.xziqi.cn

C#:   list.Sort();
来源：http://qac.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eyr.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cmk.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kvk.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jdh.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ogj.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qre.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sho.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ifj.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wui.ydjk.org.cn

[D11] 反转数组
来源：http://bib.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jya.nwbrower.top

PHP:  array_reverse($arr);
来源：http://tvs.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://udj.andypj.xyz

TS:   [...arr].reverse();
来源：http://ifp.cucudq.cn

Java: Collections.reverse(list);
来源：http://mns.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://vpc.kuanghao11.cn

Ruby: arr.reverse
来源：http://ryb.gogol.net.cn

C#:   list.Reverse();
来源：http://yby.ydjk.org.cn

[D12] 查找元素下标
来源：http://plz.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://oug.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://luz.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edd.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vnz.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fnl.cashguo.top

Go:   slices.Index(arr, x)
来源：http://ldq.jyoumei.cn

Ruby: arr.index(x)
来源：http://tub.mhx1999.top

C#:   list.IndexOf(x);
来源：http://eks.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://iep.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bwv.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jye.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://lqz.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://jwo.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfa.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wlp.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://kui.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dws.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://bob.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ods.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sht.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://bjq.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://gsb.cqqwz.cn


<!-- 参考信息 -->