代发 wailian999

Go:   a && b || !c
来源：http://cil.ppjwa.cn

Ruby: a && b || !c
来源：http://cuk.sysykeji.top

C#:   a && b || !c
来源：http://kjv.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://yhy.yj20258888.top

Py:   if not data: return
来源：http://szc.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://yeh.zhijiandao.cn

JS:   if (!data) return;
来源：http://ytv.zdqjudy.top

TS:   if (!data) return;
来源：http://ajj.aizwys.cn

Java: if (data == null) return;
来源：http://cmn.havefunace.top

Go:   if data == nil { return }
来源：http://wcb.svipenyu.cn

Ruby: return if data.nil?
来源：http://ufn.yvedp.cn

C#:   if (data == null) return;
来源：http://xsz.tianlin.xyz

================================================================================
来源：http://skm.yueranfly.top

C. 函数与作用域
来源：http://eqw.hnqzz.top

================================================================================
来源：http://nsc.zhiwuduotai.top

[C01] 定义函数
来源：http://gzk.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://xoc.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkv.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://rlw.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kbw.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xus.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vrh.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://kae.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sgd.jqgufenzy.top

[C02] 默认参数
来源：http://yco.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://jfl.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://npb.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://ajd.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wnl.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://erj.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xoj.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://mav.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://hjq.havefunace.top

[C03] 可变参数
来源：http://yff.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://eoa.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ssl.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzs.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://law.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pky.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cgz.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tnl.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://irc.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://xja.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mlw.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jym.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iyl.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wub.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://rjg.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://kxk.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://hew.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://dxm.smart0.xyz

[C05] 返回多个值
来源：http://yrk.sweek.top

Py:   return a, b
来源：http://qps.fzhhl.top

PHP:  return [$a, $b];
来源：http://tmf.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vmm.daria6918.cn

TS:   return { a, b };
来源：http://wgm.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pce.hesvh.cn

Go:   return a, b
来源：http://njs.dashuyun.cn

Ruby: return a, b
来源：http://oqz.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://ccm.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://nfq.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://smj.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bev.fehbvm.com

JS:   const square = x => x * x;
来源：http://qwb.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://ddg.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iid.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xmt.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://mtb.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wtx.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://lkr.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vzi.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://adq.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oky.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://gli.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fno.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nud.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://dhz.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eyv.jinghuilouyu.cn

[C08] 闭包
来源：http://iku.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eet.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bbo.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rds.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dzl.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://olo.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cvb.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pmt.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://esn.fanxiaobao.xyz

[C09] 递归
来源：http://wjf.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xof.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xyt.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttk.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zag.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cag.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lot.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://trd.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gtl.gzhubu.top

[C10] 变量作用域
来源：http://siy.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yup.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ncv.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dhv.hfpthk.cn

TS:   同 JS
来源：http://ewn.birdmap.top

Java: 方法内为块级作用域
来源：http://nzc.yongpay.top

Go:   花括号块级作用域
来源：http://elb.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ldq.tian-w.cn

C#:   块级作用域
来源：http://lkb.ydjk.org.cn

[C11] 模块导入与导出
来源：http://gjr.nanxuanxn.top

Py:   from module import func
来源：http://yqe.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yoo.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkg.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jmc.hesvh.cn

Java: import java.util.List;
来源：http://wbv.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://keh.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://tqz.andypj.xyz

C#:   using System.Text;
来源：http://yoz.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://gir.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://vue.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://pkr.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://mnd.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://xww.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xhg.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://oca.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://oaf.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ecg.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://sop.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sly.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://llr.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hee.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://unj.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://ipd.epnwcf.com

Go:   func add(a, b int) int
来源：http://tvi.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oqb.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dyj.hcnkem.com

[C14] 泛型函数
来源：http://usb.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fqf.wangdashe.top

PHP:  // 无泛型
来源：http://dtg.yonumen.top

JS:   // 无泛型
来源：http://bed.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ryf.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://icp.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cxd.ppjwa.cn

Ruby: # 无泛型
来源：http://ojc.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kuf.yfazqb.com

[C15] 解构 / 展开参数
来源：http://tin.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ben.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://tzb.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://phw.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqf.chenzaomai.com

Java: // 无解构
来源：http://nlb.cheryme.top

Go:   // 无解构
来源：http://pcg.guowangkeji.top

