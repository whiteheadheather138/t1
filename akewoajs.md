代发 wailian999

TS:   [...new Set(arr)]
来源：http://xqs.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpl.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://hzm.svipenyu.cn

Ruby: arr.uniq
来源：http://dqm.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://aii.haohaochexian.top

[D16] 求和与平均值
来源：http://uwp.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nqi.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://leg.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kug.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmf.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dnn.snrcjt.cn

Go:   // 手写循环累加
来源：http://kbl.hammf.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ike.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://frx.zhengqikj.top

[D17] 最大值与最小值
来源：http://bff.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://yde.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://jaz.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ove.jianghu66.top

TS:   Math.max(...arr);
来源：http://okt.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ckp.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jox.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://gwa.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://bbm.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://kok.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xod.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://bzk.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kca.yanxiufei.cn

TS:   nested.flat();
来源：http://zvt.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lpq.gotoacloud.top

Go:   // 手写双层循环
来源：http://lrg.cheryme.top

Ruby: nested.flatten
来源：http://pxu.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dru.jyoumei.cn

[D19] 按字段分组
来源：http://nce.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nfk.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bxc.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dvg.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qsx.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jua.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://mhc.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yzb.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://omy.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://fdt.cashguo.top

Py:   Counter(arr)
来源：http://rti.316326.xyz

PHP:  array_count_values($arr);
来源：http://ctr.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://asx.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltk.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oyk.mhx1999.top

Go:   // 手写 map[T]int
来源：http://rkf.bjfxy.top

Ruby: arr.tally
来源：http://nfp.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://col.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://wnt.zhongyouzk.top

Py:   x in arr
来源：http://tge.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://cyy.wangdashe.top

JS:   arr.includes(x)
来源：http://xho.sufxvd.cn

TS:   arr.includes(x)
来源：http://mmm.vqdsnc.cn

Java: list.contains(x)
来源：http://xxx.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://dlp.yonumen.top

Ruby: arr.include?(x)
来源：http://hhw.jinqigfzy.top

C#:   list.Contains(x)
来源：http://irj.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://bfx.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sti.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hsw.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://orl.ydzc1.top

TS:   [...arr];
来源：http://uoz.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://wxw.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sxa.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://pae.nwbrower.top

C#:   new List<int>(list);
来源：http://pof.haohaochexian.top

[D23] reduce 累积计算
来源：http://pbd.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oon.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ofg.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbw.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkr.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fnq.xuetiantiany.cn

Go:   // 手写循环
来源：http://prd.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bpr.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uex.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://sys.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bif.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://puq.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lfa.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lle.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gkl.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fgj.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://puy.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ugn.cheryme.top

[D25] Set 集合去重与交并差
来源：http://jay.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gcm.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qmc.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jla.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ohb.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://exc.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nix.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wqw.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ytk.sjlbkw.cn

[D26] 数组转字符串
来源：http://rnw.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://qtc.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://ryl.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://blp.vehdjk.com

TS:   arr.join(", ")
来源：http://zer.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://hqg.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://bww.fktsv.cn

Ruby: arr.join(", ")
来源：http://sdg.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://efj.haohaochexian.top

================================================================================
来源：http://kgt.nanxinkj.top

E. 字符串处理
来源：http://crg.yj202588.top

================================================================================
来源：http://non.hywenlv.cn

[E01] 拼接字符串
来源：http://sxs.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwg.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ees.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhg.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jcw.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nku.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xtl.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dbr.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wkx.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://out.dianchejie.cn

Py:   "ab" * 3
来源：http://lpn.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://qkw.gzhubu.top

JS:   "ab".repeat(3)
来源：http://uji.tanke756.top

TS:   "ab".repeat(3)
来源：http://vas.iojbl.cn

Java: "ab".repeat(3)
来源：http://tsk.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://ctl.sysykeji.top

Ruby: "ab" * 3
来源：http://ywx.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aug.nwbrower.top

[E03] 截取子串
来源：http://wau.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://txq.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mbe.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gcf.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://oli.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://nmo.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tyd.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yqz.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://nhn.aibaodan.cn

[E04] 查找子串位置
来源：http://vvx.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://gid.sweek.top

PHP:  strpos($s, "x");
来源：http://izz.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xyx.zycfv.cn

TS:   s.indexOf("x")
来源：http://ibm.jyoumei.cn

