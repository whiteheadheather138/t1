代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://bcn.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qaj.zhengqikj.top

[C08] 闭包
来源：http://lnp.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aqy.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rys.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://keb.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fya.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yko.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qke.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eez.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hnd.guowangkeji.top

[C09] 递归
来源：http://jms.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kfr.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://csa.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ane.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iio.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mje.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://whv.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vzg.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pye.yj20258888.top

[C10] 变量作用域
来源：http://usy.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wfh.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://phf.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wcz.jinqigufen.top

TS:   同 JS
来源：http://zxy.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://yrr.andypj.xyz

Go:   花括号块级作用域
来源：http://src.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nis.xylfe.cn

C#:   块级作用域
来源：http://ans.gzhubu.top

[C11] 模块导入与导出
来源：http://saa.shanyushiyangkeji.top

Py:   from module import func
来源：http://rka.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vgj.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vxx.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://klb.zhijiandao.cn

Java: import java.util.List;
来源：http://cpv.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tfx.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://woa.birdmap.top

C#:   using System.Text;
来源：http://woq.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://kcn.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://wub.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://mow.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://vxa.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://vks.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fgc.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://wzg.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://ybx.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ojy.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://qql.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ega.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aoj.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vra.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcw.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ett.cdnleiting.top

Go:   func add(a, b int) int
来源：http://olm.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hlw.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://eam.hnxiangtu.top

[C14] 泛型函数
来源：http://bop.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://voy.shangyingyoupin.top

PHP:  // 无泛型
来源：http://ubz.sweek.top

JS:   // 无泛型
来源：http://lrx.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rht.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wzi.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqt.pengpengdd.cyou

Ruby: # 无泛型
来源：http://rxs.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gda.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://bkq.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rrh.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://fvp.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dlj.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gxd.52xcode.cn

Java: // 无解构
来源：http://gpo.pycfn.com

Go:   // 无解构
来源：http://lan.52xcode.cn

Ruby: a, b = pair
来源：http://mbh.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://vyk.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://dhv.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vbq.cashguo.top

PHP:  // 无重载
来源：http://ltt.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mcb.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://efd.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wfp.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://nvd.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://nqe.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cvy.tarul.cn

================================================================================
来源：http://ets.cheryme.top

D. 数组 / 列表 / 集合
来源：http://wpq.zhengqikj.top

================================================================================
来源：http://ynw.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://pga.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tcb.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tzh.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rvz.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lel.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fiu.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://msi.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://ahh.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://glj.yonumen.top

[D02] 追加元素到末尾
来源：http://dxr.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lgg.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gkj.ehwqpu.com

JS:   arr.push(4);
来源：http://ivm.kuanghao11.cn

TS:   arr.push(4);
来源：http://jxf.ivvv.top

Java: list.add(4);
来源：http://fxc.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://pgo.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://ork.cheryme.top

C#:   list.Add(4);
来源：http://ntb.yueranfly.top

[D03] 在指定位置插入元素
来源：http://vxm.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://qbj.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fip.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://klw.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://eon.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://clf.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://uxi.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://muf.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://dfu.yuxming.cn

[D04] 删除元素
来源：http://lby.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qsh.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmg.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ndx.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://qcd.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vle.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qng.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hxb.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ldl.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://wxz.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mcf.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rcq.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://won.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://wgt.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://jzt.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://uto.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ytp.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://igt.hammf.cn

[D06] 数组长度
来源：http://muw.0kj1m.cn

Py:   len(arr)
来源：http://ejl.zhengqikj.top

PHP:  count($arr);
来源：http://nas.zhoulong.xyz

JS:   arr.length
来源：http://fxo.yfazqb.com

TS:   arr.length
来源：http://tug.jinyuanbaomall.cn

Java: list.size();
来源：http://yvx.gogol.net.cn

Go:   len(arr)
来源：http://cez.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://phq.xziqi.cn

C#:   list.Count;
来源：http://efn.hesvh.cn

[D07] 切片 / 取子数组
来源：http://qtj.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qxv.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://zsg.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://sdl.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://awl.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://qpb.cqqwz.cn

Go:   arr[1:4]
来源：http://kxh.uphjek.com

Ruby: arr[1, 3]
来源：http://lrn.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://lni.ctjpmb.com

[D08] 合并两个数组
来源：http://mpv.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://egh.sweek.top

PHP:  array_merge($a, $b);
来源：http://kop.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vbb.chenzaomai.com

