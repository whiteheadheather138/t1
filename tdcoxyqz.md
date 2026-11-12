代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kqy.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://cxr.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qkp.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://czh.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ohk.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jhi.fzhhl.top

[D05] 访问与修改元素
来源：http://ymr.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjt.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vqf.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pvr.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://xjs.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://vqi.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://tbe.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ndj.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://goo.yj20258.top

[D06] 数组长度
来源：http://ebj.svipenyu.cn

Py:   len(arr)
来源：http://ziy.tarul.cn

PHP:  count($arr);
来源：http://igi.jlsjyb.cn

JS:   arr.length
来源：http://kck.jianghu66.top

TS:   arr.length
来源：http://idf.c1oappe.top

Java: list.size();
来源：http://yva.zhengqikj.top

Go:   len(arr)
来源：http://egd.tarul.cn

Ruby: arr.length; arr.size
来源：http://jdy.zhaomingkeji.xyz

C#:   list.Count;
来源：http://ger.sysykeji.top

[D07] 切片 / 取子数组
来源：http://vug.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lfw.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://qlv.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://oam.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://myp.sysykeji.top

Java: list.subList(1, 4);
来源：http://rpr.zhixingplan.top

Go:   arr[1:4]
来源：http://tsq.zdqjudy.top

Ruby: arr[1, 3]
来源：http://cbz.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://vri.daria6918.cn

[D08] 合并两个数组
来源：http://oqj.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://pbz.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://pmr.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dkd.jqgufenzy.top

TS:   [...a, ...b];
来源：http://zec.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nyr.yj20258.top

Go:   append(a, b...)
来源：http://ywd.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://yyk.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://nsr.yonumen.top

[D09] 排序（升序）
来源：http://iqn.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://uep.meibo888.top

PHP:  sort($arr);
来源：http://loa.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hkh.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://khu.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eec.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://liv.meibo888.top

Ruby: arr.sort
来源：http://ntl.jiagoushi.top

C#:   list.Sort();
来源：http://feo.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nwr.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kuj.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzc.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lcc.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eyq.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejf.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pgt.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qjm.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vip.gzhubu.top

[D11] 反转数组
来源：http://mtb.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://taj.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://zzh.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hwk.sweek.top

TS:   [...arr].reverse();
来源：http://wtd.gogol.net.cn

Java: Collections.reverse(list);
来源：http://gzn.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://hkv.cashguo.top

Ruby: arr.reverse
来源：http://exu.fehbvm.com

C#:   list.Reverse();
来源：http://aoo.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://bvd.sweek.top

Py:   arr.index(x);  x in arr
来源：http://hbj.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rex.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://caw.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldd.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gvu.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://dtz.cdnleiting.top

Ruby: arr.index(x)
来源：http://gjg.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://hpv.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://poe.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sdm.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rwp.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://bth.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://rws.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gdq.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zse.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://yfr.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pod.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://igr.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vhk.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zlw.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://qlt.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://qxh.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fzp.chenzaomai.com

Go:   // 手写循环
来源：http://nzk.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://tzg.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zcr.ydjk.org.cn

[D15] 去重
来源：http://wll.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fpr.gotoacloud.top

PHP:  array_unique($arr);
来源：http://vmw.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://ulm.zycfv.cn

TS:   [...new Set(arr)]
来源：http://etd.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fyn.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://tpp.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://yjj.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://exb.tarul.cn

[D16] 求和与平均值
来源：http://onb.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lpx.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bvp.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iia.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gtv.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nwe.zhongyouzk.top

Go:   // 手写循环累加
来源：http://jah.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exw.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://qrj.tian-w.cn

[D17] 最大值与最小值
来源：http://rln.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://gcn.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://wyp.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://plm.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://mnn.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hpt.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://inm.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://ppj.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://ncv.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://iyw.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ael.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://uuy.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xic.chenzaomai.com

TS:   nested.flat();
来源：http://dzz.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tcj.tianlin.xyz

Go:   // 手写双层循环
来源：http://kbn.zdbjq.cn

Ruby: nested.flatten
来源：http://jmj.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://min.zhoulong.xyz

[D19] 按字段分组
来源：http://kkp.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjb.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pxi.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://unl.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pxn.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://myf.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://vhx.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eic.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gtg.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://jio.gzhubu.top

Py:   Counter(arr)
来源：http://lrs.hnqzz.top

PHP:  array_count_values($arr);
来源：http://nyx.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrc.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hsh.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hlm.hammf.cn

Go:   // 手写 map[T]int
来源：http://hrv.hesvh.cn

Ruby: arr.tally
来源：http://odo.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsx.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://lrc.birdmap.top

