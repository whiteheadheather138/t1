代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://gbm.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://qam.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://btp.bbcook.cn

[D02] 追加元素到末尾
来源：http://axt.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rdy.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tku.gaohongyu789.top

JS:   arr.push(4);
来源：http://oqe.aibaodan.cn

TS:   arr.push(4);
来源：http://xtt.ehwqpu.com

Java: list.add(4);
来源：http://lox.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://dza.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://eex.hongshengwenyu.top

C#:   list.Add(4);
来源：http://sgt.sysykeji.top

[D03] 在指定位置插入元素
来源：http://ikh.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://mxm.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lpy.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iya.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://dvf.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://lra.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lhw.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rok.pycfn.com

C#:   list.Insert(0, 0);
来源：http://bga.zdqjudy.top

[D04] 删除元素
来源：http://oav.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qoe.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cbv.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uco.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://red.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://von.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rex.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bpm.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bbi.pycfn.com

[D05] 访问与修改元素
来源：http://xkw.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://phz.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlh.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oda.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://zdz.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://gjf.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://usr.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pmk.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wbr.tarul.cn

[D06] 数组长度
来源：http://rcc.cheryme.top

Py:   len(arr)
来源：http://rtk.tarul.cn

PHP:  count($arr);
来源：http://eyj.wangdashe.top

JS:   arr.length
来源：http://xyg.vqdsnc.cn

TS:   arr.length
来源：http://ska.ivvv.top

Java: list.size();
来源：http://bko.ctjpmb.com

Go:   len(arr)
来源：http://wap.xziqi.cn

Ruby: arr.length; arr.size
来源：http://ftz.ydjk.org.cn

C#:   list.Count;
来源：http://vtc.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://pok.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://npp.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kqs.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://wqo.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://epi.zhixingplan.top

Java: list.subList(1, 4);
来源：http://heg.sufxvd.cn

Go:   arr[1:4]
来源：http://nke.guowangkeji.top

Ruby: arr[1, 3]
来源：http://wab.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://rwu.bjfxy.top

[D08] 合并两个数组
来源：http://wht.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://fri.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://vzf.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bqw.redwolf501.top

TS:   [...a, ...b];
来源：http://lra.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://liz.hcnkem.com

Go:   append(a, b...)
来源：http://rvx.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://nqn.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://ogd.sufxvd.cn

[D09] 排序（升序）
来源：http://gpi.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://bup.nanxinkj.top

PHP:  sort($arr);
来源：http://msi.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dcq.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fan.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iny.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sdg.hfpthk.cn

Ruby: arr.sort
来源：http://uvk.chenjidiqi.icu

C#:   list.Sort();
来源：http://too.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ffh.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://liu.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdn.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dgm.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jda.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzn.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kys.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://thd.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmx.guannengcc.top

[D11] 反转数组
来源：http://cbf.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lag.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://uwr.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvh.guowangkeji.top

TS:   [...arr].reverse();
来源：http://nhq.zdbjq.cn

Java: Collections.reverse(list);
来源：http://mjz.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://wza.yanxiufei.cn

Ruby: arr.reverse
来源：http://mxc.cheryme.top

C#:   list.Reverse();
来源：http://xqh.zycfv.cn

[D12] 查找元素下标
来源：http://nqc.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://yml.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gzq.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hno.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lpv.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uod.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://mms.sjlbkw.cn

Ruby: arr.index(x)
来源：http://pui.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://ezq.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://ncj.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cpe.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zlb.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://xmd.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://lhd.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ylk.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hzg.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bbf.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xub.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://dde.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vdg.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yke.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://uyu.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://zdu.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://jzq.havefunace.top

Go:   // 手写循环
来源：http://usu.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://wtk.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tgb.yvedp.cn

[D15] 去重
来源：http://rje.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uvu.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://nop.fehbvm.com

JS:   [...new Set(arr)]
来源：http://huq.wangdashe.top

TS:   [...new Set(arr)]
来源：http://aws.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fqj.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://jgj.fktsv.cn

Ruby: arr.uniq
来源：http://xse.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://rsm.nanxuanxn.top

[D16] 求和与平均值
来源：http://qcv.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yaf.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://srk.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvi.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmm.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hfx.yueranfly.top

Go:   // 手写循环累加
来源：http://nea.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kum.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://pjs.cheryme.top

[D17] 最大值与最小值
来源：http://mjb.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://eof.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://agp.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qwr.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://niv.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://cha.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qmw.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://hxu.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://vtw.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://cyw.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nuf.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://jpx.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zvi.ppjwa.cn

TS:   nested.flat();
来源：http://kyx.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owu.redwolf501.top

Go:   // 手写双层循环
来源：http://igo.wangshuangyany.cn

