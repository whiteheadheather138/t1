代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ybe.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pde.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wzz.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://foa.haohaochexian.top

[D11] 反转数组
来源：http://fzg.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fpw.ybcxt.top

PHP:  array_reverse($arr);
来源：http://xzr.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sug.cucudq.cn

TS:   [...arr].reverse();
来源：http://gkb.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://yfq.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://fgz.xuetiantiany.cn

Ruby: arr.reverse
来源：http://zeu.yfazqb.com

C#:   list.Reverse();
来源：http://vre.cheryme.top

[D12] 查找元素下标
来源：http://gwe.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://kod.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aki.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ojl.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cii.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gac.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://ixa.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://fhp.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://wix.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://wgf.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mww.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qgm.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://aif.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://kxa.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mij.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://twu.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://enm.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://duj.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://byg.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://caz.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tiq.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://ddi.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://rvh.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ffy.daxiang520.top

Go:   // 手写循环
来源：http://izw.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://tnn.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lsh.aizwys.cn

[D15] 去重
来源：http://cmq.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://plz.hysaishi.cn

PHP:  array_unique($arr);
来源：http://gdh.yongpay.top

JS:   [...new Set(arr)]
来源：http://bqd.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://qsf.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fvb.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jte.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://xxr.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://fye.sufxvd.cn

[D16] 求和与平均值
来源：http://rzb.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://orb.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wvy.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iil.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixr.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mvt.tian-w.cn

Go:   // 手写循环累加
来源：http://imp.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ubq.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://pqo.cqqwz.cn

[D17] 最大值与最小值
来源：http://obi.pycfn.com

Py:   max(arr);  min(arr)
来源：http://jup.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://mte.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rin.yfazqb.com

TS:   Math.max(...arr);
来源：http://mqj.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ljh.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://isj.pycfn.com

Ruby: arr.max;  arr.min
来源：http://jxs.yongpay.top

C#:   list.Max();  list.Min()
来源：http://qqz.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://zfm.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dwf.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://wzx.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lid.hammf.cn

TS:   nested.flat();
来源：http://ois.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nrv.xuanzx.com

Go:   // 手写双层循环
来源：http://mze.xinyue.icu

Ruby: nested.flatten
来源：http://gct.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cca.iojbl.cn

[D19] 按字段分组
来源：http://ubv.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ltq.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cwb.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zox.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://yvq.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://khu.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://rdi.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zwl.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iqw.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://gif.yuanzhike.top

Py:   Counter(arr)
来源：http://zyi.uphjek.com

PHP:  array_count_values($arr);
来源：http://kxc.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cdq.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ugc.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bnv.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://guz.uphjek.com

Ruby: arr.tally
来源：http://bol.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zis.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://zyw.cashguo.top

Py:   x in arr
来源：http://dxn.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://iaa.chenzaomai.com

JS:   arr.includes(x)
来源：http://wga.zdbjq.cn

TS:   arr.includes(x)
来源：http://lkd.fehbvm.com

Java: list.contains(x)
来源：http://vqi.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://rgi.bbcook.cn

Ruby: arr.include?(x)
来源：http://gky.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://ubf.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://jul.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qxs.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cks.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wss.xuetiantiany.cn

TS:   [...arr];
来源：http://zjv.tian-w.cn

Java: new ArrayList<>(list);
来源：http://ljx.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://awk.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://dyv.yuanzhike.top

C#:   new List<int>(list);
来源：http://jtt.birdmap.top

[D23] reduce 累积计算
来源：http://wdf.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bia.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pah.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnx.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzw.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://plq.hammf.cn

Go:   // 手写循环
来源：http://jdr.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ecx.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wmp.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://jfh.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qpm.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://slb.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mhy.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qqw.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://epl.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kko.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ycz.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyg.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://xho.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://inu.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwv.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ohs.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yzb.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ire.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lka.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ros.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vvs.cucudq.cn

[D26] 数组转字符串
来源：http://lst.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://mkg.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://vrk.ydzc1.top

JS:   arr.join(", ")
来源：http://rkh.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://fsf.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://bqe.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://jqw.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://mqp.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://nti.zhijiandao.cn

