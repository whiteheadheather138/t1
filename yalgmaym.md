代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://tit.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://voh.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://glz.cucudq.cn

[D06] 数组长度
来源：http://dre.nanxuanxn.top

Py:   len(arr)
来源：http://reu.cqqwz.cn

PHP:  count($arr);
来源：http://vxt.redwolf501.top

JS:   arr.length
来源：http://pyr.sufxvd.cn

TS:   arr.length
来源：http://ojw.jinyuanbaomall.cn

Java: list.size();
来源：http://gdv.haohaochexian.top

Go:   len(arr)
来源：http://ovs.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://gvc.jianghu66.top

C#:   list.Count;
来源：http://cgh.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://ojl.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://okq.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://aic.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://ewt.yonumen.top

TS:   arr.slice(1, 4);
来源：http://hzr.dashuyun.cn

Java: list.subList(1, 4);
来源：http://smn.ybcxt.top

Go:   arr[1:4]
来源：http://mab.redwolf501.top

Ruby: arr[1, 3]
来源：http://jrp.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://wnf.sysykeji.top

[D08] 合并两个数组
来源：http://ups.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://xmi.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://tgd.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ded.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://xml.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oyc.snrcjt.cn

Go:   append(a, b...)
来源：http://toa.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://rsx.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://rze.hesvh.cn

[D09] 排序（升序）
来源：http://uzj.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://qgu.haohaochexian.top

PHP:  sort($arr);
来源：http://tky.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nul.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oex.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wld.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://muy.yuanzhike.top

Ruby: arr.sort
来源：http://bcg.jqgufenzy.top

C#:   list.Sort();
来源：http://tob.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ehb.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cbo.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ioz.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yvk.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vhj.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fmj.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xqp.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pqg.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nzf.nanxinkj.top

[D11] 反转数组
来源：http://lsr.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tpy.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://xzn.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cek.cdnleiting.top

TS:   [...arr].reverse();
来源：http://mki.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://xzm.yj20258.top

Go:   slices.Reverse(arr)
来源：http://cjr.zhijiandao.cn

Ruby: arr.reverse
来源：http://hdb.zhiwuduotai.top

C#:   list.Reverse();
来源：http://tds.chenjidiqi.icu

[D12] 查找元素下标
来源：http://mbm.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://hpj.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dbv.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zxy.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gre.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://twe.yonumen.top

Go:   slices.Index(arr, x)
来源：http://aix.0kj1m.cn

Ruby: arr.index(x)
来源：http://iud.yueranfly.top

C#:   list.IndexOf(x);
来源：http://lxd.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://qmy.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mbr.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nsz.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://hzv.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://pyi.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djm.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ild.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pma.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ihq.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://yjs.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qvh.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://acb.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://gfr.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://urp.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bya.fktsv.cn

Go:   // 手写循环
来源：http://ide.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://aih.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qzb.wangdashe.top

[D15] 去重
来源：http://xsr.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ope.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://eaq.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://jrm.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://zli.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jud.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://kwt.hysaishi.cn

Ruby: arr.uniq
来源：http://ftn.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://xgw.bjfxy.top

[D16] 求和与平均值
来源：http://vsl.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gmr.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uly.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajy.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjf.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rvs.daxiang520.top

Go:   // 手写循环累加
来源：http://xft.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rqv.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://vpb.shuidangran.top

[D17] 最大值与最小值
来源：http://lmc.sweek.top

Py:   max(arr);  min(arr)
来源：http://izs.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://yny.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://set.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://cyc.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nag.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exg.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://tdm.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://eon.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://okt.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zdi.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://fag.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eai.wangdashe.top

TS:   nested.flat();
来源：http://nem.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qnm.ctjpmb.com

Go:   // 手写双层循环
来源：http://yfe.cqqwz.cn

Ruby: nested.flatten
来源：http://iyy.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cty.jianghu66.top

[D19] 按字段分组
来源：http://iuc.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aae.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zje.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://phd.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://nff.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oej.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://bom.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vph.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mvh.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://lpn.zhoulong.xyz

Py:   Counter(arr)
来源：http://hzf.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://nab.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lry.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://phy.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kao.andypj.xyz

Go:   // 手写 map[T]int
来源：http://ioe.0kj1m.cn

Ruby: arr.tally
来源：http://lgl.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hlp.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://koq.yuxming.cn

Py:   x in arr
来源：http://vmm.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://mio.zhongyouzk.top

JS:   arr.includes(x)
来源：http://xfn.9152youxi.cn

TS:   arr.includes(x)
来源：http://amo.yueranfly.top

Java: list.contains(x)
来源：http://ttx.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://qij.meibo888.top

Ruby: arr.include?(x)
来源：http://hrc.vqdsnc.cn

