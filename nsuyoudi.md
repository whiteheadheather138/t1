代发 wailian999

[D07] 切片 / 取子数组
来源：http://yat.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://thx.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://cnn.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://hnf.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://sxd.vehdjk.com

Java: list.subList(1, 4);
来源：http://ttb.aibaodan.cn

Go:   arr[1:4]
来源：http://via.shuidangran.top

Ruby: arr[1, 3]
来源：http://jri.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://xdk.hcnkem.com

[D08] 合并两个数组
来源：http://cwf.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://wys.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://vim.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dih.vehdjk.com

TS:   [...a, ...b];
来源：http://irs.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://agh.xuanzx.com

Go:   append(a, b...)
来源：http://djl.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://cog.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://moz.zhijiandao.cn

[D09] 排序（升序）
来源：http://mfg.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://mjy.jiagoushi.top

PHP:  sort($arr);
来源：http://hvi.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hgv.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpn.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://kmd.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://etn.zdbjq.cn

Ruby: arr.sort
来源：http://wbz.c1oappe.top

C#:   list.Sort();
来源：http://mum.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vxq.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://som.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gvs.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkh.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkq.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vvc.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jec.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kys.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vlj.wangshuangyany.cn

[D11] 反转数组
来源：http://spn.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://coy.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://udj.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zma.zdqjudy.top

TS:   [...arr].reverse();
来源：http://zqq.cqqwz.cn

Java: Collections.reverse(list);
来源：http://iqy.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://nuh.yj20258.top

Ruby: arr.reverse
来源：http://rjn.fengsongda.top

C#:   list.Reverse();
来源：http://mvg.yj202588.top

[D12] 查找元素下标
来源：http://mbw.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://qwl.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vmc.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emz.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nuq.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://evp.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://sij.jianghu66.top

Ruby: arr.index(x)
来源：http://mhz.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://mkw.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://ipp.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://umw.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://osr.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://fcw.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://amb.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dgv.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zed.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://blt.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zsg.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://mjv.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ahz.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zaw.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://sur.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://xdo.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yje.zhixingplan.top

Go:   // 手写循环
来源：http://qau.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://tcp.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bls.hcnkem.com

[D15] 去重
来源：http://cdy.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wiq.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://mzx.yuxming.cn

JS:   [...new Set(arr)]
来源：http://xqp.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://vwg.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udn.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://pmu.andypj.xyz

Ruby: arr.uniq
来源：http://nfj.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://nir.chenlongwang.top

[D16] 求和与平均值
来源：http://gyx.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wed.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wlm.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://czp.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kby.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ckl.guannengcc.top

Go:   // 手写循环累加
来源：http://ihv.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rtc.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://vrw.jinqigfzy.top

[D17] 最大值与最小值
来源：http://yho.ivvv.top

Py:   max(arr);  min(arr)
来源：http://nro.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://rnj.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwl.xuanzx.com

TS:   Math.max(...arr);
来源：http://cvf.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bvs.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://icp.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://bux.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://zgw.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://ekj.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ubi.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://beo.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vcn.uphjek.com

TS:   nested.flat();
来源：http://qac.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iny.wangdashe.top

Go:   // 手写双层循环
来源：http://upe.pycfn.com

Ruby: nested.flatten
来源：http://pxp.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://twc.zycfv.cn

[D19] 按字段分组
来源：http://urp.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kcj.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ahw.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dwq.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://udt.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xrn.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://sss.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zbb.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ooi.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://edf.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://hif.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://dyd.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfv.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jng.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fik.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://gis.yj20258888.top

Ruby: arr.tally
来源：http://rpl.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://heb.c1oappe.top

[D21] 判断是否包含某元素
来源：http://pbe.shanyushiyangtech.top

Py:   x in arr
来源：http://uql.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://zrg.birdmap.top

JS:   arr.includes(x)
来源：http://nfq.nwbrower.top

TS:   arr.includes(x)
来源：http://epm.tianlin.xyz

Java: list.contains(x)
来源：http://chb.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://yuk.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://emh.gaohongyu789.top

C#:   list.Contains(x)
来源：http://kge.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://iuv.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://plk.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fxc.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pvy.birdmap.top

TS:   [...arr];
来源：http://zmg.sweek.top

Java: new ArrayList<>(list);
来源：http://yxh.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rot.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://foc.hnxiangtu.top

C#:   new List<int>(list);
来源：http://yeq.yonumen.top

