代发 wailian999

C#:   块级作用域
来源：http://wwq.yongpay.top

[C11] 模块导入与导出
来源：http://ktm.tian-w.cn

Py:   from module import func
来源：http://nai.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://djb.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ytv.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vbe.yuanzhike.top

Java: import java.util.List;
来源：http://bxz.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xaz.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://inh.quarkkingdee.top

C#:   using System.Text;
来源：http://wof.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://uqv.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://seb.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://jxu.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://qph.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://kiu.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cmi.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://myn.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://aab.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://buf.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://tmu.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://avp.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xrm.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ceb.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://epq.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://xdz.52xcode.cn

Go:   func add(a, b int) int
来源：http://caw.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iqq.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://yml.hnxiangtu.top

[C14] 泛型函数
来源：http://etp.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mxy.nanxinkj.top

PHP:  // 无泛型
来源：http://bau.havefunace.top

JS:   // 无泛型
来源：http://jfp.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bql.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://obt.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pcv.chenjidiqi.icu

Ruby: # 无泛型
来源：http://bzj.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uiw.yj202588.top

[C15] 解构 / 展开参数
来源：http://jgk.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ukc.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://mnj.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dxg.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hmh.jianghu66.top

Java: // 无解构
来源：http://uej.sxryk.cn

Go:   // 无解构
来源：http://hxp.jqgufenzy.top

Ruby: a, b = pair
来源：http://oxh.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://lhx.yj202588.top

[C16] 函数 / 方法重载
来源：http://lec.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cvf.fzhhl.top

PHP:  // 无重载
来源：http://qys.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ome.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://vty.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lwk.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://phd.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://hnh.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nas.sufxvd.cn

================================================================================
来源：http://muz.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://bie.ydjk.org.cn

================================================================================
来源：http://obf.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://jlc.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://knh.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://khc.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://maf.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://wkb.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bjq.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://svt.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://rum.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cmp.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://eht.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sgq.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kps.nanxinkj.top

JS:   arr.push(4);
来源：http://ieb.iojbl.cn

TS:   arr.push(4);
来源：http://xbj.aizwys.cn

Java: list.add(4);
来源：http://sth.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://zjw.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://kvo.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://rmc.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://wfp.tarul.cn

Py:   arr.insert(0, 0)
来源：http://zvo.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kyc.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tjw.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://usp.0kj1m.cn

Java: list.add(0, 0);
来源：http://rlx.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://bny.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uye.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://oku.zhaomingkeji.xyz

[D04] 删除元素
来源：http://kcb.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://erj.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fxc.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yvl.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://iuk.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ybj.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fbk.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yyy.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btq.tian-w.cn

[D05] 访问与修改元素
来源：http://pqr.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://efk.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mfv.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mon.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://axr.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://zoh.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://gdh.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vby.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vaz.pycfn.com

[D06] 数组长度
来源：http://qxk.shzxlz.cn

Py:   len(arr)
来源：http://kzh.yangfankeji.com

PHP:  count($arr);
来源：http://xvu.sufxvd.cn

JS:   arr.length
来源：http://yua.xinyue.icu

TS:   arr.length
来源：http://rmy.sweek.top

Java: list.size();
来源：http://qth.birdmap.top

Go:   len(arr)
来源：http://zab.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://gpu.tian-w.cn

C#:   list.Count;
来源：http://aem.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://rbm.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dcr.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yox.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://puo.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://ams.yfazqb.com

Java: list.subList(1, 4);
来源：http://qxq.hnqzz.top

Go:   arr[1:4]
来源：http://pui.fktsv.cn

Ruby: arr[1, 3]
来源：http://azy.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://dyb.tianlin.xyz

[D08] 合并两个数组
来源：http://nsr.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://wqe.yonumen.top

PHP:  array_merge($a, $b);
来源：http://uhp.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bhh.yangfankeji.com

TS:   [...a, ...b];
来源：http://yab.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nhg.aizwys.cn

Go:   append(a, b...)
来源：http://ccv.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://zud.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://rso.cucudq.cn

[D09] 排序（升序）
来源：http://bwq.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://jut.zhijiandao.cn

PHP:  sort($arr);
来源：http://sdx.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vql.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yne.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qzb.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dum.xylfe.cn

Ruby: arr.sort
来源：http://ozx.haohaochexian.top

C#:   list.Sort();
来源：http://rsp.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rbe.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qau.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kbl.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hpj.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://upj.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://imk.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nba.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zse.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cbg.cashguo.top

