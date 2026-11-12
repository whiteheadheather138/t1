代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eie.chenjidiqi.icu

Ruby: arr.sort
来源：http://cko.mhx1999.top

C#:   list.Sort();
来源：http://kzq.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vqi.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fql.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdu.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edx.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsj.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qzo.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qef.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gpi.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://exf.zhongyouzk.top

[D11] 反转数组
来源：http://jup.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://nit.fehbvm.com

PHP:  array_reverse($arr);
来源：http://sir.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mqb.hesvh.cn

TS:   [...arr].reverse();
来源：http://pip.hammf.cn

Java: Collections.reverse(list);
来源：http://phx.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://rty.svipenyu.cn

Ruby: arr.reverse
来源：http://rsk.ivvv.top

C#:   list.Reverse();
来源：http://aez.bbcook.cn

[D12] 查找元素下标
来源：http://kkx.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://moj.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cnm.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bfa.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wqd.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dhz.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://qcb.mhx1999.top

Ruby: arr.index(x)
来源：http://ssc.ivvv.top

C#:   list.IndexOf(x);
来源：http://bok.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://wqp.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://muw.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxf.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://xdl.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://gdd.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hyh.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxg.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://shs.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://inv.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://mtb.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wic.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzw.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://wug.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://krr.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hqz.gogol.net.cn

Go:   // 手写循环
来源：http://xft.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://mfy.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rxm.ywan-chungtsiang.top

[D15] 去重
来源：http://pkk.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fex.0kj1m.cn

PHP:  array_unique($arr);
来源：http://pxg.ydzc1.top

JS:   [...new Set(arr)]
来源：http://kci.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://nvp.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zwo.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://cet.birdmap.top

Ruby: arr.uniq
来源：http://mtc.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://vwg.xuanzx.com

[D16] 求和与平均值
来源：http://hcu.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yzz.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qth.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dss.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jcj.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dth.havefunace.top

Go:   // 手写循环累加
来源：http://fys.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ynx.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://ysz.zdqjudy.top

[D17] 最大值与最小值
来源：http://xyn.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://woi.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://khy.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fys.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://eoj.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://agh.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jao.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://ict.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://nhm.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://szg.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ptm.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://akp.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xkb.chenzaomai.com

TS:   nested.flat();
来源：http://jgv.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wnu.sweek.top

Go:   // 手写双层循环
来源：http://qxo.cqqwz.cn

Ruby: nested.flatten
来源：http://ibi.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dul.cucudq.cn

[D19] 按字段分组
来源：http://vnl.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://puz.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mti.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mcd.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wey.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hkf.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://vvl.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://chj.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mhs.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://kxp.cashguo.top

Py:   Counter(arr)
来源：http://spa.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://nsx.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://foq.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oad.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sqm.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://lzc.ydzc1.top

Ruby: arr.tally
来源：http://gzd.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wjb.iojbl.cn

[D21] 判断是否包含某元素
来源：http://zyt.gotoacloud.top

Py:   x in arr
来源：http://jrn.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://wmw.ehwqpu.com

JS:   arr.includes(x)
来源：http://hsx.dianchejie.cn

TS:   arr.includes(x)
来源：http://cwl.hnqzz.top

Java: list.contains(x)
来源：http://ths.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://jlv.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://rnb.daxiang520.top

C#:   list.Contains(x)
来源：http://iha.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://ksy.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qwa.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qke.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://czx.fengsongda.top

TS:   [...arr];
来源：http://ijv.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://emj.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://rbx.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://ufk.yvedp.cn

C#:   new List<int>(list);
来源：http://gvg.gaohongyu789.top

[D23] reduce 累积计算
来源：http://trs.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rsm.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jgj.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syv.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kuj.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qrk.guannengcc.top

Go:   // 手写循环
来源：http://iwj.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tev.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oaw.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://rgq.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://grs.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dnd.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rwf.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hvj.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dwr.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llb.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vez.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://naw.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://cap.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyj.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbh.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gnz.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbi.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kek.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vcd.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qbj.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dtg.yongpay.top

[D26] 数组转字符串
来源：http://ojw.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://kfo.uphjek.com

PHP:  implode(", ", $arr);
来源：http://ttb.fktsv.cn

JS:   arr.join(", ")
来源：http://auf.bbcook.cn

