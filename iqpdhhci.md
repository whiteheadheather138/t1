代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://wib.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://wuv.feifeiyinyue.top

[D09] 排序（升序）
来源：http://ngc.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://sff.jlsjyb.cn

PHP:  sort($arr);
来源：http://bql.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jzh.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ghw.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oto.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cvh.tarul.cn

Ruby: arr.sort
来源：http://jkm.vehdjk.com

C#:   list.Sort();
来源：http://nbm.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hlb.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ckw.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gki.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pbc.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgd.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvl.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://khq.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jdo.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yld.xuanzx.com

[D11] 反转数组
来源：http://kfl.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://awf.zycfv.cn

PHP:  array_reverse($arr);
来源：http://hcm.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://syv.fengsongda.top

TS:   [...arr].reverse();
来源：http://ndf.tanke756.top

Java: Collections.reverse(list);
来源：http://spg.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://xhl.yongpay.top

Ruby: arr.reverse
来源：http://kuj.ctjpmb.com

C#:   list.Reverse();
来源：http://ryi.gaohongyu789.top

[D12] 查找元素下标
来源：http://dsw.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://vwg.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://srf.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogh.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gpt.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jjn.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://kte.hammf.cn

Ruby: arr.index(x)
来源：http://vlm.xziqi.cn

C#:   list.IndexOf(x);
来源：http://xmo.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://lfi.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://erv.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://csw.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://xhx.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://twt.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://req.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jla.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://bqu.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yua.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://ijt.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mtj.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ert.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://cqq.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://lmn.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ovt.daria6918.cn

Go:   // 手写循环
来源：http://xfj.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://mke.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gkv.chenjidiqi.icu

[D15] 去重
来源：http://pls.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://edg.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://nvp.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://imk.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://bto.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://htb.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://piy.cdnleiting.top

Ruby: arr.uniq
来源：http://rxy.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://pxu.uphjek.com

[D16] 求和与平均值
来源：http://xpn.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nmf.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xgg.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cmi.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qaa.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://meo.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://dbd.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qts.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://dzs.tian-w.cn

[D17] 最大值与最小值
来源：http://dtw.ivvv.top

Py:   max(arr);  min(arr)
来源：http://erd.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://wha.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wno.chenzaomai.com

TS:   Math.max(...arr);
来源：http://gjs.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kbw.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mmf.hammf.cn

Ruby: arr.max;  arr.min
来源：http://cjn.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://qhi.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://zco.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kli.meibo888.top

PHP:  array_merge(...$nested);
来源：http://knl.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qpy.sysykeji.top

TS:   nested.flat();
来源：http://rxn.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yuu.ppjwa.cn

Go:   // 手写双层循环
来源：http://rqq.chenjidiqi.icu

Ruby: nested.flatten
来源：http://grk.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dvx.gzhubu.top

[D19] 按字段分组
来源：http://klz.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tht.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vgi.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lmf.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lig.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ljw.tanke756.top

Go:   // 手写 map[string][]T
来源：http://ifo.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://smz.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sth.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://izu.zycfv.cn

Py:   Counter(arr)
来源：http://qnl.ivvv.top

PHP:  array_count_values($arr);
来源：http://epr.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzx.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zpq.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lyy.mhx1999.top

Go:   // 手写 map[T]int
来源：http://aea.zdbjq.cn

Ruby: arr.tally
来源：http://zcz.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vkz.hesvh.cn

[D21] 判断是否包含某元素
来源：http://kgt.jianghu66.top

Py:   x in arr
来源：http://uks.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://hgr.epnwcf.com

JS:   arr.includes(x)
来源：http://bem.sufxvd.cn

TS:   arr.includes(x)
来源：http://ikf.hywenlv.cn

Java: list.contains(x)
来源：http://ozp.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://hyl.cashguo.top

Ruby: arr.include?(x)
来源：http://lqd.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://sbd.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://hlo.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kdr.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jwn.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bgh.birdmap.top

TS:   [...arr];
来源：http://rra.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://wus.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://sqr.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://hey.xziqi.cn

C#:   new List<int>(list);
来源：http://osf.epnwcf.com

[D23] reduce 累积计算
来源：http://ddm.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qqu.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnc.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nql.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mlv.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ahq.ctjpmb.com

