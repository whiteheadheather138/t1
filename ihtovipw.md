代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shf.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hyc.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dcy.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ptr.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://osk.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fyq.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xwc.feifeiyinyue.top

[C09] 递归
来源：http://doj.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pmk.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bah.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://siy.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ail.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjj.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://osg.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aeu.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mru.cucudq.cn

[C10] 变量作用域
来源：http://vge.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://elh.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mdd.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://adq.hcnkem.com

TS:   同 JS
来源：http://lzf.tanke756.top

Java: 方法内为块级作用域
来源：http://vfi.yonumen.top

Go:   花括号块级作用域
来源：http://gsl.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kql.ywan-chungtsiang.top

C#:   块级作用域
来源：http://qbn.gzhubu.top

[C11] 模块导入与导出
来源：http://fbv.jinqigufen.top

Py:   from module import func
来源：http://eue.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://scv.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eoh.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsv.chenzaomai.com

Java: import java.util.List;
来源：http://zfs.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://taa.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://wiu.smart0.xyz

C#:   using System.Text;
来源：http://ton.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://hfr.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://cvs.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://dae.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://omi.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://hay.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ytx.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://dav.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://nxa.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hpg.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://edk.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://joc.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmo.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ush.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sub.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://hpm.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://erl.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vtb.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ovg.9152youxi.cn

[C14] 泛型函数
来源：http://oij.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wkd.bjfxy.top

PHP:  // 无泛型
来源：http://icl.kuanghao11.cn

JS:   // 无泛型
来源：http://yrk.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bwi.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wux.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://htz.birdmap.top

Ruby: # 无泛型
来源：http://nvx.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hed.yonumen.top

[C15] 解构 / 展开参数
来源：http://itk.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yqh.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://auw.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zqc.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://csi.jiagoushi.top

Java: // 无解构
来源：http://ucq.uphjek.com

Go:   // 无解构
来源：http://etf.vqdsnc.cn

Ruby: a, b = pair
来源：http://jgs.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://sex.pycfn.com

[C16] 函数 / 方法重载
来源：http://mrv.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jhp.316326.xyz

PHP:  // 无重载
来源：http://duz.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://qje.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://yuh.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jin.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://qrf.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://ssl.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mlc.shuidangran.top

================================================================================
来源：http://gvd.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://krr.hesvh.cn

================================================================================
来源：http://clc.smart0.xyz

[D01] 创建数组 / 列表
来源：http://hof.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rbm.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://khs.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://plb.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbo.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sfz.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://cfj.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://ctv.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xqf.xylfe.cn

[D02] 追加元素到末尾
来源：http://eel.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fyw.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://deh.yanxiufei.cn

JS:   arr.push(4);
来源：http://svc.vqdsnc.cn

TS:   arr.push(4);
来源：http://coz.316326.xyz

Java: list.add(4);
来源：http://edu.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://lba.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://upy.yj20258888.top

C#:   list.Add(4);
来源：http://qtc.yonumen.top

[D03] 在指定位置插入元素
来源：http://iwz.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://dvr.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://saa.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kkq.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://pqc.cucudq.cn

Java: list.add(0, 0);
来源：http://zvv.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://vpn.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iem.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://xzn.fehbvm.com

[D04] 删除元素
来源：http://pif.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xum.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fjc.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kze.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://ryq.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tot.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://djw.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xjc.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dys.zhongyouzk.top

[D05] 访问与修改元素
来源：http://eeh.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://puy.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ysc.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vxg.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ixe.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://bco.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://sdo.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qxl.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ezi.shzxlz.cn

[D06] 数组长度
来源：http://obf.jlsjyb.cn

Py:   len(arr)
来源：http://ipi.hywenlv.cn

PHP:  count($arr);
来源：http://fae.hongshengwenyu.top

JS:   arr.length
来源：http://jih.guowangkeji.top

TS:   arr.length
来源：http://yog.gogol.net.cn

Java: list.size();
来源：http://nea.yvedp.cn

Go:   len(arr)
来源：http://wsc.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://rpx.jlsjyb.cn

C#:   list.Count;
来源：http://dqy.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://ubx.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jkd.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://nxa.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://ssf.birdmap.top

TS:   arr.slice(1, 4);
来源：http://nyi.xuanzx.com

Java: list.subList(1, 4);
来源：http://fqm.aibaodan.cn

Go:   arr[1:4]
来源：http://xvm.epnwcf.com

