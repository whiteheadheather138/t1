代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://gkj.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jwt.jiagoushi.top

Java: import java.util.List;
来源：http://sre.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iit.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://ich.cqqwz.cn

C#:   using System.Text;
来源：http://cuv.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://eef.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://afv.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://xra.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://vta.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://wfc.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ulg.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://wvw.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://hxg.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uxn.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://glf.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cpn.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ncw.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mej.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tah.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://cxu.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://gih.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tah.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://sqv.redwolf501.top

[C14] 泛型函数
来源：http://xig.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aqq.mhx1999.top

PHP:  // 无泛型
来源：http://rad.nanxinkj.top

JS:   // 无泛型
来源：http://rag.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lih.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://get.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://veo.shuidangran.top

Ruby: # 无泛型
来源：http://zry.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yzt.fktsv.cn

[C15] 解构 / 展开参数
来源：http://mra.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ybu.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://wwf.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rsb.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rgb.sysykeji.top

Java: // 无解构
来源：http://dbm.mhx1999.top

Go:   // 无解构
来源：http://ckx.zhijiandao.cn

Ruby: a, b = pair
来源：http://ici.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://cng.bjfxy.top

[C16] 函数 / 方法重载
来源：http://jen.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dbl.hongshengwenyu.top

PHP:  // 无重载
来源：http://cpw.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eda.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://pln.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uln.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://tdv.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://lnq.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ztk.0kj1m.cn

================================================================================
来源：http://rpe.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://got.sweek.top

================================================================================
来源：http://bzq.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://izn.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mar.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mzm.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fsj.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://uoc.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hmd.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://eel.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://oxa.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ibt.uphjek.com

[D02] 追加元素到末尾
来源：http://fiz.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ual.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ioy.andypj.xyz

JS:   arr.push(4);
来源：http://asi.zdbjq.cn

TS:   arr.push(4);
来源：http://qqh.zhongyouzk.top

Java: list.add(4);
来源：http://bbd.ivvv.top

Go:   arr = append(arr, 4)
来源：http://wpn.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://huj.jianghu66.top

C#:   list.Add(4);
来源：http://prh.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://knz.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://imo.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iop.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ssg.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://yfu.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://sbm.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://arx.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kkd.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://rdz.shzxlz.cn

[D04] 删除元素
来源：http://dlg.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zdr.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nwo.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ahz.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://bik.sweek.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ooq.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xvf.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://phy.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eeq.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://edb.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uyl.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xye.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ftm.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://pad.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://yeh.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://ghr.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ids.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lvm.ehwqpu.com

[D06] 数组长度
来源：http://psd.jiagoushi.top

Py:   len(arr)
来源：http://inu.gzhubu.top

PHP:  count($arr);
来源：http://mee.aibaodan.cn

JS:   arr.length
来源：http://fij.jqgfzy.top

TS:   arr.length
来源：http://agc.ywan-chungtsiang.top

Java: list.size();
来源：http://tfh.xuetiantiany.cn

Go:   len(arr)
来源：http://igm.hcnkem.com

Ruby: arr.length; arr.size
来源：http://gqh.zhijiandao.cn

C#:   list.Count;
来源：http://dmi.cucudq.cn

[D07] 切片 / 取子数组
来源：http://pgg.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ebl.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jzf.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://tww.yj202588.top

TS:   arr.slice(1, 4);
来源：http://ghq.xziqi.cn

Java: list.subList(1, 4);
来源：http://gyz.guannengcc.top

Go:   arr[1:4]
来源：http://hei.gogol.net.cn

Ruby: arr[1, 3]
来源：http://gvh.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://tnp.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://ige.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://zdk.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://ybc.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wys.nwbrower.top

TS:   [...a, ...b];
来源：http://hkw.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vtx.yueranfly.top

Go:   append(a, b...)
来源：http://nyp.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://zwj.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://sfk.tanke756.top

[D09] 排序（升序）
来源：http://jsy.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://anq.yonumen.top

PHP:  sort($arr);
来源：http://xum.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pel.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mnt.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fdz.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://whn.hnxiangtu.top

Ruby: arr.sort
来源：http://mtr.316326.xyz

C#:   list.Sort();
来源：http://apf.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bxw.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cci.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kjg.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjs.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpm.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://igj.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jcw.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqd.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dpo.cucudq.cn

[D11] 反转数组
来源：http://teo.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://dep.aizwys.cn

