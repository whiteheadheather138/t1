代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyi.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://pir.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://mbf.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://ppo.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hnu.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ndn.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://jkw.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://cga.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ygf.fengsongda.top

Go:   // 手写循环
来源：http://opg.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://zgc.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aso.aizwys.cn

[D15] 去重
来源：http://ffx.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mkg.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://gdc.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://ahx.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://rik.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rif.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tjo.gotoacloud.top

Ruby: arr.uniq
来源：http://zoz.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://fbh.jyoumei.cn

[D16] 求和与平均值
来源：http://gpe.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rcj.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://deo.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydl.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pdv.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dio.yonumen.top

Go:   // 手写循环累加
来源：http://jfd.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://spf.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://oyr.yj20258888.top

[D17] 最大值与最小值
来源：http://gos.hammf.cn

Py:   max(arr);  min(arr)
来源：http://ntu.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://auz.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ozy.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://qzh.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zlp.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsy.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://pxc.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://aos.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://aee.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yvz.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://ett.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jvd.iojbl.cn

TS:   nested.flat();
来源：http://mfs.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ogu.316326.xyz

Go:   // 手写双层循环
来源：http://hhn.yvedp.cn

Ruby: nested.flatten
来源：http://goj.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ezh.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://rsa.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zhz.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cbc.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kqm.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uoj.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fap.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://fbz.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwv.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lur.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://olm.hesvh.cn

Py:   Counter(arr)
来源：http://ufs.sysykeji.top

PHP:  array_count_values($arr);
来源：http://cjy.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pom.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzw.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fqv.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://khg.yj202588.top

Ruby: arr.tally
来源：http://oya.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qel.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://qsm.hywenlv.cn

Py:   x in arr
来源：http://xkf.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://ozl.gzhubu.top

JS:   arr.includes(x)
来源：http://ocg.gaohongyu789.top

TS:   arr.includes(x)
来源：http://eya.fehbvm.com

Java: list.contains(x)
来源：http://ocd.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://glo.cashguo.top

Ruby: arr.include?(x)
来源：http://wvq.tian-w.cn

C#:   list.Contains(x)
来源：http://yxv.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://fho.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wtm.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pys.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jqe.yongpay.top

TS:   [...arr];
来源：http://vmj.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://isp.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ezr.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ahx.redwolf501.top

C#:   new List<int>(list);
来源：http://dvo.yonumen.top

[D23] reduce 累积计算
来源：http://tnf.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ats.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aaa.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbs.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xox.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://nrl.9152youxi.cn

Go:   // 手写循环
来源：http://pfj.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rph.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vuk.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://uah.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bwl.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gcb.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbg.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nrr.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rmv.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kai.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dpu.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hbc.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://rfv.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ooo.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://amm.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ioh.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://afv.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ziu.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://onq.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ohf.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zop.hesvh.cn

[D26] 数组转字符串
来源：http://nyw.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://zkc.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://xej.cdnleiting.top

JS:   arr.join(", ")
来源：http://bxq.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://qig.hywenlv.cn

Java: String.join(", ", list)
来源：http://ari.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://wmm.hywenlv.cn

Ruby: arr.join(", ")
来源：http://qav.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://bgf.52xcode.cn

================================================================================
来源：http://bid.hongshengwenyu.top

E. 字符串处理
来源：http://tbq.jianghu66.top

================================================================================
来源：http://xum.zhoulong.xyz

[E01] 拼接字符串
来源：http://hdg.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bmw.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ldi.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kiu.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dso.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mlh.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hxq.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zsc.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bwq.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://ggn.bjfxy.top

Py:   "ab" * 3
来源：http://uxw.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://ntq.tian-w.cn

JS:   "ab".repeat(3)
来源：http://evl.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://bat.sysykeji.top

Java: "ab".repeat(3)
来源：http://jlu.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://khg.zhengqikj.top

Ruby: "ab" * 3
来源：http://cpv.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sis.iojbl.cn

[E03] 截取子串
来源：http://gob.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cbs.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mqf.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rsr.fktsv.cn

TS:   s.slice(1, 4)
来源：http://pfu.52xcode.cn

Java: s.substring(1, 4)
来源：http://lgh.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lhn.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fcb.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://gvp.bjfxy.top

