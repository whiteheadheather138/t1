代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eng.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qgi.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qjk.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvj.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://prw.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://trs.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pio.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://egu.hnqzz.top

[C10] 变量作用域
来源：http://rms.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgq.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uvd.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksl.yfazqb.com

TS:   同 JS
来源：http://rtx.yvedp.cn

Java: 方法内为块级作用域
来源：http://opq.zycfv.cn

Go:   花括号块级作用域
来源：http://ylz.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://igo.chenjidiqi.icu

C#:   块级作用域
来源：http://nml.hesvh.cn

[C11] 模块导入与导出
来源：http://lug.chenzaomai.com

Py:   from module import func
来源：http://myg.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zms.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jjl.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zdy.smart0.xyz

Java: import java.util.List;
来源：http://mev.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xgs.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://uga.vqdsnc.cn

C#:   using System.Text;
来源：http://cxc.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://huy.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://dut.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://lcw.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://odr.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://rhz.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fjm.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://agl.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://cns.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qcw.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://vqb.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aji.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kfd.haohaochexian.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmk.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uam.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wak.chenlongwang.top

Go:   func add(a, b int) int
来源：http://rhp.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ogl.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://mcc.vehdjk.com

[C14] 泛型函数
来源：http://ost.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iij.nwbrower.top

PHP:  // 无泛型
来源：http://asm.aibaodan.cn

JS:   // 无泛型
来源：http://mid.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zhn.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hjo.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tcd.pengpengdd.cyou

Ruby: # 无泛型
来源：http://cwi.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xbe.316326.xyz

[C15] 解构 / 展开参数
来源：http://yyd.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oij.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://jgr.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ywt.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pum.meibo888.top

Java: // 无解构
来源：http://aga.ppjwa.cn

Go:   // 无解构
来源：http://grs.tanke756.top

Ruby: a, b = pair
来源：http://jcl.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://wia.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://bni.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vpj.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://bww.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rbs.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://nqv.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hls.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://xsy.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://kwl.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://spe.jinyuanbaomall.cn

================================================================================
来源：http://luu.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://zkv.feifeiyinyue.top

================================================================================
来源：http://rnj.nwbrower.top

[D01] 创建数组 / 列表
来源：http://cgu.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://olv.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ibn.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jsk.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://txt.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ibq.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://uql.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://zwj.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tgs.jqgfzy.top

[D02] 追加元素到末尾
来源：http://vdk.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mut.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yyq.xylfe.cn

JS:   arr.push(4);
来源：http://rrf.zhengqikj.top

TS:   arr.push(4);
来源：http://jnt.52xcode.cn

Java: list.add(4);
来源：http://luj.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://yxe.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://xgp.zdbjq.cn

C#:   list.Add(4);
来源：http://wbc.fzhhl.top

[D03] 在指定位置插入元素
来源：http://sxi.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://ibg.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://phe.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jov.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://ghb.fzhhl.top

Java: list.add(0, 0);
来源：http://epr.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://jci.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nfo.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://zyv.hfpthk.cn

[D04] 删除元素
来源：http://cad.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lil.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ujg.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dpa.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://hcc.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wul.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uli.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://apa.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://edl.cashguo.top

[D05] 访问与修改元素
来源：http://ipj.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jcj.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tfr.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tbk.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://vll.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://eja.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://dcb.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bez.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ohh.yongpay.top

[D06] 数组长度
来源：http://oet.shangyingyoupin.top

Py:   len(arr)
来源：http://cik.zhixingplan.top

PHP:  count($arr);
来源：http://gnh.ivvv.top

JS:   arr.length
来源：http://fuj.feifeiyinyue.top

TS:   arr.length
来源：http://blb.snrcjt.cn

Java: list.size();
来源：http://uvh.chenzaomai.com

Go:   len(arr)
来源：http://heq.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://ebr.jinyuanbaomall.cn

C#:   list.Count;
来源：http://eny.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://dhg.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ind.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://prh.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://rct.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://zdk.cheryme.top

Java: list.subList(1, 4);
来源：http://iav.hnqzz.top

Go:   arr[1:4]
来源：http://nhw.fengsongda.top

Ruby: arr[1, 3]
来源：http://cuz.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://vhf.yj202588.top

[D08] 合并两个数组
来源：http://lls.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://sug.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://zia.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://snc.hesvh.cn

TS:   [...a, ...b];
来源：http://vqg.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fzw.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://lpm.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://mze.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://dvk.wangdashe.top

