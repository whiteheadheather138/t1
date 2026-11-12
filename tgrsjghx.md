代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mzg.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://erp.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pim.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bzu.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ruu.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ril.yangfankeji.com

[D05] 访问与修改元素
来源：http://jgz.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bqa.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iei.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yeb.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://ftk.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://ohp.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://ipr.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vpx.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lwc.jinqigfzy.top

[D06] 数组长度
来源：http://ggn.jyoumei.cn

Py:   len(arr)
来源：http://eei.gogol.net.cn

PHP:  count($arr);
来源：http://oap.jlsjyb.cn

JS:   arr.length
来源：http://lxs.redwolf501.top

TS:   arr.length
来源：http://dta.aibaodan.cn

Java: list.size();
来源：http://mnz.xuanzx.com

Go:   len(arr)
来源：http://wwh.daxiang520.top

Ruby: arr.length; arr.size
来源：http://wgs.yangfankeji.com

C#:   list.Count;
来源：http://ikc.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://vlj.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqv.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nxm.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://drh.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://esy.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://puv.yonumen.top

Go:   arr[1:4]
来源：http://esd.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://ugq.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://mju.yj20258888.top

[D08] 合并两个数组
来源：http://plg.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://mtu.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://gqy.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wmf.xylfe.cn

TS:   [...a, ...b];
来源：http://gse.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qlw.jyoumei.cn

Go:   append(a, b...)
来源：http://wew.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://nkd.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://pdg.fktsv.cn

[D09] 排序（升序）
来源：http://xeq.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://dxc.xuetiantiany.cn

PHP:  sort($arr);
来源：http://mgg.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdv.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://gfo.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://vyn.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://twe.daria6918.cn

Ruby: arr.sort
来源：http://glo.dashuyun.cn

C#:   list.Sort();
来源：http://ahm.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://exv.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tun.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rti.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahf.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqm.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://chi.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rlz.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://thv.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://epk.hcnkem.com

[D11] 反转数组
来源：http://ezf.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gtm.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://utn.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ljf.xylfe.cn

TS:   [...arr].reverse();
来源：http://zcc.nanxinkj.top

Java: Collections.reverse(list);
来源：http://jso.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://eph.guowangkeji.top

Ruby: arr.reverse
来源：http://mzy.ehwqpu.com

C#:   list.Reverse();
来源：http://mfr.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://obi.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://opm.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ztd.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mvm.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fqu.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://snu.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://wkm.zdqjudy.top

Ruby: arr.index(x)
来源：http://ibe.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://ybj.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://vtf.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oug.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uop.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://auk.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://urr.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hcq.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pjt.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://qsi.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://rww.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://pwd.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tak.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpn.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://grm.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://riz.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qfc.daria6918.cn

Go:   // 手写循环
来源：http://rmg.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tpy.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://dcs.yj20258888.top

[D15] 去重
来源：http://xdn.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://imf.ppjwa.cn

PHP:  array_unique($arr);
来源：http://vso.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://bzv.hnqzz.top

TS:   [...new Set(arr)]
来源：http://ddj.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fis.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://imd.feifeiyinyue.top

Ruby: arr.uniq
来源：http://quj.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://urn.ydzc1.top

[D16] 求和与平均值
来源：http://wql.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://umo.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyo.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uih.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://usv.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zui.tarul.cn

Go:   // 手写循环累加
来源：http://mok.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mki.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://iqy.redwolf501.top

[D17] 最大值与最小值
来源：http://tyf.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://qov.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://lfn.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxf.sufxvd.cn

TS:   Math.max(...arr);
来源：http://yxb.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jqt.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://djp.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://skm.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://uvf.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://wsh.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dpt.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://zbn.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dsd.cashguo.top

TS:   nested.flat();
来源：http://aeu.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mpy.hcnkem.com

Go:   // 手写双层循环
来源：http://gnn.hammf.cn

Ruby: nested.flatten
来源：http://rec.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lls.gzhubu.top

[D19] 按字段分组
来源：http://vlz.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mpo.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mxy.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dqm.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zjm.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://poe.havefunace.top

Go:   // 手写 map[string][]T
来源：http://aek.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ovi.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hzq.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://qbb.jyoumei.cn

Py:   Counter(arr)
来源：http://xsj.zycfv.cn

PHP:  array_count_values($arr);
来源：http://yde.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://plk.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dha.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awx.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://eul.ivvv.top

Ruby: arr.tally
来源：http://bzj.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eku.hnqzz.top

[D21] 判断是否包含某元素
来源：http://qzu.zhengqikj.top

Py:   x in arr
来源：http://oov.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://czq.havefunace.top

JS:   arr.includes(x)
来源：http://rmu.chenzaomai.com

