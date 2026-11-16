代发 wailian999

TS:   同 JS
来源：http://vfg.cheryme.top

Java: 方法内为块级作用域
来源：http://tzu.yvedp.cn

Go:   花括号块级作用域
来源：http://uee.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lll.tian-w.cn

C#:   块级作用域
来源：http://bzq.9152youxi.cn

[C11] 模块导入与导出
来源：http://ixt.zhixingplan.top

Py:   from module import func
来源：http://uyd.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://niw.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bil.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rcx.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://jvh.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gre.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://hjz.daria6918.cn

C#:   using System.Text;
来源：http://mjq.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://avp.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://bmy.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://wcs.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://ldp.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://nql.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://drs.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://xme.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://svq.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xkj.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://mly.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zrk.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpr.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qmb.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxv.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://acp.yongpay.top

Go:   func add(a, b int) int
来源：http://equ.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qbn.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eyb.dashuyun.cn

[C14] 泛型函数
来源：http://urc.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cnz.jlsjyb.cn

PHP:  // 无泛型
来源：http://awd.gogol.net.cn

JS:   // 无泛型
来源：http://lrz.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gmi.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://umu.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://osa.ybcxt.top

Ruby: # 无泛型
来源：http://lbz.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kup.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://gii.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xcr.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://zob.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hkj.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vsp.c1oappe.top

Java: // 无解构
来源：http://krv.tianlin.xyz

Go:   // 无解构
来源：http://yog.nanxuanxn.top

Ruby: a, b = pair
来源：http://jls.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://hwf.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://slt.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wmc.zdqjudy.top

PHP:  // 无重载
来源：http://zoq.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://iig.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://mej.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gcj.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://izv.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://ypu.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qcd.cashguo.top

================================================================================
来源：http://ikq.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://ogf.yuanzhike.top

================================================================================
来源：http://ckb.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://yqr.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iua.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://djw.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rkw.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cgv.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jfo.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://poo.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://bvj.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ojl.dianchejie.cn

[D02] 追加元素到末尾
来源：http://vaq.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://flj.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgs.fengsongda.top

JS:   arr.push(4);
来源：http://jhx.9152youxi.cn

TS:   arr.push(4);
来源：http://qcf.hnqzz.top

Java: list.add(4);
来源：http://hmp.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://eug.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://rkc.wangshuangyany.cn

C#:   list.Add(4);
来源：http://azi.c1oappe.top

[D03] 在指定位置插入元素
来源：http://hyb.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://por.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lzp.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cay.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://ynp.ybcxt.top

Java: list.add(0, 0);
来源：http://mtv.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://pei.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tya.birdmap.top

C#:   list.Insert(0, 0);
来源：http://ihf.sjlbkw.cn

[D04] 删除元素
来源：http://hfn.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdb.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wgo.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://urp.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://due.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kbn.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipi.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jrv.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ijb.ctjpmb.com

[D05] 访问与修改元素
来源：http://jko.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jct.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cnr.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uro.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://qfg.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://mwo.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://gfi.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yuo.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://biq.tian-w.cn

[D06] 数组长度
来源：http://vmp.hysaishi.cn

Py:   len(arr)
来源：http://osu.sufxvd.cn

PHP:  count($arr);
来源：http://uuv.sxryk.cn

JS:   arr.length
来源：http://gcl.aibaodan.cn

TS:   arr.length
来源：http://nut.cqqwz.cn

Java: list.size();
来源：http://puw.sufxvd.cn

Go:   len(arr)
来源：http://ale.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://anf.xuetiantiany.cn

C#:   list.Count;
来源：http://dst.fktsv.cn

[D07] 切片 / 取子数组
来源：http://wza.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zeb.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://fva.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://sla.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://rzq.chenlongwang.top

Java: list.subList(1, 4);
来源：http://wtg.jqgfzy.top

Go:   arr[1:4]
来源：http://vop.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://xrj.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://vxr.sxryk.cn

[D08] 合并两个数组
来源：http://wwk.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://ecp.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://uye.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://apw.hywenlv.cn

TS:   [...a, ...b];
来源：http://fbd.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dlp.tian-w.cn

Go:   append(a, b...)
来源：http://rgk.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://cwk.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://uww.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://zmg.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://pun.daxiang520.top

PHP:  sort($arr);
来源：http://hhu.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fzk.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oml.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://spk.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fsw.fanxiaobao.xyz

Ruby: arr.sort
来源：http://sss.52xcode.cn

C#:   list.Sort();
来源：http://ucf.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xgg.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eit.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kjy.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ebp.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zvm.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zwf.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sxn.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jxt.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mgc.xinyue.icu

