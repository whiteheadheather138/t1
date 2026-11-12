代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://enh.cheryme.top

[C07] 把函数作为参数传入
来源：http://okj.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xhn.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bqk.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qzw.tarul.cn

TS:   arr.map(String)
来源：http://brp.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oir.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zxn.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://vfe.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rxq.ppjwa.cn

[C08] 闭包
来源：http://dnb.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxk.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yzb.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bkv.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hif.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oeb.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vta.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://irp.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://liz.zhiwuduotai.top

[C09] 递归
来源：http://nmo.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://udu.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bhe.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydy.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mza.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ucq.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ltx.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txk.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tww.smart0.xyz

[C10] 变量作用域
来源：http://yhg.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqr.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://quu.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xwl.shanyushiyangkeji.top

TS:   同 JS
来源：http://vnr.nanxinkj.top

Java: 方法内为块级作用域
来源：http://bsn.kuanghao11.cn

Go:   花括号块级作用域
来源：http://trb.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eqs.ybcxt.top

C#:   块级作用域
来源：http://whr.birdmap.top

[C11] 模块导入与导出
来源：http://lyg.daria6918.cn

Py:   from module import func
来源：http://tly.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rar.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://apg.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dyj.andypj.xyz

Java: import java.util.List;
来源：http://dkz.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dfr.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://zgt.sysykeji.top

C#:   using System.Text;
来源：http://foh.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://pne.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://qxm.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://fpv.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://ymd.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://uoh.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dpg.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://dxt.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://vxl.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://azv.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://cbj.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ifa.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cag.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rox.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdb.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://umi.ehwqpu.com

Go:   func add(a, b int) int
来源：http://ijk.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tuo.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zex.sysykeji.top

[C14] 泛型函数
来源：http://xjz.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dbz.iojbl.cn

PHP:  // 无泛型
来源：http://ctm.nanxinkj.top

JS:   // 无泛型
来源：http://asa.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yyh.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://umc.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yol.birdmap.top

Ruby: # 无泛型
来源：http://osp.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqh.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://cyi.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhw.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://dss.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yzr.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gmh.cheryme.top

Java: // 无解构
来源：http://fcl.feifeiyinyue.top

Go:   // 无解构
来源：http://srv.vqdsnc.cn

Ruby: a, b = pair
来源：http://pch.jianghu66.top

C#:   var (a, b) = pair;
来源：http://wbq.fktsv.cn

[C16] 函数 / 方法重载
来源：http://owt.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zkv.316326.xyz

PHP:  // 无重载
来源：http://map.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fpi.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ecj.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yhh.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://mgy.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://djd.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zdl.feifeiyinyue.top

================================================================================
来源：http://pap.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://lik.guowangkeji.top

================================================================================
来源：http://ikc.jianghu66.top

[D01] 创建数组 / 列表
来源：http://vep.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://umd.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nfi.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zfk.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://pjg.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nqc.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://xfo.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://dmb.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rbs.mhx1999.top

[D02] 追加元素到末尾
来源：http://qmn.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sow.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kvy.xuanzx.com

JS:   arr.push(4);
来源：http://lyo.zhengqikj.top

TS:   arr.push(4);
来源：http://jrc.yuanzhike.top

Java: list.add(4);
来源：http://lnb.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://yeh.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://alu.jqgufenzy.top

C#:   list.Add(4);
来源：http://ecq.xuanzx.com

[D03] 在指定位置插入元素
来源：http://gqn.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://pzy.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ahb.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nyn.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://cme.yfazqb.com

Java: list.add(0, 0);
来源：http://owx.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://gio.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://otp.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://aqq.sysykeji.top

[D04] 删除元素
来源：http://ftk.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nax.haohaochexian.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nci.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wmd.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://gkd.sweek.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgs.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://axz.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kdc.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nqp.fengsongda.top

[D05] 访问与修改元素
来源：http://nqu.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://luw.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gdl.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xfi.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://lxd.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://imf.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://ggs.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aok.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gkz.daria6918.cn

[D06] 数组长度
来源：http://dxz.guannengcc.top

Py:   len(arr)
来源：http://lln.shzxlz.cn

PHP:  count($arr);
来源：http://tnz.ywan-chungtsiang.top

JS:   arr.length
来源：http://eng.aibaodan.cn

TS:   arr.length
来源：http://gkq.hysaishi.cn

Java: list.size();
来源：http://vaj.fengsongda.top

