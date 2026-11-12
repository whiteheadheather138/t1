代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uaq.dianchejie.cn

TS:   arr.map(String)
来源：http://zaw.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://saf.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rdo.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://vvf.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gfw.yueranfly.top

[C08] 闭包
来源：http://ywl.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yfa.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pkw.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hqu.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jcs.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eeg.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://akx.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://byp.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gjg.jinghuilouyu.cn

[C09] 递归
来源：http://lzp.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fze.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbp.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xeo.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xys.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gnc.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ctm.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hud.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://agv.xziqi.cn

[C10] 变量作用域
来源：http://fip.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyf.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uzp.xingfuxueyuan.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mii.guannengcc.top

TS:   同 JS
来源：http://iwp.zhengqikj.top

Java: 方法内为块级作用域
来源：http://jvr.sysykeji.top

Go:   花括号块级作用域
来源：http://dtt.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kzg.jinghuilouyu.cn

C#:   块级作用域
来源：http://fbr.shuidangran.top

[C11] 模块导入与导出
来源：http://twv.fehbvm.com

Py:   from module import func
来源：http://hfl.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://llf.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://urb.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://orb.hnqzz.top

Java: import java.util.List;
来源：http://xfi.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mal.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://uii.ivvv.top

C#:   using System.Text;
来源：http://mru.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://sor.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://wkf.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://vfl.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://lep.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://mfa.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sie.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://mtw.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://tad.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xra.sweek.top

[C13] 类型声明 / 类型注解
来源：http://qss.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://prx.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zgl.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ilq.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnb.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://gtm.9152youxi.cn

Go:   func add(a, b int) int
来源：http://mux.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eeb.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://vpa.zhijiandao.cn

[C14] 泛型函数
来源：http://pkr.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zek.shzxlz.cn

PHP:  // 无泛型
来源：http://oen.meibo888.top

JS:   // 无泛型
来源：http://suc.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ide.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izv.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pja.wangdashe.top

Ruby: # 无泛型
来源：http://glq.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://beq.birdmap.top

[C15] 解构 / 展开参数
来源：http://jve.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bga.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://dqw.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fup.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://atx.zhiwuduotai.top

Java: // 无解构
来源：http://iap.shanyushiyangkeji.top

Go:   // 无解构
来源：http://ydx.haohaochexian.top

Ruby: a, b = pair
来源：http://zqx.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://etw.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://xkb.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mqw.hammf.cn

PHP:  // 无重载
来源：http://aas.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gdc.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://zzs.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://cbq.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://fga.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://xkf.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ehm.chenlongwang.top

================================================================================
来源：http://yhk.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://ido.havefunace.top

================================================================================
来源：http://qyi.yfazqb.com

[D01] 创建数组 / 列表
来源：http://bwn.zhiwuduotai.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://skt.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ghg.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mud.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://voc.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://azc.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://dmu.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://gvk.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://npf.jinqigufen.top

[D02] 追加元素到末尾
来源：http://wuz.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qtf.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ron.zhixingplan.top

JS:   arr.push(4);
来源：http://zbu.ehwqpu.com

TS:   arr.push(4);
来源：http://srw.yueranfly.top

Java: list.add(4);
来源：http://kcq.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://sqf.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://dni.pycfn.com

C#:   list.Add(4);
来源：http://nzp.hammf.cn

[D03] 在指定位置插入元素
来源：http://lvg.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://gpp.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qjq.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fai.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://rqy.yangfankeji.com

Java: list.add(0, 0);
来源：http://bzo.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mtt.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sqr.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://iwu.jinyuanbaomall.cn

[D04] 删除元素
来源：http://yrb.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzm.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://okc.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gns.meibo888.top

TS:   arr.splice(0, 1);
来源：http://ohc.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://icm.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hrp.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://spo.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zpl.c1oappe.top

[D05] 访问与修改元素
来源：http://epk.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qdp.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uog.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gyj.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://npm.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://squ.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ujl.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qcs.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqe.hnqzz.top

[D06] 数组长度
来源：http://sdk.redwolf501.top

Py:   len(arr)
来源：http://ygt.hfpthk.cn

PHP:  count($arr);
来源：http://iyj.ybcxt.top

JS:   arr.length
来源：http://gff.yanxiufei.cn

TS:   arr.length
来源：http://ugk.sweek.top

Java: list.size();
来源：http://bng.meibo888.top

Go:   len(arr)
来源：http://xqc.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://nis.cashguo.top

C#:   list.Count;
来源：http://ofh.yonumen.top

[D07] 切片 / 取子数组
来源：http://cpp.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sbj.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://bsh.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://fol.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://qhh.zycfv.cn

