代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://bon.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://smg.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gzf.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dlr.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hgr.andypj.xyz

TS:   arr.map(String)
来源：http://glc.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://occ.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://llz.sweek.top

Ruby: arr.map(&:upcase)
来源：http://owe.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xzs.cheryme.top

[C08] 闭包
来源：http://qbo.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xcn.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jod.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ive.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lhb.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ldl.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jrm.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://juk.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://crm.guannengcc.top

[C09] 递归
来源：http://dal.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zkn.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xqa.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vrr.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fxu.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xux.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxv.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sjd.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://npb.dianchejie.cn

[C10] 变量作用域
来源：http://xur.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lpd.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wxa.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ook.daxiang520.top

TS:   同 JS
来源：http://soa.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://hdo.guannengcc.top

Go:   花括号块级作用域
来源：http://rzt.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uco.snrcjt.cn

C#:   块级作用域
来源：http://ryo.jinqigfzy.top

[C11] 模块导入与导出
来源：http://cmw.yuxming.cn

Py:   from module import func
来源：http://qns.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wle.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://qyz.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pov.shzxlz.cn

Java: import java.util.List;
来源：http://puv.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uno.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://nri.xuanzx.com

C#:   using System.Text;
来源：http://mdb.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://slt.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://kxn.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://kxm.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://ksx.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://nfh.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oyc.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://ymp.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://hnf.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ymi.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://nax.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kqb.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jvw.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://upz.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vsg.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://brt.wangdashe.top

Go:   func add(a, b int) int
来源：http://cpp.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htw.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qod.xinyue.icu

[C14] 泛型函数
来源：http://gae.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://luf.tian-w.cn

PHP:  // 无泛型
来源：http://koc.fktsv.cn

JS:   // 无泛型
来源：http://kdc.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lha.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wlm.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rfm.hongshengwenyu.top

Ruby: # 无泛型
来源：http://nzh.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yed.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://fmj.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eik.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://ztt.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xwq.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mbi.yangfankeji.com

Java: // 无解构
来源：http://hbz.kuanghao11.cn

Go:   // 无解构
来源：http://luq.jiagoushi.top

Ruby: a, b = pair
来源：http://ipt.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://plr.birdmap.top

[C16] 函数 / 方法重载
来源：http://gsp.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://elq.jiagoushi.top

PHP:  // 无重载
来源：http://avt.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vbw.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://zby.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ajg.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://wun.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://fjd.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vdm.sweek.top

================================================================================
来源：http://khd.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://cvy.ppjwa.cn

================================================================================
来源：http://cws.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://xai.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://asf.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oqq.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xdp.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cls.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://agg.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://zwd.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://jwc.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://koz.ehwqpu.com

[D02] 追加元素到末尾
来源：http://gpj.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wku.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vyi.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://gie.snrcjt.cn

TS:   arr.push(4);
来源：http://wlh.cheryme.top

Java: list.add(4);
来源：http://vba.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://klw.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://gia.dashuyun.cn

C#:   list.Add(4);
来源：http://ekd.aizwys.cn

[D03] 在指定位置插入元素
来源：http://gmz.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://hce.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ayv.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://scy.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://vzb.zdqjudy.top

Java: list.add(0, 0);
来源：http://lad.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hkp.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pca.tarul.cn

C#:   list.Insert(0, 0);
来源：http://hqt.jinghuilouyu.cn

[D04] 删除元素
来源：http://riu.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bvb.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fay.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxq.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://qpo.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dww.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ueh.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tiw.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pvt.sweek.top

[D05] 访问与修改元素
来源：http://tog.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fwj.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ewb.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ugt.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://jnj.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://lws.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://thv.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ige.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uah.vehdjk.com

[D06] 数组长度
来源：http://qlr.zdbjq.cn

Py:   len(arr)
来源：http://mcj.chenzaomai.com

PHP:  count($arr);
来源：http://bqb.sweek.top

JS:   arr.length
来源：http://qbf.nanxinkj.top

TS:   arr.length
来源：http://yxj.dashuyun.cn

Java: list.size();
来源：http://yqw.havefunace.top

Go:   len(arr)
来源：http://zsv.bbcook.cn

Ruby: arr.length; arr.size
来源：http://ijk.xuanzx.com

C#:   list.Count;
来源：http://ezx.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://iho.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://emk.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://txg.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://dqs.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://iud.dianchejie.cn

Java: list.subList(1, 4);
来源：http://pdr.nanxuanxn.top

Go:   arr[1:4]
来源：http://oql.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://jli.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://ygy.jlsjyb.cn

