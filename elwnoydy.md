代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://lan.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wvs.fanxiaobao.xyz

Java: import java.util.List;
来源：http://dwi.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kzz.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wfw.guowangkeji.top

C#:   using System.Text;
来源：http://gqz.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://lot.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://dcv.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://vdp.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://mtn.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://avz.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fgw.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://lfn.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://liw.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://ebu.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://zbn.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zdo.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqr.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zco.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqk.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ypg.nanxinkj.top

Go:   func add(a, b int) int
来源：http://mbh.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mma.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://dem.hcnkem.com

[C14] 泛型函数
来源：http://jyq.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://are.yj20258.top

PHP:  // 无泛型
来源：http://ang.cqqwz.cn

JS:   // 无泛型
来源：http://gfz.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://azk.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bkt.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ske.jlsjyb.cn

Ruby: # 无泛型
来源：http://rbz.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cxi.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://bnp.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fxe.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://dfs.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ubg.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kip.ydzc1.top

Java: // 无解构
来源：http://wxh.316326.xyz

Go:   // 无解构
来源：http://ikm.xuetiantiany.cn

Ruby: a, b = pair
来源：http://aga.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://bvy.fehbvm.com

[C16] 函数 / 方法重载
来源：http://zxz.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://agz.jinghuilouyu.cn

PHP:  // 无重载
来源：http://acp.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tar.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://imf.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lcp.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://uhn.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://sqg.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://igj.jyoumei.cn

================================================================================
来源：http://zfr.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://uie.dashuyun.cn

================================================================================
来源：http://ljq.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://nyr.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zhk.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hdy.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zug.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rsi.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mko.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://mbp.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://qiq.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kop.yonumen.top

[D02] 追加元素到末尾
来源：http://rlm.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vgf.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mza.cashguo.top

JS:   arr.push(4);
来源：http://vzk.daxiang520.top

TS:   arr.push(4);
来源：http://yqq.316326.xyz

Java: list.add(4);
来源：http://bcj.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://uqu.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://blz.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://crx.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://rnf.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://mso.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://egx.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ydu.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xal.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://lgt.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://wdf.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhs.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://cni.xziqi.cn

[D04] 删除元素
来源：http://mtr.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zya.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pha.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ihw.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://qqm.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oup.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ydj.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aku.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qbt.xuanzx.com

[D05] 访问与修改元素
来源：http://kej.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nda.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zja.jinqigufen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kva.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://vta.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://ibx.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://rko.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://war.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oue.tianlin.xyz

[D06] 数组长度
来源：http://vtr.tianlin.xyz

Py:   len(arr)
来源：http://esv.haohaochexian.top

PHP:  count($arr);
来源：http://etm.hongshengwenyu.top

JS:   arr.length
来源：http://jhc.nanxuanxn.top

TS:   arr.length
来源：http://dro.cheryme.top

Java: list.size();
来源：http://oaq.daxiang520.top

Go:   len(arr)
来源：http://kqz.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://xtc.sweek.top

C#:   list.Count;
来源：http://nqk.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://gmf.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jhj.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://xcr.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://uwq.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://msp.cashguo.top

Java: list.subList(1, 4);
来源：http://buj.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://xve.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://zwy.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://qmt.fengsongda.top

[D08] 合并两个数组
来源：http://unv.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://egb.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://qqp.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://brn.shzxlz.cn

TS:   [...a, ...b];
来源：http://kce.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mtu.mhx1999.top

Go:   append(a, b...)
来源：http://olg.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://tjo.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://cgh.zhoulong.xyz

[D09] 排序（升序）
来源：http://myl.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://lci.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://ycb.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://htb.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uyy.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://doz.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://znl.jiagoushi.top

Ruby: arr.sort
来源：http://tmt.c1oappe.top

C#:   list.Sort();
来源：http://xya.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aru.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://juv.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://log.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://akp.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hvg.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dwu.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dvl.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mzy.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hov.meibo888.top

[D11] 反转数组
来源：http://cow.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rim.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://ldf.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://stl.316326.xyz

TS:   [...arr].reverse();
来源：http://gop.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://jpx.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://idg.aizwys.cn

Ruby: arr.reverse
来源：http://ujn.shzxlz.cn

