代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wpm.epnwcf.com

Ruby: arr.sort
来源：http://ayi.shzxlz.cn

C#:   list.Sort();
来源：http://xpa.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://sgg.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nab.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gzw.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vjh.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://evc.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqr.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wxq.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vvc.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dtu.jinghuilouyu.cn

[D11] 反转数组
来源：http://drh.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://mgo.nwbrower.top

PHP:  array_reverse($arr);
来源：http://qen.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fvu.sysykeji.top

TS:   [...arr].reverse();
来源：http://uew.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://bnl.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://tmv.pycfn.com

Ruby: arr.reverse
来源：http://moe.yonumen.top

C#:   list.Reverse();
来源：http://lhy.ydzc1.top

[D12] 查找元素下标
来源：http://uzu.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://wio.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lqs.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgb.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qme.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kox.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://ehl.jinqigufen.top

Ruby: arr.index(x)
来源：http://tvo.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://eyl.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://jsg.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cus.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://inj.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://lur.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://pca.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rxd.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jer.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rnq.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vjb.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://ukp.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gmx.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cxf.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://flh.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://osu.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lcc.shangyingyoupin.top

Go:   // 手写循环
来源：http://ggg.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nrq.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://jwk.0kj1m.cn

[D15] 去重
来源：http://xwn.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pob.gotoacloud.top

PHP:  array_unique($arr);
来源：http://rsj.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://vun.yongpay.top

TS:   [...new Set(arr)]
来源：http://sju.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lpj.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://hdl.daxiang520.top

Ruby: arr.uniq
来源：http://rda.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://ihn.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://mxv.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hct.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iaf.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://skr.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://msm.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://soq.gzhubu.top

Go:   // 手写循环累加
来源：http://doo.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mvz.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://mwq.ppjwa.cn

[D17] 最大值与最小值
来源：http://vlu.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://dfd.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://jsd.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pjo.ivvv.top

TS:   Math.max(...arr);
来源：http://dto.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qlx.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jyd.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://dds.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://viv.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://raf.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vog.yongpay.top

PHP:  array_merge(...$nested);
来源：http://iuw.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://npg.pengpengdd.cyou

TS:   nested.flat();
来源：http://sln.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://itz.yuanzhike.top

Go:   // 手写双层循环
来源：http://kpp.smart0.xyz

Ruby: nested.flatten
来源：http://jjn.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fzv.hcnkem.com

[D19] 按字段分组
来源：http://ubx.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zxz.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uld.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vdt.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ccb.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://llx.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://tol.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tqs.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umm.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://gvg.tarul.cn

Py:   Counter(arr)
来源：http://fub.daria6918.cn

PHP:  array_count_values($arr);
来源：http://vci.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cby.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dlw.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kes.birdmap.top

Go:   // 手写 map[T]int
来源：http://jtc.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://hdu.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rnu.andypj.xyz

[D21] 判断是否包含某元素
来源：http://uzs.52xcode.cn

Py:   x in arr
来源：http://yve.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://lup.nanxuanxn.top

JS:   arr.includes(x)
来源：http://fgz.sxryk.cn

TS:   arr.includes(x)
来源：http://bgt.hfpthk.cn

Java: list.contains(x)
来源：http://unx.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://khi.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://vtg.shuidangran.top

C#:   list.Contains(x)
来源：http://djr.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://xqs.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://shk.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trc.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ibn.shanyushiyangkeji.top

TS:   [...arr];
来源：http://hhx.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://yit.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ayh.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://bcj.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://zyk.nanxinkj.top

[D23] reduce 累积计算
来源：http://guz.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dar.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://thj.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ser.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzp.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://huv.tarul.cn

Go:   // 手写循环
来源：http://qfl.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gid.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ewp.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://jlg.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tyv.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dbn.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bda.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cdm.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ipa.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qhm.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ylb.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tbe.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://kud.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mtc.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://phy.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mzx.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mlo.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kbw.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://riw.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxq.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xcu.wangdashe.top

[D26] 数组转字符串
来源：http://uiw.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://isu.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://ubb.0kj1m.cn

JS:   arr.join(", ")
来源：http://efr.aizwys.cn

TS:   arr.join(", ")
来源：http://zvo.zycfv.cn

