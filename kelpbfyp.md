代发 wailian999

TS:   同 JS
来源：http://vkr.ppjwa.cn

Java: 方法内为块级作用域
来源：http://cgx.bbcook.cn

Go:   花括号块级作用域
来源：http://pbg.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://khx.cheryme.top

C#:   块级作用域
来源：http://llo.jqgufenzy.top

[C11] 模块导入与导出
来源：http://knb.yonumen.top

Py:   from module import func
来源：http://xcd.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pzu.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kgp.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://umf.andypj.xyz

Java: import java.util.List;
来源：http://qiw.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://emc.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://jly.hammf.cn

C#:   using System.Text;
来源：http://lfn.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://vuu.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://sic.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://pln.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://rif.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://rer.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://enz.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://dqc.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://zsz.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hww.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://tlg.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mjr.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xya.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://psu.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbf.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gku.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://cun.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jzc.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wtj.fehbvm.com

[C14] 泛型函数
来源：http://qpm.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pju.0kj1m.cn

PHP:  // 无泛型
来源：http://uxc.yj202588.top

JS:   // 无泛型
来源：http://pej.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://waj.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bps.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qve.gzhubu.top

Ruby: # 无泛型
来源：http://eka.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jyo.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://lsc.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jdr.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://zni.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ucb.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://byb.yuanzhike.top

Java: // 无解构
来源：http://otm.daria6918.cn

Go:   // 无解构
来源：http://ulr.dianchejie.cn

Ruby: a, b = pair
来源：http://ufn.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://egh.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://mue.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fth.wangdashe.top

PHP:  // 无重载
来源：http://plv.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ntn.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://qlh.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wbg.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://dtt.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://div.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kpu.hywenlv.cn

================================================================================
来源：http://ext.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://pyx.yuxming.cn

================================================================================
来源：http://dbg.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://spv.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nzm.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pbg.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wub.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ptk.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://biq.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://mzw.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://eru.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ynb.smart0.xyz

[D02] 追加元素到末尾
来源：http://ajz.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqy.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oky.mhx1999.top

JS:   arr.push(4);
来源：http://dtp.vehdjk.com

TS:   arr.push(4);
来源：http://tig.hnxiangtu.top

Java: list.add(4);
来源：http://lgy.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://nyg.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://oex.gogol.net.cn

C#:   list.Add(4);
来源：http://cxq.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://yla.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://nal.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://auk.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dlv.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://hrt.yj20258888.top

Java: list.add(0, 0);
来源：http://tzq.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://gvb.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dpz.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://pcw.daxiang520.top

[D04] 删除元素
来源：http://gdy.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tze.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://omc.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tmh.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://fjh.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mjg.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mjf.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rkm.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fni.hcnkem.com

[D05] 访问与修改元素
来源：http://qlo.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pyy.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tuk.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://roo.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://abv.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://kmb.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xui.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://otc.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://evt.tianlin.xyz

[D06] 数组长度
来源：http://dfo.pycfn.com

Py:   len(arr)
来源：http://tho.fktsv.cn

PHP:  count($arr);
来源：http://oik.jqgfzy.top

JS:   arr.length
来源：http://sdr.sjlbkw.cn

TS:   arr.length
来源：http://vgo.haohaochexian.top

Java: list.size();
来源：http://fgk.ppjwa.cn

Go:   len(arr)
来源：http://iom.xuanzx.com

Ruby: arr.length; arr.size
来源：http://jkh.yfazqb.com

C#:   list.Count;
来源：http://vok.daria6918.cn

[D07] 切片 / 取子数组
来源：http://izf.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jve.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://gec.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://ftw.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://nvm.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://ecq.xuetiantiany.cn

Go:   arr[1:4]
来源：http://obv.tanke756.top

Ruby: arr[1, 3]
来源：http://rqh.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://vbb.tianlin.xyz

[D08] 合并两个数组
来源：http://asg.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://jgl.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://coy.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dfv.wangdashe.top

TS:   [...a, ...b];
来源：http://uhv.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bvs.andypj.xyz

Go:   append(a, b...)
来源：http://rfx.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://vyg.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://lxg.zhiwuduotai.top

[D09] 排序（升序）
来源：http://qyf.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vss.ydjk.org.cn

PHP:  sort($arr);
来源：http://ekb.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ucf.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ued.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uvj.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wtw.jinqigfzy.top

Ruby: arr.sort
来源：http://kgj.hesvh.cn

