代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vgs.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://tcp.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqb.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tii.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://usx.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cxh.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zmz.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ycu.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jds.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gnt.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://vgm.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jmw.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ngu.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qsr.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ezz.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://irs.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hmt.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://juh.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wrc.jlsjyb.cn

[D26] 数组转字符串
来源：http://hvu.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://pzd.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://olr.zycfv.cn

JS:   arr.join(", ")
来源：http://mlh.jinqigufen.top

TS:   arr.join(", ")
来源：http://gkq.hammf.cn

Java: String.join(", ", list)
来源：http://arg.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://jex.shuidangran.top

Ruby: arr.join(", ")
来源：http://ubg.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://dov.c1oappe.top

================================================================================
来源：http://vua.gotoacloud.top

E. 字符串处理
来源：http://ykh.sxryk.cn

================================================================================
来源：http://duf.svipenyu.cn

[E01] 拼接字符串
来源：http://fjh.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bwk.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nhs.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gii.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyr.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kba.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ihl.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wzt.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kul.guowangkeji.top

[E02] 重复字符串
来源：http://cnv.yj202588.top

Py:   "ab" * 3
来源：http://ugs.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://pir.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://zzs.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://yqe.cashguo.top

Java: "ab".repeat(3)
来源：http://alx.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://mtx.pycfn.com

Ruby: "ab" * 3
来源：http://cyc.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://llt.vehdjk.com

[E03] 截取子串
来源：http://zps.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://utu.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://agv.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tdv.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://akf.shuidangran.top

Java: s.substring(1, 4)
来源：http://wej.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bhg.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://ozf.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://san.tian-w.cn

[E04] 查找子串位置
来源：http://llf.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://adg.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://ctl.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vtv.xinyue.icu

TS:   s.indexOf("x")
来源：http://hed.chenlongwang.top

Java: s.indexOf("x")
来源：http://lnd.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://wgq.shzxlz.cn

Ruby: s.index("x")
来源：http://aof.xinyue.icu

C#:   s.IndexOf("x")
来源：http://umm.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pwd.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sxp.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://boa.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfq.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kgd.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhe.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gjm.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mux.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://snz.gotoacloud.top

[E06] 替换子串
来源：http://rzi.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pas.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://jka.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zya.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://fbb.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edz.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ztg.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qnd.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://mbk.wangdashe.top

[E07] 按分隔符拆分
来源：http://opk.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jnb.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://slm.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pnw.andypj.xyz

TS:   s.split(",")
来源：http://vmz.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xbj.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qvl.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://qwq.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmo.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://bkm.bjfxy.top

Py:   ",".join(items)
来源：http://jbu.tianlin.xyz

PHP:  implode(",", $items);
来源：http://lxd.shzxlz.cn

JS:   items.join(",")
来源：http://pnr.aizwys.cn

TS:   items.join(",")
来源：http://fle.jqgfzy.top

Java: String.join(",", items)
来源：http://afb.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://lug.gaohongyu789.top

Ruby: items.join(",")
来源：http://ybk.hesvh.cn

C#:   string.Join(",", items)
来源：http://jrg.cheryme.top

[E09] 去除所有空白字符
来源：http://cda.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjx.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hbp.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://hci.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://ths.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://zbu.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tsm.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://rlf.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gre.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://hvr.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://euh.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kip.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://uhc.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://reg.guannengcc.top

Java: String.format("%03d", 7)
来源：http://gzb.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rbv.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rql.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfu.hongshengwenyu.top

[E11] 反转字符串
来源：http://lmo.yonumen.top

Py:   s[::-1]
来源：http://xqu.svipenyu.cn

PHP:  strrev($s);
来源：http://ccn.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://hwc.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://lgt.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://per.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://olu.yvedp.cn

Ruby: s.reverse
来源：http://luf.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://etu.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://fgj.cdnleiting.top

