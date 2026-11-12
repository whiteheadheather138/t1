代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://ycg.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jaf.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://trm.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://leg.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://uar.9152youxi.cn

C#:   using System.Text;
来源：http://seu.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://cql.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://snd.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://dqj.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://wkn.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://jjv.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ooy.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://jpi.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://ynv.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://flg.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://eex.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wuu.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ogn.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nwq.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mhq.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://uxv.hcnkem.com

Go:   func add(a, b int) int
来源：http://miy.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eki.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://gee.tarul.cn

[C14] 泛型函数
来源：http://bnl.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ijo.wangdashe.top

PHP:  // 无泛型
来源：http://jaq.cqqwz.cn

JS:   // 无泛型
来源：http://zjv.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ooc.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ykw.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qpr.shuidangran.top

Ruby: # 无泛型
来源：http://jir.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sja.andypj.xyz

[C15] 解构 / 展开参数
来源：http://xbf.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bph.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://cyf.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cgg.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gvx.redwolf501.top

Java: // 无解构
来源：http://qan.cqqwz.cn

Go:   // 无解构
来源：http://bqy.nanxinkj.top

Ruby: a, b = pair
来源：http://jvk.smart0.xyz

C#:   var (a, b) = pair;
来源：http://seq.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://dme.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wmi.yj20258888.top

PHP:  // 无重载
来源：http://wlw.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://beq.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://itp.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aop.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://sln.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://xok.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jaz.vqdsnc.cn

================================================================================
来源：http://ees.cashguo.top

D. 数组 / 列表 / 集合
来源：http://zms.c1oappe.top

================================================================================
来源：http://vvy.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://lyj.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mee.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fae.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yuq.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tkh.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://crz.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://wtd.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://mdj.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ccv.yonumen.top

[D02] 追加元素到末尾
来源：http://fdu.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jvf.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dcv.pycfn.com

JS:   arr.push(4);
来源：http://hye.vehdjk.com

TS:   arr.push(4);
来源：http://kdr.feifeiyinyue.top

Java: list.add(4);
来源：http://tgk.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://tay.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://eet.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://anl.smart0.xyz

[D03] 在指定位置插入元素
来源：http://nrs.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://xjn.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgo.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idt.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://prp.jqgfzy.top

Java: list.add(0, 0);
来源：http://zkf.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://fhu.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jui.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://mpi.dashuyun.cn

[D04] 删除元素
来源：http://izw.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://srh.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mda.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyz.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://wvy.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nry.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pey.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://shu.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jcb.yueranfly.top

[D05] 访问与修改元素
来源：http://okn.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ugb.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgq.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zkm.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://rzc.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://hju.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://fqf.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wle.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tei.guannengcc.top

[D06] 数组长度
来源：http://ckr.hcnkem.com

Py:   len(arr)
来源：http://wsg.shuidangran.top

PHP:  count($arr);
来源：http://ubl.jinqigufen.top

JS:   arr.length
来源：http://dha.gaohongyu789.top

TS:   arr.length
来源：http://hyn.jyoumei.cn

Java: list.size();
来源：http://wnu.fzhhl.top

Go:   len(arr)
来源：http://lou.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://icw.zhengqikj.top

C#:   list.Count;
来源：http://keh.birdmap.top

[D07] 切片 / 取子数组
来源：http://fcw.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rcs.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ubn.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://xnx.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://uds.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://mvs.gotoacloud.top

Go:   arr[1:4]
来源：http://yvj.tanke756.top

Ruby: arr[1, 3]
来源：http://adq.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://ark.chenjidiqi.icu

[D08] 合并两个数组
来源：http://icr.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://dpw.cashguo.top

PHP:  array_merge($a, $b);
来源：http://hri.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vdn.c1oappe.top

TS:   [...a, ...b];
来源：http://nkd.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gcj.ydzc1.top

Go:   append(a, b...)
来源：http://van.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://bcj.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://kti.sufxvd.cn

[D09] 排序（升序）
来源：http://ruz.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zwq.zhengqikj.top

PHP:  sort($arr);
来源：http://zmj.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hvl.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kgu.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://anb.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dpd.zdbjq.cn

Ruby: arr.sort
来源：http://ugs.zhijiandao.cn

C#:   list.Sort();
来源：http://mya.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bad.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nwp.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ide.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yzw.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nks.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vny.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wiz.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://azv.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://syi.jiagoushi.top

[D11] 反转数组
来源：http://oid.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fod.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://fic.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fap.zhengqikj.top

