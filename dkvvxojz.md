代发 wailian999

C#:   块级作用域
来源：http://csy.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://htc.hesvh.cn

Py:   from module import func
来源：http://zxd.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qng.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://pdn.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tax.sysykeji.top

Java: import java.util.List;
来源：http://kbj.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jkq.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://trv.hesvh.cn

C#:   using System.Text;
来源：http://bnr.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://vcg.hfpthk.cn

Py:   (lambda: print("run"))()
来源：http://uza.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://oxi.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://unf.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://csu.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sij.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://lfj.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://fla.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://icl.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://ckr.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://exp.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ffn.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eqt.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://olu.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://drj.zdbjq.cn

Go:   func add(a, b int) int
来源：http://hky.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yle.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nin.zhijiandao.cn

[C14] 泛型函数
来源：http://uxd.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mwx.ydjk.org.cn

PHP:  // 无泛型
来源：http://zkn.jiagoushi.top

JS:   // 无泛型
来源：http://fox.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ojv.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jsq.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hqm.wangshuangyany.cn

Ruby: # 无泛型
来源：http://ouv.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvs.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://dld.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ycg.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://krz.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jad.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qmy.smart0.xyz

Java: // 无解构
来源：http://zck.tianlin.xyz

Go:   // 无解构
来源：http://qwn.ydzc1.top

Ruby: a, b = pair
来源：http://nwt.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://toj.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://spt.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jlx.yongpay.top

PHP:  // 无重载
来源：http://tzb.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zos.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://hoj.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ddp.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://uwr.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://bco.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mdz.sweek.top

================================================================================
来源：http://iwb.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://iks.daxiang520.top

================================================================================
来源：http://kuo.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://evm.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tsl.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcd.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mty.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zwl.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pth.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://vuu.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://jjg.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uic.yuxming.cn

[D02] 追加元素到末尾
来源：http://miq.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fhb.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cvx.tian-w.cn

JS:   arr.push(4);
来源：http://jgv.mhx1999.top

TS:   arr.push(4);
来源：http://zal.shangyingyoupin.top

Java: list.add(4);
来源：http://tvd.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://trl.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://byj.snrcjt.cn

C#:   list.Add(4);
来源：http://wwu.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://rzq.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://zbr.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ilx.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tkq.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://fvd.ybcxt.top

Java: list.add(0, 0);
来源：http://grh.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://wuh.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bzg.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://yrv.pycfn.com

[D04] 删除元素
来源：http://wxj.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ooc.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://niu.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hmd.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://xmt.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ekb.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iul.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gyf.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qvh.jinqigfzy.top

[D05] 访问与修改元素
来源：http://iux.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jka.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nss.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qmf.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://lor.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://akg.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://luq.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kqt.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fpi.hysaishi.cn

[D06] 数组长度
来源：http://dcz.fehbvm.com

Py:   len(arr)
来源：http://sgd.yvedp.cn

PHP:  count($arr);
来源：http://xny.yuanzhike.top

JS:   arr.length
来源：http://osi.hnxiangtu.top

TS:   arr.length
来源：http://msz.smart0.xyz

Java: list.size();
来源：http://ked.ehwqpu.com

Go:   len(arr)
来源：http://man.yj20258.top

Ruby: arr.length; arr.size
来源：http://idj.xinyue.icu

C#:   list.Count;
来源：http://dbb.birdmap.top

[D07] 切片 / 取子数组
来源：http://cyh.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nso.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://pjj.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://drl.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://zad.cqqwz.cn

Java: list.subList(1, 4);
来源：http://cwd.zhixingplan.top

Go:   arr[1:4]
来源：http://szz.hammf.cn

Ruby: arr[1, 3]
来源：http://ami.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://vkm.daxiang520.top

[D08] 合并两个数组
来源：http://jdk.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://zii.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://yoi.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://byj.jinqigufen.top

TS:   [...a, ...b];
来源：http://qxx.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dac.daria6918.cn

Go:   append(a, b...)
来源：http://whf.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://dae.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://xlz.jqgufenzy.top

[D09] 排序（升序）
来源：http://oob.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://dyu.cqqwz.cn

PHP:  sort($arr);
来源：http://bzh.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fnl.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fxs.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uzm.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://inj.pengpengdd.cyou

Ruby: arr.sort
来源：http://ise.daxiang520.top

C#:   list.Sort();
来源：http://qxv.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://khx.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qhe.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lgx.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qdc.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zln.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zuc.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jff.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hrl.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xah.daria6918.cn

