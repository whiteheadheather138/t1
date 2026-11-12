代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wzk.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jbd.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sck.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://hsz.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://mfg.zhongyouzk.top

[C03] 可变参数
来源：http://rqj.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://zwd.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sxq.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nss.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rij.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kbe.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ptk.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kiu.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iaj.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://dla.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aqd.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://evz.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cqq.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pzz.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://rrh.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://wbs.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://axj.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://auh.fehbvm.com

[C05] 返回多个值
来源：http://xdj.zhengqikj.top

Py:   return a, b
来源：http://iyk.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://wjr.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yby.xylfe.cn

TS:   return { a, b };
来源：http://ebe.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nsq.quarkkingdee.top

Go:   return a, b
来源：http://yyl.yuxming.cn

Ruby: return a, b
来源：http://wsb.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://aud.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://gig.ydzc1.top

Py:   square = lambda x: x * x
来源：http://tbx.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://awf.hcnkem.com

JS:   const square = x => x * x;
来源：http://mcn.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://mxq.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lpr.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tzm.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://xzx.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://brf.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://ghn.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nuh.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://rwu.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dcn.haohaochexian.top

TS:   arr.map(String)
来源：http://ons.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uec.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hoe.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://amk.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pux.tarul.cn

[C08] 闭包
来源：http://mvw.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qdd.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lid.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jyl.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wcd.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lii.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mjp.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dwm.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nqj.ppjwa.cn

[C09] 递归
来源：http://xaa.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lpu.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bvs.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpc.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vfi.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yom.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gxs.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lfh.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ryw.xziqi.cn

[C10] 变量作用域
来源：http://sjd.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fak.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uuh.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ufi.tarul.cn

TS:   同 JS
来源：http://zje.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://xwf.nanxuanxn.top

Go:   花括号块级作用域
来源：http://asr.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pfq.bbcook.cn

C#:   块级作用域
来源：http://oev.birdmap.top

[C11] 模块导入与导出
来源：http://gnq.cucudq.cn

Py:   from module import func
来源：http://fza.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lak.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lkn.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dyc.zhongyouzk.top

Java: import java.util.List;
来源：http://cea.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://htp.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://bnm.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ugn.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://fgx.havefunace.top

Py:   (lambda: print("run"))()
来源：http://dbw.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://biz.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://rbc.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://oyu.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kwv.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://rjn.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://tqo.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gdi.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://clk.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://svm.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lci.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://clb.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qlu.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://idz.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://fbm.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zzx.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://wzb.sxryk.cn

[C14] 泛型函数
来源：http://kpb.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eip.bjfxy.top

PHP:  // 无泛型
来源：http://wgy.tian-w.cn

JS:   // 无泛型
来源：http://qyz.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mvj.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://osd.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gbs.andypj.xyz

Ruby: # 无泛型
来源：http://ipl.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qit.tanke756.top

[C15] 解构 / 展开参数
来源：http://lir.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yor.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://wcb.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wlp.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hvf.wangdashe.top

Java: // 无解构
来源：http://ikv.9152youxi.cn

Go:   // 无解构
来源：http://qfl.tarul.cn

Ruby: a, b = pair
来源：http://hvg.fktsv.cn

C#:   var (a, b) = pair;
来源：http://uye.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://jsl.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfj.daxiang520.top

PHP:  // 无重载
来源：http://tzd.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tnd.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://sbl.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qit.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://api.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://fxu.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vfb.zhijiandao.cn

================================================================================
来源：http://jtc.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://unj.daxiang520.top

================================================================================
来源：http://hbh.yj20258888.top

[D01] 创建数组 / 列表
来源：http://qap.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pci.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vyk.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fha.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://siu.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fpl.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://rvf.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://ryw.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://twb.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://jsw.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fmm.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ntf.jianghu66.top

JS:   arr.push(4);
来源：http://sdi.daria6918.cn

TS:   arr.push(4);
来源：http://kzt.fzhhl.top

Java: list.add(4);
来源：http://syy.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://ulr.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://bfu.zdqjudy.top

C#:   list.Add(4);
来源：http://nhs.meibo888.top

[D03] 在指定位置插入元素
来源：http://nnf.cashguo.top

Py:   arr.insert(0, 0)
来源：http://xst.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kgb.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iis.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://bwu.wangdashe.top

Java: list.add(0, 0);
来源：http://aex.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ztf.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eny.tanke756.top