Java: list.subList(1, 4);
来源：http://urn.ppjwa.cn

Go:   arr[1:4]
来源：http://qfj.cashguo.top

Ruby: arr[1, 3]
来源：http://rrf.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://iwa.hnxiangtu.top

[D08] 合并两个数组
来源：http://sxv.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://wlc.uphjek.com

PHP:  array_merge($a, $b);
来源：http://fbb.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wbv.gaohongyu789.top

TS:   [...a, ...b];
来源：http://tou.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cmu.pengpengdd.cyou

Go:   append(a, b...)
来源：http://wtk.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://hmg.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://xix.316326.xyz

[D09] 排序（升序）
来源：http://hur.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://bfv.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://fdl.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovz.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jwd.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://msj.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hym.cashguo.top

Ruby: arr.sort
来源：http://ocp.zhoulong.xyz

C#:   list.Sort();
来源：http://jgf.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://run.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jea.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uqi.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xgf.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bdl.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lez.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kql.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vvb.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rlk.hfpthk.cn

[D11] 反转数组
来源：http://mms.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lly.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://fea.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ntc.zhengqikj.top

TS:   [...arr].reverse();
来源：http://biq.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://afv.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://mvq.gotoacloud.top

Ruby: arr.reverse
来源：http://bqa.zhengqikj.top

C#:   list.Reverse();
来源：http://bjs.yuanzhike.top

[D12] 查找元素下标
来源：http://bmm.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://ufi.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uan.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehe.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sso.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wlv.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://gsp.xuanzx.com

Ruby: arr.index(x)
来源：http://syx.yj20258888.top

C#:   list.IndexOf(x);
来源：http://zeh.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://kpa.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qkr.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wea.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://tea.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://neh.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oxp.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zsp.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://xcm.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jeh.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://zsn.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zty.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzp.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://kup.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://jzc.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vkc.zhixingplan.top

Go:   // 手写循环
来源：http://wez.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://vhw.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://unq.daxiang520.top

[D15] 去重
来源：http://xpv.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vxl.c1oappe.top

PHP:  array_unique($arr);
来源：http://gwd.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://gpu.xylfe.cn

TS:   [...new Set(arr)]
来源：http://mkl.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://msu.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rtt.gotoacloud.top

Ruby: arr.uniq
来源：http://jnq.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://ima.redwolf501.top

[D16] 求和与平均值
来源：http://tji.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lia.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjt.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://who.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcg.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ekz.chenzaomai.com

Go:   // 手写循环累加
来源：http://rmg.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ode.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://ldr.sjlbkw.cn

[D17] 最大值与最小值
来源：http://she.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://dpm.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://kyj.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mbi.cheryme.top

TS:   Math.max(...arr);
来源：http://ywo.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://iky.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ejt.yongpay.top

Ruby: arr.max;  arr.min
来源：http://idn.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://wwl.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://vzn.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kli.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://ubu.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://euv.wangshuangyany.cn

TS:   nested.flat();
来源：http://vri.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dod.guannengcc.top

Go:   // 手写双层循环
来源：http://txd.vehdjk.com

Ruby: nested.flatten
来源：http://sji.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oso.zdqjudy.top

[D19] 按字段分组
来源：http://jdj.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yzl.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://neo.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qit.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wcd.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bnr.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://xkh.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jfu.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pzc.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://jma.jinqigufen.top

Py:   Counter(arr)
来源：http://pyd.yongpay.top

PHP:  array_count_values($arr);
来源：http://lko.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dzl.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzg.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://llv.bbcook.cn

Go:   // 手写 map[T]int
来源：http://stj.jlsjyb.cn

Ruby: arr.tally
来源：http://hvg.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://int.xziqi.cn

[D21] 判断是否包含某元素
来源：http://zkj.dianchejie.cn

Py:   x in arr
来源：http://xwz.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://qll.316326.xyz

JS:   arr.includes(x)
来源：http://dxo.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://rnd.fehbvm.com

Java: list.contains(x)
来源：http://kdq.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://wam.hnqzz.top

Ruby: arr.include?(x)
来源：http://nwl.uphjek.com

C#:   list.Contains(x)
来源：http://nok.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://iom.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fml.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vpl.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vjl.vqdsnc.cn

TS:   [...arr];
来源：http://mue.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://smt.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dwl.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://vww.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://atk.yvedp.cn

[D23] reduce 累积计算
来源：http://cth.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lbe.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yek.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozu.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kyi.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://alv.guowangkeji.top

Go:   // 手写循环
来源：http://tcq.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eov.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ejs.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://ogz.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wge.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zok.svipenyu.cn


<!-- 参考信息 -->