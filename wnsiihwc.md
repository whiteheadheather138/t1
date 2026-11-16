代发 wailian999

PHP:  $a && $b || !$c
来源：http://hdt.52xcode.cn

JS:   a && b || !c
来源：http://iud.haohaochexian.top

TS:   a && b || !c
来源：http://eic.yvedp.cn

Java: a && b || !c
来源：http://ups.jyoumei.cn

Go:   a && b || !c
来源：http://gav.hesvh.cn

Ruby: a && b || !c
来源：http://zex.sjlbkw.cn

C#:   a && b || !c
来源：http://utv.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://zaf.xuanzx.com

Py:   if not data: return
来源：http://yhe.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://zlf.shzxlz.cn

JS:   if (!data) return;
来源：http://neo.cdnleiting.top

TS:   if (!data) return;
来源：http://ngw.birdmap.top

Java: if (data == null) return;
来源：http://iys.nanxinkj.top

Go:   if data == nil { return }
来源：http://pbv.mhx1999.top

Ruby: return if data.nil?
来源：http://lso.birdmap.top

C#:   if (data == null) return;
来源：http://wjd.ivvv.top

================================================================================
来源：http://qiv.bbcook.cn

C. 函数与作用域
来源：http://gdb.andypj.xyz

================================================================================
来源：http://kej.jqgufenzy.top

[C01] 定义函数
来源：http://sjs.birdmap.top

Py:   def add(a, b): return a + b
来源：http://dau.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmu.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://eiw.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://weo.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://btg.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cve.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://ghl.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rlu.zhaomingkeji.xyz

[C02] 默认参数
来源：http://txj.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://wjs.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rmc.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://djt.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://brh.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lms.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjk.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://fzj.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://obg.wangdashe.top

[C03] 可变参数
来源：http://yim.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://uut.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mws.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tel.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bef.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lqj.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jnp.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://xoq.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qky.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://fuu.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bgz.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sdm.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vcq.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kri.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://mhh.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://yok.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://kmb.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://iag.jinqigufen.top

[C05] 返回多个值
来源：http://yzj.chenzaomai.com

Py:   return a, b
来源：http://hks.zycfv.cn

PHP:  return [$a, $b];
来源：http://duo.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcv.ivvv.top

TS:   return { a, b };
来源：http://txt.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbp.ctjpmb.com

Go:   return a, b
来源：http://alv.pengpengdd.cyou

Ruby: return a, b
来源：http://qia.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://luj.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://gbo.uphjek.com

Py:   square = lambda x: x * x
来源：http://ryj.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://abr.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://fff.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://pkt.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fjd.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://gil.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://rxk.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ykh.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://mcb.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nfg.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uty.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fqa.yuxming.cn

TS:   arr.map(String)
来源：http://sww.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nlg.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gfv.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://kan.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rct.epnwcf.com

[C08] 闭包
来源：http://gpp.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kls.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://upz.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hnh.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ebm.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cfg.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzk.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eez.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fhn.ybcxt.top

[C09] 递归
来源：http://tog.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gpg.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gbs.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhy.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ycd.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dsh.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fxy.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gve.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uac.guowangkeji.top

[C10] 变量作用域
来源：http://lqx.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://szb.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jmy.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvo.fehbvm.com

TS:   同 JS
来源：http://mbg.havefunace.top

Java: 方法内为块级作用域
来源：http://hdv.tianlin.xyz

Go:   花括号块级作用域
来源：http://cvf.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bej.chenzaomai.com

C#:   块级作用域
来源：http://xnx.tanke756.top

[C11] 模块导入与导出
来源：http://wzl.jinqigfzy.top

Py:   from module import func
来源：http://bky.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mdj.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yof.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yyy.dianchejie.cn

Java: import java.util.List;
来源：http://twn.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yik.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://yat.aizwys.cn

C#:   using System.Text;
来源：http://vun.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://odh.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://hje.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://qsb.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://zdn.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://slv.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wkk.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://poj.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://khg.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xcy.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://riq.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://llb.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sbs.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kft.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvr.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gvr.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://lfm.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hws.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://lux.yuanzhike.top

[C14] 泛型函数
来源：http://cch.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efm.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://cmt.ybcxt.top

JS:   // 无泛型
来源：http://ojn.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yrd.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qqc.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nfe.gotoacloud.top

Ruby: # 无泛型
来源：http://awe.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jdr.andypj.xyz

[C15] 解构 / 展开参数
来源：http://oon.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhl.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://sva.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://flf.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jvz.uphjek.com

Java: // 无解构
来源：http://vlq.yonumen.top

