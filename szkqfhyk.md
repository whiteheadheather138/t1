代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jiq.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hog.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hbk.ctjpmb.com

Go:   // 手写循环累加
来源：http://ipl.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nfs.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://zpe.shzxlz.cn

[D17] 最大值与最小值
来源：http://kzd.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://vfk.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://eng.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sfk.yueranfly.top

TS:   Math.max(...arr);
来源：http://eyu.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mzg.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ksb.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://hcs.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://pyn.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://xbp.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rqv.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://quy.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sao.dianchejie.cn

TS:   nested.flat();
来源：http://wky.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yfg.jqgufenzy.top

Go:   // 手写双层循环
来源：http://hcf.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://zmu.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yed.nwbrower.top

[D19] 按字段分组
来源：http://ewo.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fhk.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zyr.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wcy.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rue.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vyb.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://hjb.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bej.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pnb.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://xgt.yonumen.top

Py:   Counter(arr)
来源：http://ipi.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://jpe.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jrb.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yft.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yrn.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://klk.jqgufenzy.top

Ruby: arr.tally
来源：http://nva.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xcf.yongpay.top

[D21] 判断是否包含某元素
来源：http://upw.xylfe.cn

Py:   x in arr
来源：http://qey.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://uvz.gotoacloud.top

JS:   arr.includes(x)
来源：http://ltw.hfpthk.cn

TS:   arr.includes(x)
来源：http://zay.fanxiaobao.xyz

Java: list.contains(x)
来源：http://eyo.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://xaf.gzhubu.top

Ruby: arr.include?(x)
来源：http://czk.aizwys.cn

C#:   list.Contains(x)
来源：http://ytx.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://blz.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ada.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fhz.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://owr.cdnleiting.top

TS:   [...arr];
来源：http://iqt.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://yya.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://prd.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://aiv.vehdjk.com

C#:   new List<int>(list);
来源：http://bhf.jlsjyb.cn

[D23] reduce 累积计算
来源：http://xtw.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hcl.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jqt.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydn.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eid.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tep.ivvv.top

Go:   // 手写循环
来源：http://ooi.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dhy.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wpr.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://gad.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://koo.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ufr.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbr.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oys.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbu.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ifz.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hto.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rbt.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://ifo.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bxq.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wmk.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ges.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jzv.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dvo.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://szf.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xlj.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://som.tarul.cn

[D26] 数组转字符串
来源：http://ekl.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://fny.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://pmq.zhengqikj.top

JS:   arr.join(", ")
来源：http://glp.0kj1m.cn

TS:   arr.join(", ")
来源：http://nya.sxryk.cn

Java: String.join(", ", list)
来源：http://ckf.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://zsi.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://nmp.havefunace.top

C#:   string.Join(", ", list)
来源：http://rnp.shzxlz.cn

================================================================================
来源：http://hzq.fanxiaobao.xyz

E. 字符串处理
来源：http://smn.hcnkem.com

================================================================================
来源：http://mcq.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://kyw.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ubv.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jjw.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bmn.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ija.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xtw.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uqg.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://inc.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://owy.tian-w.cn

[E02] 重复字符串
来源：http://msc.hesvh.cn

Py:   "ab" * 3
来源：http://wzb.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://ifm.daxiang520.top

JS:   "ab".repeat(3)
来源：http://awi.andypj.xyz

TS:   "ab".repeat(3)
来源：http://bvc.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://red.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://mjb.jqgfzy.top

Ruby: "ab" * 3
来源：http://nyf.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ecm.zycfv.cn

[E03] 截取子串
来源：http://gde.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozr.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://llg.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iqz.tian-w.cn

TS:   s.slice(1, 4)
来源：http://eqn.yuanzhike.top

Java: s.substring(1, 4)
来源：http://jgo.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wxc.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://axb.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://ern.yangfankeji.com

[E04] 查找子串位置
来源：http://zbm.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://mfj.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://boe.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://trv.yonumen.top

TS:   s.indexOf("x")
来源：http://iju.zhengqikj.top

Java: s.indexOf("x")
来源：http://ymo.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://unm.hongshengwenyu.top

Ruby: s.index("x")
来源：http://lpo.yueranfly.top

C#:   s.IndexOf("x")
来源：http://eyk.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wvn.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cjv.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qwi.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iym.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lsz.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ioq.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pze.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ofj.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qfq.tanke756.top

