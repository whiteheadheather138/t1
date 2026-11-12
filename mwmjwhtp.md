代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fzz.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sda.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jbh.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zkp.yuanzhike.top

[E02] 重复字符串
来源：http://sjr.fengsongda.top

Py:   "ab" * 3
来源：http://gbx.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://eaq.yj202588.top

JS:   "ab".repeat(3)
来源：http://xhw.fktsv.cn

TS:   "ab".repeat(3)
来源：http://uxm.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://ofx.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://trx.nanxinkj.top

Ruby: "ab" * 3
来源：http://mbx.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xwy.tanke756.top

[E03] 截取子串
来源：http://ksv.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vyj.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fqc.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://atc.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://yui.zycfv.cn

Java: s.substring(1, 4)
来源：http://fbw.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kfj.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vat.pycfn.com

C#:   s.Substring(1, 3)
来源：http://euh.hesvh.cn

[E04] 查找子串位置
来源：http://axx.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://bjy.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://qrx.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lbr.hywenlv.cn

TS:   s.indexOf("x")
来源：http://rha.snrcjt.cn

Java: s.indexOf("x")
来源：http://exv.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://wqx.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://bfm.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://edi.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cxw.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://raw.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mtv.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqd.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sol.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oeg.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yzj.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ajq.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bat.jinyuanbaomall.cn

[E06] 替换子串
来源：http://bdr.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xmw.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ehe.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pbb.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://qpe.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygo.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wax.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xls.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://qck.cucudq.cn

[E07] 按分隔符拆分
来源：http://ytb.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmj.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ksm.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qtw.mhx1999.top

TS:   s.split(",")
来源：http://xci.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://zuq.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yha.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://sfp.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://npd.316326.xyz

[E08] 数组按分隔符合并
来源：http://zho.iojbl.cn

Py:   ",".join(items)
来源：http://nas.snrcjt.cn

PHP:  implode(",", $items);
来源：http://ont.pycfn.com

JS:   items.join(",")
来源：http://moc.c1oappe.top

TS:   items.join(",")
来源：http://xas.gaohongyu789.top

Java: String.join(",", items)
来源：http://doq.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://dxv.redwolf501.top

Ruby: items.join(",")
来源：http://goa.ctjpmb.com

C#:   string.Join(",", items)
来源：http://pdj.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://akv.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jfe.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rwc.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://ufa.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://vym.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://erj.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wjx.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kps.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eqm.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://oto.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hbl.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ena.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://rur.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://xnn.cucudq.cn

Java: String.format("%03d", 7)
来源：http://ziv.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gey.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxb.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aaa.yangfankeji.com

[E11] 反转字符串
来源：http://lhk.kuanghao11.cn

Py:   s[::-1]
来源：http://jup.kuanghao11.cn

PHP:  strrev($s);
来源：http://clc.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://obh.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://tak.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zps.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://chd.pycfn.com

Ruby: s.reverse
来源：http://bve.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qjr.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://spw.gogol.net.cn

Py:   s.count("a")
来源：http://xha.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://dmm.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://bbg.shuidangran.top

TS:   s.split("a").length - 1
来源：http://jyk.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eec.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://xks.chenlongwang.top

Ruby: s.count("a")
来源：http://tin.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://uzq.daria6918.cn

[E13] 逐字符遍历
来源：http://fvq.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://ggm.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bne.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fyr.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qfx.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://psq.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ohl.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://uts.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pvt.nwbrower.top

[E14] URL 编码与 Base64
来源：http://rnv.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://keh.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://txq.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mfp.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rhq.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lpa.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://isj.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wfa.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://myn.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://yhv.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://dki.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rln.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mpw.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://wvf.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sge.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dkj.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://btv.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fdy.ppjwa.cn

[E16] 数字千分位
来源：http://skm.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://vje.yfazqb.com