C#:   list.Contains(x)
来源：http://ykc.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://cia.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jir.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jsz.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kwx.daria6918.cn

TS:   [...arr];
来源：http://imo.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://cgh.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://rjj.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://wgt.yvedp.cn

C#:   new List<int>(list);
来源：http://gsh.cqqwz.cn

[D23] reduce 累积计算
来源：http://ubc.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kyo.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wgz.zhiwuduotai.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qnv.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rme.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqz.mhx1999.top

Go:   // 手写循环
来源：http://vfz.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ufi.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hch.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://axv.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dgk.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kpv.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://esj.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kpb.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://paj.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwe.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gek.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ssz.ivvv.top

[D25] Set 集合去重与交并差
来源：http://brm.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zxi.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gzj.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fqn.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nax.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zwy.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bwu.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wcn.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zdw.wangshuangyany.cn

[D26] 数组转字符串
来源：http://wkr.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://auz.tarul.cn

PHP:  implode(", ", $arr);
来源：http://pdr.xinyue.icu

JS:   arr.join(", ")
来源：http://rww.hesvh.cn

TS:   arr.join(", ")
来源：http://dau.uphjek.com

Java: String.join(", ", list)
来源：http://lcn.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://ypn.dashuyun.cn

Ruby: arr.join(", ")
来源：http://afz.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://vbu.vehdjk.com

================================================================================
来源：http://yrs.ydzc1.top

E. 字符串处理
来源：http://rgy.zhijiandao.cn

================================================================================
来源：http://dke.9152youxi.cn

[E01] 拼接字符串
来源：http://kft.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://con.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdr.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jmo.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kbt.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fwq.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ngl.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hqm.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rlr.yj202588.top

[E02] 重复字符串
来源：http://mnw.jinqigfzy.top

Py:   "ab" * 3
来源：http://qsw.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://qlv.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ohj.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://wxd.316326.xyz

Java: "ab".repeat(3)
来源：http://uve.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://dqs.hammf.cn

Ruby: "ab" * 3
来源：http://nui.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgc.shangyingyoupin.top

[E03] 截取子串
来源：http://bya.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wsc.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jie.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ntr.tanke756.top

TS:   s.slice(1, 4)
来源：http://tqv.meibo888.top

Java: s.substring(1, 4)
来源：http://jlv.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vaj.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://ody.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://pix.sxryk.cn

[E04] 查找子串位置
来源：http://eye.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://fad.yj202588.top

PHP:  strpos($s, "x");
来源：http://hrl.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ehr.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://vew.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://pzr.ivvv.top

Go:   strings.Index(s, "x")
来源：http://sdt.tanke756.top

Ruby: s.index("x")
来源：http://cvp.iojbl.cn

C#:   s.IndexOf("x")
来源：http://ydg.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://heb.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qqz.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sdw.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zho.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ypt.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcb.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://koj.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uax.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xim.pengpengdd.cyou

[E06] 替换子串
来源：http://dsk.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pcs.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://tdq.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjv.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://edf.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrf.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rnc.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://exj.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://tte.iojbl.cn

[E07] 按分隔符拆分
来源：http://clv.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wyl.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qyb.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://var.kuanghao11.cn

TS:   s.split(",")
来源：http://oni.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gqe.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://frs.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://ntq.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmy.ivvv.top

[E08] 数组按分隔符合并
来源：http://ckv.yongpay.top

Py:   ",".join(items)
来源：http://uud.birdmap.top

PHP:  implode(",", $items);
来源：http://ywq.dianchejie.cn

JS:   items.join(",")
来源：http://gmu.sxryk.cn

TS:   items.join(",")
来源：http://bhw.tianlin.xyz

Java: String.join(",", items)
来源：http://ctn.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://nun.vehdjk.com

Ruby: items.join(",")
来源：http://yup.aizwys.cn

C#:   string.Join(",", items)
来源：http://dwn.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://duc.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lml.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zpp.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://bpc.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://ugq.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://mry.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fqs.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://aer.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uhz.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://ocw.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://njk.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bjb.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://kii.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://vbh.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://huj.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ewh.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ckm.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dfo.jiagoushi.top

[E11] 反转字符串
来源：http://mjw.pycfn.com

Py:   s[::-1]
来源：http://kyz.birdmap.top

PHP:  strrev($s);
来源：http://mbf.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://hym.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://bbu.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pjk.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cjf.uphjek.com

Ruby: s.reverse
来源：http://tew.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://rxq.daria6918.cn

[E12] 统计某字符出现次数
来源：http://gie.snrcjt.cn

Py:   s.count("a")
来源：http://ubm.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://uhe.epnwcf.com

JS:   s.split("a").length - 1
来源：http://cil.guannengcc.top

TS:   s.split("a").length - 1
来源：http://qnt.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lpl.yfazqb.com


<!-- 参考信息 -->