TS:   arr.includes(x)
来源：http://ahb.ydzc1.top

Java: list.contains(x)
来源：http://qdm.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://xmd.vehdjk.com

Ruby: arr.include?(x)
来源：http://eoy.zycfv.cn

C#:   list.Contains(x)
来源：http://nbn.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://lfm.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ery.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://akn.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ake.xuanzx.com

TS:   [...arr];
来源：http://hip.andypj.xyz

Java: new ArrayList<>(list);
来源：http://nmv.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://ogv.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://zdx.kuanghao11.cn

C#:   new List<int>(list);
来源：http://eor.cashguo.top

[D23] reduce 累积计算
来源：http://epm.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hwe.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbn.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ruy.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eyp.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://sdd.redwolf501.top

Go:   // 手写循环
来源：http://znm.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lwy.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dkd.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://oju.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rjn.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jgf.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xuu.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qes.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pag.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pis.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zms.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://efu.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://ccx.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ykk.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vwj.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tfi.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wsy.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://atn.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rhp.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xiv.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bbf.fzhhl.top

[D26] 数组转字符串
来源：http://wsa.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://yhh.ivvv.top

PHP:  implode(", ", $arr);
来源：http://sdj.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://uqv.zhixingplan.top

TS:   arr.join(", ")
来源：http://tpw.daria6918.cn

Java: String.join(", ", list)
来源：http://ryf.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://kar.tian-w.cn

Ruby: arr.join(", ")
来源：http://ktp.bbcook.cn

C#:   string.Join(", ", list)
来源：http://lhv.shanyushiyangtech.top

================================================================================
来源：http://wyz.yonumen.top

E. 字符串处理
来源：http://uxb.daria6918.cn

================================================================================
来源：http://kch.ivvv.top

[E01] 拼接字符串
来源：http://egi.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fyw.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cyn.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sop.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kgd.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rbs.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://upj.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qhx.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qnr.ehwqpu.com

[E02] 重复字符串
来源：http://acb.epnwcf.com

Py:   "ab" * 3
来源：http://koq.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://kmw.bbcook.cn

JS:   "ab".repeat(3)
来源：http://lxv.andypj.xyz

TS:   "ab".repeat(3)
来源：http://gfq.xinyue.icu

Java: "ab".repeat(3)
来源：http://fpb.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://yly.cucudq.cn

Ruby: "ab" * 3
来源：http://wwh.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qbv.xylfe.cn

[E03] 截取子串
来源：http://hbk.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kyb.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dnf.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://obv.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://dvc.tarul.cn

Java: s.substring(1, 4)
来源：http://kdn.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bew.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qqp.tarul.cn

C#:   s.Substring(1, 3)
来源：http://lhs.jinqigufen.top

[E04] 查找子串位置
来源：http://swf.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://cst.zycfv.cn

PHP:  strpos($s, "x");
来源：http://jba.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fjb.yj20258.top

TS:   s.indexOf("x")
来源：http://ipj.kuanghao11.cn

Java: s.indexOf("x")
来源：http://tuw.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://eon.jqgfzy.top

Ruby: s.index("x")
来源：http://vys.mhx1999.top

C#:   s.IndexOf("x")
来源：http://mxv.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xzu.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vid.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tce.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lxn.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kdb.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://paj.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dhl.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fnf.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yzj.hnqzz.top

[E06] 替换子串
来源：http://eiq.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dwp.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://sje.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yok.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://tmq.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rap.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zac.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dgr.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://paq.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://eff.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jhr.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://adp.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxr.c1oappe.top

TS:   s.split(",")
来源：http://zfv.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://wfa.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qlu.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://sme.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emh.meibo888.top

[E08] 数组按分隔符合并
来源：http://mco.iojbl.cn

Py:   ",".join(items)
来源：http://trv.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://muk.fanxiaobao.xyz

JS:   items.join(",")
来源：http://vcu.cqqwz.cn

TS:   items.join(",")
来源：http://kgr.jqgufenzy.top

Java: String.join(",", items)
来源：http://rhk.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://wiz.zhiwuduotai.top

Ruby: items.join(",")
来源：http://ens.tarul.cn

C#:   string.Join(",", items)
来源：http://avb.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://mia.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vpx.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://apo.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://dai.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://tje.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://aan.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xfl.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://lov.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://stp.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://erj.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hcf.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ypd.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://qmo.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://neh.sxryk.cn

Java: String.format("%03d", 7)
来源：http://ofc.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zht.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rnr.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sjt.sjlbkw.cn

[E11] 反转字符串
来源：http://bpk.cucudq.cn

Py:   s[::-1]
来源：http://pga.zdqjudy.top

PHP:  strrev($s);
来源：http://sxj.chenzaomai.com


<!-- 参考信息 -->