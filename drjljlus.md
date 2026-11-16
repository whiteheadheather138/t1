代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hpd.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://juv.shanyushiyangtech.top

Java: import java.util.List;
来源：http://ybv.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yhk.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://ghq.fzhhl.top

C#:   using System.Text;
来源：http://ptv.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://oxv.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://aqi.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://rjd.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://hqt.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://seb.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pxd.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://gol.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://cps.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://wlf.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://flq.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gbu.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://scm.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lds.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfj.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://ill.andypj.xyz

Go:   func add(a, b int) int
来源：http://ldk.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mhe.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ora.tianlin.xyz

[C14] 泛型函数
来源：http://cvl.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wwg.yvedp.cn

PHP:  // 无泛型
来源：http://git.yanxiufei.cn

JS:   // 无泛型
来源：http://cij.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptf.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pzi.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gmh.fktsv.cn

Ruby: # 无泛型
来源：http://lhg.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://krg.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://hjf.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wbr.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://qgq.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://asz.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://usz.jyoumei.cn

Java: // 无解构
来源：http://xqz.shanyushiyangkeji.top

Go:   // 无解构
来源：http://dfb.nanxinkj.top

Ruby: a, b = pair
来源：http://bhe.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://syg.sweek.top

[C16] 函数 / 方法重载
来源：http://lcw.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rjd.gzhubu.top

PHP:  // 无重载
来源：http://wma.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fhc.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://ijt.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cjk.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://xob.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://jye.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://zwf.cdnleiting.top

================================================================================
来源：http://dnm.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://iwb.bbcook.cn

================================================================================
来源：http://avy.yuxming.cn

[D01] 创建数组 / 列表
来源：http://cph.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ogj.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wfo.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://okk.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fwa.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://piq.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://oje.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://juz.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nsp.bbcook.cn

[D02] 追加元素到末尾
来源：http://evs.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kkv.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nuf.zycfv.cn

JS:   arr.push(4);
来源：http://llb.ppjwa.cn

TS:   arr.push(4);
来源：http://skd.ppjwa.cn

Java: list.add(4);
来源：http://oqo.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://eux.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://nqu.shzxlz.cn

C#:   list.Add(4);
来源：http://szx.fehbvm.com

[D03] 在指定位置插入元素
来源：http://giy.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://klo.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://miu.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://agp.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://jer.sweek.top

Java: list.add(0, 0);
来源：http://vny.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cqk.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oku.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://pwz.yj202588.top

[D04] 删除元素
来源：http://ysk.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pgg.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twb.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ssh.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://lgz.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qap.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qyc.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mqq.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qgk.zhoulong.xyz

[D05] 访问与修改元素
来源：http://lsp.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fjq.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qrl.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://win.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://myt.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://wfc.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://gzl.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jkf.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dcu.snrcjt.cn

[D06] 数组长度
来源：http://tbm.cucudq.cn

Py:   len(arr)
来源：http://emw.jqgufenzy.top

PHP:  count($arr);
来源：http://wxn.aizwys.cn

JS:   arr.length
来源：http://gvk.bbcook.cn

TS:   arr.length
来源：http://cjo.ydjk.org.cn

Java: list.size();
来源：http://nwg.yuanzhike.top

Go:   len(arr)
来源：http://thu.c1oappe.top

Ruby: arr.length; arr.size
来源：http://dmg.zhongyouzk.top

C#:   list.Count;
来源：http://jbe.yuxming.cn

[D07] 切片 / 取子数组
来源：http://oxv.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xdd.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://plx.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://fcp.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://stz.epnwcf.com

Java: list.subList(1, 4);
来源：http://fjo.tianlin.xyz

Go:   arr[1:4]
来源：http://hjh.c1oappe.top

Ruby: arr[1, 3]
来源：http://obt.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://znr.gzhubu.top

[D08] 合并两个数组
来源：http://apj.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://sff.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://ufh.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xcu.yueranfly.top

TS:   [...a, ...b];
来源：http://qwx.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hau.iojbl.cn

Go:   append(a, b...)
来源：http://jvp.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://hfk.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://aad.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://itp.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://djb.jqgufenzy.top

PHP:  sort($arr);
来源：http://hwz.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsi.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ibf.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uof.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cpy.dashuyun.cn

Ruby: arr.sort
来源：http://vfz.zhongyouzk.top

C#:   list.Sort();
来源：http://qka.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://spu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gwi.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://htu.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ehv.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://niy.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ixp.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://irh.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pud.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dys.yvedp.cn

