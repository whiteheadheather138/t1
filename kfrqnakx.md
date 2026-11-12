代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://jkt.guannengcc.top

[C07] 把函数作为参数传入
来源：http://vsr.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zqy.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://bux.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ctd.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://cqt.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kvc.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://abz.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://ucu.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vwz.ppjwa.cn

[C08] 闭包
来源：http://mhl.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://olt.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dyk.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zzm.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pry.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fea.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yry.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lxh.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://owe.yj20258888.top

[C09] 递归
来源：http://nwc.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iyp.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gma.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhu.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tja.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eam.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fdj.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hkk.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xeq.nanxinkj.top

[C10] 变量作用域
来源：http://ofr.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://inc.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fjy.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://agp.kuanghao11.cn

TS:   同 JS
来源：http://fql.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://rgm.zhengqikj.top

Go:   花括号块级作用域
来源：http://ddy.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jxm.316326.xyz

C#:   块级作用域
来源：http://vli.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://wwt.9152youxi.cn

Py:   from module import func
来源：http://qfs.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://ams.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://igd.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ssv.xuanzx.com

Java: import java.util.List;
来源：http://ecf.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ftl.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://cwn.52xcode.cn

C#:   using System.Text;
来源：http://xal.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://txl.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://nos.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://ttg.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://dyg.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://cin.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tdk.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://nqb.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://twr.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wos.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://hss.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://irl.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxa.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlu.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://apy.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://bgj.ivvv.top

Go:   func add(a, b int) int
来源：http://utq.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ssj.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://wyr.fktsv.cn

[C14] 泛型函数
来源：http://shb.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iel.tian-w.cn

PHP:  // 无泛型
来源：http://fjx.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://zmx.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nge.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pwa.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jie.xuanzx.com

Ruby: # 无泛型
来源：http://oif.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oft.fehbvm.com

[C15] 解构 / 展开参数
来源：http://gea.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dau.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://zez.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pgs.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://afq.nanxuanxn.top

Java: // 无解构
来源：http://oeu.ydjk.org.cn

Go:   // 无解构
来源：http://ujn.epnwcf.com

Ruby: a, b = pair
来源：http://ogs.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://ryz.yueranfly.top

[C16] 函数 / 方法重载
来源：http://ojk.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mhx.hnqzz.top

PHP:  // 无重载
来源：http://oow.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ost.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://nga.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ual.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://nux.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://qmg.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://esd.zdbjq.cn

================================================================================
来源：http://whx.hammf.cn

D. 数组 / 列表 / 集合
来源：http://viw.cashguo.top

================================================================================
来源：http://wdi.hnqzz.top

[D01] 创建数组 / 列表
来源：http://czk.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://enx.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uzq.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sfm.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ypx.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tcm.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://pny.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://zua.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qza.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://ixv.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yfi.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://afc.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://nmp.sweek.top

TS:   arr.push(4);
来源：http://yas.fengsongda.top

Java: list.add(4);
来源：http://oaq.yj202588.top

Go:   arr = append(arr, 4)
来源：http://nqg.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://tml.fengsongda.top

C#:   list.Add(4);
来源：http://eos.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://vwf.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://wlg.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ttl.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fpg.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://yqu.gotoacloud.top

Java: list.add(0, 0);
来源：http://gms.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://lul.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qua.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://lby.ybcxt.top

[D04] 删除元素
来源：http://tyl.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fzl.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://efe.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://leg.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://cmw.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqv.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kcm.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xsw.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ewy.guannengcc.top

[D05] 访问与修改元素
来源：http://efo.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tkk.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://guw.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://roi.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://zwx.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://dfh.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://tmb.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qvl.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jcz.daxiang520.top

[D06] 数组长度
来源：http://bgw.svipenyu.cn

Py:   len(arr)
来源：http://ohs.nwbrower.top

PHP:  count($arr);
来源：http://vry.yuanzhike.top

JS:   arr.length
来源：http://jur.daria6918.cn

TS:   arr.length
来源：http://wxk.ctjpmb.com

Java: list.size();
来源：http://zvc.hcnkem.com

Go:   len(arr)
来源：http://jxq.hammf.cn

Ruby: arr.length; arr.size
来源：http://msd.smart0.xyz

C#:   list.Count;
来源：http://lbm.jianghu66.top

[D07] 切片 / 取子数组
来源：http://asd.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jcp.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zcj.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://ell.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://wdc.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://rvn.chenlongwang.top

