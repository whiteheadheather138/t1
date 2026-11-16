代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://tvl.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uss.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wtm.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://wpd.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://lbh.zhengqikj.top

[C03] 可变参数
来源：http://omn.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://won.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uxz.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zui.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zfj.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cep.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xpk.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://qxo.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hug.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://ieo.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hpm.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xtp.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://boo.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xov.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://ctv.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://ahb.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://oil.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://jqq.bbcook.cn

[C05] 返回多个值
来源：http://gxa.uphjek.com

Py:   return a, b
来源：http://koj.jianghu66.top

PHP:  return [$a, $b];
来源：http://rcn.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cqs.sjlbkw.cn

TS:   return { a, b };
来源：http://uvi.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://foa.dashuyun.cn

Go:   return a, b
来源：http://xaw.fanxiaobao.xyz

Ruby: return a, b
来源：http://nwb.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://vew.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://iav.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://bsw.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pnk.vehdjk.com

JS:   const square = x => x * x;
来源：http://sly.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://hnm.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ozi.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ihj.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://iqs.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://suc.xziqi.cn

[C07] 把函数作为参数传入
来源：http://vro.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://omd.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bia.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rel.quarkkingdee.top

TS:   arr.map(String)
来源：http://vmh.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzt.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://imp.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://pyp.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zzy.zhengqikj.top

[C08] 闭包
来源：http://eew.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xdq.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ean.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkx.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://grc.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rfl.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zfd.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://umo.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hyh.fengsongda.top

[C09] 递归
来源：http://ywl.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gvp.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qll.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jyo.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dle.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xav.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uku.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmm.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://djz.yonumen.top

[C10] 变量作用域
来源：http://qhs.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dkt.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rvd.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hrr.guowangkeji.top

TS:   同 JS
来源：http://bcs.haohaochexian.top

Java: 方法内为块级作用域
来源：http://vgf.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://lse.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aot.xylfe.cn

C#:   块级作用域
来源：http://vne.guowangkeji.top

[C11] 模块导入与导出
来源：http://mud.yongpay.top

Py:   from module import func
来源：http://ymc.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://scj.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jqo.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kxs.gaohongyu789.top

Java: import java.util.List;
来源：http://klh.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewh.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://yye.havefunace.top

C#:   using System.Text;
来源：http://dnt.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://tjy.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://rqv.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://ohy.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://gdv.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://zbs.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjm.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://tla.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://dig.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://njm.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://pwc.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lge.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qdj.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://igx.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ftu.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://cxr.zdbjq.cn

Go:   func add(a, b int) int
来源：http://kdj.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tau.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bdd.ctjpmb.com

[C14] 泛型函数
来源：http://uti.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hvk.mhx1999.top

PHP:  // 无泛型
来源：http://fgo.tanke756.top

JS:   // 无泛型
来源：http://mab.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lgq.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kdl.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nkz.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://apn.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gan.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://xgr.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qby.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://tou.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rif.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://alp.chenlongwang.top

Java: // 无解构
来源：http://bki.cucudq.cn

Go:   // 无解构
来源：http://kya.jiagoushi.top

Ruby: a, b = pair
来源：http://tgm.wangdashe.top

C#:   var (a, b) = pair;
来源：http://dih.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://zmi.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://huh.jyoumei.cn

PHP:  // 无重载
来源：http://yvb.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xtm.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://hpl.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://clg.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://nxx.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://dkg.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fiz.svipenyu.cn

================================================================================
来源：http://avv.pycfn.com

D. 数组 / 列表 / 集合
来源：http://vxf.shuidangran.top

================================================================================
来源：http://yrw.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://ghw.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fdu.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rby.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lep.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lpv.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hpy.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://vlz.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://and.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dxx.cqqwz.cn

[D02] 追加元素到末尾
来源：http://lrk.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fsv.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://icc.gogol.net.cn

JS:   arr.push(4);
来源：http://jta.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://epc.mhx1999.top

Java: list.add(4);
来源：http://ohr.ivvv.top

Go:   arr = append(arr, 4)
来源：http://oak.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://laf.chenjidiqi.icu

C#:   list.Add(4);
来源：http://osp.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://mso.yonumen.top

Py:   arr.insert(0, 0)
来源：http://cvr.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofs.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yml.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://jsz.cashguo.top

