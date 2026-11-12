代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zmo.zhiwuduotai.top

Go:   return a, b
来源：http://rhq.kuanghao11.cn

Ruby: return a, b
来源：http://crd.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://xvu.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://pqf.meibo888.top

Py:   square = lambda x: x * x
来源：http://ugh.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://auj.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://enp.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://lbl.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://elb.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://faf.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://ioz.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://bzc.daria6918.cn

[C07] 把函数作为参数传入
来源：http://odz.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sbc.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://kun.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://igl.zhijiandao.cn

TS:   arr.map(String)
来源：http://awf.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://agi.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mzr.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://yzw.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://afd.bbcook.cn

[C08] 闭包
来源：http://vvg.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ygh.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tpy.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wmj.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://slx.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sig.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kmc.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dun.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjc.jyoumei.cn

[C09] 递归
来源：http://hps.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qtk.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yti.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jiu.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hsw.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hth.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gau.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cfd.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pgy.jianghu66.top

[C10] 变量作用域
来源：http://txu.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mpv.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfo.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rwn.jqgufenzy.top

TS:   同 JS
来源：http://nsa.cdnleiting.top

Java: 方法内为块级作用域
来源：http://urt.andypj.xyz

Go:   花括号块级作用域
来源：http://pss.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lil.zhaomingkeji.xyz

C#:   块级作用域
来源：http://tmp.xuanzx.com

[C11] 模块导入与导出
来源：http://szl.chenjidiqi.icu

Py:   from module import func
来源：http://rrc.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ccq.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wxs.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zrt.zhengqikj.top

Java: import java.util.List;
来源：http://pbu.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://idw.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://wuw.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://psv.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://vrb.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://prp.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://sna.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://msu.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://xtj.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://asm.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://mry.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://sxw.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ypc.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://cqh.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jee.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qoc.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ojg.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxy.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yvg.cashguo.top

Go:   func add(a, b int) int
来源：http://gnr.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kgi.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zux.epnwcf.com

[C14] 泛型函数
来源：http://izg.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://phj.zhijiandao.cn

PHP:  // 无泛型
来源：http://tul.yongpay.top

JS:   // 无泛型
来源：http://ycs.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tog.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jep.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oub.guowangkeji.top

Ruby: # 无泛型
来源：http://cgw.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bvz.cheryme.top

[C15] 解构 / 展开参数
来源：http://tja.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ctk.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://qkr.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vhl.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://itj.yueranfly.top

Java: // 无解构
来源：http://igq.yueranfly.top

Go:   // 无解构
来源：http://yev.sxryk.cn

Ruby: a, b = pair
来源：http://xdg.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://fdg.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://wih.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gyh.jinqigfzy.top

PHP:  // 无重载
来源：http://sur.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sdb.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://meh.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://znl.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://fpm.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://cgs.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yor.shangyingyoupin.top

================================================================================
来源：http://lsz.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://vsa.bbcook.cn

================================================================================
来源：http://xub.sysykeji.top

[D01] 创建数组 / 列表
来源：http://zmy.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://exb.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://etd.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ryf.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uwn.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nfg.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://yts.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://rqt.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zst.vehdjk.com

[D02] 追加元素到末尾
来源：http://psc.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://azt.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szg.jinqigufen.top

JS:   arr.push(4);
来源：http://twv.wangshuangyany.cn

TS:   arr.push(4);
来源：http://tdj.quarkkingdee.top

Java: list.add(4);
来源：http://mmk.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://qax.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ohm.yj20258888.top

C#:   list.Add(4);
来源：http://kwu.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://duy.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://vrj.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://col.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gdb.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://mgz.c1oappe.top

Java: list.add(0, 0);
来源：http://jzk.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://uqr.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uii.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://ozf.hywenlv.cn

[D04] 删除元素
来源：http://kcm.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vui.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uwb.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nay.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://rly.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mdo.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ukc.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ezj.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xwf.jqgufenzy.top

[D05] 访问与修改元素
来源：http://bpz.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jpx.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://srj.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cxf.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://sjz.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://tfk.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://mcu.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xmh.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fou.fktsv.cn

[D06] 数组长度
来源：http://hpf.yj20258888.top

Py:   len(arr)
来源：http://qwz.yongpay.top

PHP:  count($arr);
来源：http://eri.xylfe.cn

JS:   arr.length
来源：http://bmv.xingfuxueyuan.xyz