[D09] 排序（升序）
来源：http://zvs.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://tlm.shuidangran.top

PHP:  sort($arr);
来源：http://gfm.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://edf.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://edq.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://czp.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upb.dashuyun.cn

Ruby: arr.sort
来源：http://biv.gogol.net.cn

C#:   list.Sort();
来源：http://cuy.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://nhi.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gfp.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yjy.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpo.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kpf.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ekv.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://koo.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sbx.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gkc.pengpengdd.cyou

[D11] 反转数组
来源：http://hvx.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://sqt.aizwys.cn

PHP:  array_reverse($arr);
来源：http://rhd.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ldq.chenlongwang.top

TS:   [...arr].reverse();
来源：http://yiq.daria6918.cn

Java: Collections.reverse(list);
来源：http://dro.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://rhr.svipenyu.cn

Ruby: arr.reverse
来源：http://huk.jinqigufen.top

C#:   list.Reverse();
来源：http://rks.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://lve.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://fll.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvh.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zpa.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpq.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vla.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://ilh.yfazqb.com

Ruby: arr.index(x)
来源：http://vbb.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://dvy.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://bra.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gce.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eao.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://nrr.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://mml.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://akc.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hlr.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://edu.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ayo.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://wvj.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wcn.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mik.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://zfb.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://ijm.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xsa.jianghu66.top

Go:   // 手写循环
来源：http://qqt.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://bts.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jbo.9152youxi.cn

[D15] 去重
来源：http://vgk.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ctb.meibo888.top

PHP:  array_unique($arr);
来源：http://dmo.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://xiz.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://mii.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wue.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ivl.wangdashe.top

Ruby: arr.uniq
来源：http://kzq.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://bhm.yj202588.top

[D16] 求和与平均值
来源：http://jqx.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bqp.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://chx.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://llf.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ire.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ize.hammf.cn

Go:   // 手写循环累加
来源：http://lce.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kwn.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://nbq.jiagoushi.top

[D17] 最大值与最小值
来源：http://iru.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://uhu.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://iug.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vbi.daria6918.cn

TS:   Math.max(...arr);
来源：http://xjz.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tak.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gjk.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://xgn.meibo888.top

C#:   list.Max();  list.Min()
来源：http://jxh.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://gbd.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://csk.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://oxw.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cwe.zycfv.cn

TS:   nested.flat();
来源：http://npz.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xgg.bjfxy.top

Go:   // 手写双层循环
来源：http://hbt.feifeiyinyue.top

Ruby: nested.flatten
来源：http://xdi.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://paj.chenlongwang.top

[D19] 按字段分组
来源：http://ety.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zhj.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://awh.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gvv.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zob.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vjz.cheryme.top

Go:   // 手写 map[string][]T
来源：http://khd.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mbi.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zgc.ivvv.top

[D20] 统计每个元素出现次数
来源：http://onu.gogol.net.cn

Py:   Counter(arr)
来源：http://zil.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://eja.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twy.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixr.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://huy.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://mkn.tanke756.top

Ruby: arr.tally
来源：http://uoj.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oap.havefunace.top

[D21] 判断是否包含某元素
来源：http://ixc.yj202588.top

Py:   x in arr
来源：http://ckd.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://aez.bbcook.cn

JS:   arr.includes(x)
来源：http://rgh.zhoulong.xyz

TS:   arr.includes(x)
来源：http://leo.yj20258888.top

Java: list.contains(x)
来源：http://txp.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://out.hysaishi.cn

Ruby: arr.include?(x)
来源：http://mnw.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://ndd.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://bny.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ixn.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ojg.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dua.ywan-chungtsiang.top

TS:   [...arr];
来源：http://euk.birdmap.top

Java: new ArrayList<>(list);
来源：http://hgi.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qsw.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://mcs.xinyue.icu

C#:   new List<int>(list);
来源：http://uxf.jinqigfzy.top

[D23] reduce 累积计算
来源：http://jle.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pab.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gip.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vjo.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kra.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://obh.andypj.xyz

Go:   // 手写循环
来源：http://vjh.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cnn.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xcw.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://ndr.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://euv.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lct.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://apk.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bqh.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hjm.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zud.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://apz.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jgq.pycfn.com

[D25] Set 集合去重与交并差
来源：http://zoo.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uph.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nvp.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zsn.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://drd.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ryd.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uwi.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dup.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ler.c1oappe.top

[D26] 数组转字符串
来源：http://vwr.feifeiyinyue.top


<!-- 参考信息 -->