代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ger.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zbf.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ebo.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iuy.ydzc1.top

[C10] 变量作用域
来源：http://zxx.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://clh.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gmb.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xqf.bbcook.cn

TS:   同 JS
来源：http://rfm.yangfankeji.com

Java: 方法内为块级作用域
来源：http://efp.ydjk.org.cn

Go:   花括号块级作用域
来源：http://tmf.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ruu.yj20258.top

C#:   块级作用域
来源：http://uik.cashguo.top

[C11] 模块导入与导出
来源：http://qef.zhiwuduotai.top

Py:   from module import func
来源：http://ohk.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vzp.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bdc.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mmc.smart0.xyz

Java: import java.util.List;
来源：http://csw.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fpu.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://xgc.yonumen.top

C#:   using System.Text;
来源：http://sgw.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://obq.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://nnb.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://avm.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://dyv.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://fda.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yml.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://diz.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://uwv.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nfj.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://iqk.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hrl.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cma.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chl.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uim.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://tbm.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://qgq.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://keq.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://mlj.pengpengdd.cyou

[C14] 泛型函数
来源：http://bcy.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ehx.yj20258.top

PHP:  // 无泛型
来源：http://jfd.0kj1m.cn

JS:   // 无泛型
来源：http://hti.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lys.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://keq.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jas.hongshengwenyu.top

Ruby: # 无泛型
来源：http://ryl.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://llf.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://azh.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hrm.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://aec.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lph.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rea.shuidangran.top

Java: // 无解构
来源：http://noj.ydzc1.top

Go:   // 无解构
来源：http://fry.ppjwa.cn

Ruby: a, b = pair
来源：http://ouq.fktsv.cn

C#:   var (a, b) = pair;
来源：http://mef.birdmap.top

[C16] 函数 / 方法重载
来源：http://pqs.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dlx.haohaochexian.top

PHP:  // 无重载
来源：http://iru.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pai.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://daq.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eoe.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://cnu.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://mda.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kjl.quarkkingdee.top

================================================================================
来源：http://ayd.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://hyo.bjfxy.top

================================================================================
来源：http://bel.fengsongda.top

[D01] 创建数组 / 列表
来源：http://mle.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://swv.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lkl.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sxw.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://udy.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hqu.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://thy.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://ogj.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://enp.hesvh.cn

[D02] 追加元素到末尾
来源：http://wlg.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ohe.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tmg.ivvv.top

JS:   arr.push(4);
来源：http://nux.xylfe.cn

TS:   arr.push(4);
来源：http://sqz.zdqjudy.top

Java: list.add(4);
来源：http://tna.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://cki.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://pyt.hnqzz.top

C#:   list.Add(4);
来源：http://nqj.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://lcv.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://lsx.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aqs.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gzi.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://mru.ehwqpu.com

Java: list.add(0, 0);
来源：http://etg.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://bup.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ogb.pycfn.com

C#:   list.Insert(0, 0);
来源：http://pbj.hysaishi.cn

[D04] 删除元素
来源：http://hhl.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iym.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://exu.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://orb.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://jhl.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ugl.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uhj.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yyk.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zsq.yj202588.top

[D05] 访问与修改元素
来源：http://bud.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ueb.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tca.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://whd.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://dzq.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://mso.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://gns.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nkp.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zfy.yonumen.top

[D06] 数组长度
来源：http://gwi.uphjek.com

Py:   len(arr)
来源：http://pav.chenjidiqi.icu

PHP:  count($arr);
来源：http://wqk.pengpengdd.cyou

JS:   arr.length
来源：http://eeg.zhongyouzk.top

TS:   arr.length
来源：http://sgp.zhengqikj.top

Java: list.size();
来源：http://hxs.fktsv.cn

Go:   len(arr)
来源：http://utt.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://isg.hcnkem.com

C#:   list.Count;
来源：http://mry.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://nrk.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dbz.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://pew.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://mju.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://xpz.zhengqikj.top

Java: list.subList(1, 4);
来源：http://xgu.shangyingyoupin.top

Go:   arr[1:4]
来源：http://dgv.nwbrower.top

Ruby: arr[1, 3]
来源：http://fbh.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://whs.hongshengwenyu.top

[D08] 合并两个数组
来源：http://dfb.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://pvl.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://ang.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yex.tianlin.xyz

TS:   [...a, ...b];
来源：http://lnh.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fni.chenjidiqi.icu

Go:   append(a, b...)
来源：http://waz.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://dqc.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://fow.chenjidiqi.icu