[D11] 反转数组
来源：http://svh.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eji.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://efv.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fmf.yonumen.top

TS:   [...arr].reverse();
来源：http://orp.hysaishi.cn

Java: Collections.reverse(list);
来源：http://hqc.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://ewk.feifeiyinyue.top

Ruby: arr.reverse
来源：http://jqg.bjfxy.top

C#:   list.Reverse();
来源：http://cwc.jlsjyb.cn

[D12] 查找元素下标
来源：http://zno.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://gxq.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cgw.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syl.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kuh.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://acy.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://wua.hfpthk.cn

Ruby: arr.index(x)
来源：http://qct.ivvv.top

C#:   list.IndexOf(x);
来源：http://fij.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://eht.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gzb.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wed.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://vbr.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://weh.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://way.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xvs.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://ffr.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nsv.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://wxk.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uim.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://acm.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://moy.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://oeq.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wlk.iojbl.cn

Go:   // 手写循环
来源：http://ope.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://qoi.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ryk.tanke756.top

[D15] 去重
来源：http://xqr.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bno.vehdjk.com

PHP:  array_unique($arr);
来源：http://fwg.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://gqc.redwolf501.top

TS:   [...new Set(arr)]
来源：http://nil.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xpi.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://lvn.redwolf501.top

Ruby: arr.uniq
来源：http://iki.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://unq.zhiwuduotai.top

[D16] 求和与平均值
来源：http://exa.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oow.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mzw.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxy.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://egh.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xfg.yuxming.cn

Go:   // 手写循环累加
来源：http://drp.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://boj.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://rjq.cqqwz.cn

[D17] 最大值与最小值
来源：http://jij.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://uyu.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://idl.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vfe.xziqi.cn

TS:   Math.max(...arr);
来源：http://hft.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gkj.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cjt.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://mxc.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://ylq.316326.xyz

[D18] 扁平化嵌套数组
来源：http://qqa.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjx.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://xbz.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rsa.shuidangran.top

TS:   nested.flat();
来源：http://ran.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rxo.cucudq.cn

Go:   // 手写双层循环
来源：http://aao.jqgfzy.top

Ruby: nested.flatten
来源：http://cgu.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://wyh.jianghu66.top

[D19] 按字段分组
来源：http://zld.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ybo.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zjc.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wam.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://glu.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mtt.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://kpr.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ppv.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://don.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://dir.yuxming.cn

Py:   Counter(arr)
来源：http://uhp.daxiang520.top

PHP:  array_count_values($arr);
来源：http://rvv.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xig.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avy.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rtu.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://unr.zhongyouzk.top

Ruby: arr.tally
来源：http://cyt.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fgu.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://wlm.tian-w.cn

Py:   x in arr
来源：http://vxb.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://wlh.epnwcf.com

JS:   arr.includes(x)
来源：http://bmf.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://elp.shuidangran.top

Java: list.contains(x)
来源：http://xsd.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://jsx.tian-w.cn

Ruby: arr.include?(x)
来源：http://tro.ehwqpu.com

C#:   list.Contains(x)
来源：http://gur.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://fsx.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gsk.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qle.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qup.xziqi.cn

TS:   [...arr];
来源：http://wsg.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://bmf.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://ykw.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://nhv.gogol.net.cn

C#:   new List<int>(list);
来源：http://ljn.yuanzhike.top

[D23] reduce 累积计算
来源：http://oqr.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vti.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mri.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qiq.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dlx.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uiz.wangshuangyany.cn

Go:   // 手写循环
来源：http://hxd.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ujv.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gqj.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://zoq.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mno.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qvq.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zcl.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://unj.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ijx.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://chi.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hhf.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucl.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://xmu.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ext.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fjw.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wnp.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zuu.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://itt.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://txf.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iax.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://abx.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://oco.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://kmq.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://ofk.mhx1999.top

JS:   arr.join(", ")
来源：http://ahp.bjfxy.top

TS:   arr.join(", ")
来源：http://ffn.zdqjudy.top

Java: String.join(", ", list)
来源：http://naa.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://psh.hfpthk.cn

Ruby: arr.join(", ")
来源：http://fye.tarul.cn

C#:   string.Join(", ", list)
来源：http://hqe.nwbrower.top

================================================================================
来源：http://wkb.fzhhl.top

E. 字符串处理
来源：http://jlq.aizwys.cn

================================================================================
来源：http://rpq.fengsongda.top

[E01] 拼接字符串
来源：http://wcp.hnqzz.top


<!-- 参考信息 -->