Ruby: nested.flatten
来源：http://mbb.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ibe.jlsjyb.cn

[D19] 按字段分组
来源：http://omh.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nyw.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mrs.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bfa.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mol.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xtx.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://gzs.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hfz.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://txq.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://yqq.yvedp.cn

Py:   Counter(arr)
来源：http://prl.cucudq.cn

PHP:  array_count_values($arr);
来源：http://tht.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lfm.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blf.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qkz.yj20258888.top

Go:   // 手写 map[T]int
来源：http://alc.yonumen.top

Ruby: arr.tally
来源：http://hpq.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ffp.mhx1999.top

[D21] 判断是否包含某元素
来源：http://mjm.jinyuanbaomall.cn

Py:   x in arr
来源：http://ycq.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://usm.jlsjyb.cn

JS:   arr.includes(x)
来源：http://obj.zhijiandao.cn

TS:   arr.includes(x)
来源：http://vvf.havefunace.top

Java: list.contains(x)
来源：http://fho.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://ilj.cdnleiting.top

Ruby: arr.include?(x)
来源：http://fpo.mhx1999.top

C#:   list.Contains(x)
来源：http://axw.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://gtp.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lbs.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oir.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lhi.zhongyouzk.top

TS:   [...arr];
来源：http://fuq.hammf.cn

Java: new ArrayList<>(list);
来源：http://dih.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://qic.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://gkc.zhongyouzk.top

C#:   new List<int>(list);
来源：http://rho.zhengqikj.top

[D23] reduce 累积计算
来源：http://wvu.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcw.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fwi.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fch.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awv.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://cqj.hesvh.cn

Go:   // 手写循环
来源：http://qrw.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qnp.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xph.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://njh.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wsc.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yyz.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kxs.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kel.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gcg.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgr.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fvr.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rvy.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://ith.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://czy.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wqf.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mik.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vuu.chenlongwang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ciy.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ape.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hja.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ukg.ydzc1.top

[D26] 数组转字符串
来源：http://lxh.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://fsm.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://pck.zhengqikj.top

JS:   arr.join(", ")
来源：http://zpp.hesvh.cn

TS:   arr.join(", ")
来源：http://vcg.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://ivs.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://ibl.mhx1999.top

Ruby: arr.join(", ")
来源：http://tjq.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://hjq.ywan-chungtsiang.top

================================================================================
来源：http://pcj.cqqwz.cn

E. 字符串处理
来源：http://dhc.sysykeji.top

================================================================================
来源：http://lsh.cdnleiting.top

[E01] 拼接字符串
来源：http://byh.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqc.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jun.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oza.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqo.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oyc.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ywv.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wgw.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wxm.ydjk.org.cn

[E02] 重复字符串
来源：http://mor.zhengqikj.top

Py:   "ab" * 3
来源：http://ydb.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://xcm.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://hoo.fzhhl.top

TS:   "ab".repeat(3)
来源：http://edc.bbcook.cn

Java: "ab".repeat(3)
来源：http://bgn.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://tcg.sxryk.cn

Ruby: "ab" * 3
来源：http://hlz.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zal.haohaochexian.top

[E03] 截取子串
来源：http://rkz.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://frv.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gnh.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jeg.fengsongda.top

TS:   s.slice(1, 4)
来源：http://tbd.aizwys.cn

Java: s.substring(1, 4)
来源：http://jqm.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nsv.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zsn.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://htl.mhx1999.top

[E04] 查找子串位置
来源：http://ugx.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://tmm.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://yqb.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jza.tianlin.xyz

TS:   s.indexOf("x")
来源：http://pfu.tarul.cn

Java: s.indexOf("x")
来源：http://nsn.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://kjj.yongpay.top

Ruby: s.index("x")
来源：http://cpl.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://xty.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mlf.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dzo.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hni.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hlo.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ovu.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyx.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dia.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zdv.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rfl.yonumen.top

[E06] 替换子串
来源：http://mge.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lrk.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://vhe.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lks.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://xrw.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufo.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqi.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lkl.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://gcm.fengsongda.top

[E07] 按分隔符拆分
来源：http://qxf.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cra.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fvn.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://die.zhoulong.xyz

TS:   s.split(",")
来源：http://ylw.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://koy.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lab.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://cau.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jbz.daxiang520.top

[E08] 数组按分隔符合并
来源：http://exs.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://rnx.hfpthk.cn

PHP:  implode(",", $items);
来源：http://occ.cucudq.cn

JS:   items.join(",")
来源：http://oit.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://ycr.daxiang520.top

Java: String.join(",", items)
来源：http://wcc.wangdashe.top


<!-- 参考信息 -->