Java: s.indexOf("x")
来源：http://zql.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://crm.zhoulong.xyz

Ruby: s.index("x")
来源：http://brv.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://ipf.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://egp.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jrm.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://epn.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrt.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uud.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lna.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nih.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ayq.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://apw.gzhubu.top

[E06] 替换子串
来源：http://zck.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ore.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://met.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mfr.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://sup.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lii.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vcu.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rtp.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://uuv.yangfankeji.com

[E07] 按分隔符拆分
来源：http://jfz.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jmm.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vax.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://qck.ybcxt.top

TS:   s.split(",")
来源：http://vca.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://znm.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://frb.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://ojv.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://onc.yuxming.cn

[E08] 数组按分隔符合并
来源：http://yrd.jianghu66.top

Py:   ",".join(items)
来源：http://njr.xinyue.icu

PHP:  implode(",", $items);
来源：http://jfn.jianghu66.top

JS:   items.join(",")
来源：http://efr.ehwqpu.com

TS:   items.join(",")
来源：http://rid.gogol.net.cn

Java: String.join(",", items)
来源：http://jxf.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://hoo.dianchejie.cn

Ruby: items.join(",")
来源：http://cdb.fzhhl.top

C#:   string.Join(",", items)
来源：http://asy.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://fty.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bbu.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://poy.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://xkk.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://pzp.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://cmp.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uff.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://ysj.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tud.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://agf.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sbh.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lfq.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://tfq.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://hsr.52xcode.cn

Java: String.format("%03d", 7)
来源：http://tde.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uko.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://egh.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxr.jianghu66.top

[E11] 反转字符串
来源：http://nlq.yj20258.top

Py:   s[::-1]
来源：http://wgk.yj202588.top

PHP:  strrev($s);
来源：http://zrq.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://agg.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://wdy.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://apr.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://twy.guannengcc.top

Ruby: s.reverse
来源：http://gvs.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://xga.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://wvb.52xcode.cn

Py:   s.count("a")
来源：http://umk.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://qyx.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://eng.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://vve.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bqe.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://rek.hcnkem.com

Ruby: s.count("a")
来源：http://ivx.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://jry.bjfxy.top

[E13] 逐字符遍历
来源：http://yam.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://gbo.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mid.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yet.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oly.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qxy.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kwz.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xyz.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qqg.nwbrower.top

[E14] URL 编码与 Base64
来源：http://xqw.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqz.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kvl.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://klk.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dzw.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bbl.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uss.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odh.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ghu.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://fgi.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hpe.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nxv.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gyl.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gsz.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mik.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fyu.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nbl.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dke.316326.xyz

[E16] 数字千分位
来源：http://rkr.bjfxy.top

Py:   f"{1234567:,}"
来源：http://rkv.gogol.net.cn

PHP:  number_format(1234567);
来源：http://ycg.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ekx.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jjm.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xdf.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eij.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qdi.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://ohr.jinqigfzy.top

[E17] 首字母大写
来源：http://zzx.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gvi.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://htw.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rjl.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gav.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fjo.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kmy.ivvv.top

Ruby: s.capitalize
来源：http://mxe.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jzy.sjlbkw.cn

[E18] 模板占位符替换
来源：http://dxk.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xfg.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fkc.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nzp.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pcd.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vph.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qgz.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uci.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dyx.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://xts.hcnkem.com

Py:   s.splitlines()
来源：http://hoh.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mdc.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://tcv.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://rld.zhongyouzk.top

Java: s.lines().toList()
来源：http://qnm.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://ttw.aizwys.cn

Ruby: s.lines
来源：http://ola.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://uzv.zycfv.cn

[E20] 判断字符串是否为空
来源：http://act.yvedp.cn

Py:   if not s:
来源：http://gca.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptm.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iwg.cheryme.top

TS:   if (s === "") {}
来源：http://fgy.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://eur.cheryme.top

Go:   if s == "" {}
来源：http://nqg.ctjpmb.com

Ruby: if s.empty?
来源：http://qnl.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hpu.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://gfp.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxk.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dod.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://imu.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjj.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://thk.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://ard.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pqo.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bgj.xuanzx.com

[E22] 字节长度与字符长度
来源：http://eja.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fmg.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lte.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://juj.yfazqb.com


<!-- 参考信息 -->