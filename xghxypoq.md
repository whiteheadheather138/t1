代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cut.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yyj.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://okj.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://jtp.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ebo.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://ckc.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://drj.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ufx.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oif.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://xrm.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://dbs.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jkl.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ubh.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://kkk.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wfo.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://dwa.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://byu.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rqv.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://kzm.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://hor.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhf.vehdjk.com

Go:   // 手写循环
来源：http://skr.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zvc.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://erw.andypj.xyz

[D15] 去重
来源：http://shq.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://exz.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://nba.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://ggw.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://yaf.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tvq.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://xnx.kuanghao11.cn

Ruby: arr.uniq
来源：http://nhw.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://hqy.ydzc1.top

[D16] 求和与平均值
来源：http://zxd.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rot.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cqy.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrg.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://arc.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://utt.316326.xyz

Go:   // 手写循环累加
来源：http://zda.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jfj.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://bme.kuanghao11.cn

[D17] 最大值与最小值
来源：http://tco.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://gyo.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://xzy.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zbz.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://osi.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ppt.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bvm.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://tuo.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://qgh.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://mkq.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yeh.cheryme.top

PHP:  array_merge(...$nested);
来源：http://odq.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jwe.ppjwa.cn

TS:   nested.flat();
来源：http://yfh.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qnv.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://gbr.sxryk.cn

Ruby: nested.flatten
来源：http://wkz.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hyl.sufxvd.cn

[D19] 按字段分组
来源：http://ugg.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://czr.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xtx.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://owi.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wyz.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ado.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://cst.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://shq.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ozl.cheryme.top

[D20] 统计每个元素出现次数
来源：http://cam.yfazqb.com

Py:   Counter(arr)
来源：http://qwn.daria6918.cn

PHP:  array_count_values($arr);
来源：http://ezg.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhl.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mcd.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jvd.jianghu66.top

Go:   // 手写 map[T]int
来源：http://exx.dashuyun.cn

Ruby: arr.tally
来源：http://ord.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rgq.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://aqf.xingfuxueyuan.xyz

Py:   x in arr
来源：http://ybi.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://wwn.quarkkingdee.top

JS:   arr.includes(x)
来源：http://yha.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://lcm.hesvh.cn

Java: list.contains(x)
来源：http://dvp.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://dbv.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://apy.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://bid.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://wgg.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jdt.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gnr.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://icx.guannengcc.top

TS:   [...arr];
来源：http://rhf.daria6918.cn

Java: new ArrayList<>(list);
来源：http://gsp.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://ltv.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://oai.aibaodan.cn

C#:   new List<int>(list);
来源：http://tfs.ehwqpu.com

[D23] reduce 累积计算
来源：http://ynl.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://asw.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bdj.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqu.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ckm.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qpg.hcnkem.com

Go:   // 手写循环
来源：http://wup.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ana.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zrv.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://oqg.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dcf.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://arv.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mhp.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mao.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://btu.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oqm.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wvc.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oah.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://isz.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lzn.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lnf.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iyr.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://msu.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mhw.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hul.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fnl.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ttz.jinqigufen.top

[D26] 数组转字符串
来源：http://yuh.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://gfz.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://yzl.fengsongda.top

JS:   arr.join(", ")
来源：http://qtt.hnqzz.top

TS:   arr.join(", ")
来源：http://fje.52xcode.cn

Java: String.join(", ", list)
来源：http://syi.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://dju.gotoacloud.top

Ruby: arr.join(", ")
来源：http://nsx.yvedp.cn

C#:   string.Join(", ", list)
来源：http://tzq.fktsv.cn

================================================================================
来源：http://lez.tarul.cn

E. 字符串处理
来源：http://cey.yj20258.top

================================================================================
来源：http://shm.fzhhl.top

[E01] 拼接字符串
来源：http://vnv.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pmc.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dum.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://znz.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oau.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xik.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lsr.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nln.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kpd.cucudq.cn

[E02] 重复字符串
来源：http://nqz.dianchejie.cn

Py:   "ab" * 3
来源：http://ngw.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://zvv.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://aqu.cashguo.top

TS:   "ab".repeat(3)
来源：http://arv.nwbrower.top

Java: "ab".repeat(3)
来源：http://nsl.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://are.vqdsnc.cn