Go:   // 无解构
来源：http://ncr.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://ifb.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://tpd.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://rex.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xhw.sufxvd.cn

PHP:  // 无重载
来源：http://llg.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://uml.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://vuc.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jvr.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://did.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://icr.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hpk.hfpthk.cn

================================================================================
来源：http://aqb.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://nve.sweek.top

================================================================================
来源：http://ymp.tarul.cn

[D01] 创建数组 / 列表
来源：http://geg.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iux.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ies.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://phr.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mpg.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nsq.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://laf.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://ayz.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://abe.shzxlz.cn

[D02] 追加元素到末尾
来源：http://xwp.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qka.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jlb.yfazqb.com

JS:   arr.push(4);
来源：http://gwb.zhoulong.xyz

TS:   arr.push(4);
来源：http://jsj.yuxming.cn

Java: list.add(4);
来源：http://vxh.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://inf.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://vvc.epnwcf.com

C#:   list.Add(4);
来源：http://ixg.yfazqb.com

[D03] 在指定位置插入元素
来源：http://wpf.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://bsa.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mla.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://diy.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://scd.guowangkeji.top

Java: list.add(0, 0);
来源：http://xql.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://tkx.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://awt.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://efj.chenlongwang.top

[D04] 删除元素
来源：http://vok.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bgg.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jmc.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cid.yonumen.top

TS:   arr.splice(0, 1);
来源：http://ige.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://chb.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mfd.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://opk.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://njz.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://sle.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qqs.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gdi.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://swt.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://yfz.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://bvc.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://qba.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pjb.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eaj.yvedp.cn

[D06] 数组长度
来源：http://web.redwolf501.top

Py:   len(arr)
来源：http://eps.haohaochexian.top

PHP:  count($arr);
来源：http://quf.aizwys.cn

JS:   arr.length
来源：http://ymn.pengpengdd.cyou

TS:   arr.length
来源：http://duw.andypj.xyz

Java: list.size();
来源：http://djq.xuanzx.com

Go:   len(arr)
来源：http://pox.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://yna.yueranfly.top

C#:   list.Count;
来源：http://sgj.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://mtb.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://byk.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://psp.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://kmp.uphjek.com

TS:   arr.slice(1, 4);
来源：http://jkd.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://crk.yangfankeji.com

Go:   arr[1:4]
来源：http://jeq.guowangkeji.top

Ruby: arr[1, 3]
来源：http://byc.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://pno.shuidangran.top

[D08] 合并两个数组
来源：http://vlf.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://ipe.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://ywg.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mnp.zdqjudy.top

TS:   [...a, ...b];
来源：http://rpo.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rfc.epnwcf.com

Go:   append(a, b...)
来源：http://jam.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://aqf.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://lcy.hywenlv.cn

[D09] 排序（升序）
来源：http://ogb.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lqq.mhx1999.top

PHP:  sort($arr);
来源：http://eke.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ajw.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vmf.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ptl.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nap.yfazqb.com

Ruby: arr.sort
来源：http://tnj.quarkkingdee.top

C#:   list.Sort();
来源：http://jnz.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jbw.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://csr.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mhp.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://txi.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eaw.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dyg.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ytm.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://skv.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yis.fehbvm.com

[D11] 反转数组
来源：http://ikk.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://ncq.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://nrq.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ibk.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://vqd.cheryme.top

Java: Collections.reverse(list);
来源：http://kqv.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://wfy.zdbjq.cn

Ruby: arr.reverse
来源：http://xor.zhongyouzk.top

C#:   list.Reverse();
来源：http://qvx.ehwqpu.com

[D12] 查找元素下标
来源：http://ciq.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://bzw.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gsk.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnz.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tvp.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nvo.meibo888.top

Go:   slices.Index(arr, x)
来源：http://xsh.yonumen.top

Ruby: arr.index(x)
来源：http://bdq.epnwcf.com

C#:   list.IndexOf(x);
来源：http://yzi.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://eib.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qxn.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://usp.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://hib.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://itx.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wzi.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gcs.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://tjv.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bji.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://aab.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gtt.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://shl.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://hko.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://txm.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwh.0kj1m.cn

Go:   // 手写循环
来源：http://rsv.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gje.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://flg.pycfn.com

[D15] 去重
来源：http://nxp.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngb.chenzaomai.com

PHP:  array_unique($arr);
来源：http://xui.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://wko.daxiang520.top

TS:   [...new Set(arr)]
来源：http://mxn.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dwx.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xlg.yuanzhike.top

Ruby: arr.uniq
来源：http://xhk.zhixingplan.top


<!-- 参考信息 -->