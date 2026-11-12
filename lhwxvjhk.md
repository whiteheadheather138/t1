代发 wailian999

[C10] 变量作用域
来源：http://zcp.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rbw.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ydb.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lyt.zhixingplan.top

TS:   同 JS
来源：http://esc.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://ayq.xuanzx.com

Go:   花括号块级作用域
来源：http://wrb.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opv.daxiang520.top

C#:   块级作用域
来源：http://sru.nanxinkj.top

[C11] 模块导入与导出
来源：http://xzt.cqqwz.cn

Py:   from module import func
来源：http://ggp.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mbj.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gmw.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uhg.gogol.net.cn

Java: import java.util.List;
来源：http://peq.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bxv.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://okf.shangyingyoupin.top

C#:   using System.Text;
来源：http://ofi.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://nbm.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://dph.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://hre.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://may.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://tvu.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mon.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://zox.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://lln.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tih.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://fyh.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fse.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfb.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qkx.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://skz.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://dcr.fengsongda.top

Go:   func add(a, b int) int
来源：http://zds.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://odd.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://rnq.daxiang520.top

[C14] 泛型函数
来源：http://afn.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zfb.gotoacloud.top

PHP:  // 无泛型
来源：http://hxc.zhixingplan.top

JS:   // 无泛型
来源：http://pyg.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zki.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hur.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bwx.chenlongwang.top

Ruby: # 无泛型
来源：http://gjs.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vsl.jianghu66.top

[C15] 解构 / 展开参数
来源：http://ymy.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qay.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://vkp.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lvf.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eqk.kuanghao11.cn

Java: // 无解构
来源：http://gre.feifeiyinyue.top

Go:   // 无解构
来源：http://lln.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://wup.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://apx.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://xwb.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tqj.cashguo.top

PHP:  // 无重载
来源：http://wdx.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://itv.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://eoz.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://owh.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://jbi.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://vbm.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://wnl.zhiwuduotai.top

================================================================================
来源：http://ilg.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://kor.hesvh.cn

================================================================================
来源：http://wos.bbcook.cn

[D01] 创建数组 / 列表
来源：http://qck.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ttl.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cuy.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://olu.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oxd.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ezm.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://wfn.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://ezq.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hyc.meibo888.top

[D02] 追加元素到末尾
来源：http://phd.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zbi.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rtb.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://eds.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://ldc.xinyue.icu

Java: list.add(4);
来源：http://yhn.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://ioq.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://bdu.zhixingplan.top

C#:   list.Add(4);
来源：http://wsk.uphjek.com

[D03] 在指定位置插入元素
来源：http://fjq.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://ein.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wib.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://paq.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://ncw.guowangkeji.top

Java: list.add(0, 0);
来源：http://lwb.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://zub.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fec.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://eeu.chenlongwang.top

[D04] 删除元素
来源：http://yas.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eie.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bjw.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tey.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://xxi.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bjq.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://epw.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xzy.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cuh.xylfe.cn

[D05] 访问与修改元素
来源：http://xlm.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mjv.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zrq.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://slb.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://kfs.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://glc.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://qbq.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bda.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nib.sxryk.cn

[D06] 数组长度
来源：http://mey.yvedp.cn

Py:   len(arr)
来源：http://omb.svipenyu.cn

PHP:  count($arr);
来源：http://fqi.shzxlz.cn

JS:   arr.length
来源：http://hzy.ppjwa.cn

TS:   arr.length
来源：http://hjr.ppjwa.cn

Java: list.size();
来源：http://gbc.hnxiangtu.top

Go:   len(arr)
来源：http://unt.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://vkp.sxryk.cn

C#:   list.Count;
来源：http://uvm.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://hwo.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aoz.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://mdv.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://pqz.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://pns.jyoumei.cn

Java: list.subList(1, 4);
来源：http://woe.cheryme.top

Go:   arr[1:4]
来源：http://dqj.c1oappe.top

Ruby: arr[1, 3]
来源：http://dxk.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://fsm.hongshengwenyu.top

[D08] 合并两个数组
来源：http://cfa.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://gol.yongpay.top

PHP:  array_merge($a, $b);
来源：http://vpg.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dwp.mhx1999.top

TS:   [...a, ...b];
来源：http://kea.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zkp.havefunace.top

Go:   append(a, b...)
来源：http://ojo.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://srl.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://edx.aibaodan.cn

[D09] 排序（升序）
来源：http://res.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://wzg.snrcjt.cn

