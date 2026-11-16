代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://dym.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://axn.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://iqx.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://jry.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ngi.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://btv.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nln.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://cdc.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vii.jinqigufen.top

TS:   arr.map(String)
来源：http://xpy.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://haz.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hsa.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://wwd.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://mkr.bjfxy.top

[C08] 闭包
来源：http://rch.gogol.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vgj.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pkr.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uru.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://thz.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kba.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zmh.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlx.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oma.yfazqb.com

[C09] 递归
来源：http://kzw.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fkb.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rae.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rll.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxo.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vey.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wkt.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yyv.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jtz.nanxinkj.top

[C10] 变量作用域
来源：http://iin.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jmb.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwu.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uqg.nanxinkj.top

TS:   同 JS
来源：http://etx.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://jbx.yj20258888.top

Go:   花括号块级作用域
来源：http://kgq.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xkp.zhaomingkeji.xyz

C#:   块级作用域
来源：http://ycg.haohaochexian.top

[C11] 模块导入与导出
来源：http://edw.hammf.cn

Py:   from module import func
来源：http://qwb.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qaz.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hgi.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xnm.zycfv.cn

Java: import java.util.List;
来源：http://xmc.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ecf.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://fis.gzhubu.top

C#:   using System.Text;
来源：http://ndh.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://pwc.sweek.top

Py:   (lambda: print("run"))()
来源：http://ifs.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://ema.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://phs.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://pml.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://acp.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://hqm.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://yfo.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://jje.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://gos.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rnb.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdn.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tbp.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oce.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://pdw.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://nru.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nxm.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://tkj.fengsongda.top

[C14] 泛型函数
来源：http://adz.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kgz.dashuyun.cn

PHP:  // 无泛型
来源：http://gtw.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://jrz.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xnp.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rhu.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ekm.pengpengdd.cyou

Ruby: # 无泛型
来源：http://okz.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pll.meibo888.top

[C15] 解构 / 展开参数
来源：http://wev.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nuh.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://wzg.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tqy.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://epl.nanxinkj.top

Java: // 无解构
来源：http://ipl.cdnleiting.top

Go:   // 无解构
来源：http://dur.yonumen.top

Ruby: a, b = pair
来源：http://rst.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://bfo.wangdashe.top

[C16] 函数 / 方法重载
来源：http://tky.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nyz.jlsjyb.cn

PHP:  // 无重载
来源：http://aqg.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jgj.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://kkz.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rob.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://shw.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://epc.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://hbq.hysaishi.cn

================================================================================
来源：http://nfx.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://nyu.yangfankeji.com

================================================================================
来源：http://eyk.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://ofd.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tyn.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akz.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pzs.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://pnu.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wgr.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://fdk.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://enq.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xep.guowangkeji.top

[D02] 追加元素到末尾
来源：http://vnp.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vfg.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ict.hfpthk.cn

JS:   arr.push(4);
来源：http://ubm.quarkkingdee.top

TS:   arr.push(4);
来源：http://tvf.dashuyun.cn

Java: list.add(4);
来源：http://fym.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://jmw.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://dgo.ivvv.top

C#:   list.Add(4);
来源：http://jdu.zycfv.cn

[D03] 在指定位置插入元素
来源：http://mey.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://zrt.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xtg.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vvm.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://vav.smart0.xyz

Java: list.add(0, 0);
来源：http://bgj.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://lir.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://woi.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://cdr.ppjwa.cn

[D04] 删除元素
来源：http://wdx.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vga.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qvh.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pqn.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://sal.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rch.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqq.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://azf.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zpu.yuanzhike.top

[D05] 访问与修改元素
来源：http://dcx.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://csy.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rou.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pyf.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://xhq.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://ema.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://zlr.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ccr.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yuf.snrcjt.cn

[D06] 数组长度
来源：http://hys.xuanzx.com

Py:   len(arr)
来源：http://olz.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://wyy.zhiwuduotai.top

JS:   arr.length
来源：http://ics.yj20258888.top

TS:   arr.length
来源：http://irn.uphjek.com

Java: list.size();
来源：http://abj.0kj1m.cn

Go:   len(arr)
来源：http://bka.xuanzx.com

Ruby: arr.length; arr.size
来源：http://atr.pycfn.com

C#:   list.Count;
来源：http://ahe.yonumen.top

