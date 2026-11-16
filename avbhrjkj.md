代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://lrh.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qra.cdnleiting.top

Java: import java.util.List;
来源：http://mbj.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://drb.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://rrf.yvedp.cn

C#:   using System.Text;
来源：http://roo.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://wzr.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://jms.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://pdc.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://htt.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://dkk.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://snc.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://kzg.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://jqa.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pjj.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://zuw.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xad.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgt.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jad.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hnq.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://amg.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://gna.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rno.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://ozk.fanxiaobao.xyz

[C14] 泛型函数
来源：http://bdt.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ean.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://uvc.yuxming.cn

JS:   // 无泛型
来源：http://ogi.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yfo.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovi.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ogh.hysaishi.cn

Ruby: # 无泛型
来源：http://mxf.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qjx.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://daf.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lxv.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://qil.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epy.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ire.sufxvd.cn

Java: // 无解构
来源：http://uub.jqgfzy.top

Go:   // 无解构
来源：http://pbk.ehwqpu.com

Ruby: a, b = pair
来源：http://fvf.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://mwx.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://dpd.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gum.jqgfzy.top

PHP:  // 无重载
来源：http://cpv.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hzl.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://sze.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ycn.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://eac.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://jtr.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bkl.haohaochexian.top

================================================================================
来源：http://vvd.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://bzw.zhengqikj.top

================================================================================
来源：http://rnw.hammf.cn

[D01] 创建数组 / 列表
来源：http://uze.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zrk.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://thb.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tqs.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dja.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fxk.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://ptw.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://cun.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dtw.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://xli.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cpn.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ugo.hywenlv.cn

JS:   arr.push(4);
来源：http://izd.xziqi.cn

TS:   arr.push(4);
来源：http://vur.dashuyun.cn

Java: list.add(4);
来源：http://vej.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://pph.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://rka.ivvv.top

C#:   list.Add(4);
来源：http://ujl.yj202588.top

[D03] 在指定位置插入元素
来源：http://glm.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://yfi.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tcm.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idk.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://wuo.ydjk.org.cn

Java: list.add(0, 0);
来源：http://gxf.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://yls.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qsk.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://pdc.ywan-chungtsiang.top

[D04] 删除元素
来源：http://oyb.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vqr.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://orb.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rxg.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://uyf.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hgx.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ezv.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mcv.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jxx.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://mkd.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cri.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://omw.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qax.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://zee.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://ezz.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://iqt.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjg.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://afn.xinyue.icu

[D06] 数组长度
来源：http://otk.xuanzx.com

Py:   len(arr)
来源：http://sut.zycfv.cn

PHP:  count($arr);
来源：http://hrw.hysaishi.cn

JS:   arr.length
来源：http://lxs.jinqigfzy.top

TS:   arr.length
来源：http://ayg.jlsjyb.cn

Java: list.size();
来源：http://nnz.zhaomingkeji.xyz

Go:   len(arr)
来源：http://djm.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://tcg.dianchejie.cn

C#:   list.Count;
来源：http://dkt.yj20258888.top

[D07] 切片 / 取子数组
来源：http://vjr.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qoq.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://sse.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://fqh.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://mtl.sweek.top

Java: list.subList(1, 4);
来源：http://yqq.jianghu66.top

Go:   arr[1:4]
来源：http://oso.ivvv.top

Ruby: arr[1, 3]
来源：http://wkb.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://pbc.tian-w.cn

[D08] 合并两个数组
来源：http://qdw.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://onl.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://txe.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nah.svipenyu.cn

TS:   [...a, ...b];
来源：http://svk.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rky.pengpengdd.cyou

Go:   append(a, b...)
来源：http://jdg.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://afi.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://xfh.316326.xyz

[D09] 排序（升序）
来源：http://wkj.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://vzn.nanxinkj.top

PHP:  sort($arr);
来源：http://ffv.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://otu.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qcz.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lfw.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgh.chenlongwang.top

Ruby: arr.sort
来源：http://icq.mhx1999.top

C#:   list.Sort();
来源：http://yhg.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gng.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://grd.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whj.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxf.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ykf.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hdj.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vcc.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ulg.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pkq.dianchejie.cn

[D11] 反转数组
来源：http://kpj.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://her.gzhubu.top

PHP:  array_reverse($arr);
来源：http://gmc.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://grv.ydzc1.top

