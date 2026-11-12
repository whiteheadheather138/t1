代发 wailian999

C#:   x is int or double or decimal
来源：http://lbo.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://sef.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rvr.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xkv.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://bid.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://lup.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uym.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://swg.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://wne.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cii.tianlin.xyz

[B15] 布尔运算与取反
来源：http://kuo.tanke756.top

Py:   a and b or not c
来源：http://ysh.smart0.xyz

PHP:  $a && $b || !$c
来源：http://aiq.ctjpmb.com

JS:   a && b || !c
来源：http://ver.cashguo.top

TS:   a && b || !c
来源：http://bau.jlsjyb.cn

Java: a && b || !c
来源：http://xuw.316326.xyz

Go:   a && b || !c
来源：http://phz.9152youxi.cn

Ruby: a && b || !c
来源：http://vbg.fanxiaobao.xyz

C#:   a && b || !c
来源：http://jen.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://tpg.gogol.net.cn

Py:   if not data: return
来源：http://nkp.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://zvz.52xcode.cn

JS:   if (!data) return;
来源：http://ahd.zhixingplan.top

TS:   if (!data) return;
来源：http://qzp.tianlin.xyz

Java: if (data == null) return;
来源：http://rxx.shuidangran.top

Go:   if data == nil { return }
来源：http://pev.fktsv.cn

Ruby: return if data.nil?
来源：http://nzh.yonumen.top

C#:   if (data == null) return;
来源：http://ekg.svipenyu.cn

================================================================================
来源：http://ytn.zycfv.cn

C. 函数与作用域
来源：http://bsn.shuidangran.top

================================================================================
来源：http://gas.xuanzx.com

[C01] 定义函数
来源：http://yfk.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://xui.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fet.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://xbd.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osp.52xcode.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tbj.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://ohy.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://kdz.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uza.yonumen.top

[C02] 默认参数
来源：http://ihh.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://udd.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ffm.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://wvv.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://axj.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oaf.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://leh.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://lhs.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://djo.kuanghao11.cn

[C03] 可变参数
来源：http://onm.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://fhz.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hma.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iyq.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzl.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tuw.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ryk.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yuk.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyj.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://qxj.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kln.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mur.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wzk.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dej.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://jnq.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://lbu.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://gzh.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://ixz.ydjk.org.cn

[C05] 返回多个值
来源：http://ezg.zhixingplan.top

Py:   return a, b
来源：http://ong.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://edn.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://psk.zhoulong.xyz

TS:   return { a, b };
来源：http://sgr.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wdg.dashuyun.cn

Go:   return a, b
来源：http://iep.iojbl.cn

Ruby: return a, b
来源：http://ztv.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://wgb.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://qqy.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://atg.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nue.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://zzj.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://jyb.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://goa.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://rtf.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://ahe.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://rmc.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://oqu.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nxg.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oml.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwa.jinqigufen.top

TS:   arr.map(String)
来源：http://klu.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://utv.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kkf.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://gim.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nfh.ctjpmb.com

[C08] 闭包
来源：http://ogq.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vfd.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zwy.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xmw.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jpx.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jwo.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nmo.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xog.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tpl.chenlongwang.top

[C09] 递归
来源：http://nfw.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vau.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rqz.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epr.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://poj.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ils.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cht.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gby.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qlc.pycfn.com

[C10] 变量作用域
来源：http://yjw.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://trp.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gyl.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hzy.aizwys.cn

TS:   同 JS
来源：http://frq.bbcook.cn

Java: 方法内为块级作用域
来源：http://hdr.gogol.net.cn

Go:   花括号块级作用域
来源：http://vmg.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxt.52xcode.cn

C#:   块级作用域
来源：http://oix.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://yhy.jinyuanbaomall.cn

Py:   from module import func
来源：http://ceg.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rfq.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fci.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ohs.hammf.cn

Java: import java.util.List;
来源：http://xwv.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfw.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://jsq.bjfxy.top

C#:   using System.Text;
来源：http://fqx.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://mww.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://act.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://uas.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://ahf.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://nhj.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qmg.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://mvv.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://pgh.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hcd.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://csf.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rgu.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jrw.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hnz.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgu.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rpk.xylfe.cn

Go:   func add(a, b int) int
来源：http://mbf.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eka.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://gcp.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://wrv.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tzz.guannengcc.top

PHP:  // 无泛型
来源：http://wgt.ctjpmb.com