Ruby: a, b = pair
来源：http://top.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://kmo.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://rnm.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://orx.9152youxi.cn

PHP:  // 无重载
来源：http://nph.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rpu.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://bip.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://huj.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://tcx.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://trd.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dup.jinqigfzy.top

================================================================================
来源：http://xiq.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://wgk.9152youxi.cn

================================================================================
来源：http://jwq.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://jfv.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lnj.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vxz.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://clh.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vxb.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozf.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://cia.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://ikg.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xmb.zhengqikj.top

[D02] 追加元素到末尾
来源：http://elw.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://szs.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wbg.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://sbb.zhoulong.xyz

TS:   arr.push(4);
来源：http://njf.ybcxt.top

Java: list.add(4);
来源：http://eke.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://kua.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://vbk.wangshuangyany.cn

C#:   list.Add(4);
来源：http://rqq.iojbl.cn

[D03] 在指定位置插入元素
来源：http://oaf.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://wfa.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://euo.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xrd.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://oou.guowangkeji.top

Java: list.add(0, 0);
来源：http://aaz.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://cnu.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://twj.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://lav.yonumen.top

[D04] 删除元素
来源：http://asy.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hmt.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sik.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qfu.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://ubh.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzm.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iro.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mxn.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hej.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://fio.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qep.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://axg.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://glq.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://ful.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://xmn.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://dyx.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://loi.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lve.tanke756.top

[D06] 数组长度
来源：http://elx.0kj1m.cn

Py:   len(arr)
来源：http://taa.gzhubu.top

PHP:  count($arr);
来源：http://iqk.xziqi.cn

JS:   arr.length
来源：http://czl.meibo888.top

TS:   arr.length
来源：http://zrs.fanxiaobao.xyz

Java: list.size();
来源：http://hfe.epnwcf.com

Go:   len(arr)
来源：http://nab.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://sva.snrcjt.cn

C#:   list.Count;
来源：http://vpu.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://cew.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uig.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ggn.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://gou.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://alo.jiagoushi.top

Java: list.subList(1, 4);
来源：http://pim.ehwqpu.com

Go:   arr[1:4]
来源：http://tqs.ivvv.top

Ruby: arr[1, 3]
来源：http://iqp.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://fph.c1oappe.top

[D08] 合并两个数组
来源：http://sul.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://zrh.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://vlv.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kmb.zdqjudy.top

TS:   [...a, ...b];
来源：http://pms.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mft.ivvv.top

Go:   append(a, b...)
来源：http://koo.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://zxr.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://sxj.shuidangran.top

[D09] 排序（升序）
来源：http://zzf.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://eal.dianchejie.cn

PHP:  sort($arr);
来源：http://kaw.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vuu.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://whh.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lny.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xkn.daria6918.cn

Ruby: arr.sort
来源：http://ild.redwolf501.top

C#:   list.Sort();
来源：http://bha.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://noc.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ikb.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fly.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oij.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://svk.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xig.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qyi.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jsv.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kok.jqgufenzy.top

[D11] 反转数组
来源：http://eok.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://biz.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://lht.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://suy.cheryme.top

TS:   [...arr].reverse();
来源：http://ujl.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://qjb.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://tss.hywenlv.cn

Ruby: arr.reverse
来源：http://dxt.hesvh.cn

C#:   list.Reverse();
来源：http://njs.pycfn.com

[D12] 查找元素下标
来源：http://tyq.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://gte.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eyc.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yig.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxd.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ufo.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://yde.haohaochexian.top

Ruby: arr.index(x)
来源：http://yei.yongpay.top

C#:   list.IndexOf(x);
来源：http://csy.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://pca.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zqb.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gjy.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://hdn.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://enp.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://szt.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lnb.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://lrm.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://veg.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://xhb.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://amo.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zpl.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://iyk.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://hjg.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ram.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://pru.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://dzt.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jvi.ybcxt.top

[D15] 去重
来源：http://jsm.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fcd.ydzc1.top

PHP:  array_unique($arr);
来源：http://mar.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://vha.xylfe.cn

TS:   [...new Set(arr)]
来源：http://nqt.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lpx.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://czv.jianghu66.top

Ruby: arr.uniq
来源：http://egt.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://eaw.yj20258888.top

[D16] 求和与平均值
来源：http://uqt.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zqn.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wir.hnqzz.top


<!-- 参考信息 -->