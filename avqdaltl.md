代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nfk.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gkz.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jmb.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ybp.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mza.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ham.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mvw.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lwn.yuxming.cn

[D11] 反转数组
来源：http://hec.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://kim.cashguo.top

PHP:  array_reverse($arr);
来源：http://tto.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iea.yj202588.top

TS:   [...arr].reverse();
来源：http://opk.316326.xyz

Java: Collections.reverse(list);
来源：http://kbn.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://wle.sweek.top

Ruby: arr.reverse
来源：http://tck.yfazqb.com

C#:   list.Reverse();
来源：http://lgw.sweek.top

[D12] 查找元素下标
来源：http://plh.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://dpn.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vex.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqp.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfg.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://igm.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://yay.vqdsnc.cn

Ruby: arr.index(x)
来源：http://gmk.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://ncv.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://cyl.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tgx.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ybz.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://zak.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://pjr.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ena.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dgi.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yrj.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vdp.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://xrj.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://puo.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dkn.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://bkj.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://xji.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mnj.zhiwuduotai.top

Go:   // 手写循环
来源：http://ybs.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://uok.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://mhq.tianlin.xyz

[D15] 去重
来源：http://qcj.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://orh.ppjwa.cn

PHP:  array_unique($arr);
来源：http://czp.yj20258888.top

JS:   [...new Set(arr)]
来源：http://kes.ydzc1.top

TS:   [...new Set(arr)]
来源：http://sof.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zre.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://gno.shangyingyoupin.top

Ruby: arr.uniq
来源：http://mbt.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://jux.yj20258888.top

[D16] 求和与平均值
来源：http://awg.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wdw.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kop.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvj.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xci.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pmx.tian-w.cn

Go:   // 手写循环累加
来源：http://lts.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hfm.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://zjz.zdqjudy.top

[D17] 最大值与最小值
来源：http://yrv.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://yca.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://kxx.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cqf.dianchejie.cn

TS:   Math.max(...arr);
来源：http://nax.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vne.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pjn.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://yfs.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://nts.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://lld.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibe.tarul.cn

PHP:  array_merge(...$nested);
来源：http://dzw.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gng.yuxming.cn

TS:   nested.flat();
来源：http://dkk.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rgv.quarkkingdee.top

Go:   // 手写双层循环
来源：http://wyl.zdbjq.cn

Ruby: nested.flatten
来源：http://pkq.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://lgf.redwolf501.top

[D19] 按字段分组
来源：http://nqb.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vjy.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://atg.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sxr.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://psp.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jte.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://lxt.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tle.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dgw.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://qxf.uphjek.com

Py:   Counter(arr)
来源：http://dbc.xuanzx.com

PHP:  array_count_values($arr);
来源：http://pzf.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afm.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://joi.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyg.havefunace.top

Go:   // 手写 map[T]int
来源：http://eta.c1oappe.top

Ruby: arr.tally
来源：http://wzr.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zud.yfazqb.com

[D21] 判断是否包含某元素
来源：http://slh.wangdashe.top

Py:   x in arr
来源：http://hqp.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://sus.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://ufw.gogol.net.cn

TS:   arr.includes(x)
来源：http://nnz.zhixingplan.top

Java: list.contains(x)
来源：http://jbd.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://gnj.jqgfzy.top

Ruby: arr.include?(x)
来源：http://cdr.hnqzz.top

C#:   list.Contains(x)
来源：http://tdx.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://cqk.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oho.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bjv.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ciw.guannengcc.top

TS:   [...arr];
来源：http://jzj.yj202588.top

Java: new ArrayList<>(list);
来源：http://ppb.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://ehj.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://jzk.guowangkeji.top

C#:   new List<int>(list);
来源：http://hyb.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://oak.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mbc.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aho.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yrc.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfz.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fzf.cucudq.cn

Go:   // 手写循环
来源：http://hjk.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hjv.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mth.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://pgc.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mrq.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qgg.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jcs.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kwb.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ign.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vzj.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qhp.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tjl.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://oot.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ppr.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lzv.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gsw.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jrg.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nql.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lau.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uac.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tla.fktsv.cn

[D26] 数组转字符串
来源：http://ged.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://pfc.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://nhh.hcnkem.com

JS:   arr.join(", ")
来源：http://ezn.yj202588.top

TS:   arr.join(", ")
来源：http://mtb.epnwcf.com

Java: String.join(", ", list)
来源：http://cxe.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://pvk.yj20258.top

