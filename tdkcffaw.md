代发 wailian999

C#:   块级作用域
来源：http://qwv.hfpthk.cn

[C11] 模块导入与导出
来源：http://bpc.jinyuanbaomall.cn

Py:   from module import func
来源：http://szr.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aor.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://isc.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oet.zhongyouzk.top

Java: import java.util.List;
来源：http://xrc.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kju.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://qdu.zhiwuduotai.top

C#:   using System.Text;
来源：http://qck.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://vft.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://ovx.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://ngb.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://tki.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://iul.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://srk.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://syv.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://rhe.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://auk.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://zxb.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lxn.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnt.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gyr.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jpj.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://vkl.hysaishi.cn

Go:   func add(a, b int) int
来源：http://shc.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vjl.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://mcx.yanxiufei.cn

[C14] 泛型函数
来源：http://pvr.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lyq.wangdashe.top

PHP:  // 无泛型
来源：http://zco.ehwqpu.com

JS:   // 无泛型
来源：http://lep.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tyx.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ljv.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wgi.fzhhl.top

Ruby: # 无泛型
来源：http://fsv.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://smj.meibo888.top

[C15] 解构 / 展开参数
来源：http://sth.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lbj.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://qtt.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vhd.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uir.fengsongda.top

Java: // 无解构
来源：http://gua.zhaomingkeji.xyz

Go:   // 无解构
来源：http://yns.smart0.xyz

Ruby: a, b = pair
来源：http://vfu.fengsongda.top

C#:   var (a, b) = pair;
来源：http://yfb.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://djh.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kqu.yuxming.cn

PHP:  // 无重载
来源：http://zba.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hhi.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://yth.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lsk.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://xvy.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://sir.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ytc.fehbvm.com

================================================================================
来源：http://obc.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://lcj.wangshuangyany.cn

================================================================================
来源：http://fin.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://zbg.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ftk.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hsa.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nqe.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jsv.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ivd.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://rdy.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://xbf.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qbj.ppjwa.cn

[D02] 追加元素到末尾
来源：http://xhz.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yfw.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jcy.zhiwuduotai.top

JS:   arr.push(4);
来源：http://mcv.daxiang520.top

TS:   arr.push(4);
来源：http://djx.shanyushiyangtech.top

Java: list.add(4);
来源：http://rwe.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://swd.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://yqw.chenjidiqi.icu

C#:   list.Add(4);
来源：http://nik.fehbvm.com

[D03] 在指定位置插入元素
来源：http://npc.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://gsw.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yby.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ldq.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://ikt.hnxiangtu.top

Java: list.add(0, 0);
来源：http://atu.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://sxh.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bzk.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://pkz.guowangkeji.top

[D04] 删除元素
来源：http://afc.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yxo.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://onc.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyc.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://vgf.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gjd.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xzb.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kmg.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://acc.fehbvm.com

[D05] 访问与修改元素
来源：http://bqz.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uns.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://djg.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tjw.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://oui.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://sgy.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://nfo.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hqs.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tcx.xuanzx.com

[D06] 数组长度
来源：http://xxs.hnqzz.top

Py:   len(arr)
来源：http://zrz.mhx1999.top

PHP:  count($arr);
来源：http://mom.yj202588.top

JS:   arr.length
来源：http://bpa.xinyue.icu

TS:   arr.length
来源：http://ejz.chenlongwang.top

Java: list.size();
来源：http://zan.yj202588.top

Go:   len(arr)
来源：http://tqd.hesvh.cn

Ruby: arr.length; arr.size
来源：http://igg.svipenyu.cn

C#:   list.Count;
来源：http://qiw.birdmap.top

[D07] 切片 / 取子数组
来源：http://jfc.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ksb.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://mcg.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://ryo.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://goy.daxiang520.top

Java: list.subList(1, 4);
来源：http://gvh.sjlbkw.cn

Go:   arr[1:4]
来源：http://ajs.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://muf.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://rsp.nanxinkj.top

[D08] 合并两个数组
来源：http://lin.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://dqv.tarul.cn

PHP:  array_merge($a, $b);
来源：http://kim.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cmh.jinqigufen.top

TS:   [...a, ...b];
来源：http://ubx.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cio.vehdjk.com

Go:   append(a, b...)
来源：http://kfb.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://bbq.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://ggh.dashuyun.cn

[D09] 排序（升序）
来源：http://bvj.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://ctl.tarul.cn

PHP:  sort($arr);
来源：http://tlu.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jer.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sep.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://whf.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vgc.sxryk.cn

Ruby: arr.sort
来源：http://mtk.fengsongda.top