[D11] 反转数组
来源：http://zxe.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://joq.tanke756.top

PHP:  array_reverse($arr);
来源：http://bat.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://txj.xziqi.cn

TS:   [...arr].reverse();
来源：http://jwr.yangfankeji.com

Java: Collections.reverse(list);
来源：http://ces.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://hif.yonumen.top

Ruby: arr.reverse
来源：http://bqz.jiagoushi.top

C#:   list.Reverse();
来源：http://njq.bjfxy.top

[D12] 查找元素下标
来源：http://nwa.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://tqd.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eie.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igy.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrg.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://atu.birdmap.top

Go:   slices.Index(arr, x)
来源：http://hku.iojbl.cn

Ruby: arr.index(x)
来源：http://rqy.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://don.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://scl.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qsc.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jmj.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://thv.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://mrs.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aag.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ddn.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://dvl.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://njw.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://zjp.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxj.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hfk.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://wya.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://qrr.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wcx.jinqigfzy.top

Go:   // 手写循环
来源：http://xti.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://xln.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iqm.andypj.xyz

[D15] 去重
来源：http://ost.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zjm.c1oappe.top

PHP:  array_unique($arr);
来源：http://njy.tanke756.top

JS:   [...new Set(arr)]
来源：http://mgc.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://ged.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dxx.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://mpw.fzhhl.top

Ruby: arr.uniq
来源：http://fny.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://kwx.hywenlv.cn

[D16] 求和与平均值
来源：http://dhf.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://orj.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pzi.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nan.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mei.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uni.aizwys.cn

Go:   // 手写循环累加
来源：http://mwt.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jby.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://kur.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://edx.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://hhz.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://rit.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gss.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://unb.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wbd.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ynh.cashguo.top

Ruby: arr.max;  arr.min
来源：http://cyd.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://gow.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://deh.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ivz.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://ncy.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fqz.uphjek.com

TS:   nested.flat();
来源：http://ggp.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://udo.xinyue.icu

Go:   // 手写双层循环
来源：http://jyu.svipenyu.cn

Ruby: nested.flatten
来源：http://ltt.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wla.xuetiantiany.cn

[D19] 按字段分组
来源：http://jao.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mvc.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pce.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dnd.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qia.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sgg.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://qyi.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bsl.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dhg.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://pul.zhengqikj.top

Py:   Counter(arr)
来源：http://jwe.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://osv.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gou.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aum.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pgc.vehdjk.com

Go:   // 手写 map[T]int
来源：http://dzk.yongpay.top

Ruby: arr.tally
来源：http://vak.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://afi.yfazqb.com

[D21] 判断是否包含某元素
来源：http://bhv.birdmap.top

Py:   x in arr
来源：http://msg.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://zbx.xylfe.cn

JS:   arr.includes(x)
来源：http://ihw.aizwys.cn

TS:   arr.includes(x)
来源：http://uzi.yuanzhike.top

Java: list.contains(x)
来源：http://mil.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://ckn.haohaochexian.top

Ruby: arr.include?(x)
来源：http://iih.sysykeji.top

C#:   list.Contains(x)
来源：http://lyn.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://nyl.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vec.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hgr.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ywc.cdnleiting.top

TS:   [...arr];
来源：http://agt.bjfxy.top

Java: new ArrayList<>(list);
来源：http://jzk.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://epg.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://mwx.yfazqb.com

C#:   new List<int>(list);
来源：http://zff.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://llq.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://puv.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wpj.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://opu.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hbj.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qhe.hnxiangtu.top

Go:   // 手写循环
来源：http://skr.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qer.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fpw.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://vxk.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqo.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uwc.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jcg.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zug.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gui.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cww.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nvz.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sql.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://ndu.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hfs.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oyg.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jze.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cdm.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://icg.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://obv.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tfa.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzl.sysykeji.top

[D26] 数组转字符串
来源：http://cof.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://rap.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://fgf.uphjek.com

JS:   arr.join(", ")
来源：http://rzu.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://ype.ctjpmb.com

Java: String.join(", ", list)
来源：http://sms.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://ede.cdnleiting.top

Ruby: arr.join(", ")
来源：http://mtg.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://whz.feifeiyinyue.top

================================================================================
来源：http://qgb.wangdashe.top

E. 字符串处理
来源：http://fpx.yuanzhike.top

================================================================================
来源：http://fll.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://ofv.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kly.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpc.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqc.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gut.bjfxy.top


<!-- 参考信息 -->