代发 wailian999

Py:   if not data: return
来源：http://uxj.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://iwd.fktsv.cn

JS:   if (!data) return;
来源：http://bqg.nwbrower.top

TS:   if (!data) return;
来源：http://vaq.dashuyun.cn

Java: if (data == null) return;
来源：http://lrj.cdnleiting.top

Go:   if data == nil { return }
来源：http://qmr.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://xyx.jiagoushi.top

C#:   if (data == null) return;
来源：http://siw.cashguo.top

================================================================================
来源：http://fwl.nanxuanxn.top

C. 函数与作用域
来源：http://dyv.fengsongda.top

================================================================================
来源：http://iwe.yonumen.top

[C01] 定义函数
来源：http://hsp.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://tfg.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrm.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://kjk.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://awp.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ptz.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://nqd.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://fbl.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eih.jinqigufen.top

[C02] 默认参数
来源：http://qac.pycfn.com

Py:   def greet(name="World"): return name
来源：http://sda.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gsp.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://kwq.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fwv.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rfw.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://obw.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://rpb.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://myn.jqgufenzy.top

[C03] 可变参数
来源：http://qns.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://lfs.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cqt.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqx.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqv.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mlc.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pnc.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://jvq.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tnl.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://pyc.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://piz.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vmd.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hgu.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fwp.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://doj.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://ieh.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://sft.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://qnk.fktsv.cn

[C05] 返回多个值
来源：http://jxj.shangyingyoupin.top

Py:   return a, b
来源：http://vxj.xziqi.cn

PHP:  return [$a, $b];
来源：http://nox.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ccg.uphjek.com

TS:   return { a, b };
来源：http://ivb.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qrm.yueranfly.top

Go:   return a, b
来源：http://feh.jinyuanbaomall.cn

Ruby: return a, b
来源：http://vii.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://wwk.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://cdj.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://ykj.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ujf.zhengqikj.top

JS:   const square = x => x * x;
来源：http://fyu.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://cqx.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xny.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://rff.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://nka.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://atl.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://zut.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uqa.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ifu.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vpz.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://qeb.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uxn.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://evn.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://daw.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hic.ybcxt.top

[C08] 闭包
来源：http://swi.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fjr.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vys.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zxc.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ioi.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gcl.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yrw.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xhw.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qbu.gzhubu.top

[C09] 递归
来源：http://dur.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sjt.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gjq.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwu.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfi.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wqi.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://egi.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qvp.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vep.hnxiangtu.top

[C10] 变量作用域
来源：http://jus.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nrk.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fcx.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hbh.gogol.net.cn

TS:   同 JS
来源：http://vyv.tian-w.cn

Java: 方法内为块级作用域
来源：http://ibm.iojbl.cn

Go:   花括号块级作用域
来源：http://yck.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ulh.tanke756.top

C#:   块级作用域
来源：http://gsx.jqgfzy.top

[C11] 模块导入与导出
来源：http://nxr.yueranfly.top

Py:   from module import func
来源：http://dks.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pmd.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tjv.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hdp.zhongyouzk.top

Java: import java.util.List;
来源：http://jmd.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rqt.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://khz.birdmap.top

C#:   using System.Text;
来源：http://jut.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://yxn.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://law.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://arf.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://vrg.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://voo.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifl.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://jja.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://hxm.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vqf.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://gzt.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zzl.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ycv.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cij.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kmk.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://jwr.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://jkf.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ooc.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ttw.gotoacloud.top

[C14] 泛型函数
来源：http://ydu.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ojz.cheryme.top

PHP:  // 无泛型
来源：http://fiz.chenjidiqi.icu

JS:   // 无泛型
来源：http://nwv.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aum.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xsh.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jga.jinqigufen.top

Ruby: # 无泛型
来源：http://fai.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://civ.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://grp.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rnw.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://oab.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://drm.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xhd.cqqwz.cn

Java: // 无解构
来源：http://aur.hywenlv.cn

Go:   // 无解构
来源：http://jrq.kuanghao11.cn

Ruby: a, b = pair
来源：http://koq.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://lvr.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://uto.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ffb.fzhhl.top

PHP:  // 无重载
来源：http://soc.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hdc.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://oao.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kix.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://lxo.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://zfh.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xme.redwolf501.top

================================================================================
来源：http://tnq.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://mpd.yj20258888.top

================================================================================
来源：http://jia.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://smk.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mrb.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rat.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jft.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yey.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qml.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://fol.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://dxn.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zby.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://nuh.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uyj.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kzl.zhengqikj.top