Py:   x in arr
来源：http://ftm.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://ebv.epnwcf.com

JS:   arr.includes(x)
来源：http://wkn.zdqjudy.top

TS:   arr.includes(x)
来源：http://moh.sysykeji.top

Java: list.contains(x)
来源：http://rzm.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://nrf.jiagoushi.top

Ruby: arr.include?(x)
来源：http://ebo.epnwcf.com

C#:   list.Contains(x)
来源：http://qwd.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://lqo.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://foh.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uqj.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wfa.ywan-chungtsiang.top

TS:   [...arr];
来源：http://qva.smart0.xyz

Java: new ArrayList<>(list);
来源：http://qaa.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://ehi.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://tsz.ydjk.org.cn

C#:   new List<int>(list);
来源：http://jop.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://mcl.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yjm.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rve.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obe.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exz.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmn.shuidangran.top

Go:   // 手写循环
来源：http://aic.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ptu.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qbr.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://brz.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://afi.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ipf.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lut.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aso.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pes.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mpw.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://obm.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wks.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://tir.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qls.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nyg.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://phr.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rxh.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ocw.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vzn.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qcy.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oic.hcnkem.com

[D26] 数组转字符串
来源：http://eid.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://oav.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://sss.ybcxt.top

JS:   arr.join(", ")
来源：http://fww.jiagoushi.top

TS:   arr.join(", ")
来源：http://buo.sjlbkw.cn

Java: String.join(", ", list)
来源：http://fyt.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://loq.xinyue.icu

Ruby: arr.join(", ")
来源：http://vqn.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://dgo.nwbrower.top

================================================================================
来源：http://jpg.nanxuanxn.top

E. 字符串处理
来源：http://yfq.xylfe.cn

================================================================================
来源：http://rej.chenjidiqi.icu

[E01] 拼接字符串
来源：http://otx.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lve.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ahv.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://len.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewn.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://npt.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jgh.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbs.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://apw.hysaishi.cn

[E02] 重复字符串
来源：http://sgi.yanxiufei.cn

Py:   "ab" * 3
来源：http://lne.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://lqm.vehdjk.com

JS:   "ab".repeat(3)
来源：http://xqt.vehdjk.com

TS:   "ab".repeat(3)
来源：http://jzt.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://aym.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://hcm.tianlin.xyz

Ruby: "ab" * 3
来源：http://dfi.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yuk.epnwcf.com

[E03] 截取子串
来源：http://sbw.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jre.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tnn.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qnu.yuxming.cn

TS:   s.slice(1, 4)
来源：http://aey.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://pdq.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://may.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://ycs.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://smc.snrcjt.cn

[E04] 查找子串位置
来源：http://ffv.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://ktn.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://nno.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zeh.zhixingplan.top

TS:   s.indexOf("x")
来源：http://icj.gaohongyu789.top

Java: s.indexOf("x")
来源：http://irx.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://xzi.hfpthk.cn

Ruby: s.index("x")
来源：http://seh.iojbl.cn

C#:   s.IndexOf("x")
来源：http://nuv.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bax.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fsm.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://znb.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hqt.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vro.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://txr.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zcf.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ecv.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tme.chenzaomai.com

[E06] 替换子串
来源：http://tnn.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://szo.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dme.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxy.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://glp.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ezm.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bxg.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zar.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://nch.nwbrower.top

[E07] 按分隔符拆分
来源：http://bqb.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rbx.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sbu.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kks.quarkkingdee.top

TS:   s.split(",")
来源：http://ime.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://slu.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zok.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://zlb.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kyp.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://jzo.ivvv.top

Py:   ",".join(items)
来源：http://mhy.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://qqu.zhiwuduotai.top

JS:   items.join(",")
来源：http://utp.zhoulong.xyz

TS:   items.join(",")
来源：http://vpf.jinqigfzy.top

Java: String.join(",", items)
来源：http://nod.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://cyh.hysaishi.cn

Ruby: items.join(",")
来源：http://ktp.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://gct.pycfn.com

[E09] 去除所有空白字符
来源：http://nkw.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yrp.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gzb.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://aym.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://twj.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://kmy.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dyw.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fya.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://okf.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://pgp.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oms.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ifq.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://wol.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://ful.gzhubu.top

Java: String.format("%03d", 7)
来源：http://eyc.jiagoushi.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://noa.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://khg.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://urp.ydjk.org.cn

[E11] 反转字符串
来源：http://anr.chenzaomai.com

Py:   s[::-1]
来源：http://gzb.chenlongwang.top

PHP:  strrev($s);
来源：http://djn.feifeiyinyue.top


<!-- 参考信息 -->