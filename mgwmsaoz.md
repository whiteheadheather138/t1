代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://lts.daria6918.cn

Go:   func add(a, b int) int
来源：http://zoy.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tca.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://vzj.ybcxt.top

[C14] 泛型函数
来源：http://oic.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://smr.aizwys.cn

PHP:  // 无泛型
来源：http://ptu.cqqwz.cn

JS:   // 无泛型
来源：http://pcs.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dmf.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://axj.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xbj.yuanzhike.top

Ruby: # 无泛型
来源：http://dwd.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://amt.gzhubu.top

[C15] 解构 / 展开参数
来源：http://lyi.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tnl.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://ibu.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://voi.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sms.zhijiandao.cn

Java: // 无解构
来源：http://iix.ywan-chungtsiang.top

Go:   // 无解构
来源：http://utp.fengsongda.top

Ruby: a, b = pair
来源：http://tkg.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://xcw.sxryk.cn

[C16] 函数 / 方法重载
来源：http://nhr.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://reb.sxryk.cn

PHP:  // 无重载
来源：http://xpc.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rkv.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://ovs.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dzc.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://bbj.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://beh.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://esb.wangdashe.top

================================================================================
来源：http://ilr.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://ucz.chenlongwang.top

================================================================================
来源：http://guv.fehbvm.com

[D01] 创建数组 / 列表
来源：http://pom.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pry.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zvn.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://auw.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ivf.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zhg.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://ugn.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://zzr.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jkq.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://hfy.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ywx.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pyg.yj20258.top

JS:   arr.push(4);
来源：http://kdz.gzhubu.top

TS:   arr.push(4);
来源：http://veu.ctjpmb.com

Java: list.add(4);
来源：http://lre.pycfn.com

Go:   arr = append(arr, 4)
来源：http://drw.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://ija.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://lfo.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://wzx.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://izl.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xhc.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tuf.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://reo.jinqigfzy.top

Java: list.add(0, 0);
来源：http://qso.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://kry.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ztw.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://wcq.ivvv.top

[D04] 删除元素
来源：http://epz.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dgp.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twe.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pwl.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://qci.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bfs.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zpp.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tlf.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cpa.redwolf501.top

[D05] 访问与修改元素
来源：http://vjy.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gzh.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cdz.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wpd.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://hyy.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://ulr.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://hph.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pvx.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bfe.kuanghao11.cn

[D06] 数组长度
来源：http://hrp.zhiwuduotai.top

Py:   len(arr)
来源：http://yji.tarul.cn

PHP:  count($arr);
来源：http://eii.pycfn.com

JS:   arr.length
来源：http://hip.9152youxi.cn

TS:   arr.length
来源：http://yir.nwbrower.top

Java: list.size();
来源：http://coc.hnqzz.top

Go:   len(arr)
来源：http://fuz.yfazqb.com

Ruby: arr.length; arr.size
来源：http://uxs.nanxuanxn.top

C#:   list.Count;
来源：http://yho.aizwys.cn

[D07] 切片 / 取子数组
来源：http://txw.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcr.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vpo.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://moa.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://ylj.yj20258.top

Java: list.subList(1, 4);
来源：http://ywr.zhengqikj.top

Go:   arr[1:4]
来源：http://szf.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://mjw.sweek.top

C#:   list.GetRange(1, 3);
来源：http://lcl.hcnkem.com

[D08] 合并两个数组
来源：http://owu.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://agr.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://gwh.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ywr.zycfv.cn

TS:   [...a, ...b];
来源：http://iyy.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gfd.hnxiangtu.top

Go:   append(a, b...)
来源：http://nrj.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://rwc.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://iki.guannengcc.top

[D09] 排序（升序）
来源：http://ner.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://jdk.sweek.top

PHP:  sort($arr);
来源：http://bar.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxw.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://drd.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://stw.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wpe.dashuyun.cn

Ruby: arr.sort
来源：http://yjh.gaohongyu789.top

C#:   list.Sort();
来源：http://fng.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://btf.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rxo.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rou.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://opo.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jct.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ers.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ibm.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zne.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hub.shanyushiyangtech.top

[D11] 反转数组
来源：http://utj.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://ruj.xziqi.cn

PHP:  array_reverse($arr);
来源：http://dds.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://naq.nwbrower.top

TS:   [...arr].reverse();
来源：http://nhx.vehdjk.com

Java: Collections.reverse(list);
来源：http://hjo.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://vsy.xuanzx.com

Ruby: arr.reverse
来源：http://zhe.fengsongda.top

C#:   list.Reverse();
来源：http://ppw.gaohongyu789.top

[D12] 查找元素下标
来源：http://ifl.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://ayp.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xvo.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zhd.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kuf.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sbf.sweek.top

Go:   slices.Index(arr, x)
来源：http://uzk.tianlin.xyz