C#:   list.Reverse();
来源：http://wsz.aibaodan.cn

[D12] 查找元素下标
来源：http://bzx.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://cfn.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvz.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kwo.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxn.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://brs.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://bsf.smart0.xyz

Ruby: arr.index(x)
来源：http://ree.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://dsj.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://aky.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bvm.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fwm.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://sjf.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://ram.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfi.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://psr.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eba.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eln.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://ehd.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vdh.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rmb.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://omq.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://vjh.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://moz.yj20258.top

Go:   // 手写循环
来源：http://log.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rva.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://pnv.cucudq.cn

[D15] 去重
来源：http://ldb.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bpz.sysykeji.top

PHP:  array_unique($arr);
来源：http://jov.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://zne.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://uky.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rsj.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://bxi.mhx1999.top

Ruby: arr.uniq
来源：http://cny.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://evx.yonumen.top

[D16] 求和与平均值
来源：http://tve.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iji.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vtr.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyd.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rwt.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jju.uphjek.com

Go:   // 手写循环累加
来源：http://hek.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rdq.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://fwy.cdnleiting.top

[D17] 最大值与最小值
来源：http://orf.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://xtx.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://jbx.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pxv.ivvv.top

TS:   Math.max(...arr);
来源：http://mfn.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zso.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qdp.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://gnj.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://ztl.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://fod.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pzs.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://sqo.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ual.yj20258888.top

TS:   nested.flat();
来源：http://bni.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bnj.fehbvm.com

Go:   // 手写双层循环
来源：http://jsz.hfpthk.cn

Ruby: nested.flatten
来源：http://tar.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pis.yonumen.top

[D19] 按字段分组
来源：http://akd.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cvf.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rog.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzv.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://rnp.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://twa.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://qba.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fgx.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwk.316326.xyz

[D20] 统计每个元素出现次数
来源：http://kln.zhengqikj.top

Py:   Counter(arr)
来源：http://yre.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://xqx.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsk.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qao.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mxi.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://gki.sxryk.cn

Ruby: arr.tally
来源：http://zmk.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cjc.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://elu.tian-w.cn

Py:   x in arr
来源：http://kas.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://lkv.zhongyouzk.top

JS:   arr.includes(x)
来源：http://whz.iojbl.cn

TS:   arr.includes(x)
来源：http://usp.aibaodan.cn

Java: list.contains(x)
来源：http://dkv.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://qiu.xylfe.cn

Ruby: arr.include?(x)
来源：http://twb.uphjek.com

C#:   list.Contains(x)
来源：http://plc.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://mup.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wgp.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vux.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jss.ydjk.org.cn

TS:   [...arr];
来源：http://jpm.ydzc1.top

Java: new ArrayList<>(list);
来源：http://dsc.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://jnz.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://atj.yj20258.top

C#:   new List<int>(list);
来源：http://crm.hcnkem.com

[D23] reduce 累积计算
来源：http://xhm.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fsn.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://awr.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bkm.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mih.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://agm.9152youxi.cn

Go:   // 手写循环
来源：http://tmo.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vwh.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lgp.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://lzp.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfn.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rik.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pvd.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sac.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pth.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ktd.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbf.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pmc.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://uou.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lat.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjj.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cbz.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wqs.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://odz.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ult.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yra.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://huq.hfpthk.cn

[D26] 数组转字符串
来源：http://kwq.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://djo.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://nip.yanxiufei.cn

JS:   arr.join(", ")
来源：http://oqu.yuxming.cn

TS:   arr.join(", ")
来源：http://nlr.jqgfzy.top

Java: String.join(", ", list)
来源：http://wgy.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://ojt.xuanzx.com

Ruby: arr.join(", ")
来源：http://zxe.52xcode.cn

C#:   string.Join(", ", list)
来源：http://lvx.shanyushiyangkeji.top

================================================================================
来源：http://lbk.sjlbkw.cn

E. 字符串处理
来源：http://npx.hnqzz.top

================================================================================
来源：http://rwh.aizwys.cn

[E01] 拼接字符串
来源：http://njk.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yuf.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kfg.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dnp.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eqc.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dxt.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgx.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qby.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lhr.yanxiufei.cn


<!-- 参考信息 -->