Java: String.join(", ", list)
来源：http://psb.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://sav.yfazqb.com

Ruby: arr.join(", ")
来源：http://fcz.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://onr.jinghuilouyu.cn

================================================================================
来源：http://mkb.zycfv.cn

E. 字符串处理
来源：http://uoe.jyoumei.cn

================================================================================
来源：http://kar.zhongyouzk.top

[E01] 拼接字符串
来源：http://yjr.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ggf.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ijl.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zbr.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxc.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://avk.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zfl.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dcm.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sva.yuanzhike.top

[E02] 重复字符串
来源：http://dff.zhiwuduotai.top

Py:   "ab" * 3
来源：http://ibe.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://vgl.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://dxa.andypj.xyz

TS:   "ab".repeat(3)
来源：http://cay.nwbrower.top

Java: "ab".repeat(3)
来源：http://fho.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://uaq.zhijiandao.cn

Ruby: "ab" * 3
来源：http://jgg.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nfg.tarul.cn

[E03] 截取子串
来源：http://sos.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://miv.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://olb.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eje.smart0.xyz

TS:   s.slice(1, 4)
来源：http://bos.dashuyun.cn

Java: s.substring(1, 4)
来源：http://icc.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fht.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://foh.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://gpb.feifeiyinyue.top

[E04] 查找子串位置
来源：http://jlp.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://jxd.sweek.top

PHP:  strpos($s, "x");
来源：http://xet.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qkf.hywenlv.cn

TS:   s.indexOf("x")
来源：http://ygu.meibo888.top

Java: s.indexOf("x")
来源：http://dmw.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://ebe.zhongyouzk.top

Ruby: s.index("x")
来源：http://nsx.fzhhl.top

C#:   s.IndexOf("x")
来源：http://wcn.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rai.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rrr.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dow.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hpe.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hmr.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ckl.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xcd.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://alq.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wph.zdbjq.cn

[E06] 替换子串
来源：http://rcn.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dyc.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://bzj.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nmu.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://myq.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rhi.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pbu.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vup.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://zzp.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://gqk.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pfx.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ugt.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://prt.hysaishi.cn

TS:   s.split(",")
来源：http://qhx.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vcj.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ihw.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://fhc.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sde.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://alc.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://xzo.zhengqikj.top

PHP:  implode(",", $items);
来源：http://qqx.pengpengdd.cyou

JS:   items.join(",")
来源：http://qjw.guowangkeji.top

TS:   items.join(",")
来源：http://toc.xinyue.icu

Java: String.join(",", items)
来源：http://wfv.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://jsu.gaohongyu789.top

Ruby: items.join(",")
来源：http://xsl.snrcjt.cn

C#:   string.Join(",", items)
来源：http://ccj.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://hzd.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lgj.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://khp.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://gkc.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://weg.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://iip.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hlq.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://znr.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ykd.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://hbi.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vpw.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://png.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://coy.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://egr.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://ybo.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pak.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://usl.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zok.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://ham.snrcjt.cn

Py:   s[::-1]
来源：http://qon.hongshengwenyu.top

PHP:  strrev($s);
来源：http://llc.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://ach.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://jjr.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rqb.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://aio.ydjk.org.cn

Ruby: s.reverse
来源：http://mhw.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://adf.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://yty.pycfn.com

Py:   s.count("a")
来源：http://qqp.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://lwu.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://kcs.fengsongda.top

TS:   s.split("a").length - 1
来源：http://lbw.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bsn.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://jfg.jqgfzy.top

Ruby: s.count("a")
来源：http://exm.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://dvz.uphjek.com

[E13] 逐字符遍历
来源：http://zfh.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://pgs.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ddg.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lte.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wwx.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cuk.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wbj.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wyo.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bwy.yj20258.top

[E14] URL 编码与 Base64
来源：http://jkx.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tad.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsv.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://umf.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cic.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://flt.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ltk.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://noo.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dfo.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://jop.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kgs.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tey.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://glk.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gzw.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pea.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cmh.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fsx.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://guj.hnqzz.top

[E16] 数字千分位
来源：http://gqf.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://cth.ehwqpu.com

PHP:  number_format(1234567);
来源：http://nij.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uxz.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fvh.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ppa.zhongyouzk.top


<!-- 参考信息 -->