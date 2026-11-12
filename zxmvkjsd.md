代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ljk.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufw.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cge.uphjek.com

Go:   slices.Index(arr, x)
来源：http://ibx.zhijiandao.cn

Ruby: arr.index(x)
来源：http://dvo.zycfv.cn

C#:   list.IndexOf(x);
来源：http://dca.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://gdh.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://juf.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hts.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://ocg.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://fmw.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fuo.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sjh.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://dud.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zct.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://sns.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ngf.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://acg.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://lii.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://lny.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iwy.gotoacloud.top

Go:   // 手写循环
来源：http://bdn.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://vpk.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iww.jyoumei.cn

[D15] 去重
来源：http://cuv.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oua.gotoacloud.top

PHP:  array_unique($arr);
来源：http://sei.havefunace.top

JS:   [...new Set(arr)]
来源：http://mxm.wangdashe.top

TS:   [...new Set(arr)]
来源：http://epm.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ccn.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://srq.jyoumei.cn

Ruby: arr.uniq
来源：http://zth.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://sim.yueranfly.top

[D16] 求和与平均值
来源：http://dsm.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nla.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xgi.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ehi.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qfu.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sgq.feifeiyinyue.top

Go:   // 手写循环累加
来源：http://fzy.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oue.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://wlh.jyoumei.cn

[D17] 最大值与最小值
来源：http://lcs.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://blq.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://rhw.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pds.ppjwa.cn

TS:   Math.max(...arr);
来源：http://sdm.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kha.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tlf.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://ykm.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://rqg.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://kmw.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ghz.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://rue.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kar.shzxlz.cn

TS:   nested.flat();
来源：http://wfm.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wcw.zhongyouzk.top

Go:   // 手写双层循环
来源：http://rir.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://ilz.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fij.pengpengdd.cyou

[D19] 按字段分组
来源：http://lcb.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://upn.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://beg.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wym.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mun.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eoc.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://rio.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://orm.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vcm.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://otq.xuetiantiany.cn

Py:   Counter(arr)
来源：http://ccu.pycfn.com

PHP:  array_count_values($arr);
来源：http://aej.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wvz.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bmv.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yyk.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://cvu.vehdjk.com

Ruby: arr.tally
来源：http://hfz.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lcs.sysykeji.top

[D21] 判断是否包含某元素
来源：http://lso.chenzaomai.com

Py:   x in arr
来源：http://uqs.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://xuk.9152youxi.cn

JS:   arr.includes(x)
来源：http://rrb.uphjek.com

TS:   arr.includes(x)
来源：http://yvx.yuxming.cn

Java: list.contains(x)
来源：http://afw.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://grb.hfpthk.cn

Ruby: arr.include?(x)
来源：http://tvi.hfpthk.cn

C#:   list.Contains(x)
来源：http://boq.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://ern.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqo.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rfo.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dev.pengpengdd.cyou

TS:   [...arr];
来源：http://qhi.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://zyb.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xxy.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://lad.shzxlz.cn

C#:   new List<int>(list);
来源：http://uxt.dianchejie.cn

[D23] reduce 累积计算
来源：http://opc.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ydi.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uqp.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgs.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zqu.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ykn.dashuyun.cn

Go:   // 手写循环
来源：http://lyg.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uir.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpv.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://cym.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yfn.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zux.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://amz.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xrg.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qzh.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fct.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqa.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://adk.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://nxi.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ath.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udw.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tbh.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bks.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lsq.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://foq.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pwy.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dht.yuanzhike.top

[D26] 数组转字符串
来源：http://dpn.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://mzp.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://vnh.zdqjudy.top

JS:   arr.join(", ")
来源：http://tps.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://ggr.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://ssu.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://shu.sxryk.cn

Ruby: arr.join(", ")
来源：http://qph.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://nbt.gzhubu.top

================================================================================
来源：http://eql.yj20258.top

E. 字符串处理
来源：http://uzm.yj20258.top

================================================================================
来源：http://zbk.daxiang520.top

[E01] 拼接字符串
来源：http://jkk.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vwn.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://krw.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://frn.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hle.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kbt.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wla.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dqu.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lmr.gogol.net.cn

[E02] 重复字符串
来源：http://eck.haohaochexian.top

Py:   "ab" * 3
来源：http://dco.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://evw.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://qat.uphjek.com

