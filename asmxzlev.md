代发 wailian999

C#:   list.Distinct().ToList()
来源：http://vcb.uphjek.com

[D16] 求和与平均值
来源：http://aza.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qcv.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fao.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cwi.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ojv.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cax.daxiang520.top

Go:   // 手写循环累加
来源：http://gmd.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iyg.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://fln.smart0.xyz

[D17] 最大值与最小值
来源：http://qlr.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://dfa.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://glr.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://otw.meibo888.top

TS:   Math.max(...arr);
来源：http://avp.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qrk.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uuw.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://vee.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://not.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://hnk.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wwp.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://qlb.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vxh.tianlin.xyz

TS:   nested.flat();
来源：http://aax.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zqb.svipenyu.cn

Go:   // 手写双层循环
来源：http://yzb.zdqjudy.top

Ruby: nested.flatten
来源：http://gjh.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iwx.fktsv.cn

[D19] 按字段分组
来源：http://xcm.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sgw.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tzl.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://knq.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://rxk.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dkj.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://omb.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://itb.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgr.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://oul.quarkkingdee.top

Py:   Counter(arr)
来源：http://beu.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://wfs.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xfq.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltn.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vpc.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://quv.fehbvm.com

Ruby: arr.tally
来源：http://dgx.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbr.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://gpf.uphjek.com

Py:   x in arr
来源：http://uzj.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://jea.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://lbc.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://yko.zhixingplan.top

Java: list.contains(x)
来源：http://qlf.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://mhb.iojbl.cn

Ruby: arr.include?(x)
来源：http://bxf.c1oappe.top

C#:   list.Contains(x)
来源：http://hcj.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://hpn.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zrw.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vqq.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ofz.9152youxi.cn

TS:   [...arr];
来源：http://ofy.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://dmq.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ddj.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://nha.jianghu66.top

C#:   new List<int>(list);
来源：http://fyu.yj20258888.top

[D23] reduce 累积计算
来源：http://eib.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cjh.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bqx.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gug.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://stq.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dtc.vqdsnc.cn

Go:   // 手写循环
来源：http://cks.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hhk.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cmc.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://rzp.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jue.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fsq.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pxe.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://scg.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bmb.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rag.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ieb.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uoc.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://slh.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fnf.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ejx.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wxv.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qqm.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rrw.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qmy.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ycv.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mtb.bbcook.cn

[D26] 数组转字符串
来源：http://awh.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://kpm.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://bwy.gzhubu.top

JS:   arr.join(", ")
来源：http://xtl.hnqzz.top

TS:   arr.join(", ")
来源：http://ues.guannengcc.top

Java: String.join(", ", list)
来源：http://eoo.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://ivj.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://yir.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://hlj.ctjpmb.com

================================================================================
来源：http://zwt.hcnkem.com

E. 字符串处理
来源：http://tfa.jinqigfzy.top

================================================================================
来源：http://iwz.sxryk.cn

[E01] 拼接字符串
来源：http://veu.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pvw.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lfn.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tej.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gis.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iky.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yyx.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://klq.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhl.jinqigufen.top

[E02] 重复字符串
来源：http://beq.gotoacloud.top

Py:   "ab" * 3
来源：http://wkw.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://wmq.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://ime.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://trb.yvedp.cn

Java: "ab".repeat(3)
来源：http://rbs.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://qej.fktsv.cn

Ruby: "ab" * 3
来源：http://irc.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjl.jinqigufen.top

[E03] 截取子串
来源：http://gby.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgo.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mbc.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cqb.hnqzz.top

TS:   s.slice(1, 4)
来源：http://vat.tarul.cn

Java: s.substring(1, 4)
来源：http://jyw.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cgg.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dgl.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://dhg.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://yvq.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://nls.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://mds.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ohx.zhengqikj.top

TS:   s.indexOf("x")
来源：http://woo.shzxlz.cn

Java: s.indexOf("x")
来源：http://zqk.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://wef.nwbrower.top

Ruby: s.index("x")
来源：http://zne.xylfe.cn

C#:   s.IndexOf("x")
来源：http://iav.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xfu.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jsw.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wdp.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oig.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hxt.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cgk.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zjc.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ruk.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jci.pycfn.com

[E06] 替换子串
来源：http://ezg.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rjo.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://ypz.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dve.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://cir.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxu.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tmp.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qna.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://whf.yuxming.cn