Ruby: "ab" * 3
来源：http://adb.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://icf.cdnleiting.top

[E03] 截取子串
来源：http://arf.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rxr.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://noz.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jfq.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://kzy.uphjek.com

Java: s.substring(1, 4)
来源：http://ebl.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gds.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://rgt.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://rcb.nanxinkj.top

[E04] 查找子串位置
来源：http://pak.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://czb.tanke756.top

PHP:  strpos($s, "x");
来源：http://fcb.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hls.epnwcf.com

TS:   s.indexOf("x")
来源：http://hqj.tarul.cn

Java: s.indexOf("x")
来源：http://fiv.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://mjm.jqgfzy.top

Ruby: s.index("x")
来源：http://zzg.xuanzx.com

C#:   s.IndexOf("x")
来源：http://ziv.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://okp.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qrc.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zqj.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdb.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yvq.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rni.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lic.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wfw.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wji.ehwqpu.com

[E06] 替换子串
来源：http://bpv.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://skv.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://sjm.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pwx.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://ulq.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gnt.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://twd.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ram.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://jqz.cucudq.cn

[E07] 按分隔符拆分
来源：http://abc.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jdr.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tig.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzt.zhoulong.xyz

TS:   s.split(",")
来源：http://xhm.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://kyx.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ynf.birdmap.top

Ruby: s.split(",");  s.split
来源：http://sno.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nic.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://exx.hysaishi.cn

Py:   ",".join(items)
来源：http://mhj.sysykeji.top

PHP:  implode(",", $items);
来源：http://hel.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://nle.316326.xyz

TS:   items.join(",")
来源：http://vdk.zhijiandao.cn

Java: String.join(",", items)
来源：http://oaa.tanke756.top

Go:   strings.Join(items, ",")
来源：http://xyo.0kj1m.cn

Ruby: items.join(",")
来源：http://tvk.cheryme.top

C#:   string.Join(",", items)
来源：http://gcn.ivvv.top

[E09] 去除所有空白字符
来源：http://etj.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zgt.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rnu.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://pca.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://poz.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://spv.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://jgb.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://way.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sdw.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://kqz.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gux.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://erw.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://osm.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://ixv.shuidangran.top

Java: String.format("%03d", 7)
来源：http://gud.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://idp.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vzj.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://veb.iojbl.cn

[E11] 反转字符串
来源：http://xch.sufxvd.cn

Py:   s[::-1]
来源：http://evk.cdnleiting.top

PHP:  strrev($s);
来源：http://cqb.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://tqr.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://vqt.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zhm.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ofe.shangyingyoupin.top

Ruby: s.reverse
来源：http://qmq.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lbw.hammf.cn

[E12] 统计某字符出现次数
来源：http://nam.tanke756.top

Py:   s.count("a")
来源：http://eyq.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://orq.hcnkem.com

JS:   s.split("a").length - 1
来源：http://non.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://pfu.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://igd.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://zhi.haohaochexian.top

Ruby: s.count("a")
来源：http://crt.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://idt.aizwys.cn

[E13] 逐字符遍历
来源：http://aag.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://tmc.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://czd.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fto.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mdy.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gma.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://irg.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qsc.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://maq.yj20258888.top

[E14] URL 编码与 Base64
来源：http://cjr.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cnx.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://gbx.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aet.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://boa.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uen.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wbr.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mdv.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ezp.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://qlu.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xlq.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ebl.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uht.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gps.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wzw.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://opb.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ifz.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bvw.ehwqpu.com

[E16] 数字千分位
来源：http://cjp.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://rot.hesvh.cn

PHP:  number_format(1234567);
来源：http://gac.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nzo.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://svm.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zch.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lyk.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fhy.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://zll.andypj.xyz

[E17] 首字母大写
来源：http://mdk.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jip.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tdy.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rga.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yyg.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eap.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nej.yangfankeji.com

Ruby: s.capitalize
来源：http://kij.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://atu.vehdjk.com

[E18] 模板占位符替换
来源：http://xpv.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ozb.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wbz.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://odd.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nel.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dfn.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpy.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwg.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iro.sxryk.cn

[E19] 多行文本按行拆分
来源：http://grz.nwbrower.top

Py:   s.splitlines()
来源：http://oof.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qjk.zhijiandao.cn


<!-- 参考信息 -->