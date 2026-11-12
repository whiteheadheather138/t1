代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wad.jianghu66.top

Go:   // 手写双层循环
来源：http://jqf.ppjwa.cn

Ruby: nested.flatten
来源：http://knw.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://khh.zhixingplan.top

[D19] 按字段分组
来源：http://jse.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gcp.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bjw.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dgg.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dex.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mic.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://trx.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ccb.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zmq.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://chb.feifeiyinyue.top

Py:   Counter(arr)
来源：http://koq.guannengcc.top

PHP:  array_count_values($arr);
来源：http://xur.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pss.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vos.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epg.uphjek.com

Go:   // 手写 map[T]int
来源：http://cus.ybcxt.top

Ruby: arr.tally
来源：http://ono.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cxy.hesvh.cn

[D21] 判断是否包含某元素
来源：http://hpv.c1oappe.top

Py:   x in arr
来源：http://pss.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://egt.hesvh.cn

JS:   arr.includes(x)
来源：http://ykf.hywenlv.cn

TS:   arr.includes(x)
来源：http://tsz.fengsongda.top

Java: list.contains(x)
来源：http://uef.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://tuu.9152youxi.cn

Ruby: arr.include?(x)
来源：http://hvh.bbcook.cn

C#:   list.Contains(x)
来源：http://dls.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://lxt.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pku.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dgj.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ijm.sjlbkw.cn

TS:   [...arr];
来源：http://ata.aizwys.cn

Java: new ArrayList<>(list);
来源：http://ngo.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wxt.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://hea.52xcode.cn

C#:   new List<int>(list);
来源：http://elt.svipenyu.cn

[D23] reduce 累积计算
来源：http://qyd.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://esn.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wrj.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mhz.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqv.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mab.yj20258888.top

Go:   // 手写循环
来源：http://hhp.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yry.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bhi.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://hud.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mcp.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fmx.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tzw.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dsl.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nis.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gnt.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://riz.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kzi.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://aqa.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://flx.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qtm.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bmr.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://etu.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fah.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vap.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fra.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qry.hfpthk.cn

[D26] 数组转字符串
来源：http://ueg.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://zol.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://zjt.kuanghao11.cn

JS:   arr.join(", ")
来源：http://qaf.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://uvw.aizwys.cn

Java: String.join(", ", list)
来源：http://elj.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://ncg.mhx1999.top

Ruby: arr.join(", ")
来源：http://sgg.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://byp.jqgfzy.top

================================================================================
来源：http://ggw.nwbrower.top

E. 字符串处理
来源：http://vzu.cqqwz.cn

================================================================================
来源：http://cgy.sjlbkw.cn

[E01] 拼接字符串
来源：http://nuj.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wrs.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uhh.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://omj.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbx.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zvp.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zrs.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hwr.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zhn.yj202588.top

[E02] 重复字符串
来源：http://lvj.smart0.xyz

Py:   "ab" * 3
来源：http://mqj.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://mme.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://fnb.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://msl.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://vjk.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://vvp.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://eev.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wwz.sjlbkw.cn

[E03] 截取子串
来源：http://oej.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uim.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mzv.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvv.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://btc.cashguo.top

Java: s.substring(1, 4)
来源：http://pyx.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lti.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kko.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://fdn.hesvh.cn

[E04] 查找子串位置
来源：http://vum.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://vqm.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://cyx.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zcy.ehwqpu.com

TS:   s.indexOf("x")
来源：http://qwf.sjlbkw.cn

Java: s.indexOf("x")
来源：http://abx.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://xvg.dianchejie.cn

Ruby: s.index("x")
来源：http://mfs.yj20258888.top

C#:   s.IndexOf("x")
来源：http://mzj.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zwe.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hao.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cal.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xox.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xcg.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtw.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hwp.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqj.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dgv.tianlin.xyz

[E06] 替换子串
来源：http://gpx.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kjz.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://uwk.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tuw.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://ccs.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usp.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qjf.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fcu.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://fka.havefunace.top

[E07] 按分隔符拆分
来源：http://vpn.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gpp.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kbl.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hee.yangfankeji.com