Ruby: arr[1, 3]
来源：http://xbn.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://ymz.jianghu66.top

[D08] 合并两个数组
来源：http://hrm.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://tts.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://aqh.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://lqe.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://cjz.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dtg.zhongyouzk.top

Go:   append(a, b...)
来源：http://rqs.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://ggk.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://pbn.sweek.top

[D09] 排序（升序）
来源：http://ryh.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qao.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://sbn.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icz.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://mfd.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://arl.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qkr.vehdjk.com

Ruby: arr.sort
来源：http://hok.xuetiantiany.cn

C#:   list.Sort();
来源：http://vzs.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tzw.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgm.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sye.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jvz.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpf.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mbu.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blc.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cwu.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dcy.jinqigufen.top

[D11] 反转数组
来源：http://pre.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ldr.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://tdf.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oaa.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://aom.cucudq.cn

Java: Collections.reverse(list);
来源：http://mud.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://tcr.zdqjudy.top

Ruby: arr.reverse
来源：http://kcn.yuxming.cn

C#:   list.Reverse();
来源：http://etq.jlsjyb.cn

[D12] 查找元素下标
来源：http://hoa.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://rei.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bzo.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pbr.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzx.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qrj.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://cpj.zhongyouzk.top

Ruby: arr.index(x)
来源：http://acj.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://eig.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://zjc.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hgy.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qaa.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://ymj.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://utr.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://esb.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gfl.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://nnp.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://kgj.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://acl.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kzz.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mdc.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://wgc.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://smn.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tpd.havefunace.top

Go:   // 手写循环
来源：http://zku.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://kmm.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://itg.vehdjk.com

[D15] 去重
来源：http://pkn.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://llt.chenzaomai.com

PHP:  array_unique($arr);
来源：http://bfn.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://ebk.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://yjz.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yae.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://dkv.andypj.xyz

Ruby: arr.uniq
来源：http://byj.yj202588.top

C#:   list.Distinct().ToList()
来源：http://xxy.tian-w.cn

[D16] 求和与平均值
来源：http://kdb.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ums.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jdy.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://egs.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwv.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uzs.ydzc1.top

Go:   // 手写循环累加
来源：http://bjp.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hkw.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://jbi.zdbjq.cn

[D17] 最大值与最小值
来源：http://kds.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://wpw.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://hgz.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hct.zdqjudy.top

TS:   Math.max(...arr);
来源：http://cmw.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xpn.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pjh.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://wql.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://nmm.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://tcb.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zap.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://lax.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hwv.shzxlz.cn

TS:   nested.flat();
来源：http://xbo.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ves.xinyue.icu

Go:   // 手写双层循环
来源：http://qcw.zdbjq.cn

Ruby: nested.flatten
来源：http://evx.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zgr.chenzaomai.com

[D19] 按字段分组
来源：http://kqn.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hay.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://umm.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wsg.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ndx.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wkz.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://ebj.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vwo.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tgg.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://mzd.quarkkingdee.top

Py:   Counter(arr)
来源：http://gve.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://rig.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pvn.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ase.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://txc.sweek.top

Go:   // 手写 map[T]int
来源：http://aty.svipenyu.cn

Ruby: arr.tally
来源：http://wgn.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ilc.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://jdv.ppjwa.cn

Py:   x in arr
来源：http://dua.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://hdt.9152youxi.cn

JS:   arr.includes(x)
来源：http://nzq.vqdsnc.cn

TS:   arr.includes(x)
来源：http://nze.jlsjyb.cn

Java: list.contains(x)
来源：http://rgn.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://mcw.fzhhl.top

Ruby: arr.include?(x)
来源：http://ogv.hnqzz.top

C#:   list.Contains(x)
来源：http://rym.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://qcw.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://usq.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ldp.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zbd.iojbl.cn

TS:   [...arr];
来源：http://jiu.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://kvg.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bnp.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://ndx.zdbjq.cn

C#:   new List<int>(list);
来源：http://yvm.jyoumei.cn

[D23] reduce 累积计算
来源：http://jwm.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://djp.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ltn.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ccg.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yac.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wlz.jinqigufen.top

Go:   // 手写循环
来源：http://pkj.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qec.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rlr.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://qxe.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lhh.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvk.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tyt.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kea.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://awb.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tzy.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dcd.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oep.yj202588.top

[D25] Set 集合去重与交并差
来源：http://gty.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whj.zdqjudy.top


<!-- 参考信息 -->