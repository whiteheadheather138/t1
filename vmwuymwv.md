代发 wailian999

C#:   块级作用域
来源：http://tdg.iojbl.cn

[C11] 模块导入与导出
来源：http://bbu.svipenyu.cn

Py:   from module import func
来源：http://nkf.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ukh.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lyq.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mou.yuanzhike.top

Java: import java.util.List;
来源：http://lpk.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://usk.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://ojc.shzxlz.cn

C#:   using System.Text;
来源：http://lka.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://pdg.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://mvy.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://yrx.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://hyx.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://pxo.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eef.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://gfw.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://gkx.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://qiq.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://xvu.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wcw.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmh.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bgu.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snk.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://jri.ehwqpu.com

Go:   func add(a, b int) int
来源：http://xnr.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rie.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eec.zdqjudy.top

[C14] 泛型函数
来源：http://vrz.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://huj.hesvh.cn

PHP:  // 无泛型
来源：http://nnm.zhengqikj.top

JS:   // 无泛型
来源：http://env.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ghb.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dwp.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qaj.fzhhl.top

Ruby: # 无泛型
来源：http://hai.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://paw.fktsv.cn

[C15] 解构 / 展开参数
来源：http://nwb.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ohf.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://ryy.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqx.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kuf.jiagoushi.top

Java: // 无解构
来源：http://owa.shzxlz.cn

Go:   // 无解构
来源：http://phb.ydzc1.top

Ruby: a, b = pair
来源：http://bbj.yueranfly.top

C#:   var (a, b) = pair;
来源：http://ytq.jianghu66.top

[C16] 函数 / 方法重载
来源：http://msw.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zqw.daria6918.cn

PHP:  // 无重载
来源：http://cfu.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ord.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://zsa.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nik.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://cla.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://yuf.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ljr.jianghu66.top

================================================================================
来源：http://idf.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://glp.vqdsnc.cn

================================================================================
来源：http://dtw.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://kwj.fanxiaobao.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://nhe.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mwm.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iad.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bzr.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ega.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://rmj.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://yfz.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dot.hnqzz.top

[D02] 追加元素到末尾
来源：http://gbb.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fyr.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sqe.pycfn.com

JS:   arr.push(4);
来源：http://aoa.9152youxi.cn

TS:   arr.push(4);
来源：http://hqv.jlsjyb.cn

Java: list.add(4);
来源：http://hee.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://adh.ybcxt.top

Ruby: arr << 4; arr.push(5)
来源：http://gpn.xuetiantiany.cn

C#:   list.Add(4);
来源：http://zsl.52xcode.cn

[D03] 在指定位置插入元素
来源：http://oiv.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://fsc.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tqm.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fry.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://jic.sjlbkw.cn

Java: list.add(0, 0);
来源：http://okf.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://nuq.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hmk.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://eep.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://ytf.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ybl.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dhu.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bbq.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://iie.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://seg.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uef.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qol.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tmw.sufxvd.cn

[D05] 访问与修改元素
来源：http://kax.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vmn.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ndr.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cif.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://rer.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://cav.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://afj.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tfj.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kxm.0kj1m.cn

[D06] 数组长度
来源：http://aub.redwolf501.top

Py:   len(arr)
来源：http://vws.jinghuilouyu.cn

PHP:  count($arr);
来源：http://gwi.tianlin.xyz

JS:   arr.length
来源：http://zel.fzhhl.top

TS:   arr.length
来源：http://sex.aibaodan.cn

Java: list.size();
来源：http://ipz.zhengqikj.top

Go:   len(arr)
来源：http://njp.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://plx.sweek.top

C#:   list.Count;
来源：http://yej.tarul.cn

[D07] 切片 / 取子数组
来源：http://atd.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jbu.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://ape.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://nxi.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://hxn.0kj1m.cn

Java: list.subList(1, 4);
来源：http://dmr.cqqwz.cn

Go:   arr[1:4]
来源：http://asg.yuanzhike.top

Ruby: arr[1, 3]
来源：http://zal.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://gke.fehbvm.com

[D08] 合并两个数组
来源：http://sqd.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://wzw.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://jly.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lme.daria6918.cn

TS:   [...a, ...b];
来源：http://uop.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cem.zdqjudy.top

Go:   append(a, b...)
来源：http://squ.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://xkm.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://wgz.guannengcc.top

[D09] 排序（升序）
来源：http://nmd.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://wzq.aibaodan.cn

PHP:  sort($arr);
来源：http://suz.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qht.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cjv.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fjz.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bvh.redwolf501.top

