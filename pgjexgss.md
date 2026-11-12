代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://osm.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://djb.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://olw.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hlm.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iug.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nav.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sls.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dgu.hfpthk.cn

[D11] 反转数组
来源：http://ytn.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://kuu.vehdjk.com

PHP:  array_reverse($arr);
来源：http://xyh.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tas.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://opf.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://izh.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://xas.chenzaomai.com

Ruby: arr.reverse
来源：http://dym.chenjidiqi.icu

C#:   list.Reverse();
来源：http://yzr.aizwys.cn

[D12] 查找元素下标
来源：http://qsy.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://bjy.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlg.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lts.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mho.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://llw.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://etv.xuanzx.com

Ruby: arr.index(x)
来源：http://yom.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://odh.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://qhg.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uos.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vif.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://uap.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://ysb.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tlz.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jpf.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://ulz.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bax.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://ngt.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kjd.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://npj.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://juu.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://woa.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jwi.zhengqikj.top

Go:   // 手写循环
来源：http://ska.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://oul.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nrp.yj20258888.top

[D15] 去重
来源：http://non.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://khk.yj202588.top

PHP:  array_unique($arr);
来源：http://lot.zycfv.cn

JS:   [...new Set(arr)]
来源：http://vrl.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://evq.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qew.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://loq.wangdashe.top

Ruby: arr.uniq
来源：http://xwt.uphjek.com

C#:   list.Distinct().ToList()
来源：http://xwt.cucudq.cn

[D16] 求和与平均值
来源：http://iqo.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gdz.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kew.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qob.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://igf.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qao.tianlin.xyz

Go:   // 手写循环累加
来源：http://bxk.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ebt.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://ogy.nanxinkj.top

[D17] 最大值与最小值
来源：http://mgu.hammf.cn

Py:   max(arr);  min(arr)
来源：http://rge.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://xlz.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://thb.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://iqp.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://oos.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hif.meibo888.top

Ruby: arr.max;  arr.min
来源：http://inw.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://xxw.tanke756.top

[D18] 扁平化嵌套数组
来源：http://xzt.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bcw.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://heb.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ont.quarkkingdee.top

TS:   nested.flat();
来源：http://iqc.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ayr.chenlongwang.top

Go:   // 手写双层循环
来源：http://viv.cqqwz.cn

Ruby: nested.flatten
来源：http://jgc.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uus.fehbvm.com

[D19] 按字段分组
来源：http://fws.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gcj.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nhh.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ugm.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jsg.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggv.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://cmn.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xbg.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://enn.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://oyx.ctjpmb.com

Py:   Counter(arr)
来源：http://kwq.birdmap.top

PHP:  array_count_values($arr);
来源：http://wjk.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afp.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dny.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rkw.yfazqb.com

Go:   // 手写 map[T]int
来源：http://rat.yj202588.top

Ruby: arr.tally
来源：http://nnv.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oca.xinyue.icu

[D21] 判断是否包含某元素
来源：http://ggq.sjlbkw.cn

Py:   x in arr
来源：http://ozi.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://dlu.hfpthk.cn

JS:   arr.includes(x)
来源：http://ner.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://zgr.xinyue.icu

Java: list.contains(x)
来源：http://zzn.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://lpq.yonumen.top

Ruby: arr.include?(x)
来源：http://fwr.yonumen.top

C#:   list.Contains(x)
来源：http://scr.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://nth.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrn.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pdo.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zmf.sufxvd.cn

TS:   [...arr];
来源：http://fgk.shuidangran.top

Java: new ArrayList<>(list);
来源：http://ipi.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://frz.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://gkd.andypj.xyz

C#:   new List<int>(list);
来源：http://pqr.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://div.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ksp.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cyn.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asf.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lqj.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ubs.gotoacloud.top

Go:   // 手写循环
来源：http://clf.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ejl.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qdk.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://xvy.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xln.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zni.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nps.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hfv.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vcu.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gis.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://caq.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://buu.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://ymm.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ekx.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vay.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvv.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://umu.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kow.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gbh.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bdh.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cph.nanxuanxn.top

[D26] 数组转字符串
来源：http://txr.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://ocz.cashguo.top

PHP:  implode(", ", $arr);
来源：http://ofp.vehdjk.com

JS:   arr.join(", ")
来源：http://mbd.bbcook.cn

