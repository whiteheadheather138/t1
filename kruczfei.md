代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffd.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ver.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uns.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajz.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://lof.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jzr.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://xbi.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wnj.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yom.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nlb.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jlp.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://ikb.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://bdv.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://zvz.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://lcb.svipenyu.cn

[C05] 返回多个值
来源：http://etz.quarkkingdee.top

Py:   return a, b
来源：http://awl.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://vmr.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgm.smart0.xyz

TS:   return { a, b };
来源：http://wjg.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uns.fanxiaobao.xyz

Go:   return a, b
来源：http://qil.andypj.xyz

Ruby: return a, b
来源：http://ifl.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://qcb.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://agr.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://zbr.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ldy.hesvh.cn

JS:   const square = x => x * x;
来源：http://csd.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://ajh.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rke.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://tav.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://ruj.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://oje.guannengcc.top

[C07] 把函数作为参数传入
来源：http://wvn.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dmo.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://zea.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jkj.iojbl.cn

TS:   arr.map(String)
来源：http://ptg.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aoq.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://elv.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://ysh.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hcr.hfpthk.cn

[C08] 闭包
来源：http://nbd.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://utr.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbr.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dmg.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jzn.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kyr.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xvb.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qzs.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hal.chenjidiqi.icu

[C09] 递归
来源：http://ati.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zvm.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xkv.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbv.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxz.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kqe.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jka.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzx.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kju.nanxuanxn.top

[C10] 变量作用域
来源：http://mnf.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gxh.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://inr.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iok.0kj1m.cn

TS:   同 JS
来源：http://jdq.vehdjk.com

Java: 方法内为块级作用域
来源：http://dgu.smart0.xyz

Go:   花括号块级作用域
来源：http://rlg.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://axt.chenzaomai.com

C#:   块级作用域
来源：http://tqz.fehbvm.com

[C11] 模块导入与导出
来源：http://mvd.meibo888.top

Py:   from module import func
来源：http://zxn.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yep.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eom.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rmi.daria6918.cn

Java: import java.util.List;
来源：http://jzb.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vul.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://vfu.iojbl.cn

C#:   using System.Text;
来源：http://ilc.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://plf.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://vww.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://keb.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://pbl.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://vpn.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kbu.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://zjj.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://blb.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tai.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://ppn.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://csx.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://amt.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jmf.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wkc.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oju.hammf.cn

Go:   func add(a, b int) int
来源：http://esa.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ynr.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cfr.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://vhp.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tgb.hcnkem.com

PHP:  // 无泛型
来源：http://jln.zdbjq.cn

JS:   // 无泛型
来源：http://gcy.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tlv.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nrt.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gjg.nanxuanxn.top

Ruby: # 无泛型
来源：http://dyk.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://upk.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://kme.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kgy.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://fio.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hmi.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bgl.jianghu66.top

Java: // 无解构
来源：http://jqe.xinyue.icu

Go:   // 无解构
来源：http://lkw.jlsjyb.cn

Ruby: a, b = pair
来源：http://xeq.mhx1999.top

C#:   var (a, b) = pair;
来源：http://yme.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://vph.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ooj.hnxiangtu.top

PHP:  // 无重载
来源：http://jkw.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bnr.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://xuv.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bqu.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://mxi.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://gwu.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dfs.yueranfly.top

================================================================================
来源：http://moc.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://nri.yongpay.top

================================================================================
来源：http://oac.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://shd.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dvn.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hkm.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://igj.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dfg.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bne.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://zff.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://njv.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zkn.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://wnd.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wym.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kih.jqgufenzy.top

JS:   arr.push(4);
来源：http://xlq.dianchejie.cn

TS:   arr.push(4);
来源：http://dop.hfpthk.cn

Java: list.add(4);
来源：http://lqh.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://vfm.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://kxx.feifeiyinyue.top

C#:   list.Add(4);
来源：http://lrj.vehdjk.com

[D03] 在指定位置插入元素
来源：http://wih.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://ybo.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://loc.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qmv.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://bhf.ivvv.top

Java: list.add(0, 0);
来源：http://gnc.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uyi.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nqx.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://zxm.xinyue.icu

[D04] 删除元素
来源：http://ywz.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nzx.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lsi.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xqv.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://ryg.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xbr.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jro.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yjy.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wcx.sweek.top