TS:   s.split(",")
来源：http://lkw.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dsm.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hmj.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://uzh.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dvt.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://beo.mhx1999.top

Py:   ",".join(items)
来源：http://dpb.iojbl.cn

PHP:  implode(",", $items);
来源：http://fls.hfpthk.cn

JS:   items.join(",")
来源：http://wjg.yj20258.top

TS:   items.join(",")
来源：http://lvm.bbcook.cn

Java: String.join(",", items)
来源：http://wem.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://dcm.iojbl.cn

Ruby: items.join(",")
来源：http://hri.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://vis.jianghu66.top

[E09] 去除所有空白字符
来源：http://ajg.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dcy.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kdt.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://voz.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://jrb.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://gan.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qnq.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ixs.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://emw.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://kyu.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://unu.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qdm.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://cpt.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://ywb.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://jks.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vpj.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ygg.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sjq.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://swg.yonumen.top

Py:   s[::-1]
来源：http://hwc.fehbvm.com

PHP:  strrev($s);
来源：http://swp.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://orw.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://kyd.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mgg.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tpa.pengpengdd.cyou

Ruby: s.reverse
来源：http://ncm.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://czc.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://wkt.tianlin.xyz

Py:   s.count("a")
来源：http://rlb.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://ade.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://ffg.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://uil.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itu.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://xcw.c1oappe.top

Ruby: s.count("a")
来源：http://zor.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://cmt.cdnleiting.top

[E13] 逐字符遍历
来源：http://abl.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://axt.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gvs.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://psj.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xeu.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zph.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vat.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kuy.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://int.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://ojh.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rfx.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://upu.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vzo.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ssl.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lur.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qqz.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jgf.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qbs.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://mym.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gbs.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ern.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jri.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mie.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yuk.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zit.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gqh.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zta.feifeiyinyue.top

[E16] 数字千分位
来源：http://wxd.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://hog.uphjek.com

PHP:  number_format(1234567);
来源：http://frs.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vyd.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cwk.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pmp.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wql.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mrz.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://fne.yangfankeji.com

[E17] 首字母大写
来源：http://kyd.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dcq.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lqm.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pwv.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cid.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pyd.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmy.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://eas.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dfn.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://uzt.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vis.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://voy.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hsh.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rba.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yzr.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ixh.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pmf.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qoq.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://jnn.ydjk.org.cn

Py:   s.splitlines()
来源：http://dur.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsh.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://yys.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://orz.yonumen.top

Java: s.lines().toList()
来源：http://snt.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://qdv.yanxiufei.cn

Ruby: s.lines
来源：http://ixn.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://qdx.yfazqb.com

[E20] 判断字符串是否为空
来源：http://jgp.hnxiangtu.top

Py:   if not s:
来源：http://kct.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hue.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mrd.zycfv.cn

TS:   if (s === "") {}
来源：http://ref.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://avt.xinyue.icu

Go:   if s == "" {}
来源：http://fah.jyoumei.cn

Ruby: if s.empty?
来源：http://fve.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zdw.chenlongwang.top

[E21] 超长截断加省略号
来源：http://jwb.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xsf.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zeb.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpp.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpb.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rqg.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://lig.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nnt.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://drt.jianghu66.top

[E22] 字节长度与字符长度
来源：http://nhf.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zzu.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xvb.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://svh.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rni.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nrv.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nxz.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://cjx.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tgp.mhx1999.top

================================================================================
来源：http://sbu.vqdsnc.cn

F. 文件与目录
来源：http://fme.fengsongda.top

================================================================================
来源：http://qzp.redwolf501.top

[F01] 读取整个文件
来源：http://jmf.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nsy.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://fyh.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hcx.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fur.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qku.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ajx.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://bkx.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://igi.ybcxt.top

[F02] 逐行读取文件
来源：http://ezi.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tqg.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rws.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nsg.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwf.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://flo.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ywh.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqe.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mxg.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://ljp.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://csj.jinghuilouyu.cn


<!-- 参考信息 -->