================================================================================
来源：http://lkr.yj202588.top

E. 字符串处理
来源：http://xhx.sufxvd.cn

================================================================================
来源：http://ofn.sufxvd.cn

[E01] 拼接字符串
来源：http://qfc.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kxa.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jzi.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://czr.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuy.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sst.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tsq.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zji.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fwj.ybcxt.top

[E02] 重复字符串
来源：http://bql.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://akq.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://cjv.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://dxa.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://hxt.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://txc.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://swf.shzxlz.cn

Ruby: "ab" * 3
来源：http://jqr.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jts.jinqigufen.top

[E03] 截取子串
来源：http://psd.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gsq.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bqp.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://crh.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://iyb.sysykeji.top

Java: s.substring(1, 4)
来源：http://egf.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxr.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bny.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://nji.zhoulong.xyz

[E04] 查找子串位置
来源：http://bny.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://afv.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://eaj.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hjx.nanxinkj.top

TS:   s.indexOf("x")
来源：http://gqv.tian-w.cn

Java: s.indexOf("x")
来源：http://gbi.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://vjo.xziqi.cn

Ruby: s.index("x")
来源：http://cmu.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://qww.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zjl.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://adn.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nyc.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btb.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yze.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmf.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hzd.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uyj.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kwn.tarul.cn

[E06] 替换子串
来源：http://ufd.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsl.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://rld.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbl.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://ksf.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxn.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rtm.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jop.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://gsn.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://vcn.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eph.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oxv.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ouk.hcnkem.com

TS:   s.split(",")
来源：http://day.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ttx.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ivq.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://afy.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wjj.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://szh.tanke756.top

Py:   ",".join(items)
来源：http://nxp.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://drw.quarkkingdee.top

JS:   items.join(",")
来源：http://fnt.zhongyouzk.top

TS:   items.join(",")
来源：http://lfq.andypj.xyz

Java: String.join(",", items)
来源：http://ber.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://plc.hongshengwenyu.top

Ruby: items.join(",")
来源：http://uhw.hfpthk.cn

C#:   string.Join(",", items)
来源：http://iwk.ivvv.top

[E09] 去除所有空白字符
来源：http://gum.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dbk.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pzk.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://bys.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://uep.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://rri.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mbs.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://fpp.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tsy.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://umx.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://taj.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ywp.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://szv.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://mku.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://cdy.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ubq.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ofh.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lad.xinyue.icu

[E11] 反转字符串
来源：http://olq.cheryme.top

Py:   s[::-1]
来源：http://jrb.hammf.cn

PHP:  strrev($s);
来源：http://hie.yongpay.top

JS:   [...s].reverse().join("")
来源：http://fqj.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://jtw.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://fia.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ehk.sysykeji.top

Ruby: s.reverse
来源：http://ffs.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jjz.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://ysj.chenlongwang.top

Py:   s.count("a")
来源：http://wfw.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://ozc.bbcook.cn

JS:   s.split("a").length - 1
来源：http://jzl.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://ixi.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aad.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://djx.hesvh.cn

Ruby: s.count("a")
来源：http://yyo.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://hfj.dashuyun.cn

[E13] 逐字符遍历
来源：http://pjw.cashguo.top

Py:   for ch in s: print(ch)
来源：http://kdl.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zlj.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://bgr.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wad.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bhk.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xkv.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rlk.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jfr.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://ubw.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pvn.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pjk.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://caz.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hsc.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mav.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wbi.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bqd.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sug.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://wht.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://cxw.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqs.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://utv.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cdu.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rqq.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mis.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://esu.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://znc.yueranfly.top

[E16] 数字千分位
来源：http://nal.havefunace.top

Py:   f"{1234567:,}"
来源：http://frz.hfpthk.cn

PHP:  number_format(1234567);
来源：http://jum.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vtw.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://svc.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ohx.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://czs.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pth.pycfn.com

C#:   1234567.ToString("N0")
来源：http://igm.dashuyun.cn

[E17] 首字母大写
来源：http://fqv.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yxp.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lwp.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yup.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qip.sysykeji.top


<!-- 参考信息 -->