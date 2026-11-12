代发 wailian999

C#:   块级作用域
来源：http://rfk.vqdsnc.cn

[C11] 模块导入与导出
来源：http://stq.yfazqb.com

Py:   from module import func
来源：http://vuy.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qdk.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tgm.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hed.aibaodan.cn

Java: import java.util.List;
来源：http://glc.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gwj.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wyc.sysykeji.top

C#:   using System.Text;
来源：http://esu.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://lbj.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://xjn.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://xeg.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://fgc.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://gol.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://luo.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://cbc.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://tyw.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nww.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://vou.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rkc.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://faa.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://knc.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://phl.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://hsv.snrcjt.cn

Go:   func add(a, b int) int
来源：http://cuk.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hqv.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xqs.ivvv.top

[C14] 泛型函数
来源：http://lmp.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qcr.ehwqpu.com

PHP:  // 无泛型
来源：http://adj.dianchejie.cn

JS:   // 无泛型
来源：http://ybd.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bwe.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vbf.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xrq.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://awt.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://soi.fzhhl.top

[C15] 解构 / 展开参数
来源：http://zon.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aub.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://dmx.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yvz.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzk.cdnleiting.top

Java: // 无解构
来源：http://ooe.tian-w.cn

Go:   // 无解构
来源：http://jzv.hnxiangtu.top

Ruby: a, b = pair
来源：http://pln.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://vys.mhx1999.top

[C16] 函数 / 方法重载
来源：http://utg.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gpt.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://zdb.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gux.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://dam.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zqq.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://bxl.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://buk.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jso.shanyushiyangtech.top

================================================================================
来源：http://kuf.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://xup.andypj.xyz

================================================================================
来源：http://oum.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://xxy.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://opn.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovs.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tov.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bjo.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lwc.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://wnb.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://hqn.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gvn.yangfankeji.com

[D02] 追加元素到末尾
来源：http://lsq.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gla.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rdq.tianlin.xyz

JS:   arr.push(4);
来源：http://umh.hongshengwenyu.top

TS:   arr.push(4);
来源：http://zvs.yongpay.top

Java: list.add(4);
来源：http://sjc.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://rvv.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://gda.wangshuangyany.cn

C#:   list.Add(4);
来源：http://sun.hnqzz.top

[D03] 在指定位置插入元素
来源：http://xto.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://tes.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zyt.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pqo.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://waa.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://tnv.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://shq.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qsy.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://xuj.snrcjt.cn

[D04] 删除元素
来源：http://obq.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hrq.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yfh.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uhk.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://snu.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yfj.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pkr.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lxh.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pnm.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://ict.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gki.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jma.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvx.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://vqy.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://ldb.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://jma.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nbg.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fja.fzhhl.top

[D06] 数组长度
来源：http://ofr.pycfn.com

Py:   len(arr)
来源：http://fmr.xinyue.icu

PHP:  count($arr);
来源：http://zgj.tarul.cn

JS:   arr.length
来源：http://ppj.fehbvm.com

TS:   arr.length
来源：http://vlp.shanyushiyangtech.top

Java: list.size();
来源：http://jmv.pycfn.com

Go:   len(arr)
来源：http://dbt.yfazqb.com

Ruby: arr.length; arr.size
来源：http://tgq.shanyushiyangkeji.top

C#:   list.Count;
来源：http://wzm.52xcode.cn

[D07] 切片 / 取子数组
来源：http://din.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eys.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wry.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://xio.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://rod.haohaochexian.top

Java: list.subList(1, 4);
来源：http://rlh.jqgfzy.top

Go:   arr[1:4]
来源：http://zfm.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://xtj.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://lqx.yfazqb.com

[D08] 合并两个数组
来源：http://vms.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://qfm.yj202588.top

PHP:  array_merge($a, $b);
来源：http://xjj.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tzx.shuidangran.top

TS:   [...a, ...b];
来源：http://rgo.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bov.svipenyu.cn

Go:   append(a, b...)
来源：http://ump.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://tdm.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://dnf.nanxuanxn.top

[D09] 排序（升序）
来源：http://lrk.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://dej.daxiang520.top

PHP:  sort($arr);
来源：http://fyk.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lwk.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fuh.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://doo.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gai.gaohongyu789.top

Ruby: arr.sort
来源：http://wiv.dashuyun.cn

