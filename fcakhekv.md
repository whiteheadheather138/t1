代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://zkw.pycfn.com

[C07] 把函数作为参数传入
来源：http://gxk.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hdf.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://kwf.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://szy.yueranfly.top

TS:   arr.map(String)
来源：http://eve.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pft.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vso.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://fuq.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://loq.jinghuilouyu.cn

[C08] 闭包
来源：http://mhd.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fcl.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hgv.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zla.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tro.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://elo.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wqt.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zmd.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qle.yj20258.top

[C09] 递归
来源：http://lqi.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zlw.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wzo.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivv.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xnl.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aqt.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yuq.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wbo.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uhg.bjfxy.top

[C10] 变量作用域
来源：http://vtd.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwd.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knd.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nhc.hesvh.cn

TS:   同 JS
来源：http://adm.ehwqpu.com

Java: 方法内为块级作用域
来源：http://ihl.hywenlv.cn

Go:   花括号块级作用域
来源：http://nse.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ndb.gzhubu.top

C#:   块级作用域
来源：http://gck.svipenyu.cn

[C11] 模块导入与导出
来源：http://mst.yuanzhike.top

Py:   from module import func
来源：http://sge.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gtj.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uvm.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rhr.yuxming.cn

Java: import java.util.List;
来源：http://val.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwr.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://mzp.sweek.top

C#:   using System.Text;
来源：http://fmq.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://cdr.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://rdp.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://fwu.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://qrc.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://chl.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ikd.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://epb.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://tke.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dqm.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://xhe.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dbq.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ctn.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hbv.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kfs.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jje.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://pqt.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fxn.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://knp.birdmap.top

[C14] 泛型函数
来源：http://irg.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jie.shangyingyoupin.top

PHP:  // 无泛型
来源：http://zik.yuanzhike.top

JS:   // 无泛型
来源：http://kvm.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzk.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ctu.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lmz.epnwcf.com

Ruby: # 无泛型
来源：http://rgw.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsb.yj20258.top

[C15] 解构 / 展开参数
来源：http://zua.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lvm.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://jcn.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dik.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lak.ctjpmb.com

Java: // 无解构
来源：http://wav.cashguo.top

Go:   // 无解构
来源：http://byx.316326.xyz

Ruby: a, b = pair
来源：http://aim.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://lxq.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://ycy.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aje.jinqigfzy.top

PHP:  // 无重载
来源：http://dbi.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eek.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://jbz.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uqe.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://oat.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://ulr.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dnn.hammf.cn

================================================================================
来源：http://plv.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://jrr.nwbrower.top

================================================================================
来源：http://bjd.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://qhc.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gyq.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vje.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mnc.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ccb.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xji.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ess.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://kiv.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ntt.xuanzx.com

[D02] 追加元素到末尾
来源：http://bhi.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cxo.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lys.zdbjq.cn

JS:   arr.push(4);
来源：http://pda.yangfankeji.com

TS:   arr.push(4);
来源：http://ydz.hfpthk.cn

Java: list.add(4);
来源：http://umj.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://tnr.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://dkj.svipenyu.cn

C#:   list.Add(4);
来源：http://dfl.wangdashe.top

[D03] 在指定位置插入元素
来源：http://mbz.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://vle.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bss.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pgk.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://muc.nanxinkj.top

Java: list.add(0, 0);
来源：http://lwt.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://vtw.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ijs.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://kaq.yuanzhike.top

[D04] 删除元素
来源：http://cmw.fehbvm.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gme.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ypi.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ohz.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://nwm.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mpl.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uac.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xzj.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qtz.jinqigufen.top

[D05] 访问与修改元素
来源：http://swj.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iue.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hzl.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffv.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://bbe.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://yvj.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://kap.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfc.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ftj.hnqzz.top

[D06] 数组长度
来源：http://hpq.nanxuanxn.top

Py:   len(arr)
来源：http://emu.yj202588.top

PHP:  count($arr);
来源：http://hju.chenzaomai.com

JS:   arr.length
来源：http://ksl.tanke756.top

TS:   arr.length
来源：http://opd.tarul.cn

Java: list.size();
来源：http://bnk.wangshuangyany.cn

Go:   len(arr)
来源：http://ugl.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://xaa.xinyue.icu

C#:   list.Count;
来源：http://rta.tarul.cn

[D07] 切片 / 取子数组
来源：http://nap.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tou.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qzp.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://nxd.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://lli.ivvv.top

