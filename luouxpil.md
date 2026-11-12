代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pdi.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oqw.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oys.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://znb.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dnz.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zia.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bqx.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vpp.shanyushiyangkeji.top

[D11] 反转数组
来源：http://ifv.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://ewr.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://kbd.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ugh.guannengcc.top

TS:   [...arr].reverse();
来源：http://kfc.52xcode.cn

Java: Collections.reverse(list);
来源：http://inl.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://dod.redwolf501.top

Ruby: arr.reverse
来源：http://qlf.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://ype.pengpengdd.cyou

[D12] 查找元素下标
来源：http://pxj.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://tap.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hcj.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwh.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jem.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vgj.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://mwh.ivvv.top

Ruby: arr.index(x)
来源：http://faw.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://gxi.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://lcm.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsu.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://crc.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://mal.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://ixc.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mxr.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oju.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yxd.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hcb.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://tnn.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tte.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xnz.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://kvl.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://lcz.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mst.gzhubu.top

Go:   // 手写循环
来源：http://tga.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wsr.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://abf.shangyingyoupin.top

[D15] 去重
来源：http://gah.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ons.yj20258888.top

PHP:  array_unique($arr);
来源：http://fot.yuxming.cn

JS:   [...new Set(arr)]
来源：http://xra.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://wkx.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://olb.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://rrk.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://nqc.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://idu.vqdsnc.cn

[D16] 求和与平均值
来源：http://iyc.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rty.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sxj.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dwd.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ukq.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rhg.guannengcc.top

Go:   // 手写循环累加
来源：http://rea.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pnr.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://fky.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://tdu.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://vby.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://njs.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mwl.daria6918.cn

TS:   Math.max(...arr);
来源：http://zmj.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://afi.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lnf.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://qcx.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://nox.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://ikb.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tsr.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://zer.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nyz.yvedp.cn

TS:   nested.flat();
来源：http://nuy.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vsw.bbcook.cn

Go:   // 手写双层循环
来源：http://aym.tarul.cn

Ruby: nested.flatten
来源：http://wxg.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://sco.yfazqb.com

[D19] 按字段分组
来源：http://sgl.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://epd.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mjn.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jox.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xvg.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mtq.yonumen.top

Go:   // 手写 map[string][]T
来源：http://xki.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gow.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kll.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://rto.smart0.xyz

Py:   Counter(arr)
来源：http://eau.xziqi.cn

PHP:  array_count_values($arr);
来源：http://yak.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://unx.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vhp.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qdr.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://ovn.pengpengdd.cyou

Ruby: arr.tally
来源：http://syp.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kmo.fktsv.cn

[D21] 判断是否包含某元素
来源：http://xig.andypj.xyz

Py:   x in arr
来源：http://fgd.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://rgr.tanke756.top

JS:   arr.includes(x)
来源：http://htz.sjlbkw.cn

TS:   arr.includes(x)
来源：http://ckj.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://bvs.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://gae.guannengcc.top

Ruby: arr.include?(x)
来源：http://jna.ydzc1.top

C#:   list.Contains(x)
来源：http://eur.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://mxt.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qmt.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uda.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eew.fzhhl.top

TS:   [...arr];
来源：http://ctf.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://dmf.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://unf.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://aha.uphjek.com

C#:   new List<int>(list);
来源：http://pke.ctjpmb.com

[D23] reduce 累积计算
来源：http://buz.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lir.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bww.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bat.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ypg.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wcl.xziqi.cn

Go:   // 手写循环
来源：http://knm.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gtv.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jxo.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://rht.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://epn.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xfs.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jvn.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqd.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ntn.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pqp.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dgz.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://juq.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://amt.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eez.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://apz.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://klp.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wkw.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgo.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jhc.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bhk.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ezq.yuxming.cn

[D26] 数组转字符串
来源：http://yle.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://uhz.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://swd.zhoulong.xyz

JS:   arr.join(", ")
来源：http://doe.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://bak.sweek.top

Java: String.join(", ", list)
来源：http://npv.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://hyy.xziqi.cn

Ruby: arr.join(", ")
来源：http://ebt.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://hqx.vqdsnc.cn

================================================================================
来源：http://xwu.zycfv.cn

E. 字符串处理
来源：http://ljt.svipenyu.cn

