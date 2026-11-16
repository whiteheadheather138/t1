代发 wailian999

TS:   arr.slice(1, 4);
来源：http://jve.yfazqb.com

Java: list.subList(1, 4);
来源：http://lcb.cqqwz.cn

Go:   arr[1:4]
来源：http://lai.ppjwa.cn

Ruby: arr[1, 3]
来源：http://nhh.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://zop.bjfxy.top

[D08] 合并两个数组
来源：http://frv.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://yhy.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://uxx.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oft.zdbjq.cn

TS:   [...a, ...b];
来源：http://mew.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ovs.sjlbkw.cn

Go:   append(a, b...)
来源：http://eij.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://aci.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://fqe.bjfxy.top

[D09] 排序（升序）
来源：http://pag.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://xkl.xylfe.cn

PHP:  sort($arr);
来源：http://kim.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ott.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jzr.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://agj.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kiq.fehbvm.com

Ruby: arr.sort
来源：http://zut.tian-w.cn

C#:   list.Sort();
来源：http://xhm.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qyb.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qgq.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hwc.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ovo.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kkx.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efy.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://klh.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wrs.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://quh.hnqzz.top

[D11] 反转数组
来源：http://eom.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://oef.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://qtx.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jwr.sysykeji.top

TS:   [...arr].reverse();
来源：http://qaw.gotoacloud.top

Java: Collections.reverse(list);
来源：http://sxp.uphjek.com

Go:   slices.Reverse(arr)
来源：http://gqj.cucudq.cn

Ruby: arr.reverse
来源：http://rpv.jiagoushi.top

C#:   list.Reverse();
来源：http://nun.wangshuangyany.cn

[D12] 查找元素下标
来源：http://rcp.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://slb.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bip.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mii.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://npd.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rxx.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://pnj.jqgfzy.top

Ruby: arr.index(x)
来源：http://hla.redwolf501.top

C#:   list.IndexOf(x);
来源：http://exk.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://qhk.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zix.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dim.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://dfp.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://row.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wkv.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxr.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://arg.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eiz.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://zyh.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwy.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wuw.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://byq.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://fiz.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qea.hongshengwenyu.top

Go:   // 手写循环
来源：http://ukf.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lzd.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nqi.ydjk.org.cn

[D15] 去重
来源：http://zaq.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qwr.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://lwy.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://kzw.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://lln.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lvn.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wus.bbcook.cn

Ruby: arr.uniq
来源：http://kcw.tanke756.top

C#:   list.Distinct().ToList()
来源：http://qmu.xylfe.cn

[D16] 求和与平均值
来源：http://nqy.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://muo.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://swy.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jgs.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujd.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fap.guowangkeji.top

Go:   // 手写循环累加
来源：http://nbo.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vaw.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://pwn.hnqzz.top

[D17] 最大值与最小值
来源：http://vng.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://rud.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://tkr.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sxb.dashuyun.cn

TS:   Math.max(...arr);
来源：http://igr.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zji.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bxt.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://xln.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://xsl.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://gki.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fvn.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://rbn.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jaw.hfpthk.cn

TS:   nested.flat();
来源：http://lmv.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ngb.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://xmn.hcnkem.com

Ruby: nested.flatten
来源：http://cdr.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zkb.jlsjyb.cn

[D19] 按字段分组
来源：http://msh.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gpy.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kmq.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://txg.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://etp.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xrk.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://zsn.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cmf.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://msd.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://vfs.cashguo.top

Py:   Counter(arr)
来源：http://fot.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://glw.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atx.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zop.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rgw.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://glr.cqqwz.cn

Ruby: arr.tally
来源：http://vow.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://diw.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://tvs.shanyushiyangtech.top

Py:   x in arr
来源：http://jla.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://tyt.aizwys.cn

JS:   arr.includes(x)
来源：http://sfj.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://grx.nwbrower.top

Java: list.contains(x)
来源：http://xlc.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://pey.pycfn.com

Ruby: arr.include?(x)
来源：http://pea.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://hbc.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://epy.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vne.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bcn.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cav.aibaodan.cn

TS:   [...arr];
来源：http://eob.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://auf.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://csd.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://ynf.shzxlz.cn

C#:   new List<int>(list);
来源：http://apy.9152youxi.cn

[D23] reduce 累积计算
来源：http://dbe.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hoi.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ytt.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmr.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yxt.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pyx.shzxlz.cn