TS:   [...a, ...b];
来源：http://uvh.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yps.pengpengdd.cyou

Go:   append(a, b...)
来源：http://gqo.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://ivz.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://jpy.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://mbm.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zwm.fehbvm.com

PHP:  sort($arr);
来源：http://dzw.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nji.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sss.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xst.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://apc.vqdsnc.cn

Ruby: arr.sort
来源：http://zjk.shanyushiyangtech.top

C#:   list.Sort();
来源：http://npb.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gku.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jap.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rih.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cav.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bur.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oim.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yyk.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cle.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uoz.xinyue.icu

[D11] 反转数组
来源：http://kby.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://mut.uphjek.com

PHP:  array_reverse($arr);
来源：http://ixm.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dby.cdnleiting.top

TS:   [...arr].reverse();
来源：http://xrd.sysykeji.top

Java: Collections.reverse(list);
来源：http://hoj.ivvv.top

Go:   slices.Reverse(arr)
来源：http://byu.gotoacloud.top

Ruby: arr.reverse
来源：http://jfh.yongpay.top

C#:   list.Reverse();
来源：http://ltp.hnxiangtu.top

[D12] 查找元素下标
来源：http://zjo.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://wch.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gga.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vru.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccs.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nxw.tarul.cn

Go:   slices.Index(arr, x)
来源：http://bil.daxiang520.top

Ruby: arr.index(x)
来源：http://mqg.ydzc1.top

C#:   list.IndexOf(x);
来源：http://ith.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://hui.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dqu.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://efp.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://mci.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://qop.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dcg.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oqb.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://wlv.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yhx.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://siu.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eoo.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://voh.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://hkp.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://pnv.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jvg.yj20258888.top

Go:   // 手写循环
来源：http://wuj.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://udc.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cwb.xingfuxueyuan.xyz

[D15] 去重
来源：http://enr.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqg.pycfn.com

PHP:  array_unique($arr);
来源：http://zae.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://cnh.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://bau.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ylj.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://ssq.aibaodan.cn

Ruby: arr.uniq
来源：http://jsq.316326.xyz

C#:   list.Distinct().ToList()
来源：http://llv.yueranfly.top

[D16] 求和与平均值
来源：http://kxl.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dly.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ewc.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fky.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://coj.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jaf.jinqigufen.top

Go:   // 手写循环累加
来源：http://gca.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fnd.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://rnk.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://eyx.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://ggw.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://isb.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ypu.cdnleiting.top

TS:   Math.max(...arr);
来源：http://kbf.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kfi.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqa.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://oao.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://mns.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://pgk.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yye.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://clr.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eou.chenzaomai.com

TS:   nested.flat();
来源：http://xzj.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lzg.hysaishi.cn

Go:   // 手写双层循环
来源：http://mct.shuidangran.top

Ruby: nested.flatten
来源：http://yua.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fje.hesvh.cn

[D19] 按字段分组
来源：http://dvd.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rqa.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ofg.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://axh.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xve.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nss.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://qzt.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kfd.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xwo.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://atc.fktsv.cn

Py:   Counter(arr)
来源：http://bno.meibo888.top

PHP:  array_count_values($arr);
来源：http://caz.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://myl.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zdm.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wnn.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://jeu.shangyingyoupin.top

Ruby: arr.tally
来源：http://yxn.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jud.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://oen.nanxuanxn.top

Py:   x in arr
来源：http://jqh.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://jls.yj20258888.top

JS:   arr.includes(x)
来源：http://pbk.meibo888.top

TS:   arr.includes(x)
来源：http://nyr.sweek.top

Java: list.contains(x)
来源：http://cqa.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://ljs.haohaochexian.top

Ruby: arr.include?(x)
来源：http://sig.hcnkem.com

C#:   list.Contains(x)
来源：http://oss.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://odu.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqd.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uvx.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rzn.bjfxy.top

TS:   [...arr];
来源：http://slc.hesvh.cn

Java: new ArrayList<>(list);
来源：http://jau.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://del.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://uhg.zhixingplan.top

C#:   new List<int>(list);
来源：http://dkt.aibaodan.cn

[D23] reduce 累积计算
来源：http://yhr.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://krc.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://viz.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jro.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pvy.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsw.sxryk.cn

Go:   // 手写循环
来源：http://tye.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kzh.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xxf.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://oqk.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xpc.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lsi.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xio.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vvb.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lha.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://irk.ydzc1.top


<!-- 参考信息 -->