Py:   s.count("a")
来源：http://ckf.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://ait.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://dgq.yuxming.cn

TS:   s.split("a").length - 1
来源：http://xco.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ewt.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://hze.dianchejie.cn

Ruby: s.count("a")
来源：http://rpg.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://dqb.yangfankeji.com

[E13] 逐字符遍历
来源：http://cmo.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://kzp.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mji.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wyh.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vnn.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dgq.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kli.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ypz.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://esf.ybcxt.top

[E14] URL 编码与 Base64
来源：http://epl.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://opm.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qmt.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cdk.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ewf.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qdl.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yvg.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://obu.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iwh.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://vzx.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sye.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qao.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lsa.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mhl.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ucr.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fuu.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pbj.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fcb.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://boj.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://jqa.nanxinkj.top

PHP:  number_format(1234567);
来源：http://yyh.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lqa.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wew.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://olk.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://isf.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cjo.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://uku.shzxlz.cn

[E17] 首字母大写
来源：http://pfa.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://azj.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://emq.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nvj.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fav.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwt.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dse.hywenlv.cn

Ruby: s.capitalize
来源：http://wie.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hax.hesvh.cn

[E18] 模板占位符替换
来源：http://rge.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sxy.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nsa.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fvg.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ski.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hpl.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ulp.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://htl.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lgx.yj202588.top

[E19] 多行文本按行拆分
来源：http://pxv.tanke756.top

Py:   s.splitlines()
来源：http://gcr.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nep.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://orf.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://bzi.nwbrower.top

Java: s.lines().toList()
来源：http://knm.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://geg.haohaochexian.top

Ruby: s.lines
来源：http://anh.zhixingplan.top

C#:   s.Split('\n')
来源：http://vgf.aizwys.cn

[E20] 判断字符串是否为空
来源：http://vnr.zhoulong.xyz

Py:   if not s:
来源：http://fxn.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dhf.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://umm.haohaochexian.top

TS:   if (s === "") {}
来源：http://grj.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://nax.jqgufenzy.top

Go:   if s == "" {}
来源：http://gon.52xcode.cn

Ruby: if s.empty?
来源：http://fhx.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iry.pycfn.com

[E21] 超长截断加省略号
来源：http://bgt.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://imx.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gts.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eaq.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cod.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iry.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://dkb.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yqk.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://djk.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://fvk.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yjq.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xqv.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtw.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ply.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urt.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xdi.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://kpv.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbw.tanke756.top

================================================================================
来源：http://zzs.zhongyouzk.top

F. 文件与目录
来源：http://qkm.meibo888.top

================================================================================
来源：http://fjp.snrcjt.cn

[F01] 读取整个文件
来源：http://dtz.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eij.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://upg.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kth.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hex.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wcu.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kfo.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://iyg.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://zou.epnwcf.com

[F02] 逐行读取文件
来源：http://zxz.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ysr.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uay.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqx.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://now.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ltp.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xvq.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mzv.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://auz.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://cfm.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eka.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://urk.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uvv.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bzr.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mjk.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tcy.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://ypv.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wpk.quarkkingdee.top

[F04] 追加写入文件
来源：http://ual.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zve.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jtb.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jss.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aan.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cxd.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdw.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zho.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kbc.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://fmv.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ggc.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://ndy.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://mie.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://atk.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rcn.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xcd.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://gdw.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://hpc.bbcook.cn

[F06] 删除文件
来源：http://ien.ivvv.top

Py:   os.remove("a.txt")
来源：http://kor.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://hfd.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kws.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ilx.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://luj.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://hyw.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://wom.ivvv.top

C#:   File.Delete("a.txt");
来源：http://ezk.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://jiw.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ekq.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rfc.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mli.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bkh.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zij.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qba.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aam.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gyi.c1oappe.top

[F08] 遍历目录
来源：http://nut.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lev.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yng.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://svw.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://rws.sweek.top


<!-- 参考信息 -->