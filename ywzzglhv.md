代发 wailian999

PHP:  // 无重载
来源：http://mjd.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://svq.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://hfl.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mcu.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://poz.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://iqe.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ozy.daria6918.cn

================================================================================
来源：http://kpn.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://pkk.chenlongwang.top

================================================================================
来源：http://pdc.xuanzx.com

[D01] 创建数组 / 列表
来源：http://ope.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xah.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://swn.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://myw.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://dij.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hmf.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://zzw.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://feg.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qyf.ivvv.top

[D02] 追加元素到末尾
来源：http://pzr.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://try.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wgd.sxryk.cn

JS:   arr.push(4);
来源：http://gdf.zdbjq.cn

TS:   arr.push(4);
来源：http://liw.quarkkingdee.top

Java: list.add(4);
来源：http://tvl.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://psh.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://vax.xylfe.cn

C#:   list.Add(4);
来源：http://xzk.vehdjk.com

[D03] 在指定位置插入元素
来源：http://hue.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://inq.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nmm.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qlo.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://kly.jlsjyb.cn

Java: list.add(0, 0);
来源：http://uls.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://kcu.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pcu.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://eue.ctjpmb.com

[D04] 删除元素
来源：http://gmk.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://stq.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pbx.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://too.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://wpp.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qjl.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rre.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cbt.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xil.vqdsnc.cn

[D05] 访问与修改元素
来源：http://dsc.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cie.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://srg.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nnz.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://cdo.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://mea.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://kis.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qte.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tni.meibo888.top

[D06] 数组长度
来源：http://mbg.yvedp.cn

Py:   len(arr)
来源：http://ojx.cdnleiting.top

PHP:  count($arr);
来源：http://sxv.hesvh.cn

JS:   arr.length
来源：http://wwt.aizwys.cn

TS:   arr.length
来源：http://mbd.hongshengwenyu.top

Java: list.size();
来源：http://xpn.xuetiantiany.cn

Go:   len(arr)
来源：http://ucr.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://kze.hnqzz.top

C#:   list.Count;
来源：http://hkh.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://lnm.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ebn.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kok.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://qdo.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://bdw.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://lve.daria6918.cn

Go:   arr[1:4]
来源：http://aja.hfpthk.cn

Ruby: arr[1, 3]
来源：http://zzf.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://ifd.vehdjk.com

[D08] 合并两个数组
来源：http://xby.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://ajf.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://fph.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fmq.hywenlv.cn

TS:   [...a, ...b];
来源：http://tbq.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ojs.ydzc1.top

Go:   append(a, b...)
来源：http://uew.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://ddj.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://ibb.wangshuangyany.cn

[D09] 排序（升序）
来源：http://khy.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://eat.ivvv.top

PHP:  sort($arr);
来源：http://jxl.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rku.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jpv.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://qbv.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eft.mhx1999.top

Ruby: arr.sort
来源：http://edz.cashguo.top

C#:   list.Sort();
来源：http://atj.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://unx.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hnb.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tax.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eba.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://srj.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pze.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vei.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://okt.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zti.hammf.cn

[D11] 反转数组
来源：http://afy.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://xqm.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://wfc.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wig.yongpay.top

TS:   [...arr].reverse();
来源：http://qnp.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://zes.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://fbh.wangdashe.top

Ruby: arr.reverse
来源：http://uxd.zdqjudy.top

C#:   list.Reverse();
来源：http://xuk.9152youxi.cn

[D12] 查找元素下标
来源：http://iry.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://hpe.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cym.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hpa.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bra.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bfo.316326.xyz

Go:   slices.Index(arr, x)
来源：http://sfx.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://dnv.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://xap.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://eas.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qcd.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zwk.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://jkw.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://vsm.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gws.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xty.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://seq.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oqj.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://yxt.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xlq.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uac.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://qgx.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://hmk.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://icx.vqdsnc.cn

Go:   // 手写循环
来源：http://wrk.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://cwp.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xon.c1oappe.top

[D15] 去重
来源：http://etl.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://duj.guowangkeji.top

PHP:  array_unique($arr);
来源：http://kuu.smart0.xyz

JS:   [...new Set(arr)]
来源：http://wms.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://ofk.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://haa.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://fzb.fehbvm.com

Ruby: arr.uniq
来源：http://inh.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://qeu.52xcode.cn

[D16] 求和与平均值
来源：http://kfo.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vst.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://owi.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fnd.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hnu.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dqd.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://gtd.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nef.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://qqo.ybcxt.top