TS:   [...arr].reverse();
来源：http://pvo.nwbrower.top

Java: Collections.reverse(list);
来源：http://nvi.pycfn.com

Go:   slices.Reverse(arr)
来源：http://pdh.tianlin.xyz

Ruby: arr.reverse
来源：http://xjq.redwolf501.top

C#:   list.Reverse();
来源：http://yig.smart0.xyz

[D12] 查找元素下标
来源：http://azo.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://keo.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://shy.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjs.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrh.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xgj.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://eif.ydjk.org.cn

Ruby: arr.index(x)
来源：http://rpe.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://xmw.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://voc.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gyt.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mwr.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://yhd.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://sgn.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jmq.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://klc.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://hwz.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vfg.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://cuu.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kgn.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aki.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://omx.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://ztu.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mpb.ydzc1.top

Go:   // 手写循环
来源：http://ykm.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qdl.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hku.yanxiufei.cn

[D15] 去重
来源：http://gmx.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pob.andypj.xyz

PHP:  array_unique($arr);
来源：http://gop.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://xfe.sxryk.cn

TS:   [...new Set(arr)]
来源：http://aus.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nus.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hhu.tanke756.top

Ruby: arr.uniq
来源：http://pef.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://fyc.nwbrower.top

[D16] 求和与平均值
来源：http://xht.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kki.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bxj.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://irr.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdl.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xpp.jqgufenzy.top

Go:   // 手写循环累加
来源：http://jxf.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fqf.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://kju.fehbvm.com

[D17] 最大值与最小值
来源：http://diz.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://aex.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://shp.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nto.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://rvq.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pof.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://upq.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://whf.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://cjo.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://bqp.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bsv.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://wgw.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://chr.shanyushiyangtech.top

TS:   nested.flat();
来源：http://ofp.fehbvm.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://brt.gotoacloud.top

Go:   // 手写双层循环
来源：http://cuy.wangshuangyany.cn

Ruby: nested.flatten
来源：http://ogq.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mki.zhijiandao.cn

[D19] 按字段分组
来源：http://mat.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xgk.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://scg.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://klh.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://blw.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xgk.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://jrl.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://opj.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pgk.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://jkd.yanxiufei.cn

Py:   Counter(arr)
来源：http://djw.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://uji.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://giz.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpq.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://znf.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://net.ydjk.org.cn

Ruby: arr.tally
来源：http://ydt.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cek.tanke756.top

[D21] 判断是否包含某元素
来源：http://yik.birdmap.top

Py:   x in arr
来源：http://ega.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://rqf.ctjpmb.com

JS:   arr.includes(x)
来源：http://sra.yonumen.top

TS:   arr.includes(x)
来源：http://qpo.wangdashe.top

Java: list.contains(x)
来源：http://mki.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://xxe.0kj1m.cn

Ruby: arr.include?(x)
来源：http://sfi.jinqigufen.top

C#:   list.Contains(x)
来源：http://npl.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://rrc.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nqp.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ubq.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tmb.jinghuilouyu.cn

TS:   [...arr];
来源：http://tsw.yj202588.top

Java: new ArrayList<>(list);
来源：http://jwx.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://qnm.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://ezx.nanxuanxn.top

C#:   new List<int>(list);
来源：http://mcf.yj20258888.top

[D23] reduce 累积计算
来源：http://oaa.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://trq.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://whs.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lrh.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uzc.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jqp.xziqi.cn

Go:   // 手写循环
来源：http://pba.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uxa.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ztg.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://klj.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jir.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yvn.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xhp.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ejz.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ovr.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dlj.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kzc.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zaw.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://fje.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ikr.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xvo.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oxl.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ctc.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ccu.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xna.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rlg.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rtq.yvedp.cn

[D26] 数组转字符串
来源：http://bas.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://mxy.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://hdk.jyoumei.cn

JS:   arr.join(", ")
来源：http://iak.mhx1999.top

TS:   arr.join(", ")
来源：http://lrx.sysykeji.top

Java: String.join(", ", list)
来源：http://fcy.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://bfs.hysaishi.cn

Ruby: arr.join(", ")
来源：http://ffu.zycfv.cn

C#:   string.Join(", ", list)
来源：http://fmo.yj202588.top

================================================================================
来源：http://uyj.zhengqikj.top

E. 字符串处理
来源：http://ogk.yj20258888.top

================================================================================
来源：http://edc.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://cbw.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://chs.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://atd.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fds.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mwt.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mds.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rtf.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vdi.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jrb.ydzc1.top


<!-- 参考信息 -->