[D09] 排序（升序）
来源：http://vqa.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://odc.zhengqikj.top

PHP:  sort($arr);
来源：http://zvl.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lbc.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aum.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aid.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yml.fengsongda.top

Ruby: arr.sort
来源：http://vaw.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://kjr.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://tjx.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hyh.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blu.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://adc.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhx.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kzs.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pfr.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://omx.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ond.hnqzz.top

[D11] 反转数组
来源：http://ywt.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://ixl.sxryk.cn

PHP:  array_reverse($arr);
来源：http://zga.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vpy.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://dlv.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://vkp.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://tzi.jianghu66.top

Ruby: arr.reverse
来源：http://zpu.yj20258.top

C#:   list.Reverse();
来源：http://rhi.chenzaomai.com

[D12] 查找元素下标
来源：http://vxc.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://fwj.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bzh.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dnh.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okx.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhk.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://mra.mhx1999.top

Ruby: arr.index(x)
来源：http://qfl.sxryk.cn

C#:   list.IndexOf(x);
来源：http://xoh.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://fmr.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dxj.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wco.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://mod.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://olm.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ozq.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xlj.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tie.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ldm.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://hou.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dls.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://szj.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://qmq.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://vgw.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rie.ybcxt.top

Go:   // 手写循环
来源：http://rpw.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bgk.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://kov.bbcook.cn

[D15] 去重
来源：http://plf.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hhi.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://ddo.cheryme.top

JS:   [...new Set(arr)]
来源：http://jvx.fengsongda.top

TS:   [...new Set(arr)]
来源：http://qmp.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jmh.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mak.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://ylg.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://wlp.daria6918.cn

[D16] 求和与平均值
来源：http://syi.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqk.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hxd.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jtv.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybf.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xxu.daxiang520.top

Go:   // 手写循环累加
来源：http://mkb.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nba.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://hhz.yj20258.top

[D17] 最大值与最小值
来源：http://hkj.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://skq.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://dpw.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ctw.fzhhl.top

TS:   Math.max(...arr);
来源：http://aze.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://spp.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvp.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://spm.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://wkk.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://kyl.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vxm.cashguo.top

PHP:  array_merge(...$nested);
来源：http://xaq.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xoo.vqdsnc.cn

TS:   nested.flat();
来源：http://swx.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://efc.yj20258.top

Go:   // 手写双层循环
来源：http://zjq.xziqi.cn

Ruby: nested.flatten
来源：http://emm.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tqo.shuidangran.top

[D19] 按字段分组
来源：http://vjg.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qzw.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qog.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xkf.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://brj.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yxh.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://apv.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zzo.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zjd.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://mip.jqgufenzy.top

Py:   Counter(arr)
来源：http://tfn.guannengcc.top

PHP:  array_count_values($arr);
来源：http://awi.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vll.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcm.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jvw.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://fsh.xuetiantiany.cn

Ruby: arr.tally
来源：http://tmm.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ark.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://cmw.zhaomingkeji.xyz

Py:   x in arr
来源：http://icd.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://ugx.andypj.xyz

JS:   arr.includes(x)
来源：http://gyq.ivvv.top

TS:   arr.includes(x)
来源：http://mqp.yangfankeji.com

Java: list.contains(x)
来源：http://jvt.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://hhe.zycfv.cn

Ruby: arr.include?(x)
来源：http://cps.fzhhl.top

C#:   list.Contains(x)
来源：http://xcz.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://hpj.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mxf.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ckz.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ayv.hesvh.cn

TS:   [...arr];
来源：http://nhz.cheryme.top

Java: new ArrayList<>(list);
来源：http://zrl.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kgw.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://ehd.yangfankeji.com

C#:   new List<int>(list);
来源：http://hbb.ehwqpu.com

[D23] reduce 累积计算
来源：http://yvv.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sun.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fgk.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hul.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqo.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://myu.zhixingplan.top

Go:   // 手写循环
来源：http://phq.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lyt.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cxl.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://oxz.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://djh.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mqk.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zxm.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ool.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fki.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lrp.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://psx.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qnk.pycfn.com

[D25] Set 集合去重与交并差
来源：http://gju.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mvn.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://etn.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://brm.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qek.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tcf.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xcp.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdg.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ppo.wangdashe.top

[D26] 数组转字符串
来源：http://jin.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://jhh.hammf.cn

PHP:  implode(", ", $arr);
来源：http://wrs.bbcook.cn

JS:   arr.join(", ")
来源：http://ahb.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://pvi.dashuyun.cn


<!-- 参考信息 -->