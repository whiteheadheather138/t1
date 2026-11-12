代发 wailian999

================================================================================
来源：http://rmo.sweek.top

E. 字符串处理
来源：http://fci.tian-w.cn

================================================================================
来源：http://yzv.uphjek.com

[E01] 拼接字符串
来源：http://qar.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ith.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://exc.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tbt.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rya.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rvu.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qrc.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wuc.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lsf.zdqjudy.top

[E02] 重复字符串
来源：http://eph.hysaishi.cn

Py:   "ab" * 3
来源：http://gtb.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://jlv.yfazqb.com

JS:   "ab".repeat(3)
来源：http://thw.yvedp.cn

TS:   "ab".repeat(3)
来源：http://nqe.nanxinkj.top

Java: "ab".repeat(3)
来源：http://blw.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zjm.0kj1m.cn

Ruby: "ab" * 3
来源：http://udp.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sfz.zycfv.cn

[E03] 截取子串
来源：http://pgj.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fgj.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kov.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jqe.yfazqb.com

TS:   s.slice(1, 4)
来源：http://vff.hywenlv.cn

Java: s.substring(1, 4)
来源：http://itu.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fsr.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vfu.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://nqq.yj202588.top

[E04] 查找子串位置
来源：http://urp.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://rmg.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://sli.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jkn.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://lrq.nwbrower.top

Java: s.indexOf("x")
来源：http://lyn.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://bke.ehwqpu.com

Ruby: s.index("x")
来源：http://izz.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://fbv.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ugw.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmx.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://seb.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://unb.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zgs.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jga.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uft.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tqv.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nof.tian-w.cn

[E06] 替换子串
来源：http://xdk.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://unt.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://msb.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ukv.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://qiz.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqt.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gua.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wna.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://pra.iojbl.cn

[E07] 按分隔符拆分
来源：http://bus.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vbw.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aww.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lui.shanyushiyangtech.top

TS:   s.split(",")
来源：http://bph.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://dek.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://inv.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://zkf.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rok.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://ntu.smart0.xyz

Py:   ",".join(items)
来源：http://fvh.cqqwz.cn

PHP:  implode(",", $items);
来源：http://qmk.zhiwuduotai.top

JS:   items.join(",")
来源：http://jmo.vehdjk.com

TS:   items.join(",")
来源：http://mmt.zdqjudy.top

Java: String.join(",", items)
来源：http://ukz.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://vqg.tian-w.cn

Ruby: items.join(",")
来源：http://qkz.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://wob.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://cud.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lpe.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://byu.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://pbm.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://slp.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://wbe.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oho.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yvf.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dca.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://kwn.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qjd.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dbl.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://fln.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://ual.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://qlp.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hpz.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yvh.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zjn.316326.xyz

[E11] 反转字符串
来源：http://qdm.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://usn.316326.xyz

PHP:  strrev($s);
来源：http://tqq.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://kox.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://bhn.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vfe.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zee.yj20258888.top

Ruby: s.reverse
来源：http://mfd.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zaz.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://qqi.zhijiandao.cn

Py:   s.count("a")
来源：http://nan.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://jsz.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://hoa.sysykeji.top

TS:   s.split("a").length - 1
来源：http://jsg.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osz.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://isx.hcnkem.com

Ruby: s.count("a")
来源：http://sji.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://rul.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://qhb.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://yrj.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ghk.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sdy.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://prj.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wra.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dam.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eoe.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kwj.cheryme.top

[E14] URL 编码与 Base64
来源：http://mqe.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qat.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fty.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ony.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fwi.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vdm.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wuw.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cvt.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wua.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://ayj.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pto.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oit.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zbs.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ery.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jxm.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwx.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://niw.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztk.feifeiyinyue.top

[E16] 数字千分位
来源：http://aor.fktsv.cn

Py:   f"{1234567:,}"
来源：http://qep.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://uxg.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://imd.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xlz.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eea.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vmt.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jan.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://grm.zycfv.cn

[E17] 首字母大写
来源：http://ikx.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fsh.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://znb.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdk.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfc.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://opu.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dpt.zdqjudy.top

Ruby: s.capitalize
来源：http://ann.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tir.yonumen.top

[E18] 模板占位符替换
来源：http://ipu.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vym.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tsg.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dpc.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rvo.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://obg.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hpk.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iyq.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://agf.yueranfly.top

[E19] 多行文本按行拆分
来源：http://brw.vqdsnc.cn

Py:   s.splitlines()
来源：http://xez.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sfv.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://rmv.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://geh.c1oappe.top

Java: s.lines().toList()
来源：http://uzg.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://zjf.guowangkeji.top

Ruby: s.lines
来源：http://wgw.gogol.net.cn

C#:   s.Split('\n')
来源：http://xxj.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://vcf.vehdjk.com

Py:   if not s:
来源：http://mkt.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vov.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ytf.jyoumei.cn

TS:   if (s === "") {}
来源：http://zbs.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://xkm.zhoulong.xyz

Go:   if s == "" {}
来源：http://afj.smart0.xyz

Ruby: if s.empty?
来源：http://ioe.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gik.dianchejie.cn

[E21] 超长截断加省略号
来源：http://gow.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://die.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://exu.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rqx.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bhn.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lhz.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://aqf.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sgm.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fjj.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://gns.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://efl.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://udm.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijv.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dyc.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jhd.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://smf.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://iwf.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kxt.uphjek.com

================================================================================
来源：http://pqi.jinyuanbaomall.cn

F. 文件与目录
来源：http://joa.shanyushiyangtech.top

================================================================================
来源：http://wll.vqdsnc.cn

[F01] 读取整个文件
来源：http://yjc.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://koy.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://enb.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sff.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gca.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dzh.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vkj.tanke756.top

Ruby: File.read("a.txt")
来源：http://eln.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://ylw.shzxlz.cn

[F02] 逐行读取文件
来源：http://tus.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xko.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://evg.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frg.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xnb.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oed.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tkr.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iuo.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://met.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://ygk.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmf.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nci.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyb.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gaj.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kjf.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lyv.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://otn.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dts.jqgfzy.top

[F04] 追加写入文件
来源：http://wzu.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ges.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nge.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxf.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vhu.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://isc.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dgz.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pfv.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qxw.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://zmg.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hnf.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://czy.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://btu.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://qnf.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gds.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eva.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://apu.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://zwr.jinqigfzy.top

[F06] 删除文件
来源：http://htr.cashguo.top

Py:   os.remove("a.txt")
来源：http://ivz.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://eqz.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wrd.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://rub.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rhe.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://ocr.cheryme.top

Ruby: File.delete("a.txt")
来源：http://rrh.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://gbo.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://prf.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://grp.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://atd.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://imy.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xko.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fxh.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aqd.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dym.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://icn.cqqwz.cn

[F08] 遍历目录
来源：http://qtt.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://eno.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fak.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://vxs.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://jft.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iwy.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zpm.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://hgh.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://xme.ivvv.top

[F09] 获取文件大小
来源：http://ugt.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://flu.sysykeji.top

PHP:  filesize("a.txt");
来源：http://tco.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://zfa.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://rsg.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uxg.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rbo.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://wzp.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://cft.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://ymq.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdt.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjj.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ops.yongpay.top

TS:   path.extname("a.txt")
来源：http://hrm.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cuj.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bsj.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mch.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kwe.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://rkb.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jlz.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://efl.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://izx.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpj.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gef.svipenyu.cn


<!-- 参考信息 -->