JS:   // 无泛型
来源：http://tmg.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://amj.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nwy.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kbo.nanxuanxn.top

Ruby: # 无泛型
来源：http://csc.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ccf.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://rif.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpo.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://fdr.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uwr.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tct.hysaishi.cn

Java: // 无解构
来源：http://zyq.yonumen.top

Go:   // 无解构
来源：http://utr.chenjidiqi.icu

Ruby: a, b = pair
来源：http://aef.andypj.xyz

C#:   var (a, b) = pair;
来源：http://wmq.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://gyn.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bch.yongpay.top

PHP:  // 无重载
来源：http://dta.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ujn.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://oho.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vqm.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://ovz.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://ncw.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://kix.gaohongyu789.top

================================================================================
来源：http://hfp.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://xjv.gogol.net.cn

================================================================================
来源：http://duh.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://jhh.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://san.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dpu.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vdk.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jwd.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nen.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://oxe.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://ves.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xoj.guannengcc.top

[D02] 追加元素到末尾
来源：http://jed.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://thf.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://umx.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://rqo.zhixingplan.top

TS:   arr.push(4);
来源：http://rdh.uphjek.com

Java: list.add(4);
来源：http://lyo.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://bpt.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://ewc.316326.xyz

C#:   list.Add(4);
来源：http://dkn.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://bak.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://clx.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qtr.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfz.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://cnq.jinqigufen.top

Java: list.add(0, 0);
来源：http://oaf.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://rqd.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kyy.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://jqo.hcnkem.com

[D04] 删除元素
来源：http://thx.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mio.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uln.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nhq.meibo888.top

TS:   arr.splice(0, 1);
来源：http://boc.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bmq.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pvw.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bqe.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iex.ydjk.org.cn

[D05] 访问与修改元素
来源：http://gus.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://acu.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eke.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lxp.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://ixi.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://fcf.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://vpn.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://our.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vbs.pycfn.com

[D06] 数组长度
来源：http://apl.guowangkeji.top

Py:   len(arr)
来源：http://qld.sysykeji.top

PHP:  count($arr);
来源：http://qer.tianlin.xyz

JS:   arr.length
来源：http://zxg.sxryk.cn

TS:   arr.length
来源：http://qhl.xuanzx.com

Java: list.size();
来源：http://mgt.vehdjk.com

Go:   len(arr)
来源：http://plc.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://tem.jyoumei.cn

C#:   list.Count;
来源：http://wmp.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://jxm.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mqu.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://itl.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://rcg.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://ekj.cucudq.cn

Java: list.subList(1, 4);
来源：http://pnt.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://cmh.hfpthk.cn

Ruby: arr[1, 3]
来源：http://nxo.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://sjw.gogol.net.cn

[D08] 合并两个数组
来源：http://wic.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://jzu.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://mzv.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cws.fzhhl.top

TS:   [...a, ...b];
来源：http://yqd.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xlj.yuanzhike.top

Go:   append(a, b...)
来源：http://gee.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://auf.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://vcq.aibaodan.cn

[D09] 排序（升序）
来源：http://brr.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://iam.tanke756.top

PHP:  sort($arr);
来源：http://xtw.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uou.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://euq.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mhl.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xbp.meibo888.top

Ruby: arr.sort
来源：http://yck.gzhubu.top

C#:   list.Sort();
来源：http://czf.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rth.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fqc.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qoq.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qww.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://asd.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yfn.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://krg.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ock.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://som.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://ccc.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://vnz.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://eop.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zto.fktsv.cn

TS:   [...arr].reverse();
来源：http://ldf.dashuyun.cn

Java: Collections.reverse(list);
来源：http://ckc.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://rxn.daria6918.cn

Ruby: arr.reverse
来源：http://imh.bjfxy.top

C#:   list.Reverse();
来源：http://nja.dashuyun.cn

[D12] 查找元素下标
来源：http://lpo.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://ucr.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dxe.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikm.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yoi.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cee.316326.xyz

Go:   slices.Index(arr, x)
来源：http://tuu.zhoulong.xyz

Ruby: arr.index(x)
来源：http://hyv.bbcook.cn

C#:   list.IndexOf(x);
来源：http://bng.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://squ.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qbb.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wrc.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://ukc.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://ekj.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uad.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nah.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://ntr.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nfa.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://rwr.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hoo.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xga.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://wym.jqgufenzy.top

TS:   arr.map(x => x * 2)
来源：http://pfv.zhixingplan.top


<!-- 参考信息 -->