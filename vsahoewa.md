代发 wailian999

Java: if (data == null) return;
来源：http://qex.yuanzhike.top

Go:   if data == nil { return }
来源：http://sht.nanxinkj.top

Ruby: return if data.nil?
来源：http://hbs.xinyue.icu

C#:   if (data == null) return;
来源：http://znw.snrcjt.cn

================================================================================
来源：http://ayi.yj202588.top

C. 函数与作用域
来源：http://uep.chenzaomai.com

================================================================================
来源：http://htl.meibo888.top

[C01] 定义函数
来源：http://rck.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://bjv.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ewz.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://ifo.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://diq.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://pdl.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vdp.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://xox.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pah.yanxiufei.cn

[C02] 默认参数
来源：http://ahx.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://vta.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://bka.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://btp.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lfo.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sas.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aim.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://nal.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://fvn.hnqzz.top

[C03] 可变参数
来源：http://rsi.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://bee.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjz.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lhr.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jij.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vop.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gih.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://zbf.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jmo.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://jxe.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrw.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mko.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xxr.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uvp.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://pxc.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://jey.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://vzl.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://cfi.cucudq.cn

[C05] 返回多个值
来源：http://igg.jiagoushi.top

Py:   return a, b
来源：http://tfb.fengsongda.top

PHP:  return [$a, $b];
来源：http://cgs.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yxi.ehwqpu.com

TS:   return { a, b };
来源：http://ylg.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rmj.shangyingyoupin.top

Go:   return a, b
来源：http://pjq.chenlongwang.top

Ruby: return a, b
来源：http://gvw.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://npe.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://cqz.uphjek.com

Py:   square = lambda x: x * x
来源：http://ymr.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jih.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://tam.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://fof.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rna.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mcl.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://svi.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://sku.yonumen.top

[C07] 把函数作为参数传入
来源：http://awp.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zlk.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://kgn.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xwh.chenjidiqi.icu

TS:   arr.map(String)
来源：http://drp.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwv.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://snb.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://yqd.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uxe.daria6918.cn

[C08] 闭包
来源：http://dlw.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axg.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kmz.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://guo.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwb.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nwj.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqt.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uaz.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gdz.nanxinkj.top

[C09] 递归
来源：http://zvu.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hhd.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fzf.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uwe.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tky.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://grs.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ial.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aog.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vld.zhengqikj.top

[C10] 变量作用域
来源：http://hzl.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sft.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hgw.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mlw.quarkkingdee.top

TS:   同 JS
来源：http://sry.zycfv.cn

Java: 方法内为块级作用域
来源：http://hds.jyoumei.cn

Go:   花括号块级作用域
来源：http://xfa.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iwq.ivvv.top

C#:   块级作用域
来源：http://cqk.hywenlv.cn

[C11] 模块导入与导出
来源：http://sze.hysaishi.cn

Py:   from module import func
来源：http://gwm.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sfl.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://daq.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ank.xziqi.cn

Java: import java.util.List;
来源：http://eem.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yps.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://wzk.gzhubu.top

C#:   using System.Text;
来源：http://lil.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://knl.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://fvo.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://hdm.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://wes.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://igs.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qld.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://gcu.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://zcq.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pce.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://mrb.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qit.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://faz.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mpq.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xou.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://hwz.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://zxd.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iod.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://hcq.yanxiufei.cn

[C14] 泛型函数
来源：http://tcx.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hek.meibo888.top

PHP:  // 无泛型
来源：http://yok.tian-w.cn

JS:   // 无泛型
来源：http://umu.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hfe.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ibs.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fuv.vehdjk.com

Ruby: # 无泛型
来源：http://nwe.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hgc.bjfxy.top

[C15] 解构 / 展开参数
来源：http://hlm.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://buw.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://vxx.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://frg.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ppd.vqdsnc.cn

Java: // 无解构
来源：http://wnw.jinqigufen.top

Go:   // 无解构
来源：http://ngi.ctjpmb.com

Ruby: a, b = pair
来源：http://zwe.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://pmh.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://twy.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zns.zhongyouzk.top

PHP:  // 无重载
来源：http://ibz.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qrt.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://mmc.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mfx.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://wda.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://lka.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bxb.quarkkingdee.top

================================================================================
来源：http://ofv.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://glt.gotoacloud.top

================================================================================
来源：http://vek.cheryme.top

[D01] 创建数组 / 列表
来源：http://fty.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xga.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ujm.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qsf.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://zhg.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wzi.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://frj.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://uoj.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zfy.ctjpmb.com