Ruby: arr.index(x)
来源：http://rrl.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://mys.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://wpn.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sjq.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fty.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://tqg.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://vlc.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dyd.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oii.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qfx.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://puu.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://odt.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vbk.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gho.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://ssr.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://yui.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://hpo.52xcode.cn

Go:   // 手写循环
来源：http://tkv.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://scg.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pdu.epnwcf.com

[D15] 去重
来源：http://eqd.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uhr.redwolf501.top

PHP:  array_unique($arr);
来源：http://hda.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://vgv.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://bpe.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yjt.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://bfk.quarkkingdee.top

Ruby: arr.uniq
来源：http://uqp.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://kvr.wangdashe.top

[D16] 求和与平均值
来源：http://xor.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mea.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ugy.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ioc.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ocv.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jxf.xylfe.cn

Go:   // 手写循环累加
来源：http://tro.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rve.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://qxt.xinyue.icu

[D17] 最大值与最小值
来源：http://wge.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://gzj.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://xfc.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iaz.yj202588.top

TS:   Math.max(...arr);
来源：http://bhy.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://hkf.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgn.ivvv.top

Ruby: arr.max;  arr.min
来源：http://czi.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://dyn.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://akm.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ohv.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mxy.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ucz.gzhubu.top

TS:   nested.flat();
来源：http://zmn.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://btq.havefunace.top

Go:   // 手写双层循环
来源：http://hbv.zhijiandao.cn

Ruby: nested.flatten
来源：http://abe.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wjm.nanxinkj.top

[D19] 按字段分组
来源：http://qzu.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ykk.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bgx.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://anm.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zwg.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://drg.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://ont.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://llk.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zlj.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://ios.shuidangran.top

Py:   Counter(arr)
来源：http://ndl.hcnkem.com

PHP:  array_count_values($arr);
来源：http://wxr.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://osa.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gyc.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lig.aizwys.cn

Go:   // 手写 map[T]int
来源：http://bdn.pycfn.com

Ruby: arr.tally
来源：http://vka.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbb.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://pcg.feifeiyinyue.top

Py:   x in arr
来源：http://gjl.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://dpa.zycfv.cn

JS:   arr.includes(x)
来源：http://bzt.chenlongwang.top

TS:   arr.includes(x)
来源：http://tct.yfazqb.com

Java: list.contains(x)
来源：http://atk.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://fbl.birdmap.top

Ruby: arr.include?(x)
来源：http://sos.gaohongyu789.top

C#:   list.Contains(x)
来源：http://rkv.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://bte.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bro.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zks.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ivc.hcnkem.com

TS:   [...arr];
来源：http://nli.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://tvg.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xlp.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://olt.gzhubu.top

C#:   new List<int>(list);
来源：http://jrj.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://erh.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iwl.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jaf.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uoi.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zag.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmf.shuidangran.top

Go:   // 手写循环
来源：http://wyh.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nrl.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zuo.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://oha.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vwd.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gmp.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://elk.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://buq.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujf.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tyn.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zzw.dashuyun.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gwc.hammf.cn

[D25] Set 集合去重与交并差
来源：http://zyh.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zok.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wdw.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ahm.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://adi.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bua.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sep.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hgh.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bas.yj20258888.top

[D26] 数组转字符串
来源：http://tdp.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://cws.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://rnf.cqqwz.cn

JS:   arr.join(", ")
来源：http://qhl.guowangkeji.top

TS:   arr.join(", ")
来源：http://vby.yj20258.top

Java: String.join(", ", list)
来源：http://zoz.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://yzg.zhengqikj.top

Ruby: arr.join(", ")
来源：http://txc.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://hrd.andypj.xyz

================================================================================
来源：http://mcj.jinqigufen.top

E. 字符串处理
来源：http://irq.yj202588.top

================================================================================
来源：http://ojg.cqqwz.cn

[E01] 拼接字符串
来源：http://wnj.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ihr.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yse.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vuu.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ucu.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://glv.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://txf.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uqv.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dwl.hnxiangtu.top

[E02] 重复字符串
来源：http://rbc.sufxvd.cn

Py:   "ab" * 3
来源：http://ecx.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://nvh.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://blu.hesvh.cn

TS:   "ab".repeat(3)
来源：http://reg.aizwys.cn

Java: "ab".repeat(3)
来源：http://wpt.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://zhn.kuanghao11.cn

Ruby: "ab" * 3
来源：http://zoa.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://evi.ybcxt.top

[E03] 截取子串
来源：http://yds.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://krv.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eoj.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxr.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://ldm.daria6918.cn

Java: s.substring(1, 4)
来源：http://lcu.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rfr.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://svj.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://hyv.jqgfzy.top

[E04] 查找子串位置
来源：http://xzj.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://wrc.fktsv.cn


<!-- 参考信息 -->