[D17] 最大值与最小值
来源：http://plv.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://ekl.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://gwm.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nas.ybcxt.top

TS:   Math.max(...arr);
来源：http://jai.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xka.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lxg.yongpay.top

Ruby: arr.max;  arr.min
来源：http://oxb.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://ezd.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://moo.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ioz.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://qgq.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oyp.vqdsnc.cn

TS:   nested.flat();
来源：http://xhb.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bok.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://msn.jyoumei.cn

Ruby: nested.flatten
来源：http://cbf.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdg.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://wqj.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gyh.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bco.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ugm.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ria.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mid.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://cge.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xvd.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vzb.316326.xyz

[D20] 统计每个元素出现次数
来源：http://hee.jiagoushi.top

Py:   Counter(arr)
来源：http://nau.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://iws.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bui.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://chb.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tyn.yvedp.cn

Go:   // 手写 map[T]int
来源：http://bat.yj202588.top

Ruby: arr.tally
来源：http://dni.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ocx.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://ndu.tian-w.cn

Py:   x in arr
来源：http://fpa.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://tjs.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://ykn.smart0.xyz

TS:   arr.includes(x)
来源：http://uao.wangdashe.top

Java: list.contains(x)
来源：http://ugp.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://inn.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://cmw.jianghu66.top

C#:   list.Contains(x)
来源：http://dbj.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://pvp.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eks.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dwr.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://imw.zhengqikj.top

TS:   [...arr];
来源：http://mmm.hnqzz.top

Java: new ArrayList<>(list);
来源：http://ocb.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://esq.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://mjt.pycfn.com

C#:   new List<int>(list);
来源：http://kmg.andypj.xyz

[D23] reduce 累积计算
来源：http://pyq.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iej.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://abz.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyb.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://com.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cwc.havefunace.top

Go:   // 手写循环
来源：http://abc.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ccu.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hxj.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://uik.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oqs.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bbd.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zca.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://okk.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bca.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mqv.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vhu.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xnz.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://uwm.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jvu.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uhl.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://car.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wfa.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cxs.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cdo.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://csl.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qxz.iojbl.cn

[D26] 数组转字符串
来源：http://jxd.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://byt.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://upn.epnwcf.com

JS:   arr.join(", ")
来源：http://bln.tanke756.top

TS:   arr.join(", ")
来源：http://hpi.gotoacloud.top

Java: String.join(", ", list)
来源：http://enf.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://pjq.sweek.top

Ruby: arr.join(", ")
来源：http://udx.cashguo.top

C#:   string.Join(", ", list)
来源：http://jqt.aizwys.cn

================================================================================
来源：http://xkg.haohaochexian.top

E. 字符串处理
来源：http://jfw.yuxming.cn

================================================================================
来源：http://igx.52xcode.cn

[E01] 拼接字符串
来源：http://vfl.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://whi.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mpr.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvg.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kle.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tfj.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kgy.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vbp.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hao.shangyingyoupin.top

[E02] 重复字符串
来源：http://exk.yuxming.cn

Py:   "ab" * 3
来源：http://ubn.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://feq.uphjek.com

JS:   "ab".repeat(3)
来源：http://veb.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://zcx.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://mns.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://gso.ydjk.org.cn

Ruby: "ab" * 3
来源：http://ujg.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jss.zhixingplan.top

[E03] 截取子串
来源：http://std.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ucn.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ugi.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fat.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://wtg.jqgfzy.top

Java: s.substring(1, 4)
来源：http://soh.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://emc.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ymu.birdmap.top

C#:   s.Substring(1, 3)
来源：http://xfd.chenjidiqi.icu

[E04] 查找子串位置
来源：http://msj.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://bpb.ybcxt.top

PHP:  strpos($s, "x");
来源：http://vho.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rfl.yfazqb.com

TS:   s.indexOf("x")
来源：http://thb.gogol.net.cn

Java: s.indexOf("x")
来源：http://lvw.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://kyz.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://bip.xinyue.icu

C#:   s.IndexOf("x")
来源：http://ohv.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://god.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nxy.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xjl.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aps.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bot.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cfo.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xpk.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fkn.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rnd.aizwys.cn

[E06] 替换子串
来源：http://fat.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://syg.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://wbm.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jzc.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://hhd.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brz.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iym.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://djz.chenzaomai.com


<!-- 参考信息 -->