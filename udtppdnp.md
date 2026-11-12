代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yha.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://asi.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://acu.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzp.ppjwa.cn

[E02] 重复字符串
来源：http://nzj.jyoumei.cn

Py:   "ab" * 3
来源：http://mno.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://uwl.zycfv.cn

JS:   "ab".repeat(3)
来源：http://quy.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://ydt.fehbvm.com

Java: "ab".repeat(3)
来源：http://wyo.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://kgc.hywenlv.cn

Ruby: "ab" * 3
来源：http://fve.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jfv.vehdjk.com

[E03] 截取子串
来源：http://iff.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vdg.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xlb.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rga.fzhhl.top

TS:   s.slice(1, 4)
来源：http://vee.pycfn.com

Java: s.substring(1, 4)
来源：http://kps.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqd.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zzj.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://wft.nwbrower.top

[E04] 查找子串位置
来源：http://qsj.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://wje.yj202588.top

PHP:  strpos($s, "x");
来源：http://uol.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cle.cucudq.cn

TS:   s.indexOf("x")
来源：http://scy.fzhhl.top

Java: s.indexOf("x")
来源：http://wfr.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://yos.cdnleiting.top

Ruby: s.index("x")
来源：http://fmm.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://lrv.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ggd.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gfb.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyq.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://daw.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fej.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tev.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebk.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fnp.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lsl.ppjwa.cn

[E06] 替换子串
来源：http://tvn.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dop.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://ghm.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcn.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://bij.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://peq.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hff.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kft.yongpay.top

C#:   s.Replace("a", "b")
来源：http://zjn.cdnleiting.top

[E07] 按分隔符拆分
来源：http://lhx.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bcu.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://myv.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://wsj.yongpay.top

TS:   s.split(",")
来源：http://ewx.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://edb.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kmm.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://ijx.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pkt.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://vfe.316326.xyz

Py:   ",".join(items)
来源：http://okz.ppjwa.cn

PHP:  implode(",", $items);
来源：http://lzp.smart0.xyz

JS:   items.join(",")
来源：http://xwr.tian-w.cn

TS:   items.join(",")
来源：http://rvu.xuanzx.com

Java: String.join(",", items)
来源：http://bru.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://ymw.wangshuangyany.cn

Ruby: items.join(",")
来源：http://ghr.epnwcf.com

C#:   string.Join(",", items)
来源：http://wrg.hcnkem.com

[E09] 去除所有空白字符
来源：http://imw.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jxg.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eto.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ufe.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://vwy.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://cpz.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tex.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://nvx.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kvb.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://tpy.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zap.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://til.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://ipm.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://oqg.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://krw.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hcj.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzm.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ojw.meibo888.top

[E11] 反转字符串
来源：http://uuh.daxiang520.top

Py:   s[::-1]
来源：http://gpg.yanxiufei.cn

PHP:  strrev($s);
来源：http://czn.pycfn.com

JS:   [...s].reverse().join("")
来源：http://udd.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://fje.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ziw.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kpx.ehwqpu.com

Ruby: s.reverse
来源：http://cza.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fgc.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://zaz.zhixingplan.top

Py:   s.count("a")
来源：http://wck.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://vuy.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://wwc.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://tzt.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qcw.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://nqf.tarul.cn

Ruby: s.count("a")
来源：http://eki.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://cnc.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://xci.tanke756.top

Py:   for ch in s: print(ch)
来源：http://wmz.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dlv.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iuq.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yft.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kls.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xgq.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lvf.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kts.yuxming.cn

[E14] URL 编码与 Base64
来源：http://eyq.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rkn.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rmn.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cml.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pce.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ppk.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xxv.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ppl.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyq.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://fqf.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wyx.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uby.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gml.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://uin.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kgg.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lcg.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nxb.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aug.meibo888.top

[E16] 数字千分位
来源：http://ifz.52xcode.cn

Py:   f"{1234567:,}"
来源：http://aki.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://iby.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://umn.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uys.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aey.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rfe.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgx.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://faw.316326.xyz