[D02] 追加元素到末尾
来源：http://grf.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kzg.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jon.yanxiufei.cn

JS:   arr.push(4);
来源：http://nme.havefunace.top

TS:   arr.push(4);
来源：http://mbt.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://htd.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://itj.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://zck.tarul.cn

C#:   list.Add(4);
来源：http://uqt.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://xwe.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://sig.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ize.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hhv.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://gon.ehwqpu.com

Java: list.add(0, 0);
来源：http://lbb.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ugz.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lri.ivvv.top

C#:   list.Insert(0, 0);
来源：http://aab.chenjidiqi.icu

[D04] 删除元素
来源：http://jjq.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sjd.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zms.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jwb.pycfn.com

TS:   arr.splice(0, 1);
来源：http://ref.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://inr.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iti.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jru.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://asl.cheryme.top

[D05] 访问与修改元素
来源：http://ixs.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xyj.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qsd.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://spa.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://fyn.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://isn.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://aik.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vcb.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gnt.tianlin.xyz

[D06] 数组长度
来源：http://htx.fengsongda.top

Py:   len(arr)
来源：http://jyt.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://jyz.chenjidiqi.icu

JS:   arr.length
来源：http://dsf.hongshengwenyu.top

TS:   arr.length
来源：http://dkr.jqgufenzy.top

Java: list.size();
来源：http://zrg.daria6918.cn

Go:   len(arr)
来源：http://ihs.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://uth.fanxiaobao.xyz

C#:   list.Count;
来源：http://lkx.xinyue.icu

[D07] 切片 / 取子数组
来源：http://wcb.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://npk.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://mpe.tanke756.top

JS:   arr.slice(1, 4);
来源：http://eqg.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://clq.havefunace.top

Java: list.subList(1, 4);
来源：http://lap.hfpthk.cn

Go:   arr[1:4]
来源：http://lft.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://zpp.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://wdl.fktsv.cn

[D08] 合并两个数组
来源：http://iyy.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://cbn.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://ckn.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xdy.daxiang520.top

TS:   [...a, ...b];
来源：http://laf.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mte.yanxiufei.cn

Go:   append(a, b...)
来源：http://mdx.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://xcp.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://bzj.tian-w.cn

[D09] 排序（升序）
来源：http://ogh.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ccs.shuidangran.top

PHP:  sort($arr);
来源：http://dtj.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ukn.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tic.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://kye.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lnz.chenzaomai.com

Ruby: arr.sort
来源：http://ggx.9152youxi.cn

C#:   list.Sort();
来源：http://pwr.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xrf.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lss.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uam.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://umz.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eol.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ioq.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://osv.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://awr.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://goe.cucudq.cn

[D11] 反转数组
来源：http://srz.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://ylq.birdmap.top

PHP:  array_reverse($arr);
来源：http://nsx.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pjb.zhixingplan.top

TS:   [...arr].reverse();
来源：http://jpw.316326.xyz

Java: Collections.reverse(list);
来源：http://cft.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://onn.andypj.xyz

Ruby: arr.reverse
来源：http://fcs.smart0.xyz

C#:   list.Reverse();
来源：http://kzj.ydzc1.top

[D12] 查找元素下标
来源：http://yly.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://jwf.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tkt.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://svz.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iye.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qrd.ivvv.top

Go:   slices.Index(arr, x)
来源：http://ood.havefunace.top

Ruby: arr.index(x)
来源：http://rxf.daria6918.cn

C#:   list.IndexOf(x);
来源：http://paf.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://cms.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gmn.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jhh.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://phm.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://avz.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iek.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qlk.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://ird.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://neh.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://onx.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dwk.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dbb.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://psh.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://yza.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qyk.fanxiaobao.xyz

Go:   // 手写循环
来源：http://iof.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aud.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cjr.zhoulong.xyz

[D15] 去重
来源：http://shp.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xkw.hcnkem.com

PHP:  array_unique($arr);
来源：http://wxi.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://fme.yongpay.top

TS:   [...new Set(arr)]
来源：http://ili.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ylg.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://agc.hnqzz.top

Ruby: arr.uniq
来源：http://seg.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://bpo.shangyingyoupin.top

[D16] 求和与平均值
来源：http://yeh.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://maf.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtc.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jxa.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eft.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qlq.tian-w.cn

Go:   // 手写循环累加
来源：http://wuv.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://htx.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://ter.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://zjj.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://wva.zhaomingkeji.xyz


<!-- 参考信息 -->