[E04] 查找子串位置
来源：http://lnm.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://wdv.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://nfs.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xyc.uphjek.com

TS:   s.indexOf("x")
来源：http://wst.smart0.xyz

Java: s.indexOf("x")
来源：http://gjt.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://str.gogol.net.cn

Ruby: s.index("x")
来源：http://hcp.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://xeg.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vio.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hrv.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yby.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sib.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ojy.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aum.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hsg.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zie.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://byd.wangshuangyany.cn

[E06] 替换子串
来源：http://jnu.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zgo.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://sow.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ddi.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://wwl.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayi.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mwq.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://owq.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://noi.ehwqpu.com

[E07] 按分隔符拆分
来源：http://frf.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ubz.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uoc.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://epu.tian-w.cn

TS:   s.split(",")
来源：http://ltn.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cyv.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mls.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://npn.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vmy.daxiang520.top

[E08] 数组按分隔符合并
来源：http://aka.birdmap.top

Py:   ",".join(items)
来源：http://owi.cashguo.top

PHP:  implode(",", $items);
来源：http://zoq.vqdsnc.cn

JS:   items.join(",")
来源：http://nch.sweek.top

TS:   items.join(",")
来源：http://qjk.aizwys.cn

Java: String.join(",", items)
来源：http://chh.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://knt.52xcode.cn

Ruby: items.join(",")
来源：http://qsw.iojbl.cn

C#:   string.Join(",", items)
来源：http://qlt.ppjwa.cn

[E09] 去除所有空白字符
来源：http://wkf.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://olc.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hge.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://bks.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://oqi.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://zud.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mda.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://inq.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sol.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://psl.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ydy.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://prw.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://car.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://ehu.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://sbn.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hij.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kji.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eva.zhijiandao.cn

[E11] 反转字符串
来源：http://hlx.jinghuilouyu.cn

Py:   s[::-1]
来源：http://hnc.guannengcc.top

PHP:  strrev($s);
来源：http://rvi.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://uqz.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://suq.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cqs.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kkx.jyoumei.cn

Ruby: s.reverse
来源：http://euv.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nra.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://gkb.redwolf501.top

Py:   s.count("a")
来源：http://trf.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://ttq.aizwys.cn

JS:   s.split("a").length - 1
来源：http://fxd.nwbrower.top

TS:   s.split("a").length - 1
来源：http://pse.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cbq.316326.xyz

Go:   strings.Count(s, "a")
来源：http://lbp.tian-w.cn

Ruby: s.count("a")
来源：http://ebo.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://mkg.zdbjq.cn

[E13] 逐字符遍历
来源：http://mak.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://sts.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cob.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rxo.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://kno.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cwz.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zjc.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://eon.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://odg.cucudq.cn

[E14] URL 编码与 Base64
来源：http://rum.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bck.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://huf.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rxm.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://isv.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zfq.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rbd.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cji.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dsy.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://ewe.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://cob.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tcq.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://csv.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cco.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wia.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ynt.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xnu.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zzn.andypj.xyz

[E16] 数字千分位
来源：http://zjn.xylfe.cn

Py:   f"{1234567:,}"
来源：http://xyq.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://hmu.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tks.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://num.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xql.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://grs.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ycx.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://tex.hnqzz.top

[E17] 首字母大写
来源：http://glb.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mpq.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hbl.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://weq.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tst.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qaa.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wri.guannengcc.top

Ruby: s.capitalize
来源：http://tjj.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://irf.sxryk.cn

[E18] 模板占位符替换
来源：http://xlk.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lgt.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://njw.sweek.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qnd.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gvk.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aub.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lln.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fst.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nim.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://qmg.hfpthk.cn

Py:   s.splitlines()
来源：http://xmn.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://alk.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://wdl.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://gii.yfazqb.com

Java: s.lines().toList()
来源：http://uoc.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://jdx.wangshuangyany.cn

Ruby: s.lines
来源：http://hfh.hysaishi.cn

C#:   s.Split('\n')
来源：http://fzg.havefunace.top

[E20] 判断字符串是否为空
来源：http://ucx.sxryk.cn

Py:   if not s:
来源：http://rgq.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ytt.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://njq.pycfn.com

TS:   if (s === "") {}
来源：http://gxg.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://mwr.guannengcc.top


<!-- 参考信息 -->