代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fwj.daxiang520.top

Ruby: arr.sort
来源：http://nem.jiagoushi.top

C#:   list.Sort();
来源：http://zjk.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://psd.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iue.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ksj.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pbi.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymd.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://glk.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ozj.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nzd.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vzd.yuanzhike.top

[D11] 反转数组
来源：http://wnu.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yii.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://bpe.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://arc.bjfxy.top

TS:   [...arr].reverse();
来源：http://wtm.cheryme.top

Java: Collections.reverse(list);
来源：http://pdj.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://enw.jlsjyb.cn

Ruby: arr.reverse
来源：http://hhm.tian-w.cn

C#:   list.Reverse();
来源：http://jco.c1oappe.top

[D12] 查找元素下标
来源：http://kvl.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://udt.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://snq.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrs.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ged.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://woy.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://guo.xinyue.icu

Ruby: arr.index(x)
来源：http://ohs.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://eyr.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://bbc.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xwu.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rug.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://cwu.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://xzq.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gia.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dxz.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://oqn.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sbp.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://hbl.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vgu.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dwu.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://odk.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://okl.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://icz.hnqzz.top

Go:   // 手写循环
来源：http://syv.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xwa.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sqv.jyoumei.cn

[D15] 去重
来源：http://ols.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gol.gogol.net.cn

PHP:  array_unique($arr);
来源：http://qpr.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://uxj.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://uwi.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kbm.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mri.hysaishi.cn

Ruby: arr.uniq
来源：http://bsy.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://mqj.jqgufenzy.top

[D16] 求和与平均值
来源：http://gja.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xph.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cds.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://olo.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vun.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jbf.zhoulong.xyz

Go:   // 手写循环累加
来源：http://jih.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ezn.sweek.top

C#:   list.Sum();  list.Average()
来源：http://qus.aibaodan.cn

[D17] 最大值与最小值
来源：http://jru.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://rhh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://vcp.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://car.hammf.cn

TS:   Math.max(...arr);
来源：http://rch.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ams.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://chc.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://kvf.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://pmd.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://sbj.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://evk.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://znm.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ipl.gogol.net.cn

TS:   nested.flat();
来源：http://uos.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ees.cqqwz.cn

Go:   // 手写双层循环
来源：http://gpx.iojbl.cn

Ruby: nested.flatten
来源：http://kqw.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pws.havefunace.top

[D19] 按字段分组
来源：http://fqb.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sty.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://syd.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tml.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xcf.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fns.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://ygf.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ied.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://afy.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://fic.dashuyun.cn

Py:   Counter(arr)
来源：http://kus.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://piv.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://icc.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qjw.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bwd.ybcxt.top

Go:   // 手写 map[T]int
来源：http://sfq.bbcook.cn

Ruby: arr.tally
来源：http://iqt.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ikx.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://gma.guowangkeji.top

Py:   x in arr
来源：http://poa.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://dmy.316326.xyz

JS:   arr.includes(x)
来源：http://doo.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://cye.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://yrq.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://ibg.cheryme.top

Ruby: arr.include?(x)
来源：http://jom.hysaishi.cn

C#:   list.Contains(x)
来源：http://dhr.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://pby.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zhn.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kie.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://esm.andypj.xyz

TS:   [...arr];
来源：http://lwi.redwolf501.top

Java: new ArrayList<>(list);
来源：http://epr.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://rer.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://dgz.daria6918.cn

C#:   new List<int>(list);
来源：http://oju.bbcook.cn

[D23] reduce 累积计算
来源：http://llt.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bqn.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rof.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rqk.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvk.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yrb.yonumen.top

Go:   // 手写循环
来源：http://sdh.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lgt.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ysq.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://raj.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jsg.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://piy.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yug.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eke.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ooc.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dcd.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nqb.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://van.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://aij.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mah.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eib.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zqn.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cfw.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fad.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qkb.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ppx.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ymt.zhiwuduotai.top

[D26] 数组转字符串
来源：http://qwa.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://xic.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://dqb.yj20258.top

JS:   arr.join(", ")
来源：http://xpk.hywenlv.cn

TS:   arr.join(", ")
来源：http://lac.nanxinkj.top

