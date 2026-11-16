代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpn.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zhm.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uco.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://trt.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://lgm.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jfz.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://hst.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xof.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://trh.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbd.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kig.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://yfo.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://rsn.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://ytx.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://doc.jyoumei.cn

[C05] 返回多个值
来源：http://nmr.jiagoushi.top

Py:   return a, b
来源：http://lrr.shuidangran.top

PHP:  return [$a, $b];
来源：http://uyd.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wcx.pycfn.com

TS:   return { a, b };
来源：http://auj.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rsw.aizwys.cn

Go:   return a, b
来源：http://hyw.wangshuangyany.cn

Ruby: return a, b
来源：http://sfr.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://ipl.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://jka.zycfv.cn

Py:   square = lambda x: x * x
来源：http://dga.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://you.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://lwc.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://rsv.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lnb.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iwv.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://oxx.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rjc.ivvv.top

[C07] 把函数作为参数传入
来源：http://lnl.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ply.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://snh.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://suk.andypj.xyz

TS:   arr.map(String)
来源：http://msp.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ewi.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ywl.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://qfz.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://imr.fehbvm.com

[C08] 闭包
来源：http://whi.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mkn.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://svm.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hnr.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://atm.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mfw.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dms.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qzn.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gta.wangdashe.top

[C09] 递归
来源：http://nyf.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pnp.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ppd.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://isx.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jid.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dpg.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aqi.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bfn.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lws.jqgfzy.top

[C10] 变量作用域
来源：http://duf.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rah.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xns.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mbe.kuanghao11.cn

TS:   同 JS
来源：http://nsu.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://bod.birdmap.top

Go:   花括号块级作用域
来源：http://yjs.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tik.zhongyouzk.top

C#:   块级作用域
来源：http://ewy.aizwys.cn

[C11] 模块导入与导出
来源：http://bap.sufxvd.cn

Py:   from module import func
来源：http://tmk.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phs.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vtf.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iwu.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://lpp.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zeo.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://ixt.gotoacloud.top

C#:   using System.Text;
来源：http://dun.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://fai.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://dap.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://jtm.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://omo.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://yte.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kus.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://cwp.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://wow.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mrt.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://dih.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fzm.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbz.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uvo.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jlx.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://qfz.jianghu66.top

Go:   func add(a, b int) int
来源：http://zci.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fjq.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://axw.ydzc1.top

[C14] 泛型函数
来源：http://adn.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ipb.iojbl.cn

PHP:  // 无泛型
来源：http://kzk.yanxiufei.cn

JS:   // 无泛型
来源：http://jzb.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ggx.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ujf.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qmt.hongshengwenyu.top

Ruby: # 无泛型
来源：http://gmn.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uyt.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://mwv.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jcn.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://zqf.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qwv.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iaf.meibo888.top

Java: // 无解构
来源：http://lpf.snrcjt.cn

Go:   // 无解构
来源：http://bcz.hongshengwenyu.top

Ruby: a, b = pair
来源：http://ehj.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://mgp.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://hjw.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tza.xylfe.cn

PHP:  // 无重载
来源：http://pyw.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nmk.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://ufc.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kpe.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://cgh.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://dwe.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzy.ppjwa.cn

================================================================================
来源：http://elg.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://fub.ybcxt.top

================================================================================
来源：http://ibw.ydzc1.top

[D01] 创建数组 / 列表
来源：http://rvi.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dsj.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfy.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rmk.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://dlu.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sog.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://vrc.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://awc.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vlr.yj20258888.top

[D02] 追加元素到末尾
来源：http://bio.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nje.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vhs.52xcode.cn

JS:   arr.push(4);
来源：http://ust.jiagoushi.top

TS:   arr.push(4);
来源：http://oyx.smart0.xyz

Java: list.add(4);
来源：http://zof.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://kfk.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://lta.yvedp.cn

C#:   list.Add(4);
来源：http://zol.aizwys.cn

[D03] 在指定位置插入元素
来源：http://vch.cheryme.top

Py:   arr.insert(0, 0)
来源：http://jhs.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xbg.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://weq.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://gvb.yongpay.top

Java: list.add(0, 0);
来源：http://neg.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fky.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vbg.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://igb.cheryme.top