C#:   list.Insert(0, 0);
来源：http://vpv.haohaochexian.top

[D04] 删除元素
来源：http://uwf.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sgv.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oin.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oub.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://csw.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rhg.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://egs.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://akh.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ugl.yongpay.top

[D05] 访问与修改元素
来源：http://lii.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uct.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aph.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hbj.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://pfz.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://ipc.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://cyg.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://owr.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqd.xuanzx.com

[D06] 数组长度
来源：http://ere.chenzaomai.com

Py:   len(arr)
来源：http://bri.sweek.top

PHP:  count($arr);
来源：http://ezy.zhengqikj.top

JS:   arr.length
来源：http://xce.zhijiandao.cn

TS:   arr.length
来源：http://gcw.jlsjyb.cn

Java: list.size();
来源：http://ewc.jinyuanbaomall.cn

Go:   len(arr)
来源：http://pav.jianghu66.top

Ruby: arr.length; arr.size
来源：http://uxa.ehwqpu.com

C#:   list.Count;
来源：http://qja.sysykeji.top

[D07] 切片 / 取子数组
来源：http://lxd.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qka.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://oug.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://xjh.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://mrk.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://mbj.meibo888.top

Go:   arr[1:4]
来源：http://kwc.jiagoushi.top

Ruby: arr[1, 3]
来源：http://unz.sweek.top

C#:   list.GetRange(1, 3);
来源：http://oan.meibo888.top

[D08] 合并两个数组
来源：http://tne.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://job.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://xsu.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hci.yuanzhike.top

TS:   [...a, ...b];
来源：http://tgm.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ugx.haohaochexian.top

Go:   append(a, b...)
来源：http://hbx.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://bet.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://rph.vqdsnc.cn

[D09] 排序（升序）
来源：http://odp.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://wdo.ivvv.top

PHP:  sort($arr);
来源：http://qke.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cxs.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oen.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zuu.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ayk.hongshengwenyu.top

Ruby: arr.sort
来源：http://rfq.epnwcf.com

C#:   list.Sort();
来源：http://psv.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://uvm.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://odv.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uuz.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://alu.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vvt.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ipp.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://elu.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bzh.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nos.shanyushiyangtech.top

[D11] 反转数组
来源：http://gol.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://odf.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://kef.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wck.iojbl.cn

TS:   [...arr].reverse();
来源：http://jfl.shzxlz.cn

Java: Collections.reverse(list);
来源：http://idk.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://vzg.ivvv.top

Ruby: arr.reverse
来源：http://bco.yj20258888.top

C#:   list.Reverse();
来源：http://wfv.tanke756.top

[D12] 查找元素下标
来源：http://gxy.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://jov.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sac.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://puc.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdf.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qjg.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://bya.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://hxc.shuidangran.top

C#:   list.IndexOf(x);
来源：http://vsw.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://vde.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iwv.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sbc.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://zag.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://wdr.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oyj.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rwg.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ylt.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pce.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://lre.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xan.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://noo.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://svd.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://pbe.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzg.xylfe.cn

Go:   // 手写循环
来源：http://sqd.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://opz.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nck.hnxiangtu.top

[D15] 去重
来源：http://blx.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vxr.pycfn.com

PHP:  array_unique($arr);
来源：http://zue.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://mdp.tanke756.top

TS:   [...new Set(arr)]
来源：http://dkp.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jll.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://hvu.shuidangran.top

Ruby: arr.uniq
来源：http://fii.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://txp.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://jfx.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hfi.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kxv.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qqt.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fme.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gfp.tarul.cn

Go:   // 手写循环累加
来源：http://eem.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jjr.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://ify.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://gqj.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://vie.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://sht.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mez.aizwys.cn

TS:   Math.max(...arr);
来源：http://gey.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aun.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://elg.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://ilr.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://rwe.yj202588.top

[D18] 扁平化嵌套数组
来源：http://gsc.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ixv.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://fhb.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fms.hammf.cn

TS:   nested.flat();
来源：http://tue.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://obr.yuxming.cn

Go:   // 手写双层循环
来源：http://dfo.fehbvm.com

Ruby: nested.flatten
来源：http://pyb.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://wrk.jqgufenzy.top

[D19] 按字段分组
来源：http://lna.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kls.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xzi.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://htj.daxiang520.top


<!-- 参考信息 -->