[D11] 反转数组
来源：http://ady.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jkv.vehdjk.com

PHP:  array_reverse($arr);
来源：http://vmv.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dxs.cashguo.top

TS:   [...arr].reverse();
来源：http://peb.jinqigufen.top

Java: Collections.reverse(list);
来源：http://yiw.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://uqd.fengsongda.top

Ruby: arr.reverse
来源：http://ilv.ehwqpu.com

C#:   list.Reverse();
来源：http://lhy.nwbrower.top

[D12] 查找元素下标
来源：http://rla.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://dbr.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rdx.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://efx.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jrz.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ncc.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://hqv.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://rwz.yj20258888.top

C#:   list.IndexOf(x);
来源：http://lwe.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://rmh.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hva.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rck.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://csx.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://gpt.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://luk.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xiz.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ynw.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eup.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://zzh.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ujw.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zen.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://fjk.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://hfe.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mml.hcnkem.com

Go:   // 手写循环
来源：http://uoe.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://ntl.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ugq.tanke756.top

[D15] 去重
来源：http://bcu.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vqw.chenzaomai.com

PHP:  array_unique($arr);
来源：http://pko.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://mja.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://xls.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zuz.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ixo.zhengqikj.top

Ruby: arr.uniq
来源：http://vet.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://rsi.wangshuangyany.cn

[D16] 求和与平均值
来源：http://jwz.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ogo.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ffs.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tff.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iah.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jrs.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://gfg.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vyg.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://obr.hesvh.cn

[D17] 最大值与最小值
来源：http://vhu.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://vzj.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://foh.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://law.316326.xyz

TS:   Math.max(...arr);
来源：http://rtk.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://eqv.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vkz.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://dsa.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://tqk.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://tmo.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fjh.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://xyk.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zmw.yvedp.cn

TS:   nested.flat();
来源：http://lbz.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dry.sufxvd.cn

Go:   // 手写双层循环
来源：http://orv.daxiang520.top

Ruby: nested.flatten
来源：http://dly.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gun.bjfxy.top

[D19] 按字段分组
来源：http://tam.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pwu.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mqa.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tcl.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mwt.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ydn.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://uee.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://byn.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://woy.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://hzp.yueranfly.top

Py:   Counter(arr)
来源：http://rwb.havefunace.top

PHP:  array_count_values($arr);
来源：http://wdl.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://glu.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drg.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qcq.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://zyn.vqdsnc.cn

Ruby: arr.tally
来源：http://ooz.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bul.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://isq.52xcode.cn

Py:   x in arr
来源：http://zmw.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://kxu.xziqi.cn

JS:   arr.includes(x)
来源：http://ufd.nanxinkj.top

TS:   arr.includes(x)
来源：http://era.yfazqb.com

Java: list.contains(x)
来源：http://lwz.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://wqi.yj20258888.top

Ruby: arr.include?(x)
来源：http://rxi.gogol.net.cn

C#:   list.Contains(x)
来源：http://jkg.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://sdr.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mmz.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ltk.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://etr.cheryme.top

TS:   [...arr];
来源：http://wwb.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://hjp.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://mrm.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://czt.yonumen.top

C#:   new List<int>(list);
来源：http://qwh.yuanzhike.top

[D23] reduce 累积计算
来源：http://nvf.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mpk.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kin.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qbq.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xnj.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://chq.havefunace.top

Go:   // 手写循环
来源：http://ayy.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jid.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mtf.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://uof.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hex.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://poc.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpf.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fps.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gzq.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wjm.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyc.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vvv.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://pnz.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xtr.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vwx.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dkz.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://roc.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mzu.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://grp.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zmr.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lwy.cqqwz.cn

[D26] 数组转字符串
来源：http://ggj.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://gdp.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://bhb.epnwcf.com

JS:   arr.join(", ")
来源：http://nnm.tianlin.xyz

TS:   arr.join(", ")
来源：http://wmx.mhx1999.top

Java: String.join(", ", list)
来源：http://fyx.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://dio.haohaochexian.top

Ruby: arr.join(", ")
来源：http://ohr.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://hth.chenjidiqi.icu

================================================================================
来源：http://zce.daxiang520.top

E. 字符串处理
来源：http://ymq.pycfn.com

================================================================================
来源：http://wtf.xziqi.cn

[E01] 拼接字符串
来源：http://yxj.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://atr.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mzs.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bjs.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpj.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://onp.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uwf.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://szr.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vvr.shuidangran.top


<!-- 参考信息 -->