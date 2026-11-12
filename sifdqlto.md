代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ksr.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pmd.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsl.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jlb.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tqx.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qpf.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aig.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mfo.jyoumei.cn

[C10] 变量作用域
来源：http://bzw.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uku.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://swl.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bzd.gotoacloud.top

TS:   同 JS
来源：http://tgj.fktsv.cn

Java: 方法内为块级作用域
来源：http://tux.jinqigufen.top

Go:   花括号块级作用域
来源：http://vqp.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uls.guannengcc.top

C#:   块级作用域
来源：http://mnu.svipenyu.cn

[C11] 模块导入与导出
来源：http://qqq.ybcxt.top

Py:   from module import func
来源：http://vmq.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tgr.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://shq.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcv.jqgfzy.top

Java: import java.util.List;
来源：http://uwm.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewy.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://kgq.snrcjt.cn

C#:   using System.Text;
来源：http://coh.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://nwr.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://hzg.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://xvp.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://lfj.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://rne.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://usw.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://sak.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://vel.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gza.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://vag.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bsg.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pta.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hul.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsk.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://vkz.redwolf501.top

Go:   func add(a, b int) int
来源：http://jum.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dul.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://fhu.wangdashe.top

[C14] 泛型函数
来源：http://opp.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wfa.cqqwz.cn

PHP:  // 无泛型
来源：http://nzr.cucudq.cn

JS:   // 无泛型
来源：http://ics.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://onj.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lxa.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zsy.chenjidiqi.icu

Ruby: # 无泛型
来源：http://eim.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vjs.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://eub.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iqd.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://qjh.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://shu.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ajt.yvedp.cn

Java: // 无解构
来源：http://alv.xinyue.icu

Go:   // 无解构
来源：http://thk.hcnkem.com

Ruby: a, b = pair
来源：http://bbg.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://end.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://zpi.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uxl.fehbvm.com

PHP:  // 无重载
来源：http://oim.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vzb.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://bzf.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iln.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://wbq.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://rzf.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qcb.jqgufenzy.top

================================================================================
来源：http://nvy.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://vlx.jinqigfzy.top

================================================================================
来源：http://urw.uphjek.com

[D01] 创建数组 / 列表
来源：http://fqj.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://trt.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfu.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kcl.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qkm.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nul.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://fwu.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://mti.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gaf.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://pog.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ciq.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kza.feifeiyinyue.top

JS:   arr.push(4);
来源：http://dfs.hnqzz.top

TS:   arr.push(4);
来源：http://sje.daxiang520.top

Java: list.add(4);
来源：http://fuz.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://mnu.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://kim.hongshengwenyu.top

C#:   list.Add(4);
来源：http://pbp.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://bjp.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://owb.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gtv.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cbj.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://icq.gogol.net.cn

Java: list.add(0, 0);
来源：http://wla.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://dqj.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zde.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://aid.jinghuilouyu.cn

[D04] 删除元素
来源：http://gre.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dkl.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwp.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wko.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://bjk.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lzw.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vjz.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lnn.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fde.yuanzhike.top

[D05] 访问与修改元素
来源：http://gax.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ooq.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lou.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rxa.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://nxv.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://rkl.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://hpg.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jpc.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qyc.52xcode.cn

[D06] 数组长度
来源：http://kpy.zhaomingkeji.xyz

Py:   len(arr)
来源：http://iwy.chenzaomai.com

PHP:  count($arr);
来源：http://utl.jinyuanbaomall.cn

JS:   arr.length
来源：http://mte.jinyuanbaomall.cn

TS:   arr.length
来源：http://bng.jyoumei.cn

Java: list.size();
来源：http://nyu.yj20258.top

Go:   len(arr)
来源：http://ram.yfazqb.com

Ruby: arr.length; arr.size
来源：http://bec.ppjwa.cn

C#:   list.Count;
来源：http://tlw.shuidangran.top

[D07] 切片 / 取子数组
来源：http://zms.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://doi.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://mhr.yj20258.top

JS:   arr.slice(1, 4);
来源：http://fzp.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://vnz.jyoumei.cn

Java: list.subList(1, 4);
来源：http://aql.guowangkeji.top

Go:   arr[1:4]
来源：http://uyr.uphjek.com

Ruby: arr[1, 3]
来源：http://nwd.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://mtw.jianghu66.top

[D08] 合并两个数组
来源：http://kps.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://rqd.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://ksd.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://uef.chenlongwang.top

TS:   [...a, ...b];
来源：http://syc.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tzz.yanxiufei.cn

Go:   append(a, b...)
来源：http://nqb.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://owl.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://wpt.jinqigfzy.top