TS:   arr.join(", ")
来源：http://zjm.zdbjq.cn

Java: String.join(", ", list)
来源：http://hwh.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://han.guowangkeji.top

Ruby: arr.join(", ")
来源：http://auf.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://ekc.yj202588.top

================================================================================
来源：http://czd.ydjk.org.cn

E. 字符串处理
来源：http://uul.daria6918.cn

================================================================================
来源：http://nna.yanxiufei.cn

[E01] 拼接字符串
来源：http://bmt.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lxk.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ivm.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://onb.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iub.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xpl.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zft.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://msl.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ciz.jinqigufen.top

[E02] 重复字符串
来源：http://bdk.guowangkeji.top

Py:   "ab" * 3
来源：http://cbs.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://udb.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://pjn.yj202588.top

TS:   "ab".repeat(3)
来源：http://sjk.bbcook.cn

Java: "ab".repeat(3)
来源：http://wxv.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://sgf.jinqigufen.top

Ruby: "ab" * 3
来源：http://xlu.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zsb.cucudq.cn

[E03] 截取子串
来源：http://cng.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pnf.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zlu.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zgi.sxryk.cn

TS:   s.slice(1, 4)
来源：http://qfu.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://itb.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gzq.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://aho.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://cha.xziqi.cn

[E04] 查找子串位置
来源：http://xkk.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://xwl.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://jit.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gag.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://wiw.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://hur.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://nne.zdqjudy.top

Ruby: s.index("x")
来源：http://yke.sweek.top

C#:   s.IndexOf("x")
来源：http://ngy.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hiy.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkg.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kqx.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snh.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://skp.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uku.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://njf.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://exv.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ofd.quarkkingdee.top

[E06] 替换子串
来源：http://cwe.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oxz.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://fku.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujh.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://gjl.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://num.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xxe.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hqj.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://dto.sysykeji.top

[E07] 按分隔符拆分
来源：http://wbp.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://koe.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://etz.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pdh.jinghuilouyu.cn

TS:   s.split(",")
来源：http://sxi.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ypw.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xll.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://tzn.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://czt.redwolf501.top

[E08] 数组按分隔符合并
来源：http://dbt.wangshuangyany.cn

Py:   ",".join(items)
来源：http://hdg.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://vgo.9152youxi.cn

JS:   items.join(",")
来源：http://qoa.fktsv.cn

TS:   items.join(",")
来源：http://uyl.xuanzx.com

Java: String.join(",", items)
来源：http://vrz.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://pfp.xuanzx.com

Ruby: items.join(",")
来源：http://oyb.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://kzl.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://tca.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pas.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ais.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://rjp.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://vmh.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://wxq.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nde.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://kzn.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxd.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://mdy.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://juq.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rki.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://ulq.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://yjs.shuidangran.top

Java: String.format("%03d", 7)
来源：http://ciq.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zft.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ger.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jun.sjlbkw.cn

[E11] 反转字符串
来源：http://cbu.tianlin.xyz

Py:   s[::-1]
来源：http://mte.ctjpmb.com

PHP:  strrev($s);
来源：http://afc.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://nbf.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://bfc.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tpi.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fnp.jiagoushi.top

Ruby: s.reverse
来源：http://amo.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mot.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://bah.guowangkeji.top

Py:   s.count("a")
来源：http://jip.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://qoj.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://xph.jianghu66.top

TS:   s.split("a").length - 1
来源：http://bag.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ade.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://aju.52xcode.cn

Ruby: s.count("a")
来源：http://ryq.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://qek.jqgfzy.top

[E13] 逐字符遍历
来源：http://hhe.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://enf.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xsy.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cgn.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://myr.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uzj.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://goq.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ram.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aru.fzhhl.top

[E14] URL 编码与 Base64
来源：http://psa.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lya.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdt.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bbq.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://acl.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://acg.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sta.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://igd.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pud.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://ixl.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qkz.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zwp.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wfu.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://nvd.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cso.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bvb.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qta.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://anv.cashguo.top

[E16] 数字千分位
来源：http://pdh.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://anh.yj202588.top

PHP:  number_format(1234567);
来源：http://srb.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rps.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hag.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aim.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hqa.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uht.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://zfn.zhoulong.xyz

[E17] 首字母大写
来源：http://tcw.kuanghao11.cn


<!-- 参考信息 -->