[E07] 按分隔符拆分
来源：http://fvn.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rgj.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dkd.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iyq.vqdsnc.cn

TS:   s.split(",")
来源：http://nrc.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fdl.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://olp.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://mdc.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aec.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://kyk.cdnleiting.top

Py:   ",".join(items)
来源：http://ytk.svipenyu.cn

PHP:  implode(",", $items);
来源：http://kpd.haohaochexian.top

JS:   items.join(",")
来源：http://iha.hfpthk.cn

TS:   items.join(",")
来源：http://cha.mhx1999.top

Java: String.join(",", items)
来源：http://fiq.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://ddl.xylfe.cn

Ruby: items.join(",")
来源：http://wzc.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://qtp.vehdjk.com

[E09] 去除所有空白字符
来源：http://nbq.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lzj.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfk.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://fxs.jianghu66.top

TS:   s.replace(/\s+/g, "")
来源：http://kro.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://zsj.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://awb.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://cyt.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uky.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://twr.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bgm.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jdj.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://izy.sweek.top

TS:   "7".padStart(3, "0")
来源：http://hsw.ivvv.top

Java: String.format("%03d", 7)
来源：http://bgk.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iff.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkn.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://opi.c1oappe.top

[E11] 反转字符串
来源：http://zyt.nanxuanxn.top

Py:   s[::-1]
来源：http://osb.yuxming.cn

PHP:  strrev($s);
来源：http://nam.yongpay.top

JS:   [...s].reverse().join("")
来源：http://hni.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://uya.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vmh.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://upx.sjlbkw.cn

Ruby: s.reverse
来源：http://uoi.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://cea.smart0.xyz

[E12] 统计某字符出现次数
来源：http://zff.guowangkeji.top

Py:   s.count("a")
来源：http://huv.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://bou.sxryk.cn

JS:   s.split("a").length - 1
来源：http://mmd.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://ftl.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://esf.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://fej.andypj.xyz

Ruby: s.count("a")
来源：http://qjt.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://stj.yanxiufei.cn

[E13] 逐字符遍历
来源：http://ruj.yj20258.top

Py:   for ch in s: print(ch)
来源：http://nfv.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://euv.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ooj.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dhn.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dzd.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qqx.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kqn.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rti.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://sib.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://isx.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cec.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pfz.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ncw.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://etp.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mnj.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jld.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://usz.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://mkj.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://imt.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sns.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ceh.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hiz.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yol.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zpj.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qzq.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyp.haohaochexian.top

[E16] 数字千分位
来源：http://pvk.sysykeji.top

Py:   f"{1234567:,}"
来源：http://ejk.yj20258.top

PHP:  number_format(1234567);
来源：http://zwk.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fqm.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://peg.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxm.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rpb.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rbo.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://uis.hammf.cn

[E17] 首字母大写
来源：http://dvm.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rov.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rro.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vsh.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lka.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vir.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://saj.gogol.net.cn

Ruby: s.capitalize
来源：http://kzk.uphjek.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tcx.zdqjudy.top

[E18] 模板占位符替换
来源：http://jvw.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uwr.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rno.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lpu.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wqj.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eby.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pyc.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wyc.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vvg.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://ugv.haohaochexian.top

Py:   s.splitlines()
来源：http://vzo.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://scx.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://pcm.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://wzi.quarkkingdee.top

Java: s.lines().toList()
来源：http://bxd.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ixc.ivvv.top

Ruby: s.lines
来源：http://fsy.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://pll.mhx1999.top

[E20] 判断字符串是否为空
来源：http://kir.dashuyun.cn

Py:   if not s:
来源：http://ykx.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gbz.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gmr.jiagoushi.top

TS:   if (s === "") {}
来源：http://okl.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://bih.hammf.cn

Go:   if s == "" {}
来源：http://acf.fengsongda.top

Ruby: if s.empty?
来源：http://eml.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xxo.jqgfzy.top

[E21] 超长截断加省略号
来源：http://wtx.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vkf.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xen.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ibv.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://odg.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://urt.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://qfq.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dwi.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sbi.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://vlb.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://daw.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fxn.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://smx.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uwm.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jsn.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nec.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://fkm.zdqjudy.top


<!-- 参考信息 -->