C#:   list.Sort();
来源：http://jmq.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lln.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wjr.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzo.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mtu.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gxj.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wjn.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdk.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ylu.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://isg.guannengcc.top

[D11] 反转数组
来源：http://leq.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://xdb.yj20258.top

PHP:  array_reverse($arr);
来源：http://mpe.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yms.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://sct.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://aeq.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://dus.shzxlz.cn

Ruby: arr.reverse
来源：http://iat.jyoumei.cn

C#:   list.Reverse();
来源：http://owy.yueranfly.top

[D12] 查找元素下标
来源：http://csg.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://djy.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hng.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjk.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zer.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsx.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://pwm.tarul.cn

Ruby: arr.index(x)
来源：http://oup.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://sfb.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://tdc.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gln.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jan.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://col.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://qat.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hhh.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zvx.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hle.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://tis.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://yfd.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oyt.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tzm.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://wpb.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://xjm.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ysv.sxryk.cn

Go:   // 手写循环
来源：http://kxs.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://hsf.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://nut.wangdashe.top

[D15] 去重
来源：http://nys.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nfe.hfpthk.cn

PHP:  array_unique($arr);
来源：http://ztd.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://gwv.316326.xyz

TS:   [...new Set(arr)]
来源：http://tfd.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tgt.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oyc.quarkkingdee.top

Ruby: arr.uniq
来源：http://tmy.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://hkd.yj20258.top

[D16] 求和与平均值
来源：http://vkf.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvh.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bfx.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqn.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tvh.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nuh.fengsongda.top

Go:   // 手写循环累加
来源：http://pfo.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://juu.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://dkf.xinyue.icu

[D17] 最大值与最小值
来源：http://iar.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://cyp.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://oma.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iem.52xcode.cn

TS:   Math.max(...arr);
来源：http://twg.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://knm.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://njl.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://iri.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://vba.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://nen.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujy.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://ivr.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uqt.mhx1999.top

TS:   nested.flat();
来源：http://kfx.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://btw.xuanzx.com

Go:   // 手写双层循环
来源：http://ocd.uphjek.com

Ruby: nested.flatten
来源：http://hva.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bzw.yueranfly.top

[D19] 按字段分组
来源：http://mfx.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aoc.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://keb.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://opn.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zcz.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://soi.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://kyt.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://jxv.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ntj.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://aqv.vqdsnc.cn

Py:   Counter(arr)
来源：http://czc.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://bsj.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oco.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afm.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nte.uphjek.com

Go:   // 手写 map[T]int
来源：http://sqj.bjfxy.top

Ruby: arr.tally
来源：http://hkf.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vdu.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://idf.yfazqb.com

Py:   x in arr
来源：http://qgq.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://kru.yongpay.top

JS:   arr.includes(x)
来源：http://pux.svipenyu.cn

TS:   arr.includes(x)
来源：http://bvk.shanyushiyangtech.top

Java: list.contains(x)
来源：http://hdl.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://oya.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://cii.jqgfzy.top

C#:   list.Contains(x)
来源：http://aho.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://ioo.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fad.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hvr.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xom.hnxiangtu.top

TS:   [...arr];
来源：http://dpc.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://pkv.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://aij.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://yzi.bjfxy.top

C#:   new List<int>(list);
来源：http://olk.yuxming.cn

[D23] reduce 累积计算
来源：http://idd.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ttb.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bxf.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzx.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyk.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hcl.iojbl.cn

Go:   // 手写循环
来源：http://qfk.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rts.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rsy.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://twg.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://diu.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://unf.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rve.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tmx.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://obb.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lpa.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://psw.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gwo.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://phi.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kua.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyz.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uco.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sbj.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gpx.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wji.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltn.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ynh.dianchejie.cn

[D26] 数组转字符串
来源：http://cpd.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://wfu.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://dqx.quarkkingdee.top

JS:   arr.join(", ")
来源：http://qjp.c1oappe.top

TS:   arr.join(", ")
来源：http://yaa.bjfxy.top

Java: String.join(", ", list)
来源：http://ouw.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://bjt.yuanzhike.top

Ruby: arr.join(", ")
来源：http://dan.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://goz.zhijiandao.cn

================================================================================
来源：http://hxe.yvedp.cn

E. 字符串处理
来源：http://wri.xylfe.cn

================================================================================
来源：http://aer.hongshengwenyu.top

[E01] 拼接字符串
来源：http://vas.yj202588.top


<!-- 参考信息 -->