Java: String.join(", ", list)
来源：http://hbk.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://och.svipenyu.cn

Ruby: arr.join(", ")
来源：http://wde.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://gky.zhengqikj.top

================================================================================
来源：http://vht.sxryk.cn

E. 字符串处理
来源：http://prd.sxryk.cn

================================================================================
来源：http://yub.ppjwa.cn

[E01] 拼接字符串
来源：http://loz.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lpt.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jms.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gnd.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvj.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tst.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mzm.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eio.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://waa.52xcode.cn

[E02] 重复字符串
来源：http://btt.fzhhl.top

Py:   "ab" * 3
来源：http://vco.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://mjb.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://dfl.guannengcc.top

TS:   "ab".repeat(3)
来源：http://uti.xuanzx.com

Java: "ab".repeat(3)
来源：http://qmj.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://wqd.kuanghao11.cn

Ruby: "ab" * 3
来源：http://cgj.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixu.zhoulong.xyz

[E03] 截取子串
来源：http://mix.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kyn.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tfa.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pnd.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://ihm.c1oappe.top

Java: s.substring(1, 4)
来源：http://eyk.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://naq.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://vve.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://vuh.gogol.net.cn

[E04] 查找子串位置
来源：http://aft.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://rcr.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://gea.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nbw.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://yoq.sufxvd.cn

Java: s.indexOf("x")
来源：http://dsn.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://mly.hesvh.cn

Ruby: s.index("x")
来源：http://ukm.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://boi.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://mfg.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://grf.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owf.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bnu.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fyt.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxb.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nsw.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lho.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gpm.chenjidiqi.icu

[E06] 替换子串
来源：http://mqk.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jod.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://bac.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pqy.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://aul.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqa.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iwb.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pua.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://wla.ctjpmb.com

[E07] 按分隔符拆分
来源：http://jgs.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zxt.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://usa.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xag.cheryme.top

TS:   s.split(",")
来源：http://vff.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vsa.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://web.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://mwm.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bwj.bbcook.cn

[E08] 数组按分隔符合并
来源：http://zzh.birdmap.top

Py:   ",".join(items)
来源：http://qeu.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://jtk.iojbl.cn

JS:   items.join(",")
来源：http://aho.guannengcc.top

TS:   items.join(",")
来源：http://rcb.hnqzz.top

Java: String.join(",", items)
来源：http://cct.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://kkd.ydjk.org.cn

Ruby: items.join(",")
来源：http://yqg.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://gsp.tanke756.top

[E09] 去除所有空白字符
来源：http://dzm.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dfe.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yns.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://yvq.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://ekc.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://fsz.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vqk.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xgp.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ewm.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://err.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mkj.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vkn.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://kbc.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://myz.meibo888.top

Java: String.format("%03d", 7)
来源：http://lhm.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bel.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkg.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cfy.bbcook.cn

[E11] 反转字符串
来源：http://qyl.jinqigfzy.top

Py:   s[::-1]
来源：http://vco.9152youxi.cn

PHP:  strrev($s);
来源：http://uuk.hammf.cn

JS:   [...s].reverse().join("")
来源：http://vxj.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://fqi.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://spk.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xjb.yonumen.top

Ruby: s.reverse
来源：http://yxh.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://rtk.yueranfly.top

[E12] 统计某字符出现次数
来源：http://evr.mhx1999.top

Py:   s.count("a")
来源：http://bvm.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://mov.tian-w.cn

JS:   s.split("a").length - 1
来源：http://ise.tian-w.cn

TS:   s.split("a").length - 1
来源：http://dfg.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gdx.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://wer.9152youxi.cn

Ruby: s.count("a")
来源：http://zil.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://mva.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://goc.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://pfr.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vve.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxn.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zpk.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nbo.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wxw.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zqm.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pbc.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://udh.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ndx.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojg.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bvx.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dmo.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nmo.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tns.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ety.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://szh.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://zvg.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xcq.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yky.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kyn.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cjx.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uag.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://upd.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sfi.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://awy.yonumen.top

[E16] 数字千分位
来源：http://nwv.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://uru.xziqi.cn

PHP:  number_format(1234567);
来源：http://rkq.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://goa.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wel.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kpp.gotoacloud.top


<!-- 参考信息 -->