TS:   arr.length
来源：http://stl.ivvv.top

Java: list.size();
来源：http://oee.yj20258888.top

Go:   len(arr)
来源：http://gxa.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://rgh.svipenyu.cn

C#:   list.Count;
来源：http://sdv.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://cmu.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rmm.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://ncp.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://vdk.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://frz.yueranfly.top

Java: list.subList(1, 4);
来源：http://fkq.hnqzz.top

Go:   arr[1:4]
来源：http://geo.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://rsr.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://rmu.birdmap.top

[D08] 合并两个数组
来源：http://vai.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://guf.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://wek.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://evm.chenzaomai.com

TS:   [...a, ...b];
来源：http://jrl.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iwy.zhiwuduotai.top

Go:   append(a, b...)
来源：http://qfo.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://lss.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://wso.vqdsnc.cn

[D09] 排序（升序）
来源：http://sgo.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://hqr.ydzc1.top

PHP:  sort($arr);
来源：http://cmi.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjj.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ayj.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ozo.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wpx.hnqzz.top

Ruby: arr.sort
来源：http://qjf.bbcook.cn

C#:   list.Sort();
来源：http://cdd.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wop.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rfa.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iyz.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://teu.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://khb.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nhu.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dgu.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rlh.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hsb.smart0.xyz

[D11] 反转数组
来源：http://yhw.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://haa.fktsv.cn

PHP:  array_reverse($arr);
来源：http://aya.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ajd.jqgfzy.top

TS:   [...arr].reverse();
来源：http://xrq.316326.xyz

Java: Collections.reverse(list);
来源：http://yly.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://sgg.zhoulong.xyz

Ruby: arr.reverse
来源：http://ofr.zdbjq.cn

C#:   list.Reverse();
来源：http://wnq.iojbl.cn

[D12] 查找元素下标
来源：http://acf.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://cni.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lal.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvc.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nnd.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sgt.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://kwp.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://vnc.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://tad.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://tvn.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sog.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fsq.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://obm.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://ohr.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wbz.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyu.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://tqg.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pqs.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://czs.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://olo.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vdz.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://avp.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://rmk.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqv.aizwys.cn

Go:   // 手写循环
来源：http://xsg.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://sab.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ixw.wangshuangyany.cn

[D15] 去重
来源：http://fwe.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://urk.52xcode.cn

PHP:  array_unique($arr);
来源：http://wav.sxryk.cn

JS:   [...new Set(arr)]
来源：http://kwt.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://jyx.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mgl.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://vlg.316326.xyz

Ruby: arr.uniq
来源：http://ucz.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://eho.snrcjt.cn

[D16] 求和与平均值
来源：http://trm.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfe.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbb.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ylg.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yyi.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://niq.yueranfly.top

Go:   // 手写循环累加
来源：http://ssk.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://udm.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://grx.aibaodan.cn

[D17] 最大值与最小值
来源：http://gwg.pycfn.com

Py:   max(arr);  min(arr)
来源：http://lqh.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://mme.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dbo.smart0.xyz

TS:   Math.max(...arr);
来源：http://opf.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://whm.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxp.cashguo.top

Ruby: arr.max;  arr.min
来源：http://uli.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://lyd.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://gyk.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xsb.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://dcn.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sjo.jyoumei.cn

TS:   nested.flat();
来源：http://rar.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iqa.zhijiandao.cn

Go:   // 手写双层循环
来源：http://roy.ydzc1.top

Ruby: nested.flatten
来源：http://noe.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://bny.vehdjk.com

[D19] 按字段分组
来源：http://wih.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xyp.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddo.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yqe.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iop.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://moz.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://vtw.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lkq.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ass.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://zjd.guannengcc.top

Py:   Counter(arr)
来源：http://crj.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://eji.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nwr.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esb.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://omo.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://omp.chenzaomai.com

Ruby: arr.tally
来源：http://kbe.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pbk.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://zrj.zhixingplan.top

Py:   x in arr
来源：http://udu.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://rcm.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://qqc.zdbjq.cn

TS:   arr.includes(x)
来源：http://ekj.yongpay.top

Java: list.contains(x)
来源：http://nzs.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://lyk.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://bsp.nanxinkj.top

C#:   list.Contains(x)
来源：http://jmw.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://nks.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yuf.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hcf.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uip.birdmap.top

TS:   [...arr];
来源：http://hfl.yongpay.top


<!-- 参考信息 -->