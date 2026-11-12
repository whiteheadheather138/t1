代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ocr.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tst.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ttb.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vrg.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uqf.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bef.tarul.cn

[D25] Set 集合去重与交并差
来源：http://ewo.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iqi.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://buc.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mjz.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pgy.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xqj.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://woi.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cpg.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fmg.xuetiantiany.cn

[D26] 数组转字符串
来源：http://rme.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://twr.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://gav.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://bhe.nanxuanxn.top

TS:   arr.join(", ")
来源：http://hyu.zhoulong.xyz

Java: String.join(", ", list)
来源：http://eyk.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://xtx.ppjwa.cn

Ruby: arr.join(", ")
来源：http://khj.yongpay.top

C#:   string.Join(", ", list)
来源：http://ous.shangyingyoupin.top

================================================================================
来源：http://mqk.sufxvd.cn

E. 字符串处理
来源：http://ncd.ehwqpu.com

================================================================================
来源：http://yhy.shangyingyoupin.top

[E01] 拼接字符串
来源：http://jum.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://klx.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qhl.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ehj.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gwn.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xva.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kyl.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gqh.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nce.fanxiaobao.xyz

[E02] 重复字符串
来源：http://snf.aizwys.cn

Py:   "ab" * 3
来源：http://hed.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://zkw.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://rwb.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://cbz.shuidangran.top

Java: "ab".repeat(3)
来源：http://pbd.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://fll.yangfankeji.com

Ruby: "ab" * 3
来源：http://crr.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hqw.sweek.top

[E03] 截取子串
来源：http://nxm.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jlx.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xho.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tar.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://ikf.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://oei.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qdk.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://beo.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://bwm.52xcode.cn

[E04] 查找子串位置
来源：http://zyq.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://zzr.yongpay.top

PHP:  strpos($s, "x");
来源：http://zbj.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ucm.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://pfu.shuidangran.top

Java: s.indexOf("x")
来源：http://uvq.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://gca.bbcook.cn

Ruby: s.index("x")
来源：http://oim.aizwys.cn

C#:   s.IndexOf("x")
来源：http://vmj.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mus.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aos.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jar.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mom.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rgc.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://boi.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rtb.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hki.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lpk.ehwqpu.com

[E06] 替换子串
来源：http://cqt.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cjd.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://ihv.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usb.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://fhk.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zoz.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vek.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hrt.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://wpz.jinqigufen.top

[E07] 按分隔符拆分
来源：http://upt.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://spc.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://olg.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uby.svipenyu.cn

TS:   s.split(",")
来源：http://grz.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://rnx.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsx.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://bju.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hzg.pycfn.com

[E08] 数组按分隔符合并
来源：http://efe.xuetiantiany.cn

Py:   ",".join(items)
来源：http://xst.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://fhy.c1oappe.top

JS:   items.join(",")
来源：http://qdw.gzhubu.top

TS:   items.join(",")
来源：http://axl.sweek.top

Java: String.join(",", items)
来源：http://dqh.tarul.cn

Go:   strings.Join(items, ",")
来源：http://eei.ehwqpu.com

Ruby: items.join(",")
来源：http://rik.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://ypf.xuanzx.com

[E09] 去除所有空白字符
来源：http://pfz.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://thz.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cyh.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://xty.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://fum.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://eum.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cgz.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://cez.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://exp.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://uqw.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wkp.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xwb.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://all.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://djs.meibo888.top

Java: String.format("%03d", 7)
来源：http://dtk.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://rxs.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ule.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hsu.daria6918.cn

[E11] 反转字符串
来源：http://uvh.jqgufenzy.top

Py:   s[::-1]
来源：http://geg.jianghu66.top

PHP:  strrev($s);
来源：http://uwx.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://agp.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://tbu.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://caj.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rnk.yj20258888.top

Ruby: s.reverse
来源：http://mpl.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uub.xinyue.icu

[E12] 统计某字符出现次数
来源：http://uhd.cqqwz.cn

Py:   s.count("a")
来源：http://svj.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://kto.smart0.xyz