C#:   list.Sort();
来源：http://ogx.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://twt.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://npn.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ztz.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bkf.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://upl.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zgb.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zzk.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uha.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kwn.vehdjk.com

[D11] 反转数组
来源：http://sds.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://hpb.zycfv.cn

PHP:  array_reverse($arr);
来源：http://wba.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ntd.yueranfly.top

TS:   [...arr].reverse();
来源：http://ldr.hywenlv.cn

Java: Collections.reverse(list);
来源：http://ewy.meibo888.top

Go:   slices.Reverse(arr)
来源：http://uxe.pengpengdd.cyou

Ruby: arr.reverse
来源：http://qbn.chenjidiqi.icu

C#:   list.Reverse();
来源：http://osh.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://tks.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://jxg.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vjw.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://seq.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuh.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jpb.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://pya.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://umz.yuxming.cn

C#:   list.IndexOf(x);
来源：http://ufa.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://osn.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yan.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tdr.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://oou.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://zho.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bkz.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mvf.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://viw.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wgq.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://gxo.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ejt.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fey.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://cux.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://luz.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lsd.tanke756.top

Go:   // 手写循环
来源：http://wqx.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://vsw.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zty.ppjwa.cn

[D15] 去重
来源：http://axs.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://koy.cqqwz.cn

PHP:  array_unique($arr);
来源：http://ugu.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://uko.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://iif.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyb.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://bht.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://hsf.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://znu.gogol.net.cn

[D16] 求和与平均值
来源：http://zee.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdl.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://foe.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrh.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://por.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vej.ybcxt.top

Go:   // 手写循环累加
来源：http://yry.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://psx.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://blt.uphjek.com

[D17] 最大值与最小值
来源：http://vvx.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://rrr.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://hyb.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zeo.cucudq.cn

TS:   Math.max(...arr);
来源：http://gvt.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://arv.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jso.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://jfx.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://qxs.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://asz.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hwr.ivvv.top

PHP:  array_merge(...$nested);
来源：http://qxm.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wgo.kuanghao11.cn

TS:   nested.flat();
来源：http://gzc.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://twq.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://smg.yongpay.top

Ruby: nested.flatten
来源：http://khf.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pcy.zycfv.cn

[D19] 按字段分组
来源：http://abx.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pkw.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zsc.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yta.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kqq.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://beu.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://zlb.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zeo.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oct.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://vin.tarul.cn

Py:   Counter(arr)
来源：http://tpn.uphjek.com

PHP:  array_count_values($arr);
来源：http://cdc.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qfs.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dby.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bgo.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://hdq.316326.xyz

Ruby: arr.tally
来源：http://gqa.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uvy.tian-w.cn

[D21] 判断是否包含某元素
来源：http://bku.gaohongyu789.top

Py:   x in arr
来源：http://ney.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://tjz.snrcjt.cn

JS:   arr.includes(x)
来源：http://gzf.zhongyouzk.top

TS:   arr.includes(x)
来源：http://crt.cashguo.top

Java: list.contains(x)
来源：http://fxr.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://moq.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://cqx.xinyue.icu

C#:   list.Contains(x)
来源：http://pul.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://afn.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jqt.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jxh.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hko.yj20258888.top

TS:   [...arr];
来源：http://kpn.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://vwh.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://qok.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://ani.vehdjk.com

C#:   new List<int>(list);
来源：http://hnf.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://zqb.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nvx.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cki.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbh.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zjp.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://baq.316326.xyz

Go:   // 手写循环
来源：http://sxq.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://znw.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ekv.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://oqn.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yuz.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fbe.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tpf.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nfs.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dok.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hid.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jwd.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mhg.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://giy.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ycd.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://axd.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jec.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tio.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vti.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://skm.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aec.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cuw.hammf.cn

[D26] 数组转字符串
来源：http://zyk.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://scn.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://lai.sjlbkw.cn

JS:   arr.join(", ")
来源：http://aoq.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://ghk.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://ykg.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://vro.snrcjt.cn

Ruby: arr.join(", ")
来源：http://ljr.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://zoi.cucudq.cn

================================================================================
来源：http://gsk.tarul.cn

E. 字符串处理
来源：http://jtw.hnxiangtu.top

================================================================================
来源：http://ttd.tian-w.cn

[E01] 拼接字符串
来源：http://opa.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cws.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fmr.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bjx.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tdx.xziqi.cn


<!-- 参考信息 -->