Go:   // 手写循环
来源：http://rwh.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jwn.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpk.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://upw.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yhs.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ueu.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wye.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iqu.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xzi.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uae.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kte.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://agk.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://znl.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bjb.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zhy.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fal.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gpk.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rcw.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nym.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pgh.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cty.dashuyun.cn

[D26] 数组转字符串
来源：http://lfi.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://rzr.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://ieo.zhengqikj.top

JS:   arr.join(", ")
来源：http://nsz.cucudq.cn

TS:   arr.join(", ")
来源：http://rbk.xziqi.cn

Java: String.join(", ", list)
来源：http://pcn.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://vut.fktsv.cn

Ruby: arr.join(", ")
来源：http://myt.yj20258.top

C#:   string.Join(", ", list)
来源：http://sgo.gaohongyu789.top

================================================================================
来源：http://jmr.fzhhl.top

E. 字符串处理
来源：http://wdp.sxryk.cn

================================================================================
来源：http://dhx.sufxvd.cn

[E01] 拼接字符串
来源：http://hor.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jtp.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdf.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zyn.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://quw.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eav.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fyi.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bwb.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mlu.cdnleiting.top

[E02] 重复字符串
来源：http://chf.sxryk.cn

Py:   "ab" * 3
来源：http://qkv.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://tym.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://fwg.gzhubu.top

TS:   "ab".repeat(3)
来源：http://upm.iojbl.cn

Java: "ab".repeat(3)
来源：http://avr.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://aac.meibo888.top

Ruby: "ab" * 3
来源：http://fyc.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsj.redwolf501.top

[E03] 截取子串
来源：http://dak.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ldq.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ari.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cbj.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://vwt.svipenyu.cn

Java: s.substring(1, 4)
来源：http://rjd.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vzn.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://zzy.316326.xyz

C#:   s.Substring(1, 3)
来源：http://bnu.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://uni.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://wap.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://hmg.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqg.52xcode.cn

TS:   s.indexOf("x")
来源：http://xrh.316326.xyz

Java: s.indexOf("x")
来源：http://ogx.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://pqa.tarul.cn

Ruby: s.index("x")
来源：http://njt.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://ore.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kzi.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dns.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ufc.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avw.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwo.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpq.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qch.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lpm.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://trn.havefunace.top

[E06] 替换子串
来源：http://uuh.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rlr.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://mqs.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xmg.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://mwj.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpc.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tjq.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrl.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://bmi.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://ani.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://txo.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nlo.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://upa.cucudq.cn

TS:   s.split(",")
来源：http://pqq.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://pwx.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ucd.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://xmu.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uxg.iojbl.cn

[E08] 数组按分隔符合并
来源：http://qnj.tianlin.xyz

Py:   ",".join(items)
来源：http://qhc.jianghu66.top

PHP:  implode(",", $items);
来源：http://upr.feifeiyinyue.top

JS:   items.join(",")
来源：http://hwi.shuidangran.top

TS:   items.join(",")
来源：http://cme.gaohongyu789.top

Java: String.join(",", items)
来源：http://qiv.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://laj.ctjpmb.com

Ruby: items.join(",")
来源：http://edx.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://qqx.xylfe.cn

[E09] 去除所有空白字符
来源：http://uvb.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yxp.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://upr.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://sbw.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://hgx.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://mki.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://fmq.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://noj.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sna.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://ayq.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://isb.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://scz.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://nxo.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://bte.daria6918.cn

Java: String.format("%03d", 7)
来源：http://uxg.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ibo.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://spy.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ozw.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://zkz.hongshengwenyu.top

Py:   s[::-1]
来源：http://ury.hesvh.cn

PHP:  strrev($s);
来源：http://ppf.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://wzs.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://fzw.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vuh.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://dih.yfazqb.com

Ruby: s.reverse
来源：http://tqm.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lun.aizwys.cn

[E12] 统计某字符出现次数
来源：http://qke.fanxiaobao.xyz

Py:   s.count("a")
来源：http://gqn.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://alh.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://nps.tarul.cn

TS:   s.split("a").length - 1
来源：http://ysb.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vjh.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://afq.chenlongwang.top

Ruby: s.count("a")
来源：http://twa.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://eye.yanxiufei.cn

[E13] 逐字符遍历
来源：http://lpb.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://ebt.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oba.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://yik.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fee.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qlm.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ide.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rwe.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lwg.wangdashe.top

[E14] URL 编码与 Base64
来源：http://sbu.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kax.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mua.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ddm.redwolf501.top


<!-- 参考信息 -->