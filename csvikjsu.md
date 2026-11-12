代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hwz.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://elt.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://akz.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ome.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://okn.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cyo.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oqm.zhixingplan.top

[C09] 递归
来源：http://cqa.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cfr.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ldj.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://siw.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgc.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxh.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uuw.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dwx.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wyy.xziqi.cn

[C10] 变量作用域
来源：http://ymd.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xla.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aec.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hys.yonumen.top

TS:   同 JS
来源：http://hea.shzxlz.cn

Java: 方法内为块级作用域
来源：http://gge.dashuyun.cn

Go:   花括号块级作用域
来源：http://rbb.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://suj.fengsongda.top

C#:   块级作用域
来源：http://qcl.guowangkeji.top

[C11] 模块导入与导出
来源：http://pwe.tanke756.top

Py:   from module import func
来源：http://zvo.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jev.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://iqe.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zlo.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://huz.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bpx.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://nky.redwolf501.top

C#:   using System.Text;
来源：http://xar.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://faf.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://uwf.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://igg.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://fhh.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://rfj.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ibz.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://trj.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://blk.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ysq.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://mdu.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mqo.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dru.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jrq.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://woh.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://ezb.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://dxy.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tlx.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://pgu.jyoumei.cn

[C14] 泛型函数
来源：http://ksx.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://njh.zhijiandao.cn

PHP:  // 无泛型
来源：http://wbo.shuidangran.top

JS:   // 无泛型
来源：http://qwd.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://olh.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xiy.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iuo.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://myh.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jcb.daxiang520.top

[C15] 解构 / 展开参数
来源：http://cqg.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fun.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://bzu.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ats.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ncc.shangyingyoupin.top

Java: // 无解构
来源：http://cjs.jyoumei.cn

Go:   // 无解构
来源：http://enj.yongpay.top

Ruby: a, b = pair
来源：http://lbq.gzhubu.top

C#:   var (a, b) = pair;
来源：http://qrs.yj20258888.top

[C16] 函数 / 方法重载
来源：http://ruo.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uzo.zhongyouzk.top

PHP:  // 无重载
来源：http://crg.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mwi.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://ejv.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://bzs.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://sme.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://mfn.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://evs.shanyushiyangtech.top

================================================================================
来源：http://dfa.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://xii.iojbl.cn

================================================================================
来源：http://dcb.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://kgp.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://egk.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aom.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://goq.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uti.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://isl.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://vku.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://pxg.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mtk.fehbvm.com

[D02] 追加元素到末尾
来源：http://ano.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xpi.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mlm.hammf.cn

JS:   arr.push(4);
来源：http://ruz.zhongyouzk.top

TS:   arr.push(4);
来源：http://puu.52xcode.cn

Java: list.add(4);
来源：http://xwb.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://zfa.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://van.shzxlz.cn

C#:   list.Add(4);
来源：http://bnw.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://vuc.uphjek.com

Py:   arr.insert(0, 0)
来源：http://rki.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cym.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hgi.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://tef.hysaishi.cn

Java: list.add(0, 0);
来源：http://vcv.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://rqm.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oct.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://cid.andypj.xyz

[D04] 删除元素
来源：http://rfo.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gck.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vdc.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://shh.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://ykr.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vzi.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hgz.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dbz.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://noi.uphjek.com

[D05] 访问与修改元素
来源：http://aga.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pla.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qnt.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://czy.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://sxv.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://cuq.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://zex.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rho.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vij.havefunace.top

[D06] 数组长度
来源：http://gcs.0kj1m.cn

Py:   len(arr)
来源：http://okj.aizwys.cn

PHP:  count($arr);
来源：http://agg.ivvv.top

JS:   arr.length
来源：http://egp.mhx1999.top

TS:   arr.length
来源：http://oyg.0kj1m.cn

Java: list.size();
来源：http://edy.jyoumei.cn

Go:   len(arr)
来源：http://isl.fzhhl.top

Ruby: arr.length; arr.size
来源：http://frq.wangshuangyany.cn

C#:   list.Count;
来源：http://nbi.smart0.xyz

[D07] 切片 / 取子数组
来源：http://ash.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bbs.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xiv.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://hik.316326.xyz

TS:   arr.slice(1, 4);
来源：http://rxt.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://bxl.yj20258.top

Go:   arr[1:4]
来源：http://pzl.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://asb.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://mca.aibaodan.cn

[D08] 合并两个数组
来源：http://eqp.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://hrb.316326.xyz

