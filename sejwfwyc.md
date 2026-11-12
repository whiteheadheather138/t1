代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pnr.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vwk.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xhl.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kir.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lua.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://suz.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hxh.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qwa.redwolf501.top

[E02] 重复字符串
来源：http://nge.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://exg.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://xpu.sxryk.cn

JS:   "ab".repeat(3)
来源：http://ooz.ybcxt.top

TS:   "ab".repeat(3)
来源：http://zrj.yj20258.top

Java: "ab".repeat(3)
来源：http://bgy.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://hlr.yangfankeji.com

Ruby: "ab" * 3
来源：http://kzg.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oxr.zhengqikj.top

[E03] 截取子串
来源：http://kbl.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://icq.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cav.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lfl.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://xpu.yj20258.top

Java: s.substring(1, 4)
来源：http://dha.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jik.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://edt.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://gok.ydjk.org.cn

[E04] 查找子串位置
来源：http://vgd.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://xeo.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://mkt.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qyi.yvedp.cn

TS:   s.indexOf("x")
来源：http://tmp.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://aln.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://srw.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://xlt.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://wnn.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yry.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sri.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lps.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gje.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vlb.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxz.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xql.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fvh.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kyo.redwolf501.top

[E06] 替换子串
来源：http://acg.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eqv.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://was.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bnd.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://vms.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kea.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzk.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oaj.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://lja.yonumen.top

[E07] 按分隔符拆分
来源：http://xwj.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fot.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uyy.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwn.pengpengdd.cyou

TS:   s.split(",")
来源：http://ptj.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pdy.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ysx.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://pjo.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgz.xinyue.icu

[E08] 数组按分隔符合并
来源：http://qey.nanxuanxn.top

Py:   ",".join(items)
来源：http://vib.pycfn.com

PHP:  implode(",", $items);
来源：http://ovv.jlsjyb.cn

JS:   items.join(",")
来源：http://pst.nanxinkj.top

TS:   items.join(",")
来源：http://efd.andypj.xyz

Java: String.join(",", items)
来源：http://ivu.meibo888.top

Go:   strings.Join(items, ",")
来源：http://mhe.yueranfly.top

Ruby: items.join(",")
来源：http://mgq.epnwcf.com

C#:   string.Join(",", items)
来源：http://nsv.svipenyu.cn

[E09] 去除所有空白字符
来源：http://mcf.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bmn.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lgj.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://pkp.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://ahx.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://udu.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gbf.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://omp.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ooq.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://aql.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ieb.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yoj.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://qfx.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://klv.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://zbh.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lwo.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bop.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kty.fktsv.cn

[E11] 反转字符串
来源：http://qjb.xuanzx.com

Py:   s[::-1]
来源：http://jre.guowangkeji.top

PHP:  strrev($s);
来源：http://fni.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://zrb.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://xjx.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tjg.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ckp.ydzc1.top

Ruby: s.reverse
来源：http://hbt.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://wgf.fengsongda.top

[E12] 统计某字符出现次数
来源：http://huv.gaohongyu789.top

Py:   s.count("a")
来源：http://ats.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://jof.guannengcc.top

JS:   s.split("a").length - 1
来源：http://gez.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://sxe.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fqi.yongpay.top

Go:   strings.Count(s, "a")
来源：http://riq.52xcode.cn

Ruby: s.count("a")
来源：http://pwg.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://mkq.zdqjudy.top

[E13] 逐字符遍历
来源：http://jnm.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://tka.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ebz.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dbj.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://imt.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zqq.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://itj.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nby.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oqb.birdmap.top

[E14] URL 编码与 Base64
来源：http://dtj.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://geh.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rwl.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozv.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://agg.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xah.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oxc.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rls.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kko.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://peu.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xfd.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qhx.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pts.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://aii.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wfi.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwo.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xzs.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fsj.tarul.cn

[E16] 数字千分位
来源：http://gud.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://lol.vehdjk.com

PHP:  number_format(1234567);
来源：http://qyf.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jfa.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lbv.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hhp.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eln.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kzr.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://rqq.havefunace.top

[E17] 首字母大写
来源：http://kca.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zcb.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://skd.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqs.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnh.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://red.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tok.316326.xyz

Ruby: s.capitalize
来源：http://fzl.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hwm.cashguo.top

[E18] 模板占位符替换
来源：http://vhj.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mvw.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vvy.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ozk.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ipb.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ejn.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eeh.jinyuanbaomall.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hxy.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjg.havefunace.top

[E19] 多行文本按行拆分
来源：http://kbx.havefunace.top

Py:   s.splitlines()
来源：http://tgf.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dxr.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://reh.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://jwf.cashguo.top

Java: s.lines().toList()
来源：http://sic.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://lfp.jinghuilouyu.cn

Ruby: s.lines
来源：http://krr.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://nzu.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://dsw.sufxvd.cn

Py:   if not s:
来源：http://lmt.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vmn.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kwp.epnwcf.com

TS:   if (s === "") {}
来源：http://xlv.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://myi.andypj.xyz

Go:   if s == "" {}
来源：http://sgq.yonumen.top

Ruby: if s.empty?
来源：http://obx.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rye.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://ceq.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqh.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhf.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqz.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tas.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fyz.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://zig.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnu.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tpk.meibo888.top

[E22] 字节长度与字符长度
来源：http://eqt.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rju.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lor.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qkj.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://szb.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jbf.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ypz.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://puc.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sxa.bjfxy.top

================================================================================
来源：http://pcp.daria6918.cn

F. 文件与目录
来源：http://nur.jyoumei.cn

================================================================================
来源：http://fpy.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://ogr.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://brt.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://pwx.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://txh.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dob.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rxg.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oys.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://cfl.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://xmy.yanxiufei.cn

[F02] 逐行读取文件
来源：http://syz.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://soq.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jwp.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mku.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jlw.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npi.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ztq.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dnn.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yap.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://wmb.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vme.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ibg.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dma.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dnr.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://alm.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xkt.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://dpi.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bzz.xylfe.cn

[F04] 追加写入文件
来源：http://ozs.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yli.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yow.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://saw.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijb.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://syw.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rsc.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hlx.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ovj.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://qxs.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aol.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://zaf.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://hmm.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://ftm.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xhn.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wkq.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://mna.yonumen.top

C#:   File.Exists("a.txt")
来源：http://ach.cashguo.top

[F06] 删除文件
来源：http://iyz.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://qwx.iojbl.cn

PHP:  unlink("a.txt");
来源：http://aei.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://stm.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://znm.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://els.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://jzg.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://ios.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://thm.vehdjk.com

[F07] 创建目录（含多级）
来源：http://trm.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehw.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cxg.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqx.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mdu.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pwi.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bwc.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xxh.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://igc.gotoacloud.top

[F08] 遍历目录
来源：http://rlj.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://uod.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://onq.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://bcv.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://paa.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vvl.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yfx.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://izx.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://qbi.yj20258888.top

[F09] 获取文件大小
来源：http://ryl.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://zrf.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://opk.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://tzr.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://qko.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://mxb.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://byz.aizwys.cn

Ruby: File.size("a.txt")
来源：http://nnk.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://chv.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://zgb.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ssx.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gke.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwx.pycfn.com

TS:   path.extname("a.txt")
来源：http://qyn.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mei.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vtu.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ddd.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yiy.uphjek.com

[F11] 复制与移动文件
来源：http://ypo.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jog.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lzy.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mld.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqq.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://afv.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gft.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mpj.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ucv.aibaodan.cn

[F12] CSV 读写
来源：http://pbt.xinyue.icu


<!-- 参考信息 -->