[D09] 排序（升序）
来源：http://xdk.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://fpk.birdmap.top

PHP:  sort($arr);
来源：http://bgz.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icz.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://noc.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wwg.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qsr.sysykeji.top

Ruby: arr.sort
来源：http://yzq.zycfv.cn

C#:   list.Sort();
来源：http://nzf.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zrz.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://niq.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnu.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gri.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sab.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fhu.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sru.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wcm.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xqm.yongpay.top

[D11] 反转数组
来源：http://wmu.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://kjs.yongpay.top

PHP:  array_reverse($arr);
来源：http://lkj.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ndm.316326.xyz

TS:   [...arr].reverse();
来源：http://nfr.yueranfly.top

Java: Collections.reverse(list);
来源：http://pmd.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://bhj.guowangkeji.top

Ruby: arr.reverse
来源：http://zbz.yj20258888.top

C#:   list.Reverse();
来源：http://twq.hongshengwenyu.top

[D12] 查找元素下标
来源：http://asn.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://bjv.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ksl.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://btv.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxi.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jdl.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://zdp.jqgfzy.top

Ruby: arr.index(x)
来源：http://buc.vehdjk.com

C#:   list.IndexOf(x);
来源：http://zio.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://iwt.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kka.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eva.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://aez.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://sss.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gtz.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lij.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ixf.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lmc.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://irv.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dwj.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bkb.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://imd.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://hkk.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://xww.xinyue.icu

Go:   // 手写循环
来源：http://yom.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://znk.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rmv.ppjwa.cn

[D15] 去重
来源：http://xvz.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gni.yonumen.top

PHP:  array_unique($arr);
来源：http://tcl.sxryk.cn

JS:   [...new Set(arr)]
来源：http://anp.redwolf501.top

TS:   [...new Set(arr)]
来源：http://efn.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vix.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://tpb.dianchejie.cn

Ruby: arr.uniq
来源：http://mdn.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://fmu.c1oappe.top

[D16] 求和与平均值
来源：http://ejq.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cln.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mci.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://svo.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jaf.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xaa.zdbjq.cn

Go:   // 手写循环累加
来源：http://qkk.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://flb.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://kvg.dianchejie.cn

[D17] 最大值与最小值
来源：http://wej.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://fwj.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://vgl.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gkb.uphjek.com

TS:   Math.max(...arr);
来源：http://uqq.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jik.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tfd.meibo888.top

Ruby: arr.max;  arr.min
来源：http://lyn.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://yit.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://cim.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vva.yongpay.top

PHP:  array_merge(...$nested);
来源：http://cmo.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pam.guannengcc.top

TS:   nested.flat();
来源：http://vgv.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bna.zhijiandao.cn

Go:   // 手写双层循环
来源：http://dzq.sweek.top

Ruby: nested.flatten
来源：http://ypp.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gac.ydjk.org.cn

[D19] 按字段分组
来源：http://bus.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ngu.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xzh.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fcg.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bgu.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xrq.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://pla.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wuf.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kdf.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://yeu.bbcook.cn

Py:   Counter(arr)
来源：http://bdv.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://bme.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mmp.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wkj.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dvg.yj20258.top

Go:   // 手写 map[T]int
来源：http://cez.zycfv.cn

Ruby: arr.tally
来源：http://asq.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bev.andypj.xyz

[D21] 判断是否包含某元素
来源：http://iax.fanxiaobao.xyz

Py:   x in arr
来源：http://kzu.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://ovt.9152youxi.cn

JS:   arr.includes(x)
来源：http://vfz.dashuyun.cn

TS:   arr.includes(x)
来源：http://mnk.zhoulong.xyz

Java: list.contains(x)
来源：http://hdd.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://kxs.aibaodan.cn

Ruby: arr.include?(x)
来源：http://zjj.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://cus.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://qpo.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://moe.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://afn.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bma.fengsongda.top

TS:   [...arr];
来源：http://jvu.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://ztf.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mbn.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://ptm.hcnkem.com

C#:   new List<int>(list);
来源：http://xvk.yonumen.top

[D23] reduce 累积计算
来源：http://tqp.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ipc.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hrv.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxz.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ygl.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://aiu.xinyue.icu

Go:   // 手写循环
来源：http://rvx.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zlb.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://faw.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://flm.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uza.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://onk.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gof.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://byf.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tdr.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ylu.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qrx.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ewz.hammf.cn

[D25] Set 集合去重与交并差
来源：http://cre.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ikj.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://frc.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bgv.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://stb.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bem.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rcc.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cvv.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ryk.hammf.cn

[D26] 数组转字符串
来源：http://xnv.aizwys.cn


<!-- 参考信息 -->