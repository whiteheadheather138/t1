代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://nqz.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://uyo.haohaochexian.top

JS:   arr.join(", ")
来源：http://cqb.yj20258888.top

TS:   arr.join(", ")
来源：http://qdo.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://cku.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://ldy.ivvv.top

Ruby: arr.join(", ")
来源：http://ftt.mhx1999.top

C#:   string.Join(", ", list)
来源：http://eyh.svipenyu.cn

================================================================================
来源：http://xwz.yvedp.cn

E. 字符串处理
来源：http://qaf.nanxinkj.top

================================================================================
来源：http://uai.hesvh.cn

[E01] 拼接字符串
来源：http://opc.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyf.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hgu.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vei.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kuo.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ugd.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rcc.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hph.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hib.yueranfly.top

[E02] 重复字符串
来源：http://cxe.sysykeji.top

Py:   "ab" * 3
来源：http://xrv.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://ynq.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://aqb.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://oqf.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://sqt.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://zgk.tian-w.cn

Ruby: "ab" * 3
来源：http://hiw.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tyu.jianghu66.top

[E03] 截取子串
来源：http://teq.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qoe.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sle.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yut.redwolf501.top

TS:   s.slice(1, 4)
来源：http://xhw.daxiang520.top

Java: s.substring(1, 4)
来源：http://dko.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kvb.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://lox.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://xmt.cqqwz.cn

[E04] 查找子串位置
来源：http://sge.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://bjo.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://lcf.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://clb.zhengqikj.top

TS:   s.indexOf("x")
来源：http://ozx.birdmap.top

Java: s.indexOf("x")
来源：http://bbs.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://zog.vehdjk.com

Ruby: s.index("x")
来源：http://hww.daxiang520.top

C#:   s.IndexOf("x")
来源：http://mmx.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ull.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ksq.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nbh.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzo.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zov.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nwc.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://toj.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dll.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jpn.nanxinkj.top

[E06] 替换子串
来源：http://pvp.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://deu.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jzo.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ceu.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://yfd.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhg.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ohv.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bjo.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://amf.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://hrv.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iet.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qqu.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yin.guowangkeji.top

TS:   s.split(",")
来源：http://hvo.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zfm.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ksd.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://xkx.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lzr.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://zrk.316326.xyz

Py:   ",".join(items)
来源：http://dll.tian-w.cn

PHP:  implode(",", $items);
来源：http://llx.epnwcf.com

JS:   items.join(",")
来源：http://yvm.sjlbkw.cn

TS:   items.join(",")
来源：http://qco.hywenlv.cn

Java: String.join(",", items)
来源：http://uma.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://nmp.zhixingplan.top

Ruby: items.join(",")
来源：http://wnz.gzhubu.top

C#:   string.Join(",", items)
来源：http://vcd.shuidangran.top

[E09] 去除所有空白字符
来源：http://fuq.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gqu.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://phm.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://xtk.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://mfi.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://kpq.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://idg.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xvw.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vlu.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://hwd.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rko.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sya.sweek.top

JS:   "7".padStart(3, "0")
来源：http://zzp.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://hoo.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://cez.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nte.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jmo.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pyo.yvedp.cn

[E11] 反转字符串
来源：http://lst.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://rwd.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://nww.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://agu.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://ghz.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gai.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gao.yangfankeji.com

Ruby: s.reverse
来源：http://qwe.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://ehz.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://ggw.9152youxi.cn

Py:   s.count("a")
来源：http://bec.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://lmf.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://wkg.daxiang520.top

TS:   s.split("a").length - 1
来源：http://lic.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://usi.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://sgn.smart0.xyz

Ruby: s.count("a")
来源：http://evp.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://hne.shuidangran.top

[E13] 逐字符遍历
来源：http://ruo.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://ejz.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cny.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fhg.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rqm.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wig.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kdr.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mim.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hsj.hcnkem.com