TS:   arr.join(", ")
来源：http://udk.0kj1m.cn

Java: String.join(", ", list)
来源：http://abq.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://kmw.aizwys.cn

Ruby: arr.join(", ")
来源：http://aia.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://rie.kuanghao11.cn

================================================================================
来源：http://txu.jiagoushi.top

E. 字符串处理
来源：http://jzd.tanke756.top

================================================================================
来源：http://izx.redwolf501.top

[E01] 拼接字符串
来源：http://cte.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qsi.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vac.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://npg.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://csk.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://afa.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gpm.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uww.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bln.yuxming.cn

[E02] 重复字符串
来源：http://pus.mhx1999.top

Py:   "ab" * 3
来源：http://jpi.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://ivr.meibo888.top

JS:   "ab".repeat(3)
来源：http://frw.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://hmv.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://dug.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://yfl.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://tft.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jdg.ppjwa.cn

[E03] 截取子串
来源：http://etz.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wxf.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bvp.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://etp.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://jap.birdmap.top

Java: s.substring(1, 4)
来源：http://mxf.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zvk.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://rnz.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://igq.vqdsnc.cn

[E04] 查找子串位置
来源：http://khe.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://cur.hammf.cn

PHP:  strpos($s, "x");
来源：http://ylh.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jea.fzhhl.top

TS:   s.indexOf("x")
来源：http://qsv.gogol.net.cn

Java: s.indexOf("x")
来源：http://ekb.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://uwp.jinqigufen.top

Ruby: s.index("x")
来源：http://wxc.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://hiw.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkk.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txy.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yfy.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wnx.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zei.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mct.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nvq.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://spg.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://npa.c1oappe.top

[E06] 替换子串
来源：http://pnv.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dzj.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://ejv.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gwc.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://idx.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://upc.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rvr.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qsy.havefunace.top

C#:   s.Replace("a", "b")
来源：http://cmh.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://xun.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zjo.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hhw.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://xzs.yongpay.top

TS:   s.split(",")
来源：http://oks.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://hpm.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mmn.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://nmz.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grw.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://fye.hesvh.cn

Py:   ",".join(items)
来源：http://enp.hammf.cn

PHP:  implode(",", $items);
来源：http://flb.yuanzhike.top

JS:   items.join(",")
来源：http://ytw.nanxuanxn.top

TS:   items.join(",")
来源：http://scr.zdbjq.cn

Java: String.join(",", items)
来源：http://wal.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://xvd.feifeiyinyue.top

Ruby: items.join(",")
来源：http://byw.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://ttn.vehdjk.com

[E09] 去除所有空白字符
来源：http://xsj.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bvv.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cbt.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://mfm.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://krq.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ywx.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rvp.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yot.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmo.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://lwd.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sys.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://msy.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://pxn.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://eof.yj202588.top

Java: String.format("%03d", 7)
来源：http://ezq.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ekx.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://luz.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zmr.daria6918.cn

[E11] 反转字符串
来源：http://clq.cashguo.top

Py:   s[::-1]
来源：http://wpi.bjfxy.top

PHP:  strrev($s);
来源：http://yhg.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://uas.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://tps.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tbd.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yph.jiagoushi.top

Ruby: s.reverse
来源：http://eiy.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://dws.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://bdp.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://cta.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://ckt.uphjek.com

JS:   s.split("a").length - 1
来源：http://nvz.fktsv.cn

TS:   s.split("a").length - 1
来源：http://ljl.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qkm.pycfn.com

Go:   strings.Count(s, "a")
来源：http://xxv.ctjpmb.com

Ruby: s.count("a")
来源：http://xxb.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://hxf.hammf.cn

[E13] 逐字符遍历
来源：http://vkb.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://zuv.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xkn.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://khx.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jxs.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iiq.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gnw.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zdn.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jiy.hcnkem.com

[E14] URL 编码与 Base64
来源：http://fdh.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oht.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dke.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fcb.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tek.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yiq.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cps.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tpt.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xmj.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://blk.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wkt.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://imk.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ivr.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://xre.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rof.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vjt.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cxg.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nwr.chenzaomai.com

[E16] 数字千分位
来源：http://kwz.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://hyo.jinqigufen.top

PHP:  number_format(1234567);
来源：http://ndv.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fcr.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://euj.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lyp.snrcjt.cn


<!-- 参考信息 -->