Go:   arr[1:4]
来源：http://dcs.dianchejie.cn

Ruby: arr[1, 3]
来源：http://wvh.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://jyr.gaohongyu789.top

[D08] 合并两个数组
来源：http://rdg.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://uil.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://dsj.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://egk.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://ewg.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jbp.yanxiufei.cn

Go:   append(a, b...)
来源：http://pok.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://xcm.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://car.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://yvy.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://rvf.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://gbn.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sot.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fgs.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://akm.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qdc.nwbrower.top

Ruby: arr.sort
来源：http://owo.cucudq.cn

C#:   list.Sort();
来源：http://pwh.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ajb.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vjo.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkg.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://adm.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ebp.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ksn.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fep.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wyo.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fgp.cdnleiting.top

[D11] 反转数组
来源：http://xlj.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qcm.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://vch.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xdk.ivvv.top

TS:   [...arr].reverse();
来源：http://uqy.xziqi.cn

Java: Collections.reverse(list);
来源：http://fni.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://vym.316326.xyz

Ruby: arr.reverse
来源：http://upq.vehdjk.com

C#:   list.Reverse();
来源：http://mek.zhixingplan.top

[D12] 查找元素下标
来源：http://gfc.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://vfg.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://evx.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcx.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xwg.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hit.birdmap.top

Go:   slices.Index(arr, x)
来源：http://atq.bbcook.cn

Ruby: arr.index(x)
来源：http://sec.yj20258888.top

C#:   list.IndexOf(x);
来源：http://drx.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://gbr.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dho.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://snh.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://qoq.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://gbo.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lip.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lcy.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bgd.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nrv.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://qyd.svipenyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://byf.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kgc.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://pfn.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://saf.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jqd.hesvh.cn

Go:   // 手写循环
来源：http://bcg.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://ozw.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wqw.svipenyu.cn

[D15] 去重
来源：http://vtp.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jhq.xylfe.cn

PHP:  array_unique($arr);
来源：http://fft.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://wnf.c1oappe.top

TS:   [...new Set(arr)]
来源：http://zyb.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ksv.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iti.meibo888.top

Ruby: arr.uniq
来源：http://nco.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://iev.nanxuanxn.top

[D16] 求和与平均值
来源：http://quw.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mfk.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ogb.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ufa.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kwv.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aqo.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://cyv.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emk.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://tnp.jiagoushi.top

[D17] 最大值与最小值
来源：http://upr.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://sbe.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://ncs.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://olz.aibaodan.cn

TS:   Math.max(...arr);
来源：http://lqg.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://irm.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ieu.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://fmp.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://ary.havefunace.top

[D18] 扁平化嵌套数组
来源：http://tmw.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sbo.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://bdu.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kya.ivvv.top

TS:   nested.flat();
来源：http://vsx.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sww.nwbrower.top

Go:   // 手写双层循环
来源：http://xdq.tianlin.xyz

Ruby: nested.flatten
来源：http://daj.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://myq.fehbvm.com

[D19] 按字段分组
来源：http://zfp.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zbr.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xcm.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://snq.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uec.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tdk.316326.xyz

Go:   // 手写 map[string][]T
来源：http://hsi.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ujp.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ijo.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://ots.daxiang520.top

Py:   Counter(arr)
来源：http://vro.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://bdn.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dws.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gzx.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hfi.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://sgg.iojbl.cn

Ruby: arr.tally
来源：http://aju.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lus.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://wga.zhixingplan.top

Py:   x in arr
来源：http://xqv.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://wdb.pycfn.com

JS:   arr.includes(x)
来源：http://wkv.mhx1999.top

TS:   arr.includes(x)
来源：http://uoe.hnxiangtu.top

Java: list.contains(x)
来源：http://vcf.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://wyl.hnqzz.top

Ruby: arr.include?(x)
来源：http://dgn.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://igd.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://dvf.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fsk.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fez.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sez.yvedp.cn

TS:   [...arr];
来源：http://tpy.vehdjk.com

Java: new ArrayList<>(list);
来源：http://wwn.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://kuz.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://lwu.yuxming.cn

C#:   new List<int>(list);
来源：http://tpy.daria6918.cn

[D23] reduce 累积计算
来源：http://cmf.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qrn.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zdi.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hku.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfj.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ffy.mhx1999.top

Go:   // 手写循环
来源：http://nru.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dkc.tarul.cn


<!-- 参考信息 -->