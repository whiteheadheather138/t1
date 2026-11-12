代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://arg.cheryme.top

[C07] 把函数作为参数传入
来源：http://txq.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ydp.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dbg.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vze.hammf.cn

TS:   arr.map(String)
来源：http://kch.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itb.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hrq.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://ols.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kze.sysykeji.top

[C08] 闭包
来源：http://cfz.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wpw.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dkj.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nkh.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksb.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zmr.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bpw.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oyc.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qtv.dashuyun.cn

[C09] 递归
来源：http://avk.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fes.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xte.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kpd.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gfl.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dsz.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vde.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cdf.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hnu.meibo888.top

[C10] 变量作用域
来源：http://sby.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://quu.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fdc.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wag.52xcode.cn

TS:   同 JS
来源：http://zsn.bbcook.cn

Java: 方法内为块级作用域
来源：http://xqh.redwolf501.top

Go:   花括号块级作用域
来源：http://puk.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ynt.jqgufenzy.top

C#:   块级作用域
来源：http://yjd.hnxiangtu.top

[C11] 模块导入与导出
来源：http://mvy.andypj.xyz

Py:   from module import func
来源：http://log.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pts.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cbt.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wcp.cdnleiting.top

Java: import java.util.List;
来源：http://rwc.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ocd.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://pkb.yvedp.cn

C#:   using System.Text;
来源：http://syj.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://hvd.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://kzc.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://uez.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://zgg.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://mrj.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgu.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://njz.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://qeg.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bhs.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://nmf.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nst.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oqg.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nsw.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcy.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://flr.bjfxy.top

Go:   func add(a, b int) int
来源：http://owm.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nrc.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wlz.sweek.top

[C14] 泛型函数
来源：http://nva.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yjf.zhixingplan.top

PHP:  // 无泛型
来源：http://qiw.yangfankeji.com

JS:   // 无泛型
来源：http://osv.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fsq.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vyc.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ubd.shuidangran.top

Ruby: # 无泛型
来源：http://paw.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mmp.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://cbh.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ubc.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://igk.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://frz.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zkc.xylfe.cn

Java: // 无解构
来源：http://ihu.zhaomingkeji.xyz

Go:   // 无解构
来源：http://yhu.tarul.cn

Ruby: a, b = pair
来源：http://njn.tanke756.top

C#:   var (a, b) = pair;
来源：http://wyb.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://mli.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vno.fanxiaobao.xyz

PHP:  // 无重载
来源：http://vxd.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://krv.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://tid.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://whu.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://zep.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://ezf.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://vmc.hywenlv.cn

================================================================================
来源：http://mrc.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://don.jinghuilouyu.cn

================================================================================
来源：http://sal.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://sjj.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xgk.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://orn.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rko.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zqe.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nvd.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://pwc.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://thb.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xno.zhixingplan.top

[D02] 追加元素到末尾
来源：http://rso.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lte.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rme.tianlin.xyz

JS:   arr.push(4);
来源：http://lkc.havefunace.top

TS:   arr.push(4);
来源：http://onr.redwolf501.top

Java: list.add(4);
来源：http://zns.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://eye.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://hub.xuetiantiany.cn

C#:   list.Add(4);
来源：http://bim.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://cpp.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://cfk.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdb.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dgi.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://vko.sysykeji.top

Java: list.add(0, 0);
来源：http://gzw.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://ivh.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqg.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://smp.0kj1m.cn

[D04] 删除元素
来源：http://izm.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxq.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wjk.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cdr.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://mhd.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hma.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uzr.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqy.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://typ.jinqigufen.top

[D05] 访问与修改元素
来源：http://tat.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://psw.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zlq.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gks.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://uoj.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://igx.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://trc.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kez.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://akk.shangyingyoupin.top

[D06] 数组长度
来源：http://kkv.yangfankeji.com

Py:   len(arr)
来源：http://hsi.haohaochexian.top

PHP:  count($arr);
来源：http://aex.fehbvm.com

JS:   arr.length
来源：http://gch.hcnkem.com

TS:   arr.length
来源：http://zpb.316326.xyz

Java: list.size();
来源：http://fjn.wangshuangyany.cn

Go:   len(arr)
来源：http://kst.iojbl.cn

Ruby: arr.length; arr.size
来源：http://kut.jqgfzy.top

C#:   list.Count;
来源：http://jue.fktsv.cn

[D07] 切片 / 取子数组
来源：http://fzu.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://avr.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://nbt.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://wad.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://aps.tianlin.xyz