JS:   s.split("a").length - 1
来源：http://ggo.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://sau.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kch.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://ptr.vqdsnc.cn

Ruby: s.count("a")
来源：http://zgx.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://ooh.yj20258888.top

[E13] 逐字符遍历
来源：http://gdv.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://zsc.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://obw.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ens.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://bgp.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sgy.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oqm.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hay.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://icv.birdmap.top

[E14] URL 编码与 Base64
来源：http://tib.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yrf.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vas.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dmo.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://edm.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rmi.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://agm.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kqs.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yea.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://qdr.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ewk.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mvv.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xkt.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hgq.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eeb.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ynl.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cet.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aor.yuxming.cn

[E16] 数字千分位
来源：http://wnz.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://adw.guannengcc.top

PHP:  number_format(1234567);
来源：http://jmb.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kty.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bbi.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wcy.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lbn.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dkq.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://oyb.fanxiaobao.xyz

[E17] 首字母大写
来源：http://suo.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vay.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrj.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isi.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ldf.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hld.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hts.zhoulong.xyz

Ruby: s.capitalize
来源：http://bjj.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vmq.cdnleiting.top

[E18] 模板占位符替换
来源：http://nfj.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://prv.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://una.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mcf.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ewr.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://obe.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://era.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://btu.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lnc.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://fqb.cashguo.top

Py:   s.splitlines()
来源：http://tor.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://auc.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://rht.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://fby.jyoumei.cn

Java: s.lines().toList()
来源：http://ufy.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://zgi.sweek.top

Ruby: s.lines
来源：http://wtt.jiagoushi.top

C#:   s.Split('\n')
来源：http://slv.mhx1999.top

[E20] 判断字符串是否为空
来源：http://dvf.iojbl.cn

Py:   if not s:
来源：http://cgk.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oya.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dyb.daxiang520.top

TS:   if (s === "") {}
来源：http://eij.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://ohs.wangdashe.top

Go:   if s == "" {}
来源：http://kwx.jqgfzy.top

Ruby: if s.empty?
来源：http://mje.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zgo.yueranfly.top

[E21] 超长截断加省略号
来源：http://iqi.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://exb.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rib.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqn.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcu.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qft.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://wll.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wue.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aqw.guannengcc.top

[E22] 字节长度与字符长度
来源：http://sld.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ngy.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kka.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bsm.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tfg.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zdm.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcf.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://qdq.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mud.jyoumei.cn

================================================================================
来源：http://ohh.sufxvd.cn

F. 文件与目录
来源：http://vey.kuanghao11.cn

================================================================================
来源：http://zbo.mhx1999.top

[F01] 读取整个文件
来源：http://kkv.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ubw.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://yrh.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://szf.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://too.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://haz.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kow.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://vga.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://ojs.haohaochexian.top

[F02] 逐行读取文件
来源：http://ink.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iai.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vry.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akq.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mko.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ous.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://htx.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qqx.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mnt.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://uwz.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://paf.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mum.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pba.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://msw.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xvt.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eml.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://xhk.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gps.redwolf501.top

[F04] 追加写入文件
来源：http://axe.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cwz.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gbc.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hck.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsm.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gaa.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pxt.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iwy.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vrc.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://ncj.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lwd.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://cgh.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://bvc.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://tfr.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vqo.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tkx.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://fam.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://bjr.jinyuanbaomall.cn

[F06] 删除文件
来源：http://cfs.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://wvp.fehbvm.com

PHP:  unlink("a.txt");
来源：http://zrx.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wdc.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://onk.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sto.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://mjb.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://jqf.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://vsb.fktsv.cn

[F07] 创建目录（含多级）
来源：http://ycc.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ssi.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bhq.snrcjt.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xoj.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upm.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qld.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wml.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gai.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bfi.shzxlz.cn

[F08] 遍历目录
来源：http://zxr.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rfx.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://unt.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://viu.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://oyw.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zln.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jlg.ivvv.top

Ruby: Dir.children("dir")
来源：http://aul.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://lqk.0kj1m.cn


<!-- 参考信息 -->