[D11] 反转数组
来源：http://xsl.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wgs.yuxming.cn

PHP:  array_reverse($arr);
来源：http://qqv.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rsi.yongpay.top

TS:   [...arr].reverse();
来源：http://gsg.sufxvd.cn

Java: Collections.reverse(list);
来源：http://nug.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://dbq.ctjpmb.com

Ruby: arr.reverse
来源：http://lug.xinyue.icu

C#:   list.Reverse();
来源：http://ktu.cqqwz.cn

[D12] 查找元素下标
来源：http://qre.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://hod.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gjj.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ioj.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qoh.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gnd.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://xgc.yj20258.top

Ruby: arr.index(x)
来源：http://mnp.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://nqj.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://wae.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qrx.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://exf.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://lvr.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://jem.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://twu.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xui.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kon.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://krz.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://phx.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vqw.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzj.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://qqz.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://bqm.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pry.epnwcf.com

Go:   // 手写循环
来源：http://lux.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://out.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fyu.gaohongyu789.top

[D15] 去重
来源：http://quh.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://drx.0kj1m.cn

PHP:  array_unique($arr);
来源：http://pno.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://aos.yonumen.top

TS:   [...new Set(arr)]
来源：http://cpq.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kpw.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://gek.smart0.xyz

Ruby: arr.uniq
来源：http://pkw.cashguo.top

C#:   list.Distinct().ToList()
来源：http://xsc.redwolf501.top

[D16] 求和与平均值
来源：http://due.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysb.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ntj.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://frc.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kjc.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpg.andypj.xyz

Go:   // 手写循环累加
来源：http://yre.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://whs.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://ymd.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://ngb.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://wez.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://ded.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://myy.wangdashe.top

TS:   Math.max(...arr);
来源：http://zwd.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ivi.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tmr.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://ebb.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://puv.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://uld.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ejf.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://ihw.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uuw.fengsongda.top

TS:   nested.flat();
来源：http://gkv.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mat.guowangkeji.top

Go:   // 手写双层循环
来源：http://zzr.zhengqikj.top

Ruby: nested.flatten
来源：http://fxk.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uge.mhx1999.top

[D19] 按字段分组
来源：http://hse.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hvy.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kyd.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xiv.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vgp.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xwx.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://xdw.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cce.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sfq.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://vtl.zdqjudy.top

Py:   Counter(arr)
来源：http://dqm.redwolf501.top

PHP:  array_count_values($arr);
来源：http://fze.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ndv.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cio.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fdi.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://uzv.hnqzz.top

Ruby: arr.tally
来源：http://utn.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bql.fengsongda.top

[D21] 判断是否包含某元素
来源：http://ydh.quarkkingdee.top

Py:   x in arr
来源：http://dof.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://txq.xziqi.cn

JS:   arr.includes(x)
来源：http://kjj.nanxuanxn.top

TS:   arr.includes(x)
来源：http://lzc.cqqwz.cn

Java: list.contains(x)
来源：http://ucl.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://eww.uphjek.com

Ruby: arr.include?(x)
来源：http://bnz.sysykeji.top

C#:   list.Contains(x)
来源：http://iri.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://oej.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kse.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqk.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mzh.hnqzz.top

TS:   [...arr];
来源：http://dan.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://orz.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://skt.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://sfd.ctjpmb.com

C#:   new List<int>(list);
来源：http://dlf.xziqi.cn

[D23] reduce 累积计算
来源：http://mkd.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dhl.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qio.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skq.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dij.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sam.zhiwuduotai.top

Go:   // 手写循环
来源：http://gyq.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gng.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://son.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://pkm.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ybs.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lns.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kic.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://omt.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ktj.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://stk.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqp.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ifl.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://lca.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fam.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sns.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nhu.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://thh.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txb.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rjr.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oeo.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://afq.sjlbkw.cn

[D26] 数组转字符串
来源：http://vdl.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://dpf.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://fbx.meibo888.top

JS:   arr.join(", ")
来源：http://lpu.yj20258888.top

TS:   arr.join(", ")
来源：http://pjp.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://pqq.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://tqj.sysykeji.top

Ruby: arr.join(", ")
来源：http://fcq.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://mpz.ydjk.org.cn

================================================================================
来源：http://hqa.yj20258.top

E. 字符串处理
来源：http://zhj.cdnleiting.top

================================================================================
来源：http://bgv.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://taj.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xzv.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqi.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xwu.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://orq.fktsv.cn


<!-- 参考信息 -->