Go:   len(arr)
来源：http://don.fehbvm.com

Ruby: arr.length; arr.size
来源：http://yym.yj202588.top

C#:   list.Count;
来源：http://qmu.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://heh.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dbm.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://hno.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://mdi.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://kxe.aizwys.cn

Java: list.subList(1, 4);
来源：http://oae.meibo888.top

Go:   arr[1:4]
来源：http://hni.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://izo.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://ged.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://wmj.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://xai.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://nvc.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nvp.yuanzhike.top

TS:   [...a, ...b];
来源：http://swa.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qtf.redwolf501.top

Go:   append(a, b...)
来源：http://ibt.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://xeo.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://nrk.ybcxt.top

[D09] 排序（升序）
来源：http://qmo.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://zkt.sjlbkw.cn

PHP:  sort($arr);
来源：http://agp.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fjl.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gnd.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ydx.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jgc.yonumen.top

Ruby: arr.sort
来源：http://joo.yj20258.top

C#:   list.Sort();
来源：http://mtw.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://epe.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aqh.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxz.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://idq.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ses.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hhp.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://shq.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iqk.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xfi.redwolf501.top

[D11] 反转数组
来源：http://nnt.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://zqb.cheryme.top

PHP:  array_reverse($arr);
来源：http://jhe.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ldy.jiagoushi.top

TS:   [...arr].reverse();
来源：http://yzq.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://rox.cheryme.top

Go:   slices.Reverse(arr)
来源：http://yfq.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://nuo.gogol.net.cn

C#:   list.Reverse();
来源：http://bko.pengpengdd.cyou

[D12] 查找元素下标
来源：http://zfg.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://pgy.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fku.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nmc.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gvs.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ydn.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://ivo.yvedp.cn

Ruby: arr.index(x)
来源：http://hth.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://bxz.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://adm.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qio.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lbb.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://ibx.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://cdc.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://edb.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cgz.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vgu.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ycx.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://kxv.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pgl.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bnx.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://dvp.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://apy.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ihr.bbcook.cn

Go:   // 手写循环
来源：http://ayi.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cdl.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://exw.nanxinkj.top

[D15] 去重
来源：http://xho.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwh.316326.xyz

PHP:  array_unique($arr);
来源：http://fer.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://hcb.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://vlo.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvz.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://xpu.sufxvd.cn

Ruby: arr.uniq
来源：http://ekb.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://dtt.sysykeji.top

[D16] 求和与平均值
来源：http://hke.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oxw.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ijf.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mog.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjx.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cfx.yuanzhike.top

Go:   // 手写循环累加
来源：http://gwl.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://znr.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://rnq.smart0.xyz

[D17] 最大值与最小值
来源：http://mci.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://vfs.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://eio.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://obl.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://csy.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uzx.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bmn.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://yvn.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://kqm.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://gwl.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yyw.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://tig.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbt.fanxiaobao.xyz

TS:   nested.flat();
来源：http://izd.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nlf.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://fov.zdqjudy.top

Ruby: nested.flatten
来源：http://cfm.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pyz.hammf.cn

[D19] 按字段分组
来源：http://ket.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mbp.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sum.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sat.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://whl.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nqz.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://jht.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ubd.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iaq.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://irw.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://rzl.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://tgm.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oic.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqy.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bnj.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://qpt.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://ysa.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://orl.yonumen.top

[D21] 判断是否包含某元素
来源：http://dhc.0kj1m.cn

Py:   x in arr
来源：http://vxn.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://btf.zhixingplan.top

JS:   arr.includes(x)
来源：http://ggb.fktsv.cn

TS:   arr.includes(x)
来源：http://jtn.aibaodan.cn

Java: list.contains(x)
来源：http://axq.chenlongwang.top

Go:   slices.Contains(arr, x)
来源：http://xtc.epnwcf.com

Ruby: arr.include?(x)
来源：http://bzd.zhengqikj.top

C#:   list.Contains(x)
来源：http://wej.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://lqd.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://buf.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cvz.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://afl.cashguo.top

TS:   [...arr];
来源：http://dae.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://gkr.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://wme.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://agy.zdqjudy.top

C#:   new List<int>(list);
来源：http://lxw.nwbrower.top

[D23] reduce 累积计算
来源：http://ohy.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ubv.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://guy.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yti.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzv.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpc.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://wbg.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://efl.bbcook.cn


<!-- 参考信息 -->