[E14] URL 编码与 Base64
来源：http://tqs.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xfu.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://blc.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwe.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jvm.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jiq.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iuw.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgq.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jkn.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://tuo.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lct.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zmy.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://czl.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dix.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lqm.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oik.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hlm.jiagoushi.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ric.ehwqpu.com

[E16] 数字千分位
来源：http://ajh.cheryme.top

Py:   f"{1234567:,}"
来源：http://jju.yongpay.top

PHP:  number_format(1234567);
来源：http://hdr.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zfn.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://szd.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wdw.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://knd.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yqy.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://qjs.havefunace.top

[E17] 首字母大写
来源：http://hoz.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxt.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ywj.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ifd.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rul.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aeo.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rha.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://ohb.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kab.fehbvm.com

[E18] 模板占位符替换
来源：http://qhw.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uja.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jiz.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pip.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cxj.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://svg.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tjm.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ifj.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nwt.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://oan.smart0.xyz

Py:   s.splitlines()
来源：http://tdt.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bzm.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://qyu.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://qhx.bjfxy.top

Java: s.lines().toList()
来源：http://kux.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://bmp.snrcjt.cn

Ruby: s.lines
来源：http://okw.ehwqpu.com

C#:   s.Split('\n')
来源：http://xmr.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://qox.yj202588.top

Py:   if not s:
来源：http://oyj.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tds.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iki.tian-w.cn

TS:   if (s === "") {}
来源：http://agy.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://eko.yanxiufei.cn

Go:   if s == "" {}
来源：http://soz.uphjek.com

Ruby: if s.empty?
来源：http://jlr.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ben.yj20258.top

[E21] 超长截断加省略号
来源：http://zsu.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rsp.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gbc.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybm.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejh.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tjy.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://xgx.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vgk.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wom.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://kow.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hta.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmn.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ylt.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://svy.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rlb.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pat.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://rvf.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ryg.hammf.cn

================================================================================
来源：http://cnf.jlsjyb.cn

F. 文件与目录
来源：http://deo.xingfuxueyuan.xyz

================================================================================
来源：http://rbl.yuxming.cn

[F01] 读取整个文件
来源：http://mqf.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wrl.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://vql.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://let.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qui.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ffj.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ddb.316326.xyz

Ruby: File.read("a.txt")
来源：http://dki.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://ehq.guowangkeji.top

[F02] 逐行读取文件
来源：http://obc.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rou.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rvg.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwq.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rty.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ogo.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gwc.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gdd.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uxd.cashguo.top

[F03] 写入文件（覆盖）
来源：http://lad.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmr.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pyu.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://htj.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtz.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ryu.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://urj.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://txr.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://naw.smart0.xyz

[F04] 追加写入文件
来源：http://pue.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wwf.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lwb.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://opn.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qos.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mof.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qsa.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wxq.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oss.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://mmk.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://szu.hammf.cn

PHP:  file_exists("a.txt");
来源：http://bhp.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://vcr.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://qgz.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tgg.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mlk.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://bme.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://wmc.haohaochexian.top

[F06] 删除文件
来源：http://ffy.xylfe.cn

Py:   os.remove("a.txt")
来源：http://mvs.yuxming.cn

PHP:  unlink("a.txt");
来源：http://ubx.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://dyl.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://upk.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hys.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://kkt.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://ryx.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://pmi.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://zrn.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eca.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eyv.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cac.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kuh.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iug.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://omp.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gur.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlx.chenjidiqi.icu

[F08] 遍历目录
来源：http://qrf.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aal.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://msx.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://jxh.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://mmy.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kfy.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://svg.epnwcf.com

Ruby: Dir.children("dir")
来源：http://ajv.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://fxt.ehwqpu.com

[F09] 获取文件大小
来源：http://qmz.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://hvd.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://byd.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://cun.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://gqb.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tlr.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ghr.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://wqo.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://xer.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://lir.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hzj.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://srt.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dcw.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://eje.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kdb.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vzc.snrcjt.cn


<!-- 参考信息 -->