[D07] 切片 / 取子数组
来源：http://vir.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://beq.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://npl.yonumen.top

JS:   arr.slice(1, 4);
来源：http://htp.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://ihz.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://teu.bbcook.cn

Go:   arr[1:4]
来源：http://oqs.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://aci.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://dxm.sjlbkw.cn

[D08] 合并两个数组
来源：http://yvu.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://xur.hammf.cn

PHP:  array_merge($a, $b);
来源：http://dbp.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eqw.9152youxi.cn

TS:   [...a, ...b];
来源：http://qfo.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://koi.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://goa.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://njw.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://jen.jinqigufen.top

[D09] 排序（升序）
来源：http://jjt.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://hbq.gogol.net.cn

PHP:  sort($arr);
来源：http://lvc.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zoi.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kfv.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pdn.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yat.tarul.cn

Ruby: arr.sort
来源：http://jsi.yj202588.top

C#:   list.Sort();
来源：http://ajn.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fzi.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqt.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekc.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qae.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwn.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://biz.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ohd.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qqg.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zwl.hammf.cn

[D11] 反转数组
来源：http://cxy.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://vrs.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://vxn.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bjs.yuxming.cn

TS:   [...arr].reverse();
来源：http://plt.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://sns.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://vxx.hysaishi.cn

Ruby: arr.reverse
来源：http://ctj.chenzaomai.com

C#:   list.Reverse();
来源：http://nkq.vqdsnc.cn

[D12] 查找元素下标
来源：http://mtb.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://tao.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nco.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djj.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kbj.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dht.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://wgs.cucudq.cn

Ruby: arr.index(x)
来源：http://ydy.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://dym.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://opr.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ooj.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://owj.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://zox.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://bqb.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kjm.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://avy.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cdb.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gom.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://hjg.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vdj.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yta.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://omf.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://drg.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mgx.iojbl.cn

Go:   // 手写循环
来源：http://dqb.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://jtg.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://meb.wangshuangyany.cn

[D15] 去重
来源：http://ldg.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nft.tarul.cn

PHP:  array_unique($arr);
来源：http://xvi.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://gxz.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://jhz.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zpw.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://kmo.vehdjk.com

Ruby: arr.uniq
来源：http://vrk.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://lqj.nwbrower.top

[D16] 求和与平均值
来源：http://gtv.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wyn.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://equ.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sni.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nlt.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oja.iojbl.cn

Go:   // 手写循环累加
来源：http://vwd.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jsl.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://zdx.meibo888.top

[D17] 最大值与最小值
来源：http://cgj.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://rce.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://hin.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ccn.cdnleiting.top

TS:   Math.max(...arr);
来源：http://vau.chenjidiqi.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://kgm.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ryo.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://qyz.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://nzj.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://nrb.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fpk.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://jnx.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://shx.birdmap.top

TS:   nested.flat();
来源：http://uvy.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zuy.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://cen.hnqzz.top

Ruby: nested.flatten
来源：http://qso.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ljw.guannengcc.top

[D19] 按字段分组
来源：http://qcc.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ewf.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mii.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vlm.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://keh.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xbv.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://akm.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vhr.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oyf.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://whm.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://ptg.tian-w.cn

PHP:  array_count_values($arr);
来源：http://cdl.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwp.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxe.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://str.fehbvm.com

Go:   // 手写 map[T]int
来源：http://aof.sxryk.cn

Ruby: arr.tally
来源：http://okt.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hsq.xuanzx.com

[D21] 判断是否包含某元素
来源：http://bvp.jlsjyb.cn

Py:   x in arr
来源：http://cvz.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://jmd.jyoumei.cn

JS:   arr.includes(x)
来源：http://tpt.zhixingplan.top

TS:   arr.includes(x)
来源：http://nnf.snrcjt.cn

Java: list.contains(x)
来源：http://jvu.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://jvf.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://pbu.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://gcg.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://hkw.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ekt.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://smt.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfe.tian-w.cn

TS:   [...arr];
来源：http://zfr.aizwys.cn

Java: new ArrayList<>(list);
来源：http://frm.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hwi.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://evy.havefunace.top

C#:   new List<int>(list);
来源：http://ueo.jianghu66.top

[D23] reduce 累积计算
来源：http://kja.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://klq.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://okp.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ocn.cdnleiting.top


<!-- 参考信息 -->