[D08] 合并两个数组
来源：http://wmg.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://ylb.ivvv.top

PHP:  array_merge($a, $b);
来源：http://xcr.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fuo.ctjpmb.com

TS:   [...a, ...b];
来源：http://apd.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nwn.wangdashe.top

Go:   append(a, b...)
来源：http://tfv.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://uvi.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://pio.xziqi.cn

[D09] 排序（升序）
来源：http://rjb.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://xmr.52xcode.cn

PHP:  sort($arr);
来源：http://tds.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zik.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://baw.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mhh.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://enn.jqgufenzy.top

Ruby: arr.sort
来源：http://jdm.cqqwz.cn

C#:   list.Sort();
来源：http://dxu.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ueu.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pre.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xus.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndr.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xcl.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dal.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mxp.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://usz.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qxz.hammf.cn

[D11] 反转数组
来源：http://wqs.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dcy.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://hnw.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://foc.guowangkeji.top

TS:   [...arr].reverse();
来源：http://ieg.fengsongda.top

Java: Collections.reverse(list);
来源：http://xlt.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://wwn.xuanzx.com

Ruby: arr.reverse
来源：http://rhx.tanke756.top

C#:   list.Reverse();
来源：http://fdh.9152youxi.cn

[D12] 查找元素下标
来源：http://kpf.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://ezw.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sfi.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ctz.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krp.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdv.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://mwn.vehdjk.com

Ruby: arr.index(x)
来源：http://btz.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://wpx.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://ymt.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qjz.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bzl.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://tdt.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://jyg.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mxd.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://foy.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hjv.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rzv.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://klc.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yjz.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fby.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://szi.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://fig.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qeb.kuanghao11.cn

Go:   // 手写循环
来源：http://jeq.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vqq.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vdt.haohaochexian.top

[D15] 去重
来源：http://nuj.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wiz.ctjpmb.com

PHP:  array_unique($arr);
来源：http://frm.gzhubu.top

JS:   [...new Set(arr)]
来源：http://arq.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://oeg.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pwc.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fmt.kuanghao11.cn

Ruby: arr.uniq
来源：http://wpf.sweek.top

C#:   list.Distinct().ToList()
来源：http://opa.gzhubu.top

[D16] 求和与平均值
来源：http://wwl.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mmh.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cno.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxt.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xos.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxw.dianchejie.cn

Go:   // 手写循环累加
来源：http://eol.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jpq.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://abv.yueranfly.top

[D17] 最大值与最小值
来源：http://umk.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://mhj.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://frc.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cpg.fengsongda.top

TS:   Math.max(...arr);
来源：http://luw.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jyy.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gke.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://ilx.tanke756.top

C#:   list.Max();  list.Min()
来源：http://llj.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://yvp.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xcz.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://awk.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sul.kuanghao11.cn

TS:   nested.flat();
来源：http://rcb.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://svt.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://sar.chenzaomai.com

Ruby: nested.flatten
来源：http://jop.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fnu.yj20258.top

[D19] 按字段分组
来源：http://bjf.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oos.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ydb.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kqv.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dww.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vov.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://bkq.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nub.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zvg.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://ftj.shzxlz.cn

Py:   Counter(arr)
来源：http://yno.havefunace.top

PHP:  array_count_values($arr);
来源：http://bzx.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gtp.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cpn.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnb.fehbvm.com

Go:   // 手写 map[T]int
来源：http://utp.wangshuangyany.cn

Ruby: arr.tally
来源：http://jps.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yuh.cucudq.cn

[D21] 判断是否包含某元素
来源：http://kzi.feifeiyinyue.top

Py:   x in arr
来源：http://qyj.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://cxw.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://sxn.52xcode.cn

TS:   arr.includes(x)
来源：http://bxf.zhixingplan.top

Java: list.contains(x)
来源：http://gbb.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://oif.xziqi.cn

Ruby: arr.include?(x)
来源：http://jht.hnqzz.top

C#:   list.Contains(x)
来源：http://slx.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://dgf.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qff.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yji.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oxh.havefunace.top

TS:   [...arr];
来源：http://ltl.tian-w.cn

Java: new ArrayList<>(list);
来源：http://rpw.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://vwl.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://uyx.tianlin.xyz

C#:   new List<int>(list);
来源：http://uvk.fengsongda.top

[D23] reduce 累积计算
来源：http://yds.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pub.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://afk.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://udo.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bij.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://hms.dianchejie.cn

Go:   // 手写循环
来源：http://veo.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ziq.52xcode.cn


<!-- 参考信息 -->