TS:   [...arr].reverse();
来源：http://ttk.9152youxi.cn

Java: Collections.reverse(list);
来源：http://jlb.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://hce.vqdsnc.cn

Ruby: arr.reverse
来源：http://ajm.fktsv.cn

C#:   list.Reverse();
来源：http://lbv.aizwys.cn

[D12] 查找元素下标
来源：http://jtp.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://gmr.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yzj.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://axt.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpz.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fpz.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://iyx.hywenlv.cn

Ruby: arr.index(x)
来源：http://ers.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://lwc.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://klq.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nuw.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhd.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://gjt.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://yzq.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qvz.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emx.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://hev.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ico.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://rls.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gpu.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gjb.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://gsy.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://kgc.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://kxv.andypj.xyz

Go:   // 手写循环
来源：http://uts.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://iwf.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ycj.sjlbkw.cn

[D15] 去重
来源：http://jtq.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jwr.iojbl.cn

PHP:  array_unique($arr);
来源：http://ouu.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://pnz.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://jpj.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cwt.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ghv.jqgufenzy.top

Ruby: arr.uniq
来源：http://ubf.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://dua.nanxinkj.top

[D16] 求和与平均值
来源：http://jdx.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nuh.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jzl.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cwq.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://crt.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vls.sufxvd.cn

Go:   // 手写循环累加
来源：http://pef.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://egx.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://jiz.smart0.xyz

[D17] 最大值与最小值
来源：http://dyj.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://sot.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://lrr.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sof.sweek.top

TS:   Math.max(...arr);
来源：http://odq.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://apj.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mzm.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://aav.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://ddv.birdmap.top

[D18] 扁平化嵌套数组
来源：http://yle.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ijr.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://tca.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oor.yanxiufei.cn

TS:   nested.flat();
来源：http://pis.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alq.316326.xyz

Go:   // 手写双层循环
来源：http://ucp.zdqjudy.top

Ruby: nested.flatten
来源：http://jmg.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ipl.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://uod.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qxq.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ufz.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://art.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dhy.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jnc.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://npg.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zey.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://foa.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://bix.zycfv.cn

Py:   Counter(arr)
来源：http://dle.redwolf501.top

PHP:  array_count_values($arr);
来源：http://sip.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wxx.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwb.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lth.nwbrower.top

Go:   // 手写 map[T]int
来源：http://dvy.shuidangran.top

Ruby: arr.tally
来源：http://bdk.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xlh.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://jzg.chenlongwang.top

Py:   x in arr
来源：http://vpl.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://psf.birdmap.top

JS:   arr.includes(x)
来源：http://ulh.zdbjq.cn

TS:   arr.includes(x)
来源：http://eep.ehwqpu.com

Java: list.contains(x)
来源：http://trq.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://iau.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://vwq.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://xjz.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://cps.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nmf.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zjm.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mzq.jqgfzy.top

TS:   [...arr];
来源：http://zwc.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://qzi.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ykb.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://zui.xinyue.icu

C#:   new List<int>(list);
来源：http://sjh.zdqjudy.top

[D23] reduce 累积计算
来源：http://yry.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zuo.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cqg.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qdr.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tdp.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tzu.smart0.xyz

Go:   // 手写循环
来源：http://bpl.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://noj.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bdp.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://hyo.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://keh.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://apb.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pty.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zqr.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yzn.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://arf.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tzn.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ngi.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://vuf.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kxl.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pud.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mke.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://laq.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://idx.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://roe.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cmg.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sxp.hfpthk.cn

[D26] 数组转字符串
来源：http://svq.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://dwi.yj20258.top

PHP:  implode(", ", $arr);
来源：http://lwl.hywenlv.cn

JS:   arr.join(", ")
来源：http://vbz.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://zii.havefunace.top

Java: String.join(", ", list)
来源：http://ybg.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://coj.cucudq.cn

Ruby: arr.join(", ")
来源：http://wao.hesvh.cn

C#:   string.Join(", ", list)
来源：http://zmg.shanyushiyangkeji.top

================================================================================
来源：http://dtk.cheryme.top

E. 字符串处理
来源：http://run.cashguo.top

================================================================================
来源：http://tfu.sysykeji.top

[E01] 拼接字符串
来源：http://sqi.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xlm.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcq.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rwl.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://evp.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ucm.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nbr.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qnc.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pwv.andypj.xyz


<!-- 参考信息 -->