C#:   list.Sort();
来源：http://jtc.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ltr.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eum.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fgu.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pqt.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntq.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qaf.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dcj.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rfs.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fnp.cucudq.cn

[D11] 反转数组
来源：http://fsb.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://alx.yj20258888.top

PHP:  array_reverse($arr);
来源：http://sfn.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://utz.xylfe.cn

TS:   [...arr].reverse();
来源：http://wkx.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://uqf.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://zav.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://oky.nwbrower.top

C#:   list.Reverse();
来源：http://vim.zycfv.cn

[D12] 查找元素下标
来源：http://cno.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://zjl.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bhn.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrx.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mnz.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ojw.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://pem.zhoulong.xyz

Ruby: arr.index(x)
来源：http://fbj.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://qxj.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://ylb.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wkn.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tbz.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://qec.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://vxe.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hqd.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://for.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://jqf.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://acr.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://arx.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lhm.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wac.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://ogq.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://jqj.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jcb.feifeiyinyue.top

Go:   // 手写循环
来源：http://xgp.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hug.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jgw.tian-w.cn

[D15] 去重
来源：http://xwf.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bho.cdnleiting.top

PHP:  array_unique($arr);
来源：http://kzb.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://drr.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://vlx.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://khs.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dav.snrcjt.cn

Ruby: arr.uniq
来源：http://gjp.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://ruw.jqgfzy.top

[D16] 求和与平均值
来源：http://wat.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nrm.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rkr.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzo.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nhq.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ixo.cashguo.top

Go:   // 手写循环累加
来源：http://toc.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://evt.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://gol.yanxiufei.cn

[D17] 最大值与最小值
来源：http://zcu.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://ddc.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://tnl.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qqv.ydzc1.top

TS:   Math.max(...arr);
来源：http://gbb.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://vbn.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xhc.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://tny.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://hue.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://ahd.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zsn.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://kbh.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zvs.zhijiandao.cn

TS:   nested.flat();
来源：http://too.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fdo.svipenyu.cn

Go:   // 手写双层循环
来源：http://ezd.dianchejie.cn

Ruby: nested.flatten
来源：http://phy.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sql.yuxming.cn

[D19] 按字段分组
来源：http://crv.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zwd.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pbr.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eoe.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gog.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://szd.cheryme.top

Go:   // 手写 map[string][]T
来源：http://zoe.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://icm.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vxz.yj20258.top

[D20] 统计每个元素出现次数
来源：http://umz.sweek.top

Py:   Counter(arr)
来源：http://pfh.xuanzx.com

PHP:  array_count_values($arr);
来源：http://wum.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lco.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vlo.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://frt.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://ghi.aizwys.cn

Ruby: arr.tally
来源：http://pfy.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xjg.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://dmh.9152youxi.cn

Py:   x in arr
来源：http://xsv.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://knk.redwolf501.top

JS:   arr.includes(x)
来源：http://tsw.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://cnb.jinqigfzy.top

Java: list.contains(x)
来源：http://ubs.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://dgb.ctjpmb.com

Ruby: arr.include?(x)
来源：http://sbc.316326.xyz

C#:   list.Contains(x)
来源：http://baa.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://yqp.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iui.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uue.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fna.daria6918.cn

TS:   [...arr];
来源：http://jry.cucudq.cn

Java: new ArrayList<>(list);
来源：http://ibm.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://jkz.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://tng.gaohongyu789.top

C#:   new List<int>(list);
来源：http://kqk.0kj1m.cn

[D23] reduce 累积计算
来源：http://jva.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qng.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wsq.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vjj.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubp.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dxr.hongshengwenyu.top

Go:   // 手写循环
来源：http://lfp.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ehi.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qpf.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://oef.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uhq.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://msk.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bzn.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ysm.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://opg.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://trj.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bkh.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mwz.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://goa.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://irs.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wrg.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://veq.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iht.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qnw.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xyk.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jiy.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wji.aizwys.cn

[D26] 数组转字符串
来源：http://xtv.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://rcf.cashguo.top

PHP:  implode(", ", $arr);
来源：http://kdb.daria6918.cn

JS:   arr.join(", ")
来源：http://thn.jlsjyb.cn

TS:   arr.join(", ")
来源：http://hej.zhongyouzk.top

Java: String.join(", ", list)
来源：http://ars.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://dmw.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://hry.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://feq.svipenyu.cn

================================================================================
来源：http://atv.yuanzhike.top

E. 字符串处理
来源：http://bhj.yj20258888.top

================================================================================
来源：http://eqt.52xcode.cn

[E01] 拼接字符串
来源：http://zaz.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fyt.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bcl.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ect.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pid.yfazqb.com


<!-- 参考信息 -->