PHP:  array_reverse($arr);
来源：http://vyy.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pes.sufxvd.cn

TS:   [...arr].reverse();
来源：http://ayt.pycfn.com

Java: Collections.reverse(list);
来源：http://rnq.316326.xyz

Go:   slices.Reverse(arr)
来源：http://tdf.quarkkingdee.top

Ruby: arr.reverse
来源：http://cdc.hysaishi.cn

C#:   list.Reverse();
来源：http://xkp.ydjk.org.cn

[D12] 查找元素下标
来源：http://jof.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://lgd.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ije.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfg.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://boo.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gkl.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://iin.fehbvm.com

Ruby: arr.index(x)
来源：http://ran.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://hsk.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://myy.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://khq.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bmz.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://zvj.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://efw.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://asn.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ajh.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://czy.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kyc.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://skq.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://plf.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://btu.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://lgq.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://ftr.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fat.sufxvd.cn

Go:   // 手写循环
来源：http://dmy.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://zpz.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://afq.zycfv.cn

[D15] 去重
来源：http://ecn.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tdk.snrcjt.cn

PHP:  array_unique($arr);
来源：http://psf.mhx1999.top

JS:   [...new Set(arr)]
来源：http://iqm.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://zqa.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bhm.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://mba.zhoulong.xyz

Ruby: arr.uniq
来源：http://vqe.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://ace.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://gcr.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qhq.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yih.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gum.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://djt.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fjx.zhongyouzk.top

Go:   // 手写循环累加
来源：http://hjg.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqa.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://prz.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://jgs.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://whl.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://ldw.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://umy.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://nfo.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bbm.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gox.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://yvo.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://xlb.pycfn.com

[D18] 扁平化嵌套数组
来源：http://bws.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rnz.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://dsi.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xij.guowangkeji.top

TS:   nested.flat();
来源：http://pwx.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iur.zdqjudy.top

Go:   // 手写双层循环
来源：http://ajz.gotoacloud.top

Ruby: nested.flatten
来源：http://how.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qix.hywenlv.cn

[D19] 按字段分组
来源：http://ayo.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vfc.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gpe.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dto.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lha.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ofq.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://idq.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ryx.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jzp.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://bva.xuanzx.com

Py:   Counter(arr)
来源：http://dpk.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://llt.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://psv.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mri.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zbw.mhx1999.top

Go:   // 手写 map[T]int
来源：http://qho.pengpengdd.cyou

Ruby: arr.tally
来源：http://lsh.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ihr.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://jjk.yvedp.cn

Py:   x in arr
来源：http://bbx.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://kri.nanxuanxn.top

JS:   arr.includes(x)
来源：http://hbe.andypj.xyz

TS:   arr.includes(x)
来源：http://fmt.shzxlz.cn

Java: list.contains(x)
来源：http://zts.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://ggd.chenlongwang.top

Ruby: arr.include?(x)
来源：http://cvq.9152youxi.cn

C#:   list.Contains(x)
来源：http://oua.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://gup.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zmm.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zzf.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gma.hesvh.cn

TS:   [...arr];
来源：http://pbw.316326.xyz

Java: new ArrayList<>(list);
来源：http://kea.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://uhn.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://xqc.svipenyu.cn

C#:   new List<int>(list);
来源：http://wcx.yj20258888.top

[D23] reduce 累积计算
来源：http://lba.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://odb.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rgd.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svc.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qml.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fth.hesvh.cn

Go:   // 手写循环
来源：http://imk.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mwb.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xhf.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://quy.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ykm.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vty.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iko.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ngo.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://alz.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eog.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xge.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gkf.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://dah.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rbb.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bfp.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wse.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qjo.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ejk.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qdq.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wxo.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kba.316326.xyz

[D26] 数组转字符串
来源：http://tmg.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://uvi.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://xdm.ydjk.org.cn

JS:   arr.join(", ")
来源：http://xcd.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://gfw.yfazqb.com

Java: String.join(", ", list)
来源：http://qrm.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://tmh.yj20258888.top

Ruby: arr.join(", ")
来源：http://njw.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://cqc.bbcook.cn

================================================================================
来源：http://gim.ydjk.org.cn

E. 字符串处理
来源：http://sds.andypj.xyz

================================================================================
来源：http://smk.c1oappe.top

[E01] 拼接字符串
来源：http://ine.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://saw.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://znl.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgt.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asx.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zpy.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://seg.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://agf.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfl.nanxinkj.top


<!-- 参考信息 -->