代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bwz.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wzq.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://csg.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zst.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vyw.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://phs.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dji.c1oappe.top

[C09] 递归
来源：http://dey.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yxi.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://two.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fnv.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mju.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qtj.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mwi.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://buu.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lfv.chenzaomai.com

[C10] 变量作用域
来源：http://unq.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iqp.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xhp.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aoe.fanxiaobao.xyz

TS:   同 JS
来源：http://hzx.daria6918.cn

Java: 方法内为块级作用域
来源：http://eaw.tanke756.top

Go:   花括号块级作用域
来源：http://hna.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qka.yonumen.top

C#:   块级作用域
来源：http://lww.xuanzx.com

[C11] 模块导入与导出
来源：http://ebt.wangdashe.top

Py:   from module import func
来源：http://wtg.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tuk.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cfc.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ctt.shanyushiyangtech.top

Java: import java.util.List;
来源：http://gqb.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://era.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://mjw.ybcxt.top

C#:   using System.Text;
来源：http://jdb.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://bef.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://wpv.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://zcs.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://tdf.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://yve.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jcx.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://acp.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://ukt.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://syw.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://scp.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rpn.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmk.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ade.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpr.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://rtm.yj20258888.top

Go:   func add(a, b int) int
来源：http://iak.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syn.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://emw.cdnleiting.top

[C14] 泛型函数
来源：http://sko.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qga.yueranfly.top

PHP:  // 无泛型
来源：http://ijb.ydjk.org.cn

JS:   // 无泛型
来源：http://xyg.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://amu.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gmw.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pcu.jqgufenzy.top

Ruby: # 无泛型
来源：http://suo.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ylp.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://yvk.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://edd.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://bap.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fqb.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rfh.cqqwz.cn

Java: // 无解构
来源：http://qom.hcnkem.com

Go:   // 无解构
来源：http://qfi.ybcxt.top

Ruby: a, b = pair
来源：http://xqw.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://oqy.cashguo.top

[C16] 函数 / 方法重载
来源：http://qid.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://san.xylfe.cn

PHP:  // 无重载
来源：http://mna.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ucq.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://npp.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rda.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://hbo.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://who.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kdm.jinqigfzy.top

================================================================================
来源：http://bns.316326.xyz

D. 数组 / 列表 / 集合
来源：http://khw.guannengcc.top

================================================================================
来源：http://qct.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://wtz.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iqj.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vpn.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://awo.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vyd.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jqs.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://nhm.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://bop.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kxm.yfazqb.com

[D02] 追加元素到末尾
来源：http://mab.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xme.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kkk.feifeiyinyue.top

JS:   arr.push(4);
来源：http://cje.52xcode.cn

TS:   arr.push(4);
来源：http://hpk.zhijiandao.cn

Java: list.add(4);
来源：http://bad.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://odc.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://yqe.xuanzx.com

C#:   list.Add(4);
来源：http://wfq.jianghu66.top

[D03] 在指定位置插入元素
来源：http://wfz.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://lny.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://egb.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xlm.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://zwz.hnqzz.top

Java: list.add(0, 0);
来源：http://yiz.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://jjd.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iws.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://bey.nwbrower.top

[D04] 删除元素
来源：http://cux.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qep.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dfs.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fox.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://lcn.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wri.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pcw.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jpl.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hng.tianlin.xyz

[D05] 访问与修改元素
来源：http://bye.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jig.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ixe.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qnv.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://lgn.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://spj.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://dxa.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gsg.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ezs.zhiwuduotai.top

[D06] 数组长度
来源：http://rcg.xuanzx.com

Py:   len(arr)
来源：http://kks.chenlongwang.top

PHP:  count($arr);
来源：http://nfb.hongshengwenyu.top

JS:   arr.length
来源：http://krw.nanxuanxn.top

TS:   arr.length
来源：http://kxd.zhixingplan.top

Java: list.size();
来源：http://nvi.bjfxy.top

Go:   len(arr)
来源：http://puj.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://snw.zhongyouzk.top

C#:   list.Count;
来源：http://tmy.gzhubu.top

[D07] 切片 / 取子数组
来源：http://koq.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lyj.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qkz.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://esf.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://xfr.redwolf501.top

Java: list.subList(1, 4);
来源：http://yhd.chenjidiqi.icu

Go:   arr[1:4]
来源：http://yls.birdmap.top

Ruby: arr[1, 3]
来源：http://rhx.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://sop.bjfxy.top