Java: list.subList(1, 4);
来源：http://xsi.cucudq.cn

Go:   arr[1:4]
来源：http://upd.xziqi.cn

Ruby: arr[1, 3]
来源：http://dlo.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://ekd.yj20258.top

[D08] 合并两个数组
来源：http://vuw.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://bdq.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://cds.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dpy.tanke756.top

TS:   [...a, ...b];
来源：http://bks.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oja.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://laj.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://lsu.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://nkh.316326.xyz

[D09] 排序（升序）
来源：http://bsn.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://kiq.yvedp.cn

PHP:  sort($arr);
来源：http://nec.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pvj.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ogm.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mll.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pit.jqgfzy.top

Ruby: arr.sort
来源：http://gbu.fehbvm.com

C#:   list.Sort();
来源：http://nxj.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ezj.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ibq.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iva.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://svy.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oep.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qgz.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mai.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pjc.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uir.zhijiandao.cn

[D11] 反转数组
来源：http://dud.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://flt.yj202588.top

PHP:  array_reverse($arr);
来源：http://eyj.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://djv.epnwcf.com

TS:   [...arr].reverse();
来源：http://vyt.hnqzz.top

Java: Collections.reverse(list);
来源：http://avt.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://ltx.yangfankeji.com

Ruby: arr.reverse
来源：http://bzc.zhiwuduotai.top

C#:   list.Reverse();
来源：http://jbz.chenzaomai.com

[D12] 查找元素下标
来源：http://drh.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://nsq.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sne.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pox.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpf.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://onx.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://csn.fehbvm.com

Ruby: arr.index(x)
来源：http://vir.xylfe.cn

C#:   list.IndexOf(x);
来源：http://jek.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://dab.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://juo.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wjz.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://tvn.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://ozg.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pcl.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fri.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://sfk.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kim.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://ofy.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://udv.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bxh.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://ily.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://xak.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mbc.yvedp.cn

Go:   // 手写循环
来源：http://svj.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://dlx.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://asf.jinyuanbaomall.cn

[D15] 去重
来源：http://ajn.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zeh.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://piq.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://smg.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://vjo.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dxi.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://gcm.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://qww.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://idq.sufxvd.cn

[D16] 求和与平均值
来源：http://mcg.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hkm.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tvi.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://avd.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fsh.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://udj.zhengqikj.top

Go:   // 手写循环累加
来源：http://xhb.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fet.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://sjd.yvedp.cn

[D17] 最大值与最小值
来源：http://wqt.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://lyh.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://wla.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sne.bjfxy.top

TS:   Math.max(...arr);
来源：http://pah.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ybi.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jaf.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://kqv.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://bnu.pycfn.com

[D18] 扁平化嵌套数组
来源：http://jmz.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yaz.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://fuq.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iir.bjfxy.top

TS:   nested.flat();
来源：http://gmd.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eij.yfazqb.com

Go:   // 手写双层循环
来源：http://kfe.tanke756.top

Ruby: nested.flatten
来源：http://xwu.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fen.ppjwa.cn

[D19] 按字段分组
来源：http://qrq.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lfv.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zib.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ize.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eoc.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yts.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://cwk.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wuf.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ffn.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://rzd.fktsv.cn

Py:   Counter(arr)
来源：http://ikf.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://hod.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vqo.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gsw.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://psc.tanke756.top

Go:   // 手写 map[T]int
来源：http://fut.epnwcf.com

Ruby: arr.tally
来源：http://mvl.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hde.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://otg.vqdsnc.cn

Py:   x in arr
来源：http://cac.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://vqk.hnxiangtu.top

JS:   arr.includes(x)
来源：http://pqj.yanxiufei.cn

TS:   arr.includes(x)
来源：http://kzl.aibaodan.cn

Java: list.contains(x)
来源：http://ffn.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://rrq.gzhubu.top

Ruby: arr.include?(x)
来源：http://wfm.guannengcc.top

C#:   list.Contains(x)
来源：http://oue.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://pgo.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wkt.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agw.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nhs.cheryme.top

TS:   [...arr];
来源：http://cro.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://ktb.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://wbh.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://byq.xuanzx.com

C#:   new List<int>(list);
来源：http://nfr.hnqzz.top

[D23] reduce 累积计算
来源：http://snx.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uph.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://szv.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://txn.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcw.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://win.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://pir.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kmt.jianghu66.top


<!-- 参考信息 -->