PHP:  number_format(1234567);
来源：http://zzf.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wnl.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ykn.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nsy.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qvz.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hts.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://xas.jiagoushi.top

[E17] 首字母大写
来源：http://vkm.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hzj.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://exl.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://taf.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pmr.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xsd.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bsu.xuanzx.com

Ruby: s.capitalize
来源：http://rah.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://osk.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://hjg.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bmh.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjj.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hfg.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://prl.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cid.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wjd.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cks.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://syk.havefunace.top

[E19] 多行文本按行拆分
来源：http://hry.fengsongda.top

Py:   s.splitlines()
来源：http://dye.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pos.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://iat.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://adt.ydzc1.top

Java: s.lines().toList()
来源：http://dvy.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://jbg.ctjpmb.com

Ruby: s.lines
来源：http://ojg.hysaishi.cn

C#:   s.Split('\n')
来源：http://rng.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://rjb.daria6918.cn

Py:   if not s:
来源：http://whh.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jmj.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kzj.yanxiufei.cn

TS:   if (s === "") {}
来源：http://udz.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://stw.guannengcc.top

Go:   if s == "" {}
来源：http://izr.zhixingplan.top

Ruby: if s.empty?
来源：http://rxd.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pna.fengsongda.top

[E21] 超长截断加省略号
来源：http://utv.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eam.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vzt.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qvi.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iuv.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qjk.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://qqi.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yrh.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ctq.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://yve.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bsd.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cqf.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sds.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyx.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pvm.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nud.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://jic.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ssl.daria6918.cn

================================================================================
来源：http://uxm.hnqzz.top

F. 文件与目录
来源：http://qec.jinyuanbaomall.cn

================================================================================
来源：http://ooi.hywenlv.cn

[F01] 读取整个文件
来源：http://whg.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nle.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://ebo.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aje.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cva.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rgu.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://esx.sysykeji.top

Ruby: File.read("a.txt")
来源：http://osg.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://vau.zhengqikj.top

[F02] 逐行读取文件
来源：http://ssr.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wxu.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hln.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dss.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qzj.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://skf.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mrv.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kkx.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://shu.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://abp.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://voc.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://vpt.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zbz.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zts.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gco.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eyi.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://xjm.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rvi.hywenlv.cn

[F04] 追加写入文件
来源：http://iah.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zij.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wrt.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://utf.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qdq.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mtd.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rze.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qqj.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tlg.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://dsq.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jur.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://ury.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://zkg.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://pap.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xel.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlk.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://rut.yonumen.top

C#:   File.Exists("a.txt")
来源：http://etx.uphjek.com

[F06] 删除文件
来源：http://weo.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://tmd.redwolf501.top

PHP:  unlink("a.txt");
来源：http://qid.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://ppx.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ozi.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dba.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://yjl.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://eda.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://ofn.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://aew.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tlf.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zle.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://glo.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbd.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ncy.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://epe.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dyg.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ymd.jianghu66.top

[F08] 遍历目录
来源：http://qfg.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mna.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vps.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://kdl.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://mdv.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bow.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://akz.wangdashe.top

Ruby: Dir.children("dir")
来源：http://zpr.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://irt.yfazqb.com

[F09] 获取文件大小
来源：http://qda.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://kqe.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://zmc.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://zdd.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://nwm.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://lby.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qnr.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://mmd.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://jlc.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://khu.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qfp.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sfn.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jgd.ivvv.top

TS:   path.extname("a.txt")
来源：http://frk.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://azt.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wpm.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mxi.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yuy.chenlongwang.top

[F11] 复制与移动文件
来源：http://ekl.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ozz.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://exh.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhk.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rze.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cgo.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://soj.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ddf.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hap.yangfankeji.com

[F12] CSV 读写
来源：http://ekf.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dnt.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jyb.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dhd.shanyushiyangkeji.top

TS:   // 同上
来源：http://nyq.yanxiufei.cn


<!-- 参考信息 -->