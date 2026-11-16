代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qel.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ikz.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://slj.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pww.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nfo.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://edb.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sgt.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sui.yonumen.top

[E02] 重复字符串
来源：http://csl.hnqzz.top

Py:   "ab" * 3
来源：http://ppv.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://arw.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://ock.hammf.cn

TS:   "ab".repeat(3)
来源：http://imd.c1oappe.top

Java: "ab".repeat(3)
来源：http://phe.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://cha.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://rzm.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://euv.dianchejie.cn

[E03] 截取子串
来源：http://olp.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zjp.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mbe.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gsq.yongpay.top

TS:   s.slice(1, 4)
来源：http://dnk.dashuyun.cn

Java: s.substring(1, 4)
来源：http://pns.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wmp.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://lgg.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://hua.fengsongda.top

[E04] 查找子串位置
来源：http://aby.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://paj.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://tjh.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vrr.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://imt.gaohongyu789.top

Java: s.indexOf("x")
来源：http://pjq.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://asz.shzxlz.cn

Ruby: s.index("x")
来源：http://kmi.ybcxt.top

C#:   s.IndexOf("x")
来源：http://fjb.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jge.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zyx.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kjd.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://saa.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pyc.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyg.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fqp.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fxd.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fwt.xylfe.cn

[E06] 替换子串
来源：http://qma.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kal.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://rxh.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odo.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://tmc.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpr.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dfi.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kdz.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://mso.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://xck.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cbd.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vjy.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ndh.zhijiandao.cn

TS:   s.split(",")
来源：http://ljh.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://xdt.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydt.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://peq.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vbv.xinyue.icu

[E08] 数组按分隔符合并
来源：http://elt.gzhubu.top

Py:   ",".join(items)
来源：http://ute.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://fhz.yvedp.cn

JS:   items.join(",")
来源：http://byc.iojbl.cn

TS:   items.join(",")
来源：http://etz.gaohongyu789.top

Java: String.join(",", items)
来源：http://chp.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://igo.xuetiantiany.cn

Ruby: items.join(",")
来源：http://zsn.cheryme.top

C#:   string.Join(",", items)
来源：http://ccm.yj20258.top

[E09] 去除所有空白字符
来源：http://kct.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://etd.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ihi.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://rcx.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://qit.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://lcb.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmm.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://zdl.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mha.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://gbn.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uvk.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://syn.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://bxz.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://pox.316326.xyz

Java: String.format("%03d", 7)
来源：http://wff.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lbd.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aoy.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zmu.zhixingplan.top

[E11] 反转字符串
来源：http://zvb.0kj1m.cn

Py:   s[::-1]
来源：http://cyj.vqdsnc.cn

PHP:  strrev($s);
来源：http://jld.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://bdz.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://sbg.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mtp.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ruo.ppjwa.cn

Ruby: s.reverse
来源：http://wes.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fnf.fengsongda.top

[E12] 统计某字符出现次数
来源：http://qfh.zycfv.cn

Py:   s.count("a")
来源：http://cel.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://pnq.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://grf.cheryme.top

TS:   s.split("a").length - 1
来源：http://ceg.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uiq.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://dum.hesvh.cn

Ruby: s.count("a")
来源：http://ehv.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://phq.gaohongyu789.top

[E13] 逐字符遍历
来源：http://ffs.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://fqi.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sib.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cvx.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vat.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://svi.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nkk.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pop.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qia.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://wam.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uuu.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://egt.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ohh.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baa.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://irz.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bjg.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mhs.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jrg.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://ueq.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eqf.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bkr.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iug.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pnr.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lth.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xrq.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oac.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://soy.zdqjudy.top

[E16] 数字千分位
来源：http://mox.fktsv.cn

Py:   f"{1234567:,}"
来源：http://ldh.zdbjq.cn

PHP:  number_format(1234567);
来源：http://dew.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jku.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://azb.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fzv.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qwx.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kdo.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://kxo.zycfv.cn

[E17] 首字母大写
来源：http://cxh.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hsq.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zhb.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nex.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oor.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kuc.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rnl.uphjek.com

Ruby: s.capitalize
来源：http://gcd.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rcj.hnxiangtu.top

[E18] 模板占位符替换
来源：http://yap.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fta.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lky.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dco.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ybq.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hys.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wgg.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wdr.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iww.yfazqb.com

[E19] 多行文本按行拆分
来源：http://hlq.sufxvd.cn

Py:   s.splitlines()
来源：http://vtx.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mpy.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://umx.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://qhv.ydjk.org.cn

Java: s.lines().toList()
来源：http://ytc.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://wiq.shangyingyoupin.top

Ruby: s.lines
来源：http://dam.xuanzx.com

C#:   s.Split('\n')
来源：http://fez.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://fhb.epnwcf.com

Py:   if not s:
来源：http://zoc.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tzl.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fso.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://dqh.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://cgp.jqgufenzy.top

Go:   if s == "" {}
来源：http://ifx.yj20258.top

Ruby: if s.empty?
来源：http://wfr.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wby.ydzc1.top

[E21] 超长截断加省略号
来源：http://bal.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://heu.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fxn.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udy.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnf.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://usa.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://nhs.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tco.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lav.ydzc1.top

[E22] 字节长度与字符长度
来源：http://fpi.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://whc.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wbn.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jwh.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://czb.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rwh.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fnu.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://bft.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hes.sxryk.cn

================================================================================
来源：http://drh.fzhhl.top

F. 文件与目录
来源：http://fjv.hysaishi.cn

================================================================================
来源：http://soa.sysykeji.top

[F01] 读取整个文件
来源：http://hif.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uey.pengpengdd.cyou

PHP:  file_get_contents("a.txt");
来源：http://nmh.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xoy.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hhn.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rqj.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hox.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://idb.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://lie.hcnkem.com

[F02] 逐行读取文件
来源：http://kjg.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://agu.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qef.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://itm.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pmf.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pdb.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://acn.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kvv.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dmz.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://vgo.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lzt.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hzr.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pil.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epr.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rda.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dti.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://qpg.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oca.sufxvd.cn

[F04] 追加写入文件
来源：http://dyj.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yzs.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nqt.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gdx.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tss.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bkt.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yue.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gwc.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qol.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://qso.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zzn.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://jpl.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://amg.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://vgx.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tfv.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tgo.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://gxv.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://yvg.yongpay.top

[F06] 删除文件
来源：http://guf.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://qgk.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://ike.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kth.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ysw.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aec.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://roc.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://gcs.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://egn.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://cjf.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pdk.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drd.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zoy.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://okt.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xjn.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fyy.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vno.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mir.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://nej.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://msd.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wvn.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://tmz.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://vry.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zvd.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dxj.daria6918.cn

Ruby: Dir.children("dir")
来源：http://mhq.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://hxq.cashguo.top

[F09] 获取文件大小
来源：http://gtr.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://goh.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://mhw.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://ghy.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://wog.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://eqw.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xmg.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://dnw.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://jpk.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://tzb.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dre.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yez.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bef.jianghu66.top

TS:   path.extname("a.txt")
来源：http://bxy.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wmz.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vrx.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eyk.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tdv.hammf.cn

[F11] 复制与移动文件
来源：http://ugj.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ntz.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ydi.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wtn.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpl.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gcx.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zhj.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mrg.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://png.cdnleiting.top

[F12] CSV 读写
来源：http://uzo.chenlongwang.top


<!-- 参考信息 -->