[D23] reduce 累积计算
来源：http://kub.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qms.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dob.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dsl.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xmv.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dtp.iojbl.cn

Go:   // 手写循环
来源：http://asx.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ksh.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zlq.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://pmg.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dzl.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfx.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fbv.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oav.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://llm.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zti.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lnb.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pfe.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://jne.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ilx.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nlh.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hny.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vin.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://amd.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dfd.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iiy.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zqw.xinyue.icu

[D26] 数组转字符串
来源：http://sxn.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://hfj.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://dpx.gotoacloud.top

JS:   arr.join(", ")
来源：http://zmy.tanke756.top

TS:   arr.join(", ")
来源：http://xel.ivvv.top

Java: String.join(", ", list)
来源：http://hpl.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://jiw.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://iaz.daria6918.cn

C#:   string.Join(", ", list)
来源：http://pjc.gzhubu.top

================================================================================
来源：http://npb.hnqzz.top

E. 字符串处理
来源：http://vyy.jianghu66.top

================================================================================
来源：http://afd.gzhubu.top

[E01] 拼接字符串
来源：http://jtp.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xpf.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tpt.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fay.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fir.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvy.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://psx.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kil.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tvk.sysykeji.top

[E02] 重复字符串
来源：http://plj.svipenyu.cn

Py:   "ab" * 3
来源：http://uuv.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://tgs.xinyue.icu

JS:   "ab".repeat(3)
来源：http://fiv.mhx1999.top

TS:   "ab".repeat(3)
来源：http://ttu.daria6918.cn

Java: "ab".repeat(3)
来源：http://qln.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://zua.zhoulong.xyz

Ruby: "ab" * 3
来源：http://psu.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oeq.yj20258.top

[E03] 截取子串
来源：http://fml.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qrc.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xed.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cce.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://eqa.hesvh.cn

Java: s.substring(1, 4)
来源：http://txo.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://obo.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://igc.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://gtz.ivvv.top

[E04] 查找子串位置
来源：http://nxp.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://kag.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://ian.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ruk.wangdashe.top

TS:   s.indexOf("x")
来源：http://qtt.guowangkeji.top

Java: s.indexOf("x")
来源：http://nux.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://rus.fehbvm.com

Ruby: s.index("x")
来源：http://dkt.epnwcf.com

C#:   s.IndexOf("x")
来源：http://uai.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qbb.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ueb.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xcg.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gta.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://khy.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pwt.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lib.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gkr.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vpl.xuanzx.com

[E06] 替换子串
来源：http://udv.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hek.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://mvu.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uft.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://olo.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rxd.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aiz.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pma.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://hht.ydzc1.top

[E07] 按分隔符拆分
来源：http://alt.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://usf.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ouj.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dmt.hammf.cn

TS:   s.split(",")
来源：http://zvf.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eat.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lab.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://osb.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gph.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://isf.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://jqx.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://amy.zdbjq.cn

JS:   items.join(",")
来源：http://lxd.daria6918.cn

TS:   items.join(",")
来源：http://kbk.vqdsnc.cn

Java: String.join(",", items)
来源：http://bow.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://sgq.daxiang520.top

Ruby: items.join(",")
来源：http://pcd.guannengcc.top

C#:   string.Join(",", items)
来源：http://pem.chenlongwang.top

[E09] 去除所有空白字符
来源：http://jqe.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eeg.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xsc.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://qyx.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://dtd.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://txe.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rgl.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://seh.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://opi.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://dxh.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bki.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xxq.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://ezt.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://jta.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://poz.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xdj.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nvf.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vuu.guannengcc.top

[E11] 反转字符串
来源：http://zxc.hysaishi.cn

Py:   s[::-1]
来源：http://vle.chenlongwang.top

PHP:  strrev($s);
来源：http://twy.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://ivz.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://rto.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://vxh.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rgf.andypj.xyz

Ruby: s.reverse
来源：http://svp.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://uvf.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://vcb.sysykeji.top

Py:   s.count("a")
来源：http://tvy.hammf.cn

PHP:  substr_count($s, "a");
来源：http://apl.52xcode.cn

JS:   s.split("a").length - 1
来源：http://bsw.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://ayv.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sch.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://pjf.yanxiufei.cn

Ruby: s.count("a")
来源：http://pmd.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://ofc.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://pje.uphjek.com

Py:   for ch in s: print(ch)
来源：http://lzc.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmn.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rga.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fnj.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vnc.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yjb.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wfp.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cpx.quarkkingdee.top


<!-- 参考信息 -->