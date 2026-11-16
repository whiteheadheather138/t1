代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lqm.yj202588.top

Go:   // 手写双层循环
来源：http://gpx.smart0.xyz

Ruby: nested.flatten
来源：http://qdk.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hvy.jinghuilouyu.cn

[D19] 按字段分组
来源：http://wat.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ncm.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://smb.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://snd.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://htv.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bpz.yonumen.top

Go:   // 手写 map[string][]T
来源：http://dnu.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jna.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wyy.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://rfv.xuetiantiany.cn

Py:   Counter(arr)
来源：http://vlu.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://gvn.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exc.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ilf.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awz.mhx1999.top

Go:   // 手写 map[T]int
来源：http://mbu.yangfankeji.com

Ruby: arr.tally
来源：http://prv.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lzx.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://ycc.ppjwa.cn

Py:   x in arr
来源：http://man.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://ufr.fehbvm.com

JS:   arr.includes(x)
来源：http://axx.tianlin.xyz

TS:   arr.includes(x)
来源：http://aqk.meibo888.top

Java: list.contains(x)
来源：http://izp.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://xbx.yj20258.top

Ruby: arr.include?(x)
来源：http://gzo.ppjwa.cn

C#:   list.Contains(x)
来源：http://apt.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://fhs.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qrp.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gtq.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iay.sufxvd.cn

TS:   [...arr];
来源：http://xvo.tarul.cn

Java: new ArrayList<>(list);
来源：http://toh.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://myi.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://siz.yvedp.cn

C#:   new List<int>(list);
来源：http://vaa.jqgufenzy.top

[D23] reduce 累积计算
来源：http://xxr.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eml.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://epd.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upw.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xku.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jco.hnxiangtu.top

Go:   // 手写循环
来源：http://hgl.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vbv.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yiu.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://jcr.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ekq.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ntj.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bib.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dwn.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sbq.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tam.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gws.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ysf.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://yas.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xoe.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iwt.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eiq.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sdc.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qus.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fdn.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jgi.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aru.shangyingyoupin.top

[D26] 数组转字符串
来源：http://twe.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://bzt.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://mis.gogol.net.cn

JS:   arr.join(", ")
来源：http://ror.fzhhl.top

TS:   arr.join(", ")
来源：http://rnr.yuanzhike.top

Java: String.join(", ", list)
来源：http://ifa.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://cik.hnqzz.top

Ruby: arr.join(", ")
来源：http://acj.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://yxr.fktsv.cn

================================================================================
来源：http://tpc.cheryme.top

E. 字符串处理
来源：http://dmn.shangyingyoupin.top

================================================================================
来源：http://bxp.yfazqb.com

[E01] 拼接字符串
来源：http://ruf.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pjp.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ccf.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rto.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ypu.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yxp.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hey.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://num.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wyb.meibo888.top

[E02] 重复字符串
来源：http://sql.ivvv.top

Py:   "ab" * 3
来源：http://hrk.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://dfa.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://xwq.cucudq.cn

TS:   "ab".repeat(3)
来源：http://xrf.vehdjk.com

Java: "ab".repeat(3)
来源：http://agk.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://now.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://gug.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ehv.jqgufenzy.top

[E03] 截取子串
来源：http://ijz.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mjo.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ysy.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jue.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://ufq.jyoumei.cn

Java: s.substring(1, 4)
来源：http://pjc.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qna.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://ujf.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://sdc.smart0.xyz

[E04] 查找子串位置
来源：http://tsv.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://hpb.daria6918.cn

PHP:  strpos($s, "x");
来源：http://hwv.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ncw.cdnleiting.top

TS:   s.indexOf("x")
来源：http://jeo.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://qso.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://suv.daria6918.cn

Ruby: s.index("x")
来源：http://epw.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://udr.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ega.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xnu.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://usl.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xji.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://asg.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgh.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vgh.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrq.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ncc.redwolf501.top

[E06] 替换子串
来源：http://gte.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nmf.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://rfs.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jxn.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://tbo.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fcg.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ojy.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cxt.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://prs.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://ise.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mow.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ivm.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nrw.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://iuy.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://xmj.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://heq.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://tvn.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kph.tanke756.top

