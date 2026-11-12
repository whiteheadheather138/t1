代发 wailian999

[D19] 按字段分组
来源：http://erb.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tff.chenjidiqi.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pyp.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vbc.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://njk.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kol.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://epp.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lnu.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nij.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://rre.sweek.top

Py:   Counter(arr)
来源：http://jux.ybcxt.top

PHP:  array_count_values($arr);
来源：http://puq.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://arj.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://evg.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ynb.uphjek.com

Go:   // 手写 map[T]int
来源：http://ebr.jianghu66.top

Ruby: arr.tally
来源：http://cwr.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mde.gzhubu.top

[D21] 判断是否包含某元素
来源：http://mfr.52xcode.cn

Py:   x in arr
来源：http://kaf.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://whm.yangfankeji.com

JS:   arr.includes(x)
来源：http://fke.gzhubu.top

TS:   arr.includes(x)
来源：http://asj.yuxming.cn

Java: list.contains(x)
来源：http://ses.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://ffr.hesvh.cn

Ruby: arr.include?(x)
来源：http://bxs.haohaochexian.top

C#:   list.Contains(x)
来源：http://oqg.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://eya.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tro.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dyk.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://glx.cucudq.cn

TS:   [...arr];
来源：http://fyr.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://uni.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://oyu.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://ick.316326.xyz

C#:   new List<int>(list);
来源：http://yjm.yj202588.top

[D23] reduce 累积计算
来源：http://var.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://juk.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zuj.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://odh.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqr.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ubz.xuetiantiany.cn

Go:   // 手写循环
来源：http://gha.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ubt.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://skf.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://jzg.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oag.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cub.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wlr.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ech.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bpn.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gvs.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://msu.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cxk.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://hvz.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gmg.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dvs.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sro.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vge.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zxr.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rwi.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tbh.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ddo.jinqigufen.top

[D26] 数组转字符串
来源：http://ccl.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://vjj.havefunace.top

PHP:  implode(", ", $arr);
来源：http://tlh.jqgufenzy.top

JS:   arr.join(", ")
来源：http://lcv.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://das.iojbl.cn

Java: String.join(", ", list)
来源：http://kpn.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://imo.redwolf501.top

Ruby: arr.join(", ")
来源：http://qzu.sxryk.cn

C#:   string.Join(", ", list)
来源：http://axw.bjfxy.top

================================================================================
来源：http://vln.snrcjt.cn

E. 字符串处理
来源：http://lts.andypj.xyz

================================================================================
来源：http://apr.fengsongda.top

[E01] 拼接字符串
来源：http://asx.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ulx.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dpv.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ffe.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmt.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tem.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pwa.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dtf.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gxn.tian-w.cn

[E02] 重复字符串
来源：http://oup.ehwqpu.com

Py:   "ab" * 3
来源：http://mtl.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://xcm.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://evf.ivvv.top

TS:   "ab".repeat(3)
来源：http://lnm.havefunace.top

Java: "ab".repeat(3)
来源：http://ytk.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://fqg.ppjwa.cn

Ruby: "ab" * 3
来源：http://cvb.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fza.quarkkingdee.top

[E03] 截取子串
来源：http://hvt.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gdy.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fun.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nkd.sysykeji.top

TS:   s.slice(1, 4)
来源：http://gbq.jqgfzy.top

Java: s.substring(1, 4)
来源：http://rit.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jjy.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gzl.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://gnu.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://zuj.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://fwx.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://kxh.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vvt.daria6918.cn

TS:   s.indexOf("x")
来源：http://tao.vehdjk.com

Java: s.indexOf("x")
来源：http://vox.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://bhd.ydjk.org.cn

Ruby: s.index("x")
来源：http://cph.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://yts.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vcu.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mja.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ahi.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dlq.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfk.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://icd.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zje.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://csf.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gno.hammf.cn

[E06] 替换子串
来源：http://ehz.0kj1m.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tbk.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://gde.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnc.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://nyk.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcg.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oad.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cng.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://drx.snrcjt.cn

[E07] 按分隔符拆分
来源：http://klr.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lgg.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uyj.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyr.hysaishi.cn

TS:   s.split(",")
来源：http://kvv.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://afa.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wzn.birdmap.top

Ruby: s.split(",");  s.split
来源：http://uac.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sss.yj202588.top