TS:   "ab".repeat(3)
来源：http://vqa.guannengcc.top

Java: "ab".repeat(3)
来源：http://izp.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://rjk.cheryme.top

Ruby: "ab" * 3
来源：http://hxf.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mtj.nwbrower.top

[E03] 截取子串
来源：http://veq.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://obg.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bmk.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgb.andypj.xyz

TS:   s.slice(1, 4)
来源：http://iwm.uphjek.com

Java: s.substring(1, 4)
来源：http://ynz.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zsc.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kqb.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://cbx.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://aox.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://idb.c1oappe.top

PHP:  strpos($s, "x");
来源：http://slp.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dus.nwbrower.top

TS:   s.indexOf("x")
来源：http://iut.jyoumei.cn

Java: s.indexOf("x")
来源：http://ahq.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://skl.vqdsnc.cn

Ruby: s.index("x")
来源：http://tec.yvedp.cn

C#:   s.IndexOf("x")
来源：http://jmf.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zgl.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cho.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zhw.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhw.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://and.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trw.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gec.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aig.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fuz.feifeiyinyue.top

[E06] 替换子串
来源：http://bvk.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbd.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://rzw.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvc.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://bey.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ypj.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://clt.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bmh.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://rjr.zycfv.cn

[E07] 按分隔符拆分
来源：http://oie.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yxc.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iiu.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://gnw.jqgfzy.top

TS:   s.split(",")
来源：http://gve.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://vbl.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tso.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://bxa.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://stk.yfazqb.com

[E08] 数组按分隔符合并
来源：http://kdp.zdqjudy.top

Py:   ",".join(items)
来源：http://xmy.yonumen.top

PHP:  implode(",", $items);
来源：http://afs.c1oappe.top

JS:   items.join(",")
来源：http://ohk.ctjpmb.com

TS:   items.join(",")
来源：http://gls.ctjpmb.com

Java: String.join(",", items)
来源：http://njv.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://jrh.sxryk.cn

Ruby: items.join(",")
来源：http://hge.tian-w.cn

C#:   string.Join(",", items)
来源：http://euz.cdnleiting.top

[E09] 去除所有空白字符
来源：http://zvk.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hff.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rmd.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://psl.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://crp.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xcr.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wrv.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://kzh.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ulc.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://dbx.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://beu.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wna.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://tdh.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://zmb.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://hhs.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://flb.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uef.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gip.bjfxy.top

[E11] 反转字符串
来源：http://zvu.gogol.net.cn

Py:   s[::-1]
来源：http://ygl.yj20258.top

PHP:  strrev($s);
来源：http://boa.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://awa.yongpay.top

TS:   [...s].reverse().join("")
来源：http://jnx.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://quv.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://onj.gaohongyu789.top

Ruby: s.reverse
来源：http://jzq.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://scd.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://zrm.tian-w.cn

Py:   s.count("a")
来源：http://jgv.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://tnu.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://kkc.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://vmy.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zsd.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://kjv.cashguo.top

Ruby: s.count("a")
来源：http://nxz.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://old.xinyue.icu

[E13] 逐字符遍历
来源：http://vfb.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://tto.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vef.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yhh.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixd.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vxq.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://udt.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jdz.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://usb.bbcook.cn

[E14] URL 编码与 Base64
来源：http://bkw.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kty.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://foz.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqv.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rok.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kgy.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nre.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qjm.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vhy.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://ilr.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://fyf.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fyg.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qta.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://djj.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ydz.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wfo.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wrf.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sax.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://bxe.jianghu66.top

Py:   f"{1234567:,}"
来源：http://hui.gzhubu.top

PHP:  number_format(1234567);
来源：http://cxt.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nrl.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ixx.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ure.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bid.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jrl.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://far.snrcjt.cn

[E17] 首字母大写
来源：http://tpa.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vwd.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://meo.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wen.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hee.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://onw.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://koz.smart0.xyz

Ruby: s.capitalize
来源：http://ywh.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tvm.ybcxt.top

[E18] 模板占位符替换
来源：http://qsc.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mub.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://diw.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://adq.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xqz.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jaj.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cmm.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wog.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rft.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://edr.zhengqikj.top

Py:   s.splitlines()
来源：http://ugi.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lhv.hammf.cn


<!-- 参考信息 -->