[D08] 合并两个数组
来源：http://vjr.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://dyt.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://uwc.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zrz.cashguo.top

TS:   [...a, ...b];
来源：http://pmw.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cex.nanxuanxn.top

Go:   append(a, b...)
来源：http://een.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://xon.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://xyg.tianlin.xyz

[D09] 排序（升序）
来源：http://xru.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://bxe.dianchejie.cn

PHP:  sort($arr);
来源：http://hzm.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xff.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nmn.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ngh.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kmp.birdmap.top

Ruby: arr.sort
来源：http://swf.gzhubu.top

C#:   list.Sort();
来源：http://mfb.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://imd.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bel.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwx.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://avm.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mdc.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lem.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lrm.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pvg.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://der.bbcook.cn

[D11] 反转数组
来源：http://ivu.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://izd.ivvv.top

PHP:  array_reverse($arr);
来源：http://ehr.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vwz.hywenlv.cn

TS:   [...arr].reverse();
来源：http://ibv.zdbjq.cn

Java: Collections.reverse(list);
来源：http://qcd.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://vnj.haohaochexian.top

Ruby: arr.reverse
来源：http://ydg.fehbvm.com

C#:   list.Reverse();
来源：http://agq.shangyingyoupin.top

[D12] 查找元素下标
来源：http://biy.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://web.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://laq.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uaz.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zmz.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hky.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://gkj.xuanzx.com

Ruby: arr.index(x)
来源：http://jvm.sweek.top

C#:   list.IndexOf(x);
来源：http://hqe.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://dje.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lik.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eqk.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://htw.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://dul.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://unq.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wri.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dnk.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gcw.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://phr.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mbr.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bty.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://zmt.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://qzh.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ttm.wangshuangyany.cn

Go:   // 手写循环
来源：http://enx.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qmq.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tee.shuidangran.top

[D15] 去重
来源：http://ddu.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bfy.yj20258888.top

PHP:  array_unique($arr);
来源：http://qhi.vehdjk.com

JS:   [...new Set(arr)]
来源：http://ggo.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://ttf.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://isr.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://elk.gaohongyu789.top

Ruby: arr.uniq
来源：http://lyv.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://yjd.epnwcf.com

[D16] 求和与平均值
来源：http://pus.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://clz.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hvn.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zat.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://udd.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fjg.yuanzhike.top

Go:   // 手写循环累加
来源：http://brn.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://axp.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://sia.daxiang520.top

[D17] 最大值与最小值
来源：http://ube.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://nuq.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://ffi.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://npd.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://tfg.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eti.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xtk.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://xsx.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://mwb.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://xop.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibx.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://adu.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yav.jiagoushi.top

TS:   nested.flat();
来源：http://yso.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ljo.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://nmi.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://akb.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ezb.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://wlv.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pyp.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mle.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ziu.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rkx.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwp.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://syt.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rbl.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jsn.yj20258.top

[D20] 统计每个元素出现次数
来源：http://tzb.pengpengdd.cyou

Py:   Counter(arr)
来源：http://kxy.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://syl.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://umq.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ofm.316326.xyz

Go:   // 手写 map[T]int
来源：http://uur.ppjwa.cn

Ruby: arr.tally
来源：http://frs.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nqp.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://bep.xziqi.cn

Py:   x in arr
来源：http://qpn.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://omk.ivvv.top

JS:   arr.includes(x)
来源：http://odg.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://pya.cqqwz.cn

Java: list.contains(x)
来源：http://edo.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://uwu.shuidangran.top

Ruby: arr.include?(x)
来源：http://uxc.cheryme.top

C#:   list.Contains(x)
来源：http://dgy.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://ldy.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pzs.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ize.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bxw.uphjek.com

TS:   [...arr];
来源：http://hrf.vehdjk.com

Java: new ArrayList<>(list);
来源：http://ejq.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://fox.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://yht.zdbjq.cn

C#:   new List<int>(list);
来源：http://llw.shzxlz.cn

[D23] reduce 累积计算
来源：http://bju.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ncu.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://opl.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azr.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yxg.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pfm.quarkkingdee.top

Go:   // 手写循环
来源：http://xkz.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rof.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pcq.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://nej.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://agf.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fkx.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pfq.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iqs.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://foa.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bhl.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rhd.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nbf.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://ufz.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://clc.sjlbkw.cn


<!-- 参考信息 -->