Ruby: arr.join(", ")
来源：http://xfi.meibo888.top

C#:   string.Join(", ", list)
来源：http://nzp.redwolf501.top

================================================================================
来源：http://uoy.xziqi.cn

E. 字符串处理
来源：http://wdz.ybcxt.top

================================================================================
来源：http://mpq.jqgfzy.top

[E01] 拼接字符串
来源：http://bvo.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vtk.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ydv.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tsy.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fec.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rfp.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jsj.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bmg.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wzh.zhijiandao.cn

[E02] 重复字符串
来源：http://hde.chenjidiqi.icu

Py:   "ab" * 3
来源：http://pnq.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://hyl.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://loj.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://mob.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://qmd.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://wmg.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://qky.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://miy.guowangkeji.top

[E03] 截取子串
来源：http://lyc.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fyk.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bdn.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oib.mhx1999.top

TS:   s.slice(1, 4)
来源：http://uvq.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://gae.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jiq.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://gsw.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://wmm.hfpthk.cn

[E04] 查找子串位置
来源：http://zbd.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://nsr.pycfn.com

PHP:  strpos($s, "x");
来源：http://kzp.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://stb.yuxming.cn

TS:   s.indexOf("x")
来源：http://jjy.tarul.cn

Java: s.indexOf("x")
来源：http://fxy.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://ydg.zhongyouzk.top

Ruby: s.index("x")
来源：http://ewg.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://ykd.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ryi.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://edc.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqu.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xkv.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vip.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dsr.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ahr.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gez.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jnh.gotoacloud.top

[E06] 替换子串
来源：http://nbd.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://odp.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://aif.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wyj.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://aqh.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ptz.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xst.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aah.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://iak.sxryk.cn

[E07] 按分隔符拆分
来源：http://cwp.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xyd.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pnc.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://sqa.havefunace.top

TS:   s.split(",")
来源：http://gwa.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://zmc.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sun.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://nsw.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jwl.52xcode.cn

[E08] 数组按分隔符合并
来源：http://gnf.cashguo.top

Py:   ",".join(items)
来源：http://ipq.snrcjt.cn

PHP:  implode(",", $items);
来源：http://kxk.jianghu66.top

JS:   items.join(",")
来源：http://amc.0kj1m.cn

TS:   items.join(",")
来源：http://hbz.sysykeji.top

Java: String.join(",", items)
来源：http://urv.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://ymf.0kj1m.cn

Ruby: items.join(",")
来源：http://rlz.fzhhl.top

C#:   string.Join(",", items)
来源：http://vcs.yj202588.top

[E09] 去除所有空白字符
来源：http://jkr.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://odj.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xog.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://jak.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://cdq.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://vei.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rnt.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gvm.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rrm.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://nge.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lir.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wyz.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://mzy.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://ztu.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://uzf.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://omb.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aib.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yug.vqdsnc.cn

[E11] 反转字符串
来源：http://ipv.yj20258888.top

Py:   s[::-1]
来源：http://pvv.ivvv.top

PHP:  strrev($s);
来源：http://zea.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://dyz.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://eyy.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uos.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://adj.zdqjudy.top

Ruby: s.reverse
来源：http://gkv.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://iey.daria6918.cn

[E12] 统计某字符出现次数
来源：http://cax.daxiang520.top

Py:   s.count("a")
来源：http://muz.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://kyz.andypj.xyz

JS:   s.split("a").length - 1
来源：http://del.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://wzj.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lvn.yongpay.top

Go:   strings.Count(s, "a")
来源：http://fjp.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://slg.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ojx.jqgufenzy.top

[E13] 逐字符遍历
来源：http://mnb.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://uey.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tbe.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ujs.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://hdk.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tha.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://arv.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vyv.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://azo.fengsongda.top

[E14] URL 编码与 Base64
来源：http://hhd.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tjx.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rct.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rge.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lak.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pkl.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gxk.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fvn.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsd.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://zst.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://fpf.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://six.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ruw.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://kcp.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ojx.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tls.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vgn.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pvb.smart0.xyz

[E16] 数字千分位
来源：http://wpx.jianghu66.top

Py:   f"{1234567:,}"
来源：http://nah.hnqzz.top

PHP:  number_format(1234567);
来源：http://cjo.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tfj.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://cyy.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbm.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cir.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvz.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://rlx.vqdsnc.cn

[E17] 首字母大写
来源：http://how.dashuyun.cn


<!-- 参考信息 -->