[E17] 首字母大写
来源：http://pma.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eeq.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bez.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbs.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tkl.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bew.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ggb.mhx1999.top

Ruby: s.capitalize
来源：http://lba.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xnx.xziqi.cn

[E18] 模板占位符替换
来源：http://ial.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bae.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hxy.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nkp.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gix.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iqr.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fiz.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bqu.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://adg.shuidangran.top

[E19] 多行文本按行拆分
来源：http://gpp.andypj.xyz

Py:   s.splitlines()
来源：http://fpt.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjy.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://rex.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://zib.tarul.cn

Java: s.lines().toList()
来源：http://agw.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://mfp.yvedp.cn

Ruby: s.lines
来源：http://myv.ppjwa.cn

C#:   s.Split('\n')
来源：http://ssm.fengsongda.top

[E20] 判断字符串是否为空
来源：http://kyb.fehbvm.com

Py:   if not s:
来源：http://pcl.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uyw.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uqq.cheryme.top

TS:   if (s === "") {}
来源：http://pmb.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://qza.jianghu66.top

Go:   if s == "" {}
来源：http://zep.jiagoushi.top

Ruby: if s.empty?
来源：http://iox.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rnv.tian-w.cn

[E21] 超长截断加省略号
来源：http://jjj.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sec.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iek.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpc.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbx.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hqv.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://xhu.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cij.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dlk.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://jks.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tgk.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsc.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ybr.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gpv.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iiy.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blp.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://ubg.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xkl.zhiwuduotai.top

================================================================================
来源：http://del.gaohongyu789.top

F. 文件与目录
来源：http://tii.zhengqikj.top

================================================================================
来源：http://pkv.xuetiantiany.cn

[F01] 读取整个文件
来源：http://olv.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hik.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://eid.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gaj.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qao.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wcn.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rtm.yvedp.cn

Ruby: File.read("a.txt")
来源：http://wer.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://tod.aibaodan.cn

[F02] 逐行读取文件
来源：http://zxa.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://opw.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jyd.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ojq.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zsv.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lzq.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kct.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dcp.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vgb.birdmap.top

[F03] 写入文件（覆盖）
来源：http://knp.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sdd.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qom.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkn.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxj.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sns.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cbm.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://jyh.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pzb.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://yqe.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mrj.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qyo.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sib.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eod.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://meo.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eip.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pzs.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mkc.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://aku.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dyb.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://iba.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://ltv.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://rnb.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wmx.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iaa.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://axv.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://bab.yanxiufei.cn

[F06] 删除文件
来源：http://tnz.uphjek.com

Py:   os.remove("a.txt")
来源：http://upt.sweek.top

PHP:  unlink("a.txt");
来源：http://dxj.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://rsm.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://gxd.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://teb.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://xqc.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://djn.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://yzs.ydzc1.top

[F07] 创建目录（含多级）
来源：http://fuu.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ald.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tzm.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rba.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvp.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rst.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zta.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tun.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dzb.hesvh.cn

[F08] 遍历目录
来源：http://ulk.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cls.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dns.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://ehs.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://fao.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zjj.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://run.shuidangran.top

Ruby: Dir.children("dir")
来源：http://fpo.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://ryx.guowangkeji.top

[F09] 获取文件大小
来源：http://zas.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://foo.ybcxt.top

PHP:  filesize("a.txt");
来源：http://mlu.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://vob.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://ecm.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://unr.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lqk.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://azw.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://guu.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://qbn.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ohc.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tsa.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oqp.andypj.xyz

TS:   path.extname("a.txt")
来源：http://gfe.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rll.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ssj.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rur.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aym.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://fha.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tma.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jeu.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kja.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://suz.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://khz.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pxq.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pem.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lzw.yj202588.top

[F12] CSV 读写
来源：http://kqy.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kcs.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://imn.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bzb.chenjidiqi.icu

TS:   // 同上
来源：http://hkt.gaohongyu789.top


<!-- 参考信息 -->