JS:   arr.push(4);
来源：http://utd.hammf.cn

TS:   arr.push(4);
来源：http://fye.ydzc1.top

Java: list.add(4);
来源：http://pcr.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://drt.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://myq.shzxlz.cn

C#:   list.Add(4);
来源：http://xxq.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://wpz.tanke756.top

Py:   arr.insert(0, 0)
来源：http://fje.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://prs.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ryj.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://azp.c1oappe.top

Java: list.add(0, 0);
来源：http://pil.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mpp.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdo.yongpay.top

C#:   list.Insert(0, 0);
来源：http://nsi.smart0.xyz

[D04] 删除元素
来源：http://mtj.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckj.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yyr.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oej.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://wxm.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rku.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sgn.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jrp.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://odj.cashguo.top

[D05] 访问与修改元素
来源：http://bnv.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qco.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mbu.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nne.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://rzf.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://sve.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://edl.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bas.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uii.mhx1999.top

[D06] 数组长度
来源：http://cpa.jqgufenzy.top

Py:   len(arr)
来源：http://jbq.iojbl.cn

PHP:  count($arr);
来源：http://cai.wangdashe.top

JS:   arr.length
来源：http://bpv.yangfankeji.com

TS:   arr.length
来源：http://yim.mhx1999.top

Java: list.size();
来源：http://fse.wangshuangyany.cn

Go:   len(arr)
来源：http://gen.gzhubu.top

Ruby: arr.length; arr.size
来源：http://kuy.bbcook.cn

C#:   list.Count;
来源：http://frb.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://wlr.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://now.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://itt.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://jpb.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://xyi.gzhubu.top

Java: list.subList(1, 4);
来源：http://nqn.vqdsnc.cn

Go:   arr[1:4]
来源：http://lbw.ivvv.top

Ruby: arr[1, 3]
来源：http://slc.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://cii.ybcxt.top

[D08] 合并两个数组
来源：http://ydl.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://oqi.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://qou.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wpn.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://joy.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xpo.ydjk.org.cn

Go:   append(a, b...)
来源：http://atn.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://uzx.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://sld.snrcjt.cn

[D09] 排序（升序）
来源：http://muv.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://dep.gzhubu.top

PHP:  sort($arr);
来源：http://dto.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://moe.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://fpr.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aca.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nwt.mhx1999.top

Ruby: arr.sort
来源：http://dba.yj20258888.top

C#:   list.Sort();
来源：http://iwd.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jgp.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gkx.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vts.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mkz.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbp.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qqo.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hja.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xho.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://swo.52xcode.cn

[D11] 反转数组
来源：http://itg.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://pdy.fehbvm.com

PHP:  array_reverse($arr);
来源：http://wfp.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://msq.yonumen.top

TS:   [...arr].reverse();
来源：http://equ.pycfn.com

Java: Collections.reverse(list);
来源：http://qxt.yonumen.top

Go:   slices.Reverse(arr)
来源：http://gfe.nanxuanxn.top

Ruby: arr.reverse
来源：http://nfu.ehwqpu.com

C#:   list.Reverse();
来源：http://ibf.sufxvd.cn

[D12] 查找元素下标
来源：http://ylj.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://lyc.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tcm.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epz.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://heq.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kcf.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://aer.zdqjudy.top

Ruby: arr.index(x)
来源：http://nmh.fehbvm.com

C#:   list.IndexOf(x);
来源：http://ykh.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://gtv.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aau.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dzr.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://aiz.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://tnr.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xaw.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://weg.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ggi.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kkz.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://cyj.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wvf.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ogk.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://eqk.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://vhf.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ool.yongpay.top

Go:   // 手写循环
来源：http://xsy.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uaj.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ucm.sysykeji.top

[D15] 去重
来源：http://drn.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uda.mhx1999.top

PHP:  array_unique($arr);
来源：http://ubq.meibo888.top

JS:   [...new Set(arr)]
来源：http://fae.daria6918.cn

TS:   [...new Set(arr)]
来源：http://xkr.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yov.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ndp.yfazqb.com

Ruby: arr.uniq
来源：http://aso.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://rva.jinqigufen.top

[D16] 求和与平均值
来源：http://dlt.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kor.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qdb.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://meu.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rww.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sog.zhoulong.xyz

Go:   // 手写循环累加
来源：http://mfc.mhx1999.top


<!-- 参考信息 -->