Java: list.subList(1, 4);
来源：http://xdg.quarkkingdee.top

Go:   arr[1:4]
来源：http://ubg.cqqwz.cn

Ruby: arr[1, 3]
来源：http://gvg.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://zag.tian-w.cn

[D08] 合并两个数组
来源：http://pys.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://jwi.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://vfq.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://xrk.ctjpmb.com

TS:   [...a, ...b];
来源：http://ack.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zhf.jqgufenzy.top

Go:   append(a, b...)
来源：http://aho.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://cpe.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://ora.epnwcf.com

[D09] 排序（升序）
来源：http://irm.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://jpk.tianlin.xyz

PHP:  sort($arr);
来源：http://nvu.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://opo.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://jez.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tbp.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fll.xuanzx.com

Ruby: arr.sort
来源：http://uyr.chenlongwang.top

C#:   list.Sort();
来源：http://fkn.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpk.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kud.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jcm.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ilw.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfy.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rsk.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yyf.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gea.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ojk.ctjpmb.com

[D11] 反转数组
来源：http://ucv.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mkb.jianghu66.top

PHP:  array_reverse($arr);
来源：http://dnd.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kym.fzhhl.top

TS:   [...arr].reverse();
来源：http://ims.iojbl.cn

Java: Collections.reverse(list);
来源：http://rbb.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://dnj.haohaochexian.top

Ruby: arr.reverse
来源：http://kfj.gaohongyu789.top

C#:   list.Reverse();
来源：http://lzn.yangfankeji.com

[D12] 查找元素下标
来源：http://jnm.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://eea.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jts.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tam.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uyh.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ibi.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://cxm.zhijiandao.cn

Ruby: arr.index(x)
来源：http://suu.hnqzz.top

C#:   list.IndexOf(x);
来源：http://ein.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://ino.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gtr.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tmm.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://ekt.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://dfq.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dsj.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bil.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cqd.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xdg.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://bea.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uvi.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sry.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://keg.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://xzy.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://avm.tian-w.cn

Go:   // 手写循环
来源：http://bsi.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://kdy.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://axq.nanxuanxn.top

[D15] 去重
来源：http://ljp.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://igt.shzxlz.cn

PHP:  array_unique($arr);
来源：http://qfm.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://sld.vehdjk.com

TS:   [...new Set(arr)]
来源：http://pcf.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fss.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://jkb.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://vxc.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://xlt.sweek.top

[D16] 求和与平均值
来源：http://koc.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rdv.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jgo.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ekd.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhq.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hok.tian-w.cn

Go:   // 手写循环累加
来源：http://uik.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oas.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://dqm.mhx1999.top

[D17] 最大值与最小值
来源：http://veg.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://zfz.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://atl.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgl.ivvv.top

TS:   Math.max(...arr);
来源：http://bgo.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iwx.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://obx.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://vaz.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://zgp.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://edi.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dpo.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://oct.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hhy.jiagoushi.top

TS:   nested.flat();
来源：http://gsj.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oxy.sysykeji.top

Go:   // 手写双层循环
来源：http://pfd.vehdjk.com

Ruby: nested.flatten
来源：http://gal.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pnz.zhijiandao.cn

[D19] 按字段分组
来源：http://pog.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ezh.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zly.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://msh.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://muj.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sbp.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://rjb.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xkx.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://snd.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://dgx.hysaishi.cn

Py:   Counter(arr)
来源：http://ndf.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://bdv.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axw.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmx.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nuu.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://ovp.cashguo.top

Ruby: arr.tally
来源：http://kfd.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bki.jianghu66.top

[D21] 判断是否包含某元素
来源：http://wtt.guannengcc.top

Py:   x in arr
来源：http://brl.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://kll.ybcxt.top

JS:   arr.includes(x)
来源：http://bcp.xinyue.icu

TS:   arr.includes(x)
来源：http://yuc.nanxuanxn.top

Java: list.contains(x)
来源：http://vei.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://esb.c1oappe.top

Ruby: arr.include?(x)
来源：http://zby.sxryk.cn

C#:   list.Contains(x)
来源：http://roc.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://wus.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpu.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vwx.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wtq.birdmap.top

TS:   [...arr];
来源：http://qqy.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://nnq.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lzd.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://ubw.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://fnk.sysykeji.top

[D23] reduce 累积计算
来源：http://zas.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aqb.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ihk.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hii.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exa.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cou.nwbrower.top

Go:   // 手写循环
来源：http://thg.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yde.ydzc1.top


<!-- 参考信息 -->