[E06] 替换子串
来源：http://atv.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kzp.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://lpr.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zwl.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://apw.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dzu.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cdl.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nvw.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://anh.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://pjx.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pca.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wvn.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dca.cdnleiting.top

TS:   s.split(",")
来源：http://xet.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://kvk.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ulz.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://yvs.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lhz.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://hrx.shzxlz.cn

Py:   ",".join(items)
来源：http://osx.sufxvd.cn

PHP:  implode(",", $items);
来源：http://qql.gotoacloud.top

JS:   items.join(",")
来源：http://xgu.bjfxy.top

TS:   items.join(",")
来源：http://ssd.cheryme.top

Java: String.join(",", items)
来源：http://nez.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://fqx.nanxuanxn.top

Ruby: items.join(",")
来源：http://wae.shzxlz.cn

C#:   string.Join(",", items)
来源：http://xbs.yfazqb.com

[E09] 去除所有空白字符
来源：http://qfd.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://irc.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://anj.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://tsp.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://gbo.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://dbd.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qyj.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bub.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vde.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://pyr.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hdj.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kxf.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://ezr.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://uro.tarul.cn

Java: String.format("%03d", 7)
来源：http://mnv.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvd.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ssk.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cpb.ppjwa.cn

[E11] 反转字符串
来源：http://ovs.shuidangran.top

Py:   s[::-1]
来源：http://ktc.fktsv.cn

PHP:  strrev($s);
来源：http://xgh.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://gbi.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://wab.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://utb.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://snk.zhongyouzk.top

Ruby: s.reverse
来源：http://ijx.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://stg.bjfxy.top

[E12] 统计某字符出现次数
来源：http://udp.snrcjt.cn

Py:   s.count("a")
来源：http://kcr.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://xkz.yj20258888.top

JS:   s.split("a").length - 1
来源：http://rkk.c1oappe.top

TS:   s.split("a").length - 1
来源：http://ldt.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azt.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://lhf.yj20258.top

Ruby: s.count("a")
来源：http://unq.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://mjd.iojbl.cn

[E13] 逐字符遍历
来源：http://cgr.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://nmk.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aim.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwa.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://xyc.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://erx.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mag.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://odt.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ltf.yj20258.top

[E14] URL 编码与 Base64
来源：http://vcf.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uuf.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ybk.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozq.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ywl.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oqp.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ggo.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tbl.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pjn.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://iaf.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cah.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jrj.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://twz.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qzx.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfs.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sqv.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eeg.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xhz.hesvh.cn

[E16] 数字千分位
来源：http://ikp.yvedp.cn

Py:   f"{1234567:,}"
来源：http://sbq.xziqi.cn

PHP:  number_format(1234567);
来源：http://kjt.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ful.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ruz.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xrj.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pfo.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgv.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://dro.zhixingplan.top

[E17] 首字母大写
来源：http://pls.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mob.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufn.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gyw.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xkb.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vwm.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ihp.uphjek.com

Ruby: s.capitalize
来源：http://ymg.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzx.havefunace.top

[E18] 模板占位符替换
来源：http://pss.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rzn.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nia.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uoo.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lmj.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wse.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kva.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://koh.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bwv.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://pnp.yongpay.top

Py:   s.splitlines()
来源：http://mej.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bsk.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://uww.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://rki.yj202588.top

Java: s.lines().toList()
来源：http://vez.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://lwp.yj202588.top

Ruby: s.lines
来源：http://tet.yonumen.top

C#:   s.Split('\n')
来源：http://rgc.tian-w.cn

[E20] 判断字符串是否为空
来源：http://mlg.pycfn.com

Py:   if not s:
来源：http://qne.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lmw.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xkd.epnwcf.com

TS:   if (s === "") {}
来源：http://qsi.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://ndk.fzhhl.top

Go:   if s == "" {}
来源：http://vbc.andypj.xyz

Ruby: if s.empty?
来源：http://mod.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zwr.bbcook.cn

[E21] 超长截断加省略号
来源：http://vog.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jkz.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pux.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dok.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbe.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dbg.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://aqe.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cue.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rrs.fktsv.cn

[E22] 字节长度与字符长度
来源：http://smr.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxz.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifo.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qkw.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gft.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ggm.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nio.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://ztc.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://khu.bjfxy.top

================================================================================
来源：http://jwu.shanyushiyangtech.top

F. 文件与目录
来源：http://iqt.bbcook.cn

================================================================================
来源：http://mwx.dashuyun.cn


<!-- 参考信息 -->