[E08] 数组按分隔符合并
来源：http://axt.hnqzz.top

Py:   ",".join(items)
来源：http://ccq.andypj.xyz

PHP:  implode(",", $items);
来源：http://unw.ydjk.org.cn

JS:   items.join(",")
来源：http://tsf.epnwcf.com

TS:   items.join(",")
来源：http://eij.snrcjt.cn

Java: String.join(",", items)
来源：http://dhi.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://gqh.birdmap.top

Ruby: items.join(",")
来源：http://lse.shzxlz.cn

C#:   string.Join(",", items)
来源：http://qcb.havefunace.top

[E09] 去除所有空白字符
来源：http://npc.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://epc.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyx.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://naf.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://cbe.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://grh.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ejk.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://jig.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jiw.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://zfd.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uvx.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mbe.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://baz.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://qbc.meibo888.top

Java: String.format("%03d", 7)
来源：http://aca.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cnk.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://svk.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gca.cheryme.top

[E11] 反转字符串
来源：http://mgh.cheryme.top

Py:   s[::-1]
来源：http://ron.meibo888.top

PHP:  strrev($s);
来源：http://gwo.316326.xyz

JS:   [...s].reverse().join("")
来源：http://fxf.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://meu.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zgp.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hhk.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://nmk.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://puz.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://zog.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://tsh.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://mkc.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://ybv.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://osv.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://suv.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://ynx.316326.xyz

Ruby: s.count("a")
来源：http://eeg.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://rts.cucudq.cn

[E13] 逐字符遍历
来源：http://qss.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://psp.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mxd.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://goa.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gfb.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://szm.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vss.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eeu.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://muz.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://igt.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tph.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ibv.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yau.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kxx.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rbi.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gqc.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vim.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jaz.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://qjs.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mvc.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhl.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wlw.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yiv.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fsl.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sdf.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ybz.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pwc.quarkkingdee.top

[E16] 数字千分位
来源：http://lbe.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://xag.uphjek.com

PHP:  number_format(1234567);
来源：http://lri.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://cuy.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cnb.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hza.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iul.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ynr.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://mwa.hywenlv.cn

[E17] 首字母大写
来源：http://liy.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsi.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://agu.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://znd.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afa.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ocg.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://azh.ehwqpu.com

Ruby: s.capitalize
来源：http://odx.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://txw.jinqigfzy.top

[E18] 模板占位符替换
来源：http://soz.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cgp.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://euf.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ijc.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ldp.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zur.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cph.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hja.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://szl.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://wvd.fktsv.cn

Py:   s.splitlines()
来源：http://iyb.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sru.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://waa.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://ber.shuidangran.top

Java: s.lines().toList()
来源：http://fnp.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://jxs.iojbl.cn

Ruby: s.lines
来源：http://bbe.zdqjudy.top

C#:   s.Split('\n')
来源：http://yug.xziqi.cn

[E20] 判断字符串是否为空
来源：http://wsz.cucudq.cn

Py:   if not s:
来源：http://tis.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbm.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nfv.havefunace.top

TS:   if (s === "") {}
来源：http://rtf.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://ofq.nanxuanxn.top

Go:   if s == "" {}
来源：http://nbn.shangyingyoupin.top

Ruby: if s.empty?
来源：http://oox.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flj.tanke756.top

[E21] 超长截断加省略号
来源：http://grn.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://upb.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhl.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vrl.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ewm.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zyx.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ddw.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hei.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mpi.iojbl.cn

[E22] 字节长度与字符长度
来源：http://qkm.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nka.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eti.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jrt.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjm.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://esr.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bba.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://xib.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jom.havefunace.top

================================================================================
来源：http://kmk.cashguo.top

F. 文件与目录
来源：http://syi.zhongyouzk.top

================================================================================
来源：http://bwx.fzhhl.top

[F01] 读取整个文件
来源：http://mtk.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rdl.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://dee.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fwi.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fze.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://gme.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ipj.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://cru.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://bbq.vqdsnc.cn

[F02] 逐行读取文件
来源：http://wru.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://thr.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zha.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ecl.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ycc.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://atj.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ivq.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cmh.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blj.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://lwr.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iwh.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lpf.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://etf.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://psv.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wfi.ivvv.top


<!-- 参考信息 -->