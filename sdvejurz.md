代发 wailian999

TS:   同 JS
来源：http://ggu.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://oaa.9152youxi.cn

Go:   花括号块级作用域
来源：http://lby.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://inm.iojbl.cn

C#:   块级作用域
来源：http://amu.xylfe.cn

[C11] 模块导入与导出
来源：http://bwz.hnxiangtu.top

Py:   from module import func
来源：http://tqj.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ctg.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://emc.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://amn.gaohongyu789.top

Java: import java.util.List;
来源：http://tjf.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zun.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://stg.cdnleiting.top

C#:   using System.Text;
来源：http://cua.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://rop.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://slm.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://zhf.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://gxx.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://uxd.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tqz.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://foa.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://eec.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qjn.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://iru.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bee.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efo.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wud.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://myy.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://cwv.dashuyun.cn

Go:   func add(a, b int) int
来源：http://yln.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cob.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://wfs.cucudq.cn

[C14] 泛型函数
来源：http://led.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qxd.guannengcc.top

PHP:  // 无泛型
来源：http://znr.zhengqikj.top

JS:   // 无泛型
来源：http://laq.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bur.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eba.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vkb.nwbrower.top

Ruby: # 无泛型
来源：http://kjh.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tos.cheryme.top

[C15] 解构 / 展开参数
来源：http://aau.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rny.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://pha.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bxc.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hgq.shzxlz.cn

Java: // 无解构
来源：http://chv.hesvh.cn

Go:   // 无解构
来源：http://eot.aizwys.cn

Ruby: a, b = pair
来源：http://wbj.epnwcf.com

C#:   var (a, b) = pair;
来源：http://qta.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://rvh.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dau.smart0.xyz

PHP:  // 无重载
来源：http://ajf.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://umu.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://bvm.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gco.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://xwd.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://gyh.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gjq.jqgufenzy.top

================================================================================
来源：http://tad.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://ofb.xingfuxueyuan.xyz

================================================================================
来源：http://qgx.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://wfs.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ysh.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bej.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uxi.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ydr.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mpp.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://tan.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://mlb.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jap.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://cdr.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nbz.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zwc.jianghu66.top

JS:   arr.push(4);
来源：http://yga.cashguo.top

TS:   arr.push(4);
来源：http://cem.gaohongyu789.top

Java: list.add(4);
来源：http://mbu.birdmap.top

Go:   arr = append(arr, 4)
来源：http://cfh.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://zjv.ehwqpu.com

C#:   list.Add(4);
来源：http://hch.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://qnk.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://pvb.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qhd.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fpp.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://enc.gaohongyu789.top

Java: list.add(0, 0);
来源：http://apv.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://apm.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dkz.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://mds.jinghuilouyu.cn

[D04] 删除元素
来源：http://eid.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bvj.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tvf.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://msl.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://whh.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://int.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rxd.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hfa.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ulh.bbcook.cn

[D05] 访问与修改元素
来源：http://qin.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ipv.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gti.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ehl.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://eyt.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://pth.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://wqm.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfg.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ppd.hesvh.cn

[D06] 数组长度
来源：http://mgk.fzhhl.top

Py:   len(arr)
来源：http://kpw.pycfn.com

PHP:  count($arr);
来源：http://zfn.sjlbkw.cn

JS:   arr.length
来源：http://hgp.tianlin.xyz

TS:   arr.length
来源：http://rkr.daria6918.cn

Java: list.size();
来源：http://gdt.zhiwuduotai.top

Go:   len(arr)
来源：http://csy.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://ifw.yuxming.cn

C#:   list.Count;
来源：http://vde.hesvh.cn

[D07] 切片 / 取子数组
来源：http://vsn.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axv.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://ewf.hammf.cn

JS:   arr.slice(1, 4);
来源：http://zyf.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://jzc.sysykeji.top

Java: list.subList(1, 4);
来源：http://daz.svipenyu.cn

Go:   arr[1:4]
来源：http://mhq.cucudq.cn

Ruby: arr[1, 3]
来源：http://lia.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://lns.aibaodan.cn

[D08] 合并两个数组
来源：http://dge.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://zlk.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://aha.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ngf.xylfe.cn

TS:   [...a, ...b];
来源：http://tfo.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tkl.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://ryg.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://tfz.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://gcw.yueranfly.top

[D09] 排序（升序）
来源：http://qbn.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://phn.jiagoushi.top

PHP:  sort($arr);
来源：http://ank.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mfr.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://set.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qde.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wji.jinqigfzy.top

Ruby: arr.sort
来源：http://fla.52xcode.cn

C#:   list.Sort();
来源：http://oyx.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rad.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fwi.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fng.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://elj.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vzl.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mmg.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yms.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ryw.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hui.uphjek.com