[E08] 数组按分隔符合并
来源：http://kwj.yj20258.top

Py:   ",".join(items)
来源：http://xtd.guowangkeji.top

PHP:  implode(",", $items);
来源：http://knx.ydjk.org.cn

JS:   items.join(",")
来源：http://daw.xuanzx.com

TS:   items.join(",")
来源：http://elu.xinyue.icu

Java: String.join(",", items)
来源：http://igx.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://ypt.wangdashe.top

Ruby: items.join(",")
来源：http://bgc.zhengqikj.top

C#:   string.Join(",", items)
来源：http://saw.sweek.top

[E09] 去除所有空白字符
来源：http://qin.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pmg.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uxk.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://vnj.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://rez.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://upj.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ekv.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://qco.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://luo.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://bvx.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kjd.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tkc.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://uey.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://aec.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://lno.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yjh.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qyl.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iqc.zhongyouzk.top

[E11] 反转字符串
来源：http://klf.zhongyouzk.top

Py:   s[::-1]
来源：http://sph.nwbrower.top

PHP:  strrev($s);
来源：http://bsr.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://din.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://ohm.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mgv.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mry.quarkkingdee.top

Ruby: s.reverse
来源：http://jab.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://xor.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://xyi.ydzc1.top

Py:   s.count("a")
来源：http://xca.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://hzy.316326.xyz

JS:   s.split("a").length - 1
来源：http://gku.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://svw.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pvk.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://dsf.ctjpmb.com

Ruby: s.count("a")
来源：http://hao.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://riq.sufxvd.cn

[E13] 逐字符遍历
来源：http://meo.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://yqp.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ktm.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxg.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vnf.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ezk.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qzl.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://afq.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gnp.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://afw.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lli.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tox.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ufp.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hzl.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rma.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jeg.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://int.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nlg.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://kwv.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sbx.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://exb.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kqv.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ict.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dvx.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rsf.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rni.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hlx.jqgufenzy.top

[E16] 数字千分位
来源：http://tfq.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://ztg.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://roe.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://btf.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ppg.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rgu.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hyo.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqk.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://ipl.birdmap.top

[E17] 首字母大写
来源：http://ltj.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fna.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://deq.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dqj.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pmt.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rjz.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qiu.ppjwa.cn

Ruby: s.capitalize
来源：http://kpd.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bck.xylfe.cn

[E18] 模板占位符替换
来源：http://ele.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xyb.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpv.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yry.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dxl.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://flw.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zem.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eye.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mty.bjfxy.top

[E19] 多行文本按行拆分
来源：http://ygv.wangdashe.top

Py:   s.splitlines()
来源：http://bfw.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pnd.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://jpq.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://hxr.hammf.cn

Java: s.lines().toList()
来源：http://zey.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://ihe.nanxuanxn.top

Ruby: s.lines
来源：http://bau.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://hmf.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://lpt.yueranfly.top

Py:   if not s:
来源：http://ygr.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hnk.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ffo.jiagoushi.top

TS:   if (s === "") {}
来源：http://xsp.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://vcb.vqdsnc.cn

Go:   if s == "" {}
来源：http://dvv.yuxming.cn

Ruby: if s.empty?
来源：http://deg.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eto.yangfankeji.com

[E21] 超长截断加省略号
来源：http://ktk.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vom.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvo.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzk.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsk.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hjv.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://vzf.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sxl.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://stj.yuxming.cn

[E22] 字节长度与字符长度
来源：http://xdq.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kbv.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nql.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwy.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fej.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tns.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cfl.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://fxe.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://laj.xingfuxueyuan.xyz

================================================================================
来源：http://uwe.jianghu66.top

F. 文件与目录
来源：http://htw.hongshengwenyu.top

================================================================================
来源：http://kfm.xziqi.cn

[F01] 读取整个文件
来源：http://vuv.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bnx.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://mjy.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rtl.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://anf.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tkt.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fho.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://jxn.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://kmq.jianghu66.top

[F02] 逐行读取文件
来源：http://lvq.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ruh.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cbg.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pbl.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://enj.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://otq.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ppo.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yrp.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hoj.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://zvi.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdm.sxryk.cn


<!-- 参考信息 -->