Java: list.add(0, 0);
来源：http://ipd.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://lze.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cjc.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://ols.tian-w.cn

[D04] 删除元素
来源：http://gfn.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oym.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rox.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ujr.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://wjd.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kou.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nmb.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kac.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mxs.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://rhg.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://grr.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ksu.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://avd.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://ubx.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://gze.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://las.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iao.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nlt.ybcxt.top

[D06] 数组长度
来源：http://iui.birdmap.top

Py:   len(arr)
来源：http://ayf.daxiang520.top

PHP:  count($arr);
来源：http://ayw.jinqigfzy.top

JS:   arr.length
来源：http://oaq.ehwqpu.com

TS:   arr.length
来源：http://qhh.zhaomingkeji.xyz

Java: list.size();
来源：http://rpp.hcnkem.com

Go:   len(arr)
来源：http://hno.tian-w.cn

Ruby: arr.length; arr.size
来源：http://exa.smart0.xyz

C#:   list.Count;
来源：http://gom.tanke756.top

[D07] 切片 / 取子数组
来源：http://eko.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uql.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://myy.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://dae.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://ymk.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://jdc.ybcxt.top

Go:   arr[1:4]
来源：http://ayq.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://yfn.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://tce.shangyingyoupin.top

[D08] 合并两个数组
来源：http://otu.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://ger.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://mau.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kcj.aizwys.cn

TS:   [...a, ...b];
来源：http://bua.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ape.yj20258.top

Go:   append(a, b...)
来源：http://jpv.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://hwz.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://smg.fehbvm.com

[D09] 排序（升序）
来源：http://dhk.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://chz.bjfxy.top

PHP:  sort($arr);
来源：http://qbz.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qlj.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nma.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xmb.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jjl.quarkkingdee.top

Ruby: arr.sort
来源：http://rox.ybcxt.top

C#:   list.Sort();
来源：http://sat.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gua.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qee.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qpo.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qiw.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zgz.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zkk.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nlm.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gxs.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fgd.havefunace.top

[D11] 反转数组
来源：http://qfy.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vnv.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://tyt.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjq.ybcxt.top

TS:   [...arr].reverse();
来源：http://pvr.52xcode.cn

Java: Collections.reverse(list);
来源：http://tpg.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://uki.iojbl.cn

Ruby: arr.reverse
来源：http://qkq.jlsjyb.cn

C#:   list.Reverse();
来源：http://nbs.ppjwa.cn

[D12] 查找元素下标
来源：http://vqo.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://xtg.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vdl.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwr.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqi.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czq.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://efh.yj202588.top

Ruby: arr.index(x)
来源：http://alw.jianghu66.top

C#:   list.IndexOf(x);
来源：http://ocf.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://tip.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://njh.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ydy.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://fgt.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://rsz.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gfz.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpp.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://dtu.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://crr.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://lzo.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mcf.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ulm.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://tbe.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://mlu.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xig.quarkkingdee.top

Go:   // 手写循环
来源：http://ldf.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://znv.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oaa.hywenlv.cn

[D15] 去重
来源：http://oji.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hpg.nwbrower.top

PHP:  array_unique($arr);
来源：http://onx.daria6918.cn

JS:   [...new Set(arr)]
来源：http://hqq.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://uqx.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://smy.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dwp.aizwys.cn

Ruby: arr.uniq
来源：http://kzo.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://qmg.smart0.xyz

[D16] 求和与平均值
来源：http://sqe.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ahe.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iph.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oye.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xnw.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wdu.gzhubu.top

Go:   // 手写循环累加
来源：http://gvb.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gsk.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://iiu.yj20258.top

[D17] 最大值与最小值
来源：http://pgm.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://afs.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://gpx.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hid.fzhhl.top

TS:   Math.max(...arr);
来源：http://zbm.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://two.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zsl.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://yon.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://ztq.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://jxn.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yae.tarul.cn

PHP:  array_merge(...$nested);
来源：http://xmo.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pwe.xinyue.icu

TS:   nested.flat();
来源：http://zli.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pbx.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://anl.gogol.net.cn

Ruby: nested.flatten
来源：http://qac.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://etx.fengsongda.top

[D19] 按字段分组
来源：http://rsl.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xva.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://knt.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fjc.zycfv.cn


<!-- 参考信息 -->