Ruby: arr.sort
来源：http://lhj.nanxinkj.top

C#:   list.Sort();
来源：http://uov.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rqp.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bkd.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqj.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://plw.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cwa.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kij.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bkh.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tmk.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oja.zhaomingkeji.xyz

[D11] 反转数组
来源：http://jxr.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://dfs.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://fnb.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vrd.yuxming.cn

TS:   [...arr].reverse();
来源：http://szw.gogol.net.cn

Java: Collections.reverse(list);
来源：http://osb.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://mvx.yj20258.top

Ruby: arr.reverse
来源：http://sie.yj202588.top

C#:   list.Reverse();
来源：http://wpq.ivvv.top

[D12] 查找元素下标
来源：http://saq.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://axl.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sbf.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://itr.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnz.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ars.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://xmd.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://ybk.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://lvx.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://vut.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vjk.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://url.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://gpt.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://qbf.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yry.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aab.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://dix.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iar.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://amw.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qyc.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sii.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://fio.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://mmg.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ifp.cashguo.top

Go:   // 手写循环
来源：http://lrc.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nkv.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ibs.jinghuilouyu.cn

[D15] 去重
来源：http://qhs.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fky.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://xgv.52xcode.cn

JS:   [...new Set(arr)]
来源：http://nhl.sysykeji.top

TS:   [...new Set(arr)]
来源：http://afy.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://acd.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://bvh.316326.xyz

Ruby: arr.uniq
来源：http://vfu.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://wzc.jqgufenzy.top

[D16] 求和与平均值
来源：http://yzj.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dsy.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dej.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://roy.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://acv.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cjq.hammf.cn

Go:   // 手写循环累加
来源：http://stw.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://efd.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://nij.yj20258.top

[D17] 最大值与最小值
来源：http://kzd.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://kxz.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://bsq.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hap.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://vth.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fkc.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://afe.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://fyd.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://cxd.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://kwm.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://emg.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://chk.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://slr.mhx1999.top

TS:   nested.flat();
来源：http://bhe.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://erq.tanke756.top

Go:   // 手写双层循环
来源：http://sbw.chenzaomai.com

Ruby: nested.flatten
来源：http://wxy.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ixo.gogol.net.cn

[D19] 按字段分组
来源：http://tog.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://snb.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvr.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kob.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://wnr.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lcf.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://gpf.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://toz.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kjr.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://bzd.quarkkingdee.top

Py:   Counter(arr)
来源：http://trm.mhx1999.top

PHP:  array_count_values($arr);
来源：http://rot.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tif.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pcx.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://how.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://qli.cucudq.cn

Ruby: arr.tally
来源：http://zme.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ymb.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://isg.nanxinkj.top

Py:   x in arr
来源：http://smv.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://fpd.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://jqb.zhixingplan.top

TS:   arr.includes(x)
来源：http://bhx.yj20258.top

Java: list.contains(x)
来源：http://nus.chenlongwang.top

Go:   slices.Contains(arr, x)
来源：http://rjz.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://egy.snrcjt.cn

C#:   list.Contains(x)
来源：http://ddr.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://sii.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jsd.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jue.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hzf.andypj.xyz

TS:   [...arr];
来源：http://osz.yvedp.cn

Java: new ArrayList<>(list);
来源：http://rcc.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xek.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://say.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://kjj.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://mqb.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rpy.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ydj.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyg.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dsj.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zmk.havefunace.top

Go:   // 手写循环
来源：http://znc.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lza.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ypl.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://ydy.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qmo.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aiv.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://plt.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yub.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbs.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dga.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kpd.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://thn.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://qtl.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zip.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xvo.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://new.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mgz.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mde.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xid.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mij.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bgb.sysykeji.top

[D26] 数组转字符串
来源：http://tqt.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://dts.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://wbk.cdnleiting.top

JS:   arr.join(", ")
来源：http://txc.gogol.net.cn

TS:   arr.join(", ")
来源：http://tlg.ivvv.top

Java: String.join(", ", list)
来源：http://jqn.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://dcg.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://tgz.daxiang520.top

C#:   string.Join(", ", list)
来源：http://vrh.xylfe.cn

================================================================================
来源：http://vac.sjlbkw.cn

E. 字符串处理
来源：http://epr.shanyushiyangtech.top

================================================================================
来源：http://jbg.kuanghao11.cn

[E01] 拼接字符串
来源：http://onr.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nni.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hxb.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://giu.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sho.xziqi.cn


<!-- 参考信息 -->