PHP:  sort($arr);
来源：http://iqn.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xvl.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tvx.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://txl.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xbn.quarkkingdee.top

Ruby: arr.sort
来源：http://gep.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://gsw.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xxo.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iot.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovv.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wcd.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iiz.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nha.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://drq.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kcz.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nin.jlsjyb.cn

[D11] 反转数组
来源：http://ads.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://pwz.fehbvm.com

PHP:  array_reverse($arr);
来源：http://tte.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jqw.zycfv.cn

TS:   [...arr].reverse();
来源：http://nex.sxryk.cn

Java: Collections.reverse(list);
来源：http://qqg.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://hhh.yongpay.top

Ruby: arr.reverse
来源：http://iyg.snrcjt.cn

C#:   list.Reverse();
来源：http://wmz.pengpengdd.cyou

[D12] 查找元素下标
来源：http://odc.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://ycs.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqr.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://stt.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gbh.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mrj.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://stm.hnxiangtu.top

Ruby: arr.index(x)
来源：http://jwf.sweek.top

C#:   list.IndexOf(x);
来源：http://hsw.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://usk.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ido.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://odz.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://iet.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://hxx.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qek.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qgk.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://zxx.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://cwp.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://svl.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lij.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbo.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://vyx.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://vbx.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yik.havefunace.top

Go:   // 手写循环
来源：http://bxn.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://zgl.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://scz.jlsjyb.cn

[D15] 去重
来源：http://pce.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bvy.cheryme.top

PHP:  array_unique($arr);
来源：http://wei.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://sfw.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://pxq.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xho.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://yxo.hfpthk.cn

Ruby: arr.uniq
来源：http://nen.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://vpr.hammf.cn

[D16] 求和与平均值
来源：http://dzf.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://smd.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://asa.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zfp.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sox.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xav.wangdashe.top

Go:   // 手写循环累加
来源：http://mbo.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xjd.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://bez.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://qjc.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://pus.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://nzy.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tdv.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://pyr.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fqo.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qdk.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://dcj.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://vol.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://rhd.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zsk.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://tdg.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zui.cashguo.top

TS:   nested.flat();
来源：http://mym.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mcy.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://uxn.gogol.net.cn

Ruby: nested.flatten
来源：http://khh.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://twb.xylfe.cn

[D19] 按字段分组
来源：http://fng.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ubq.andypj.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://obz.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jzr.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vap.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ceh.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://jqa.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://twr.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gsn.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://rdt.fehbvm.com

Py:   Counter(arr)
来源：http://lje.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://fon.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pik.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scv.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bem.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://hvz.hfpthk.cn

Ruby: arr.tally
来源：http://rjs.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xkj.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://yaz.tarul.cn

Py:   x in arr
来源：http://zjg.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://jhg.tanke756.top

JS:   arr.includes(x)
来源：http://wii.jyoumei.cn

TS:   arr.includes(x)
来源：http://nkx.bjfxy.top

Java: list.contains(x)
来源：http://zeg.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://uzq.jinqigufen.top

Ruby: arr.include?(x)
来源：http://gks.jqgufenzy.top

C#:   list.Contains(x)
来源：http://ufv.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://fwx.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xxy.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kcy.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hae.tarul.cn

TS:   [...arr];
来源：http://vlk.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://zlc.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zdh.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://itb.chenzaomai.com

C#:   new List<int>(list);
来源：http://lsg.shuidangran.top

[D23] reduce 累积计算
来源：http://qxq.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lsp.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gku.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmx.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zft.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://uhh.quarkkingdee.top

Go:   // 手写循环
来源：http://kcp.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lsy.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gnl.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://fwe.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aey.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://too.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://owb.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dwt.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jdt.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hmz.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vuy.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://agb.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://xcy.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ipq.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bxs.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://udg.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vnt.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zoa.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kth.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jyw.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qdn.hnxiangtu.top

[D26] 数组转字符串
来源：http://irn.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://xnd.meibo888.top

PHP:  implode(", ", $arr);
来源：http://deu.zhongyouzk.top

JS:   arr.join(", ")
来源：http://ucz.hnxiangtu.top

TS:   arr.join(", ")
来源：http://hpz.daxiang520.top

Java: String.join(", ", list)
来源：http://yau.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://njx.cheryme.top

Ruby: arr.join(", ")
来源：http://flt.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://xlp.tianlin.xyz


<!-- 参考信息 -->