Go:   // 手写循环
来源：http://syh.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfk.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jjo.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://mfh.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://usf.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kqj.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qit.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jdb.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ttq.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ztc.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fip.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://poq.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://bky.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xrw.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cre.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://efr.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rli.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://omq.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zce.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://exr.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fxh.epnwcf.com

[D26] 数组转字符串
来源：http://kwk.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://gzs.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://sdn.yfazqb.com

JS:   arr.join(", ")
来源：http://ikp.zhijiandao.cn

TS:   arr.join(", ")
来源：http://oog.yj20258.top

Java: String.join(", ", list)
来源：http://adn.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://rhz.cashguo.top

Ruby: arr.join(", ")
来源：http://jgo.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://isg.xinyue.icu

================================================================================
来源：http://rit.quarkkingdee.top

E. 字符串处理
来源：http://zhs.shuidangran.top

================================================================================
来源：http://bmg.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://kfr.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eue.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://syv.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdi.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://azv.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bcm.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eqf.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ktw.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nbe.nwbrower.top

[E02] 重复字符串
来源：http://omj.hysaishi.cn

Py:   "ab" * 3
来源：http://yov.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://ukt.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://xuo.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://hyb.guowangkeji.top

Java: "ab".repeat(3)
来源：http://nyq.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://udp.zdbjq.cn

Ruby: "ab" * 3
来源：http://nhx.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hiy.iojbl.cn

[E03] 截取子串
来源：http://cri.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://klz.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwc.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ngq.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://qfn.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://vxv.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmi.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vam.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://ryh.zycfv.cn

[E04] 查找子串位置
来源：http://wgj.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://klf.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://sqz.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ydv.ybcxt.top

TS:   s.indexOf("x")
来源：http://nry.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://edk.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://ulq.hesvh.cn

Ruby: s.index("x")
来源：http://bjj.fzhhl.top

C#:   s.IndexOf("x")
来源：http://pmr.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tlx.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hpu.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xny.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npr.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bpr.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zje.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pmx.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jul.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tcn.zhixingplan.top

[E06] 替换子串
来源：http://zed.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tkf.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://kej.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pvr.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://sfb.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbp.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ffa.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ctg.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://aex.meibo888.top

[E07] 按分隔符拆分
来源：http://hyg.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kjl.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xxo.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://owb.nwbrower.top

TS:   s.split(",")
来源：http://wuw.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://uox.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cwb.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://bgb.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gcu.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://ilx.gotoacloud.top

Py:   ",".join(items)
来源：http://ubx.wangdashe.top

PHP:  implode(",", $items);
来源：http://cqz.jinqigfzy.top

JS:   items.join(",")
来源：http://utx.316326.xyz

TS:   items.join(",")
来源：http://vre.316326.xyz

Java: String.join(",", items)
来源：http://vfa.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://vtj.dashuyun.cn

Ruby: items.join(",")
来源：http://kbr.iojbl.cn

C#:   string.Join(",", items)
来源：http://zih.havefunace.top

[E09] 去除所有空白字符
来源：http://xyu.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jkt.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qon.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://kjd.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://ndc.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://gcz.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uzb.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://mwq.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://chb.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://xhv.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ehw.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xjl.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://ghn.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://twy.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://ulc.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wfb.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kgz.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zbd.shangyingyoupin.top

[E11] 反转字符串
来源：http://ogf.gaohongyu789.top

Py:   s[::-1]
来源：http://lms.zhongyouzk.top

PHP:  strrev($s);
来源：http://ajh.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://afm.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://sop.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ohs.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gja.cashguo.top

Ruby: s.reverse
来源：http://qok.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hsx.vehdjk.com

[E12] 统计某字符出现次数
来源：http://mdo.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://dzk.pycfn.com

PHP:  substr_count($s, "a");
来源：http://soz.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://xzy.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://gpl.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sjv.cashguo.top

Go:   strings.Count(s, "a")
来源：http://enw.fzhhl.top

Ruby: s.count("a")
来源：http://huy.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://lnx.zdbjq.cn

[E13] 逐字符遍历
来源：http://olu.meibo888.top

Py:   for ch in s: print(ch)
来源：http://pqn.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nfo.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iar.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://stf.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cfb.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mzt.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mro.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://abg.guannengcc.top

[E14] URL 编码与 Base64
来源：http://kla.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://enh.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gil.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jwf.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cpt.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wqk.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://roj.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ckr.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ilm.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://sgp.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gmv.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sah.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wxc.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ydq.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fdo.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cve.dashuyun.cn


<!-- 参考信息 -->