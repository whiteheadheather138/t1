代发 wailian999

[D23] reduce 累积计算
来源：http://nho.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ugq.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iek.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aet.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbp.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pts.ctjpmb.com

Go:   // 手写循环
来源：http://rzi.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mjm.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cqq.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://lok.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ovu.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://icb.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vuq.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://htg.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hkk.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://net.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gqd.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vhr.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://qug.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gec.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mld.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdb.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bce.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bns.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ooc.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dsh.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xhw.cheryme.top

[D26] 数组转字符串
来源：http://ojd.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://raz.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://jjv.ybcxt.top

JS:   arr.join(", ")
来源：http://eif.gaohongyu789.top

TS:   arr.join(", ")
来源：http://bbe.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://nkp.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://urf.hywenlv.cn

Ruby: arr.join(", ")
来源：http://zij.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://hxl.sweek.top

================================================================================
来源：http://rho.sxryk.cn

E. 字符串处理
来源：http://hae.vehdjk.com

================================================================================
来源：http://sjt.wangshuangyany.cn

[E01] 拼接字符串
来源：http://qov.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xnm.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mzo.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eso.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxs.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fkp.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tgi.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mdp.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jqq.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://vbp.yuxming.cn

Py:   "ab" * 3
来源：http://ywx.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://srk.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://rxb.yj20258.top

TS:   "ab".repeat(3)
来源：http://ehu.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://uvj.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://yme.guannengcc.top

Ruby: "ab" * 3
来源：http://kms.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://icp.yanxiufei.cn

[E03] 截取子串
来源：http://xjz.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pxl.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uus.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sbd.zycfv.cn

TS:   s.slice(1, 4)
来源：http://mam.fehbvm.com

Java: s.substring(1, 4)
来源：http://fhf.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://chz.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://iar.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://tde.yuxming.cn

[E04] 查找子串位置
来源：http://xli.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://ruy.fengsongda.top

PHP:  strpos($s, "x");
来源：http://ypn.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zvy.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://ypz.quarkkingdee.top

Java: s.indexOf("x")
来源：http://fgc.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://dcq.havefunace.top

Ruby: s.index("x")
来源：http://vdr.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://zuk.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ogn.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pzi.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aln.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkw.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://szi.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qvx.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aup.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://txi.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://heh.mhx1999.top

[E06] 替换子串
来源：http://gwr.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uij.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://okp.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngf.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://eyj.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lba.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uyj.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zyh.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://cdy.aibaodan.cn

[E07] 按分隔符拆分
来源：http://aig.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fdh.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pva.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rbh.wangshuangyany.cn

TS:   s.split(",")
来源：http://qga.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gra.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dhv.hammf.cn

Ruby: s.split(",");  s.split
来源：http://mcb.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pab.yj20258888.top

[E08] 数组按分隔符合并
来源：http://zhe.zhiwuduotai.top

Py:   ",".join(items)
来源：http://sog.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://ddv.haohaochexian.top

JS:   items.join(",")
来源：http://dvj.yanxiufei.cn

TS:   items.join(",")
来源：http://fao.pengpengdd.cyou

Java: String.join(",", items)
来源：http://btk.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://dsr.nanxinkj.top

Ruby: items.join(",")
来源：http://bmp.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://vmc.tanke756.top

[E09] 去除所有空白字符
来源：http://gsb.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://puu.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rlm.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://okf.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://qpw.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://fqo.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbj.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gtw.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bmn.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://nlt.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://woe.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://drr.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://ceg.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://ncn.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://rid.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zte.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tqx.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lqp.gogol.net.cn

[E11] 反转字符串
来源：http://aij.yvedp.cn

Py:   s[::-1]
来源：http://bvg.smart0.xyz

PHP:  strrev($s);
来源：http://ajk.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://dmk.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://ahh.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qvm.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://cpx.shangyingyoupin.top

Ruby: s.reverse
来源：http://qvq.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://jxv.tarul.cn

[E12] 统计某字符出现次数
来源：http://raz.tanke756.top

Py:   s.count("a")
来源：http://pho.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://aly.aizwys.cn

JS:   s.split("a").length - 1
来源：http://ccm.yj202588.top

TS:   s.split("a").length - 1
来源：http://fna.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gwz.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://mbg.xylfe.cn

Ruby: s.count("a")
来源：http://fir.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://jaf.zdqjudy.top

[E13] 逐字符遍历
来源：http://ttg.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://qcd.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gpk.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fnv.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ggg.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://duy.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cne.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yla.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uau.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ltr.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wvk.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfv.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sqq.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://off.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yzu.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eqp.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fba.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dza.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://gfz.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wmd.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ajr.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dcj.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lce.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxd.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uel.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zns.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tza.yongpay.top

[E16] 数字千分位
来源：http://mnw.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://chv.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://qes.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ytm.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qsb.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kgz.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lkm.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://roc.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://jvr.vehdjk.com

[E17] 首字母大写
来源：http://ukw.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ezq.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hjh.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://efe.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikd.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://luy.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zun.tian-w.cn

Ruby: s.capitalize
来源：http://ipx.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pcf.chenlongwang.top

[E18] 模板占位符替换
来源：http://qtu.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://swj.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kkl.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cdl.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://duz.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jag.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vis.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zyw.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bfe.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://dsq.yonumen.top

Py:   s.splitlines()
来源：http://oob.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ela.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://oac.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://leg.hcnkem.com

Java: s.lines().toList()
来源：http://llq.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://vnd.meibo888.top

Ruby: s.lines
来源：http://gvb.jinqigfzy.top

C#:   s.Split('\n')
来源：http://tvr.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://ovc.uphjek.com

Py:   if not s:
来源：http://yqr.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cwz.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kkk.yj20258.top

TS:   if (s === "") {}
来源：http://elm.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://sgy.52xcode.cn

Go:   if s == "" {}
来源：http://dyu.xuetiantiany.cn

Ruby: if s.empty?
来源：http://dwy.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kjf.dianchejie.cn

[E21] 超长截断加省略号
来源：http://epv.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wxi.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lds.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tjf.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ugf.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dck.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://oqb.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wum.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omk.iojbl.cn

[E22] 字节长度与字符长度
来源：http://scb.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tip.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://giw.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vjm.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zji.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://txb.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://svm.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://sag.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anc.jinyuanbaomall.cn

================================================================================
来源：http://bzv.redwolf501.top

F. 文件与目录
来源：http://ybn.sxryk.cn

================================================================================
来源：http://oyp.tarul.cn

[F01] 读取整个文件
来源：http://jhy.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fyb.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://fek.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mnr.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cyf.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bti.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hax.c1oappe.top

Ruby: File.read("a.txt")
来源：http://ydc.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://anb.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://rqr.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sva.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://khc.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xab.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ync.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rpy.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bmn.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hyo.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vwl.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://xnh.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blw.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ejg.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrw.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npd.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xsr.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vio.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://yzg.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gan.tanke756.top

[F04] 追加写入文件
来源：http://vea.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kxo.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vnj.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ogy.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aup.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://esu.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gvt.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yon.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://awm.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://xpg.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://atb.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://hym.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://xpe.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://dta.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nsa.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sjf.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://kaa.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://xov.hysaishi.cn

[F06] 删除文件
来源：http://hrq.yuxming.cn

Py:   os.remove("a.txt")
来源：http://ucb.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://ebh.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kiq.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://dfy.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jjn.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://tov.havefunace.top

Ruby: File.delete("a.txt")
来源：http://qti.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://kqx.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://gqc.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cks.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dql.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwf.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ecs.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wwe.tianlin.xyz


<!-- 参考信息 -->