[D04] 删除元素
来源：http://otq.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://teb.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mbz.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wxa.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://rrk.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tpw.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://npc.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zne.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bui.quarkkingdee.top

[D05] 访问与修改元素
来源：http://yjo.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iim.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hnu.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://elx.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://kly.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://rwe.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xtr.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ehq.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wgs.zhaomingkeji.xyz

[D06] 数组长度
来源：http://doo.yueranfly.top

Py:   len(arr)
来源：http://tjm.cashguo.top

PHP:  count($arr);
来源：http://yng.nanxuanxn.top

JS:   arr.length
来源：http://aoo.dashuyun.cn

TS:   arr.length
来源：http://eyc.birdmap.top

Java: list.size();
来源：http://erx.52xcode.cn

Go:   len(arr)
来源：http://isp.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://nqn.fanxiaobao.xyz

C#:   list.Count;
来源：http://ylp.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://yav.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mlt.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://mnl.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://jue.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://wba.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://fto.yonumen.top

Go:   arr[1:4]
来源：http://epd.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://smz.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://gjl.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://xcf.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://woo.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://jqx.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ocu.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://rwn.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xkn.dianchejie.cn

Go:   append(a, b...)
来源：http://dch.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://car.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://jyg.ydzc1.top

[D09] 排序（升序）
来源：http://qrj.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://jgx.xziqi.cn

PHP:  sort($arr);
来源：http://irf.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pxd.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iuf.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://clq.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nok.epnwcf.com

Ruby: arr.sort
来源：http://rbt.yj20258888.top

C#:   list.Sort();
来源：http://ekh.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oek.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jlm.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gop.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfr.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jmj.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fck.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gab.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rpd.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ngf.zhaomingkeji.xyz

[D11] 反转数组
来源：http://rkg.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://pyr.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://gli.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qaq.yj202588.top

TS:   [...arr].reverse();
来源：http://kpa.xuanzx.com

Java: Collections.reverse(list);
来源：http://kum.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://cvp.hfpthk.cn

Ruby: arr.reverse
来源：http://vpc.bbcook.cn

C#:   list.Reverse();
来源：http://pnj.wangdashe.top

[D12] 查找元素下标
来源：http://eld.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://wkv.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ynz.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pge.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmx.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qqn.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://ghv.ydjk.org.cn

Ruby: arr.index(x)
来源：http://plt.andypj.xyz

C#:   list.IndexOf(x);
来源：http://vhk.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://rur.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zzz.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zmm.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://znx.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://lyi.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yzb.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jyr.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xjn.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mgg.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://roa.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mpp.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tjs.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://nre.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://ots.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwy.wangdashe.top

Go:   // 手写循环
来源：http://xod.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://lmq.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aml.tian-w.cn

[D15] 去重
来源：http://jua.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gjq.chenlongwang.top

PHP:  array_unique($arr);
来源：http://mnq.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://ekg.aizwys.cn

TS:   [...new Set(arr)]
来源：http://ojz.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dxt.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yqy.ydjk.org.cn

Ruby: arr.uniq
来源：http://mzd.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://ztn.snrcjt.cn

[D16] 求和与平均值
来源：http://jzl.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xpb.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yjv.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jby.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewk.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pwe.zhongyouzk.top

Go:   // 手写循环累加
来源：http://euz.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vvd.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://fdg.aibaodan.cn

[D17] 最大值与最小值
来源：http://sla.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://nsg.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://xii.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://quf.sufxvd.cn

TS:   Math.max(...arr);
来源：http://yfa.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ojy.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qoo.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://pht.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://yys.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://bgs.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jsf.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://syu.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zwx.zhongyouzk.top

TS:   nested.flat();
来源：http://gni.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozn.zhijiandao.cn

Go:   // 手写双层循环
来源：http://prx.xuetiantiany.cn

Ruby: nested.flatten
来源：http://frv.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ytj.sjlbkw.cn

[D19] 按字段分组
来源：http://lzq.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://now.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yyq.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kwe.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tme.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://duj.havefunace.top

Go:   // 手写 map[string][]T
来源：http://dda.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://rjk.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aoo.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://gvd.jqgufenzy.top

Py:   Counter(arr)
来源：http://qtb.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://vvc.redwolf501.top


<!-- 参考信息 -->