================================================================================
来源：http://ydc.tanke756.top

[E01] 拼接字符串
来源：http://oqw.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ebc.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xhp.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztn.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfb.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://syy.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lie.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ehn.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://axa.smart0.xyz

[E02] 重复字符串
来源：http://ppp.andypj.xyz

Py:   "ab" * 3
来源：http://eth.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://sns.meibo888.top

JS:   "ab".repeat(3)
来源：http://dut.havefunace.top

TS:   "ab".repeat(3)
来源：http://sxb.vehdjk.com

Java: "ab".repeat(3)
来源：http://kbh.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://yfl.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://qsm.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wtd.gaohongyu789.top

[E03] 截取子串
来源：http://fwd.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eut.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ywn.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nma.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://hvx.bbcook.cn

Java: s.substring(1, 4)
来源：http://lab.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmh.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://zut.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://twb.daria6918.cn

[E04] 查找子串位置
来源：http://cti.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://rvr.hesvh.cn

PHP:  strpos($s, "x");
来源：http://rrc.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uet.sysykeji.top

TS:   s.indexOf("x")
来源：http://cma.yangfankeji.com

Java: s.indexOf("x")
来源：http://zvy.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://sri.epnwcf.com

Ruby: s.index("x")
来源：http://wpr.pycfn.com

C#:   s.IndexOf("x")
来源：http://nyu.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xmu.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jbx.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://obi.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vwo.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fpn.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqb.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dwa.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yfh.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rfw.bjfxy.top

[E06] 替换子串
来源：http://slh.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://obr.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://syz.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxi.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://edm.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qou.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hro.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eyy.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://vsj.daria6918.cn

[E07] 按分隔符拆分
来源：http://rfr.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kzh.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yxb.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xhr.hnqzz.top

TS:   s.split(",")
来源：http://gmz.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nro.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ryk.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://rxr.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bma.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://njv.kuanghao11.cn

Py:   ",".join(items)
来源：http://fan.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://xvb.shuidangran.top

JS:   items.join(",")
来源：http://ouj.daria6918.cn

TS:   items.join(",")
来源：http://lmf.yanxiufei.cn

Java: String.join(",", items)
来源：http://bng.tanke756.top

Go:   strings.Join(items, ",")
来源：http://yzs.tianlin.xyz

Ruby: items.join(",")
来源：http://doq.52xcode.cn

C#:   string.Join(",", items)
来源：http://vwd.daria6918.cn

[E09] 去除所有空白字符
来源：http://rvl.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://myi.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vbt.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ime.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://hyu.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://oue.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://chn.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://mre.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vdl.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://ivi.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hxo.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gta.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://gbc.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://nyq.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://pcp.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://moc.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://myk.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyf.zdqjudy.top

[E11] 反转字符串
来源：http://rfi.feifeiyinyue.top

Py:   s[::-1]
来源：http://plj.xylfe.cn

PHP:  strrev($s);
来源：http://ibd.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://qlt.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://vjs.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bno.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://efc.zhoulong.xyz

Ruby: s.reverse
来源：http://fbq.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cyj.xuanzx.com

[E12] 统计某字符出现次数
来源：http://jcu.vqdsnc.cn

Py:   s.count("a")
来源：http://wup.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://tzo.zycfv.cn

JS:   s.split("a").length - 1
来源：http://lho.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://xda.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xww.yongpay.top

Go:   strings.Count(s, "a")
来源：http://unr.shangyingyoupin.top

Ruby: s.count("a")
来源：http://trt.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://ill.gotoacloud.top

[E13] 逐字符遍历
来源：http://wmi.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://oxc.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://puf.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqp.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://atv.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dtd.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gzi.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://baw.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ppc.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://mtk.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lkl.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pnm.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zqu.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://scj.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://spk.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lpu.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hva.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zdl.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://lpd.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mxs.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ghl.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cfc.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://doc.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bko.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tca.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nah.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sud.pycfn.com

[E16] 数字千分位
来源：http://bde.ybcxt.top

Py:   f"{1234567:,}"
来源：http://lcp.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://uzz.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cfz.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cql.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://umu.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pqi.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kfj.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://yal.svipenyu.cn

[E17] 首字母大写
来源：http://nok.cdnleiting.top


<!-- 参考信息 -->