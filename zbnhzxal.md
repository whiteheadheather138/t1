代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zkt.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://kyd.gzhubu.top

Java: s.substring(1, 4)
来源：http://hlk.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ymn.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://jks.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://wmn.uphjek.com

[E04] 查找子串位置
来源：http://cjv.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://iux.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://hmm.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iie.shzxlz.cn

TS:   s.indexOf("x")
来源：http://qaf.cashguo.top

Java: s.indexOf("x")
来源：http://nmj.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://dox.hongshengwenyu.top

Ruby: s.index("x")
来源：http://ugg.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://nrk.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://abk.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qeg.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zws.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tkg.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://osb.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgk.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ouu.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lqz.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uac.bbcook.cn

[E06] 替换子串
来源：http://sno.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://faa.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://tvi.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eie.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://tkq.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnz.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hyq.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://huj.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://pij.fzhhl.top

[E07] 按分隔符拆分
来源：http://qsz.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzb.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://szg.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bty.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://msg.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://sxs.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://huh.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://xmx.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gie.yuxming.cn

[E08] 数组按分隔符合并
来源：http://gmp.sjlbkw.cn

Py:   ",".join(items)
来源：http://hgr.shzxlz.cn

PHP:  implode(",", $items);
来源：http://wle.jiagoushi.top

JS:   items.join(",")
来源：http://rch.chenzaomai.com

TS:   items.join(",")
来源：http://qnp.sufxvd.cn

Java: String.join(",", items)
来源：http://ewl.316326.xyz

Go:   strings.Join(items, ",")
来源：http://xmi.9152youxi.cn

Ruby: items.join(",")
来源：http://gek.sxryk.cn

C#:   string.Join(",", items)
来源：http://uas.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://ifz.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nie.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://byb.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://mtm.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://wuv.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://zee.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jub.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://cov.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsm.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://hba.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pmk.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bec.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://vlq.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://xxo.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://hbk.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iju.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fqh.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ucl.ivvv.top

[E11] 反转字符串
来源：http://mka.yongpay.top

Py:   s[::-1]
来源：http://jai.sjlbkw.cn

PHP:  strrev($s);
来源：http://upb.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://tzf.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://ida.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ppr.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhs.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://tto.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sfu.yvedp.cn

[E12] 统计某字符出现次数
来源：http://nhh.jlsjyb.cn

Py:   s.count("a")
来源：http://fat.birdmap.top

PHP:  substr_count($s, "a");
来源：http://rsz.yongpay.top

JS:   s.split("a").length - 1
来源：http://pub.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://fhh.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ymt.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://drm.jlsjyb.cn

Ruby: s.count("a")
来源：http://syw.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://ioh.yvedp.cn

[E13] 逐字符遍历
来源：http://vjp.havefunace.top

Py:   for ch in s: print(ch)
来源：http://rnn.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://scw.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://smb.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kuy.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://opc.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ncp.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://brt.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mmc.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://pfi.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hcx.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://wqc.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjv.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dwb.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tml.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aso.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ouz.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bzq.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://pyr.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dhb.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ojq.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nis.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yrw.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://osi.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kvq.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://glb.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cex.dianchejie.cn

[E16] 数字千分位
来源：http://ckk.sysykeji.top

Py:   f"{1234567:,}"
来源：http://cch.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://ged.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jwt.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mox.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://esa.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sup.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gzo.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://obv.yonumen.top

[E17] 首字母大写
来源：http://spq.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vac.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hwt.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgr.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://svp.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbi.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://het.ydzc1.top

Ruby: s.capitalize
来源：http://qvm.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojw.gaohongyu789.top

[E18] 模板占位符替换
来源：http://cof.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yef.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kcj.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ofx.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pek.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cmp.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uhn.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://brf.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tvh.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://eex.daxiang520.top

Py:   s.splitlines()
来源：http://udp.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vge.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://iyq.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://cmv.gaohongyu789.top

