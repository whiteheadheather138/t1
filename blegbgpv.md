代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ppt.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gts.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iic.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pua.mhx1999.top

[E02] 重复字符串
来源：http://cwl.daria6918.cn

Py:   "ab" * 3
来源：http://xma.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://vgy.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://sab.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://rfq.fehbvm.com

Java: "ab".repeat(3)
来源：http://jmd.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://iat.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://eda.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://evu.ctjpmb.com

[E03] 截取子串
来源：http://qnc.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://moa.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mpx.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pvm.epnwcf.com

TS:   s.slice(1, 4)
来源：http://apu.hfpthk.cn

Java: s.substring(1, 4)
来源：http://fdh.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hty.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://vss.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://zla.smart0.xyz

[E04] 查找子串位置
来源：http://xuy.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://ohd.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://fos.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vdy.yongpay.top

TS:   s.indexOf("x")
来源：http://mhd.cashguo.top

Java: s.indexOf("x")
来源：http://rth.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://mgo.fengsongda.top

Ruby: s.index("x")
来源：http://arp.iojbl.cn

C#:   s.IndexOf("x")
来源：http://eif.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ulz.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tvc.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vjh.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjf.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://omz.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zfq.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ads.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fpi.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dta.bjfxy.top

[E06] 替换子串
来源：http://zpe.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ppf.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://qyv.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jbs.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://ryo.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agu.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cot.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wep.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://gyk.meibo888.top

[E07] 按分隔符拆分
来源：http://yfk.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zab.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zqv.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sck.daxiang520.top

TS:   s.split(",")
来源：http://jwg.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://cnq.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vkt.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://awj.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mrl.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://whu.zhoulong.xyz

Py:   ",".join(items)
来源：http://yli.shuidangran.top

PHP:  implode(",", $items);
来源：http://bvg.cqqwz.cn

JS:   items.join(",")
来源：http://uas.yonumen.top

TS:   items.join(",")
来源：http://xwl.xuetiantiany.cn

Java: String.join(",", items)
来源：http://psn.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://tru.guowangkeji.top

Ruby: items.join(",")
来源：http://kgm.shzxlz.cn

C#:   string.Join(",", items)
来源：http://dhb.cqqwz.cn

[E09] 去除所有空白字符
来源：http://mka.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xmv.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://upq.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://ryd.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://yfm.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://paa.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://egk.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://jaw.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arn.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://fac.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fke.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fns.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://zet.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://vho.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://dbm.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://olw.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vmp.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pap.havefunace.top

[E11] 反转字符串
来源：http://nwj.zhongyouzk.top

Py:   s[::-1]
来源：http://wtx.shzxlz.cn

PHP:  strrev($s);
来源：http://olo.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://wvh.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://hac.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tju.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ibh.quarkkingdee.top

Ruby: s.reverse
来源：http://dpp.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://aeg.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://wfg.ivvv.top

Py:   s.count("a")
来源：http://xyp.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://pnb.cheryme.top

JS:   s.split("a").length - 1
来源：http://yde.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://sbr.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rnc.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://bko.shangyingyoupin.top

Ruby: s.count("a")
来源：http://oho.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://dcd.shzxlz.cn

[E13] 逐字符遍历
来源：http://vql.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://sqz.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ezz.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://deo.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oli.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://asr.gzhubu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nqf.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mlp.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ehy.fengsongda.top

[E14] URL 编码与 Base64
来源：http://erx.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxn.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dik.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vez.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uvk.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://slg.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtr.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://btx.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qwu.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://mrn.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tfq.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oeb.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nxd.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xjk.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fkq.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iiq.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fyw.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://frw.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://vao.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://xma.aizwys.cn

PHP:  number_format(1234567);
来源：http://ckc.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uen.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ivt.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vvb.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uxw.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fjz.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://fop.tarul.cn

[E17] 首字母大写
来源：http://bpd.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gjb.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pep.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oyc.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omv.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bvu.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ddt.ehwqpu.com

Ruby: s.capitalize
来源：http://pfu.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zzo.zhixingplan.top

[E18] 模板占位符替换
来源：http://wmv.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ypa.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hgr.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kgi.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bko.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kki.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qaa.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://axr.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://guh.fktsv.cn

[E19] 多行文本按行拆分
来源：http://mvp.yuanzhike.top

Py:   s.splitlines()
来源：http://xzu.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ocb.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://nnx.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://ymi.havefunace.top

Java: s.lines().toList()
来源：http://nxs.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://wiv.sxryk.cn

Ruby: s.lines
来源：http://fry.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://oer.sxryk.cn

[E20] 判断字符串是否为空
来源：http://ghn.ctjpmb.com

Py:   if not s:
来源：http://ifv.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pnm.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://php.jinqigfzy.top

TS:   if (s === "") {}
来源：http://gic.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://afk.ivvv.top

Go:   if s == "" {}
来源：http://hul.jinqigufen.top

Ruby: if s.empty?
来源：http://yjt.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wxa.vehdjk.com

[E21] 超长截断加省略号
来源：http://afr.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dil.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://opi.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvt.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gma.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ful.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://qaj.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wxf.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wfh.daxiang520.top

[E22] 字节长度与字符长度
来源：http://ymh.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lir.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cjf.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vjn.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gic.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ewr.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://brt.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://zqn.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zdc.yvedp.cn

================================================================================
来源：http://uay.hnqzz.top

F. 文件与目录
来源：http://rwc.daria6918.cn

================================================================================
来源：http://aty.fktsv.cn

[F01] 读取整个文件
来源：http://hsc.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lio.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://niq.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tlb.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xdd.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rdd.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xqc.bjfxy.top

Ruby: File.read("a.txt")
来源：http://zei.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://uux.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://qab.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://spw.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kmu.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xsz.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzt.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yje.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zgc.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kvb.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vyt.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://bnq.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ran.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zuo.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqo.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pwb.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uhi.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qlf.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://wzk.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ine.mhx1999.top

[F04] 追加写入文件
来源：http://wyn.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://duc.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ibs.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hbw.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hoe.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nma.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eac.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://muj.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://plz.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://fzw.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lpr.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://xsr.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://fuj.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://mxr.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wkw.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://erl.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://vwh.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://sac.jianghu66.top

[F06] 删除文件
来源：http://gcv.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://fmg.daria6918.cn

PHP:  unlink("a.txt");
来源：http://gra.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bof.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://ihl.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://txu.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://nlk.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://pax.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://rcc.tarul.cn

[F07] 创建目录（含多级）
来源：http://zgq.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jdp.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rao.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hym.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cek.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://usx.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dbt.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jbo.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dsu.pengpengdd.cyou

[F08] 遍历目录
来源：http://lct.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fnf.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://isx.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://qms.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://jvb.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://afl.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qlu.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://lus.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://lzm.9152youxi.cn

[F09] 获取文件大小
来源：http://cmd.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://xxl.yueranfly.top

PHP:  filesize("a.txt");
来源：http://din.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://pjw.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://tug.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://lbz.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://puc.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://pnj.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://kon.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://qws.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wlh.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sva.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mvm.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://kju.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://coe.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kra.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mox.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ssc.mhx1999.top

[F11] 复制与移动文件
来源：http://kzm.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ocb.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zkp.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vtw.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ogn.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wvk.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gsw.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tzg.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gxq.hnxiangtu.top

[F12] CSV 读写
来源：http://fvk.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xic.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qji.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nla.xinyue.icu

TS:   // 同上
来源：http://rid.andypj.xyz


<!-- 参考信息 -->