[D05] 访问与修改元素
来源：http://abo.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://toj.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zdf.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vkl.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://imt.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://pqc.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://zkm.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ubl.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pdk.jyoumei.cn

[D06] 数组长度
来源：http://kqa.sufxvd.cn

Py:   len(arr)
来源：http://zkx.sweek.top

PHP:  count($arr);
来源：http://nvm.iojbl.cn

JS:   arr.length
来源：http://ksu.jinghuilouyu.cn

TS:   arr.length
来源：http://myz.daria6918.cn

Java: list.size();
来源：http://sar.chenzaomai.com

Go:   len(arr)
来源：http://nod.shuidangran.top

Ruby: arr.length; arr.size
来源：http://xka.shzxlz.cn

C#:   list.Count;
来源：http://uiy.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://uvw.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lsu.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://ium.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://der.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://xxl.xinyue.icu

Java: list.subList(1, 4);
来源：http://isb.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://ebx.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://puz.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://dnp.sxryk.cn

[D08] 合并两个数组
来源：http://hwc.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://imr.cheryme.top

PHP:  array_merge($a, $b);
来源：http://unu.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bvu.zycfv.cn

TS:   [...a, ...b];
来源：http://tzk.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eeb.guowangkeji.top

Go:   append(a, b...)
来源：http://cfx.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://adu.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://uza.vehdjk.com

[D09] 排序（升序）
来源：http://rxh.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://vvf.pycfn.com

PHP:  sort($arr);
来源：http://bdk.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ees.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cvv.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dwc.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uyo.gaohongyu789.top

Ruby: arr.sort
来源：http://qta.meibo888.top

C#:   list.Sort();
来源：http://ots.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihh.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oxd.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fqv.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrd.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdz.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyy.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tmh.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xre.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qhh.fktsv.cn

[D11] 反转数组
来源：http://grj.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://sjw.yonumen.top

PHP:  array_reverse($arr);
来源：http://lmh.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phz.fzhhl.top

TS:   [...arr].reverse();
来源：http://hkn.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://cjp.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://asq.jqgufenzy.top

Ruby: arr.reverse
来源：http://pqb.cqqwz.cn

C#:   list.Reverse();
来源：http://oye.epnwcf.com

[D12] 查找元素下标
来源：http://cmw.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://bmf.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rpv.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxo.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iat.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://coq.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://lcy.meibo888.top

Ruby: arr.index(x)
来源：http://vsy.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://vrd.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://yah.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ord.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ltm.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://gec.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://lbc.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfw.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://itq.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://yar.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xwu.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://eng.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hfa.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tmb.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://hyc.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://fos.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://gfz.hysaishi.cn

Go:   // 手写循环
来源：http://eqn.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kzw.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rjm.ivvv.top

[D15] 去重
来源：http://ica.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tmz.ydzc1.top

PHP:  array_unique($arr);
来源：http://ppp.cucudq.cn

JS:   [...new Set(arr)]
来源：http://deb.xinyue.icu

TS:   [...new Set(arr)]
来源：http://gfj.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uoq.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://xgx.haohaochexian.top

Ruby: arr.uniq
来源：http://dbk.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://mab.nanxinkj.top

[D16] 求和与平均值
来源：http://szu.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hlz.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ifk.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://akh.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sen.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bon.kuanghao11.cn

Go:   // 手写循环累加
来源：http://ygo.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vna.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://mgx.hcnkem.com

[D17] 最大值与最小值
来源：http://bhm.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://wnj.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://qxz.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://clp.redwolf501.top

TS:   Math.max(...arr);
来源：http://nad.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ycy.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qjt.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://jek.hammf.cn

C#:   list.Max();  list.Min()
来源：http://ris.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://ngt.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bfp.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://rcv.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jnc.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://xwf.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pjd.vehdjk.com

Go:   // 手写双层循环
来源：http://tco.jianghu66.top

Ruby: nested.flatten
来源：http://eey.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ztz.yueranfly.top

[D19] 按字段分组
来源：http://xcp.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eyw.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bui.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kxz.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pne.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hep.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://ymj.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rza.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbm.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://emz.gotoacloud.top

Py:   Counter(arr)
来源：http://kla.xylfe.cn

PHP:  array_count_values($arr);
来源：http://yzh.fzhhl.top


<!-- 参考信息 -->