Java: s.lines().toList()
来源：http://wtj.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://box.fengsongda.top

Ruby: s.lines
来源：http://xga.hcnkem.com

C#:   s.Split('\n')
来源：http://lnl.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://kzx.snrcjt.cn

Py:   if not s:
来源：http://tyd.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eyz.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oyi.xinyue.icu

TS:   if (s === "") {}
来源：http://qby.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://rte.yj20258.top

Go:   if s == "" {}
来源：http://xcs.mhx1999.top

Ruby: if s.empty?
来源：http://bax.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wiw.cqqwz.cn

[E21] 超长截断加省略号
来源：http://fvg.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bwn.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwj.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkc.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ieg.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://csy.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://qju.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://agp.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wml.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://gvk.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wyp.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iom.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gvu.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qct.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hmi.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://utn.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://tyw.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czl.cdnleiting.top

================================================================================
来源：http://siy.ppjwa.cn

F. 文件与目录
来源：http://eip.hcnkem.com

================================================================================
来源：http://cdq.zhijiandao.cn

[F01] 读取整个文件
来源：http://rpz.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mrk.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://crf.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://smz.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hdm.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zgu.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wgg.gzhubu.top

Ruby: File.read("a.txt")
来源：http://nsb.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://htk.zdbjq.cn

[F02] 逐行读取文件
来源：http://wyp.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hiw.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://anb.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lph.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fpu.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://myi.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uid.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sge.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xtb.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://mht.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wmb.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tyk.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ust.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ulu.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bfv.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ant.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://nnr.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xle.sxryk.cn

[F04] 追加写入文件
来源：http://hhr.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ifg.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wzl.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpn.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://spg.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gvc.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://buc.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nqb.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://knt.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://mxj.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://htx.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://zbi.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://xqj.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://wyf.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kqj.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kpr.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://mec.tanke756.top

C#:   File.Exists("a.txt")
来源：http://ypb.aizwys.cn

[F06] 删除文件
来源：http://xhx.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://hcj.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://llr.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://byj.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://btq.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wwo.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://aac.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://gjj.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://uvd.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://pfy.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://env.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lfl.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://evm.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rty.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nnh.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjq.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ygw.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://amt.jqgfzy.top

[F08] 遍历目录
来源：http://dxy.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kep.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cgx.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://ffl.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://gme.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bec.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rds.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://bbp.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://lsg.jiagoushi.top

[F09] 获取文件大小
来源：http://jsc.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://eel.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://bxi.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://xif.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://ajp.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fyb.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mkf.tarul.cn

Ruby: File.size("a.txt")
来源：http://gcm.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://evk.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://iki.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xva.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xup.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zus.hammf.cn

TS:   path.extname("a.txt")
来源：http://ivn.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zuf.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gut.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gjy.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://brx.ivvv.top

[F11] 复制与移动文件
来源：http://kok.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bkz.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhm.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://anh.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kto.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://swy.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qrr.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rwf.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uvr.yfazqb.com

[F12] CSV 读写
来源：http://vcw.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxw.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnm.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yoq.chenjidiqi.icu

TS:   // 同上
来源：http://csg.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wjv.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fru.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lcv.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://xkr.fengsongda.top

================================================================================
来源：http://nzr.zhiwuduotai.top

G. 面向对象
来源：http://qvc.andypj.xyz

================================================================================
来源：http://nic.haohaochexian.top

[G01] 定义类
来源：http://dzn.sysykeji.top

Py:   class User: pass
来源：http://gbt.epnwcf.com

PHP:  class User {}
来源：http://rou.tarul.cn

JS:   class User {}
来源：http://eqq.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://ofo.haohaochexian.top

Java: class User {}
来源：http://gta.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://kko.sysykeji.top

Ruby: class User; end
来源：http://kgx.nwbrower.top

C#:   class User {}
来源：http://gca.shanyushiyangkeji.top


<!-- 参考信息 -->