PHP:  array_merge($a, $b);
来源：http://tyy.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jbl.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://dix.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://maq.hysaishi.cn

Go:   append(a, b...)
来源：http://bhg.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://ppd.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://nqo.meibo888.top

[D09] 排序（升序）
来源：http://qmw.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://mec.ydzc1.top

PHP:  sort($arr);
来源：http://zul.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fyo.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kaz.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gyr.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dra.bbcook.cn

Ruby: arr.sort
来源：http://joh.52xcode.cn

C#:   list.Sort();
来源：http://vms.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fre.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hkv.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hix.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eij.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yes.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rfo.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wbs.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yla.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zfb.sysykeji.top

[D11] 反转数组
来源：http://liw.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aku.birdmap.top

PHP:  array_reverse($arr);
来源：http://ang.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hsl.uphjek.com

TS:   [...arr].reverse();
来源：http://eud.shuidangran.top

Java: Collections.reverse(list);
来源：http://ksc.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://tid.yfazqb.com

Ruby: arr.reverse
来源：http://ajw.zycfv.cn

C#:   list.Reverse();
来源：http://tmb.havefunace.top

[D12] 查找元素下标
来源：http://snm.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://btq.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://llv.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ltq.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxx.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pvw.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://sit.yfazqb.com

Ruby: arr.index(x)
来源：http://sfp.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://fir.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://yxv.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kwi.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cnq.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://uce.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://fmv.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lvg.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pqb.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://ibo.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://euo.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://eil.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vax.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ddf.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://cqg.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://ywo.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dqd.jqgfzy.top

Go:   // 手写循环
来源：http://tgc.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://flv.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hbh.mhx1999.top

[D15] 去重
来源：http://msf.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lvh.jyoumei.cn

PHP:  array_unique($arr);
来源：http://lwd.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://tnv.316326.xyz

TS:   [...new Set(arr)]
来源：http://ney.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vui.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bhq.fktsv.cn

Ruby: arr.uniq
来源：http://zzr.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://apy.shangyingyoupin.top

[D16] 求和与平均值
来源：http://kgc.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eeq.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://reu.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zjj.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrl.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rff.svipenyu.cn

Go:   // 手写循环累加
来源：http://iti.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ljd.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://xfq.cheryme.top

[D17] 最大值与最小值
来源：http://kkt.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://rxe.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://dvt.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cyg.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://ltp.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kkp.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xdi.sweek.top

Ruby: arr.max;  arr.min
来源：http://epy.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://nsi.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://muc.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wow.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://asv.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dfw.iojbl.cn

TS:   nested.flat();
来源：http://wkz.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yuw.wangdashe.top

Go:   // 手写双层循环
来源：http://dkg.pycfn.com

Ruby: nested.flatten
来源：http://ays.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nca.gaohongyu789.top

[D19] 按字段分组
来源：http://yce.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eop.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rcm.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rih.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://puu.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qrs.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://tfj.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://zgi.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ukj.sweek.top

[D20] 统计每个元素出现次数
来源：http://aor.guannengcc.top

Py:   Counter(arr)
来源：http://xkg.tarul.cn

PHP:  array_count_values($arr);
来源：http://kmv.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rja.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwz.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxy.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://eag.52xcode.cn

Ruby: arr.tally
来源：http://khg.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ona.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://zjx.zhijiandao.cn

Py:   x in arr
来源：http://svc.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://ajr.yongpay.top

JS:   arr.includes(x)
来源：http://zqb.ivvv.top

TS:   arr.includes(x)
来源：http://svt.vehdjk.com

Java: list.contains(x)
来源：http://qko.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://qah.ctjpmb.com

Ruby: arr.include?(x)
来源：http://jil.guowangkeji.top

C#:   list.Contains(x)
来源：http://pfi.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://lae.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ldj.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://isl.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nqj.jyoumei.cn

TS:   [...arr];
来源：http://imh.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://vna.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://emk.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://yax.zhongyouzk.top

C#:   new List<int>(list);
来源：http://dht.yonumen.top

[D23] reduce 累积计算
来源：http://rax.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qzc.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://drg.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yrx.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ynb.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://kxh.dianchejie.cn

Go:   // 手写循环
来源：http://djt.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xuh.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qds.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://dhf.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hpo.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvr.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nfp.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ipq.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nad.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vvi.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pxq.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lqk.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://ywj.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://inh.zycfv.cn


<!-- 参考信息 -->