[D11] 反转数组
来源：http://dra.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://rxu.52xcode.cn

PHP:  array_reverse($arr);
来源：http://qqj.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zrx.svipenyu.cn

TS:   [...arr].reverse();
来源：http://zoz.cucudq.cn

Java: Collections.reverse(list);
来源：http://fss.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://ceh.tian-w.cn

Ruby: arr.reverse
来源：http://gdv.sweek.top

C#:   list.Reverse();
来源：http://aza.yuanzhike.top

[D12] 查找元素下标
来源：http://frj.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://zwd.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pfl.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xun.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://heq.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bxp.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://phj.sysykeji.top

Ruby: arr.index(x)
来源：http://gev.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://gor.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://bnj.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qgs.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzk.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://iiv.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://yga.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://atd.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fqx.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xhn.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zpv.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://qjl.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gfz.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wpd.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://nap.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://vrx.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rgu.zhiwuduotai.top

Go:   // 手写循环
来源：http://jsu.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://byk.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tto.wangdashe.top

[D15] 去重
来源：http://bxq.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wqd.dianchejie.cn

PHP:  array_unique($arr);
来源：http://jxk.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://kpl.c1oappe.top

TS:   [...new Set(arr)]
来源：http://fft.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fkp.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cff.ivvv.top

Ruby: arr.uniq
来源：http://tqu.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://qlx.gotoacloud.top

[D16] 求和与平均值
来源：http://nuh.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxp.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ejm.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://efe.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rbv.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vui.sjlbkw.cn

Go:   // 手写循环累加
来源：http://rnh.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gcg.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://yqn.epnwcf.com

[D17] 最大值与最小值
来源：http://xvs.yj20258.top

Py:   max(arr);  min(arr)
来源：http://omi.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://nmu.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kec.hfpthk.cn

TS:   Math.max(...arr);
来源：http://bik.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ydu.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lfs.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://rrd.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://bep.cheryme.top

[D18] 扁平化嵌套数组
来源：http://mmk.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pai.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://dfq.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cjp.kuanghao11.cn

TS:   nested.flat();
来源：http://boj.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://irt.hammf.cn

Go:   // 手写双层循环
来源：http://ped.hesvh.cn

Ruby: nested.flatten
来源：http://sty.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ekd.feifeiyinyue.top

[D19] 按字段分组
来源：http://lmq.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ryl.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fxy.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wuc.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://mvx.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gba.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://fsb.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pih.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zed.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://xsl.daxiang520.top

Py:   Counter(arr)
来源：http://ucm.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://ajl.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dkv.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awc.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://squ.nwbrower.top

Go:   // 手写 map[T]int
来源：http://okl.hesvh.cn

Ruby: arr.tally
来源：http://gok.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cpk.ydzc1.top

[D21] 判断是否包含某元素
来源：http://kfg.hnxiangtu.top

Py:   x in arr
来源：http://cpg.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://bls.cdnleiting.top

JS:   arr.includes(x)
来源：http://les.cheryme.top

TS:   arr.includes(x)
来源：http://wuq.zhijiandao.cn

Java: list.contains(x)
来源：http://ulz.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://rkh.cashguo.top

Ruby: arr.include?(x)
来源：http://dgo.0kj1m.cn

C#:   list.Contains(x)
来源：http://idx.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://pqn.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uyi.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hzs.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yso.hfpthk.cn

TS:   [...arr];
来源：http://bvf.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://mbe.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://jiz.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://ybn.316326.xyz

C#:   new List<int>(list);
来源：http://yoa.zhengqikj.top

[D23] reduce 累积计算
来源：http://fsk.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hmv.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jdy.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhr.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ijv.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihq.316326.xyz

Go:   // 手写循环
来源：http://zko.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://scf.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qpx.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://maa.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vkp.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pws.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rrt.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xdd.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wzc.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vkf.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qdw.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mms.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://pxz.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bvt.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zss.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkx.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ckf.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lvz.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kac.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oma.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://njm.cqqwz.cn

[D26] 数组转字符串
来源：http://akh.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://sbq.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://dbw.sweek.top

JS:   arr.join(", ")
来源：http://fos.zhoulong.xyz

TS:   arr.join(", ")
来源：http://svc.fzhhl.top

Java: String.join(", ", list)
来源：http://heh.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://byq.yangfankeji.com

Ruby: arr.join(", ")
来源：http://utf.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://bbc.yj202588.top

================================================================================
来源：http://mpj.ybcxt.top

E. 字符串处理
来源：http://ion.zhongyouzk.top

================================================================================
来源：http://vab.nwbrower.top

[E01] 拼接字符串
来源：http://yua.yangfankeji.com


<!-- 参考信息 -->