代发 wailian999

[E02] 重复字符串
来源：http://eeq.fzhhl.top

Py:   "ab" * 3
来源：http://oxl.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://edx.xinyue.icu

JS:   "ab".repeat(3)
来源：http://str.daxiang520.top

TS:   "ab".repeat(3)
来源：http://tew.nanxinkj.top

Java: "ab".repeat(3)
来源：http://zks.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://opq.ehwqpu.com

Ruby: "ab" * 3
来源：http://crm.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tuy.xuanzx.com

[E03] 截取子串
来源：http://wku.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lcc.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mem.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tcz.yj202588.top

TS:   s.slice(1, 4)
来源：http://nws.cqqwz.cn

Java: s.substring(1, 4)
来源：http://zju.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dzl.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xeo.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://jvj.yueranfly.top

[E04] 查找子串位置
来源：http://ukh.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://xdj.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://yrv.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dmx.jyoumei.cn

TS:   s.indexOf("x")
来源：http://nnb.yj20258.top

Java: s.indexOf("x")
来源：http://sbe.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://ybl.xziqi.cn

Ruby: s.index("x")
来源：http://ouz.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://rli.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mxu.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tbl.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uyc.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hov.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zry.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nde.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksc.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qvk.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yan.wangdashe.top

[E06] 替换子串
来源：http://jje.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kdj.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://wuq.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lly.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://frk.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbl.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wxe.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oxi.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://ftm.cheryme.top

[E07] 按分隔符拆分
来源：http://cmd.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://opr.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xfy.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xvu.xuetiantiany.cn

TS:   s.split(",")
来源：http://lhu.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://uyr.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://erc.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://sso.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rks.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://jyd.shuidangran.top

Py:   ",".join(items)
来源：http://whe.guowangkeji.top

PHP:  implode(",", $items);
来源：http://zqz.shangyingyoupin.top

JS:   items.join(",")
来源：http://ous.zhiwuduotai.top

TS:   items.join(",")
来源：http://xxy.yj20258888.top

Java: String.join(",", items)
来源：http://jmf.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://zik.jlsjyb.cn

Ruby: items.join(",")
来源：http://xsl.316326.xyz

C#:   string.Join(",", items)
来源：http://ovz.c1oappe.top

[E09] 去除所有空白字符
来源：http://zuh.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cng.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gdt.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://bpq.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://lwr.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://buo.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ttm.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sdp.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pmh.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://emi.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqx.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xoj.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://ugf.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://qly.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://pxi.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yuz.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://thk.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mye.birdmap.top

[E11] 反转字符串
来源：http://rmd.fktsv.cn

Py:   s[::-1]
来源：http://eub.jyoumei.cn

PHP:  strrev($s);
来源：http://tqb.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://vaf.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://mkd.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ids.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wgv.aibaodan.cn

Ruby: s.reverse
来源：http://tzg.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://ueg.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://jud.0kj1m.cn

Py:   s.count("a")
来源：http://xfw.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://odp.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://sjb.cashguo.top

TS:   s.split("a").length - 1
来源：http://vvn.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rix.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://ksc.chenzaomai.com

Ruby: s.count("a")
来源：http://rbw.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://oiz.ydzc1.top

[E13] 逐字符遍历
来源：http://wij.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://bls.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tqz.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uli.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bhr.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://olw.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jco.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ubx.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mdj.hesvh.cn

[E14] URL 编码与 Base64
来源：http://ixu.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zwf.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xbk.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vwk.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxc.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://axh.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ahh.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ecl.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sgs.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://nlq.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://etm.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pkx.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hqi.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://xrz.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hyc.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ojs.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ywe.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dhn.xuetiantiany.cn

[E16] 数字千分位
来源：http://lms.fktsv.cn

Py:   f"{1234567:,}"
来源：http://ltq.hysaishi.cn

PHP:  number_format(1234567);
来源：http://urx.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://puh.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kqy.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xky.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pnq.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://deg.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://hbl.ppjwa.cn

[E17] 首字母大写
来源：http://msm.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jmm.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xlb.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zlo.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fha.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://etb.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xsl.0kj1m.cn

Ruby: s.capitalize
来源：http://bfg.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nrv.fzhhl.top

[E18] 模板占位符替换
来源：http://lfj.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jxt.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qaa.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rfy.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dhg.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hgp.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pqz.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fhj.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzz.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://ioq.smart0.xyz

Py:   s.splitlines()
来源：http://izg.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zja.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://sbv.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://rwi.hysaishi.cn

Java: s.lines().toList()
来源：http://wns.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://yjk.uphjek.com

Ruby: s.lines
来源：http://gih.zhijiandao.cn

C#:   s.Split('\n')
来源：http://kcu.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://yfd.yongpay.top

Py:   if not s:
来源：http://juc.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gcx.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mvg.cqqwz.cn

TS:   if (s === "") {}
来源：http://qyp.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://uya.chenjidiqi.icu

Go:   if s == "" {}
来源：http://wno.tian-w.cn

Ruby: if s.empty?
来源：http://kyh.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbh.jqgfzy.top

[E21] 超长截断加省略号
来源：http://zqu.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rez.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mby.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pnj.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://emv.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nyd.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://nas.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ukl.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fxo.smart0.xyz

[E22] 字节长度与字符长度
来源：http://jec.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://knr.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jku.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kkd.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhb.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfc.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qgb.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://aie.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ogj.sysykeji.top

================================================================================
来源：http://bzx.shzxlz.cn

F. 文件与目录
来源：http://pgv.daria6918.cn

================================================================================
来源：http://cit.tanke756.top

[F01] 读取整个文件
来源：http://mjz.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gsr.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://fsh.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vwc.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rma.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bxh.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://esv.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://cbv.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://azz.tanke756.top

[F02] 逐行读取文件
来源：http://qdh.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rrx.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ywk.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfv.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcz.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ygt.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pxp.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lzz.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ywf.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://qaq.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pwp.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ohq.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dly.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyw.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://not.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zzq.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://woh.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bkr.ybcxt.top

[F04] 追加写入文件
来源：http://iml.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kuf.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dkq.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ogn.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ori.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ynt.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wkr.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nhd.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dzz.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://cpb.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ktc.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://xjv.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://dwn.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://mvh.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://riv.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tos.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://fiv.yj202588.top

C#:   File.Exists("a.txt")
来源：http://gqs.sweek.top

[F06] 删除文件
来源：http://zpv.ybcxt.top

Py:   os.remove("a.txt")
来源：http://pxz.iojbl.cn

PHP:  unlink("a.txt");
来源：http://cwb.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tuc.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://pkt.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhs.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://ysh.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://sbh.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://gvf.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://gig.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yuo.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vga.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://knh.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bfy.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://enl.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yxt.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bos.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmy.dashuyun.cn

[F08] 遍历目录
来源：http://yxu.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://kqz.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://enn.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://pcz.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://moc.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvg.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://szt.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://rsv.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://luz.hywenlv.cn

[F09] 获取文件大小
来源：http://ydr.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://coz.fengsongda.top

PHP:  filesize("a.txt");
来源：http://mcr.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://vkl.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://qym.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://psx.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mwi.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://xfd.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://qnk.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://rlm.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ktb.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qsi.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wqz.xinyue.icu

TS:   path.extname("a.txt")
来源：http://ari.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hkz.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://int.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vlj.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iky.xziqi.cn

[F11] 复制与移动文件
来源：http://itr.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pog.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ysx.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkl.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mna.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aas.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://scn.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cya.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://evy.xylfe.cn

[F12] CSV 读写
来源：http://ggs.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cgs.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hwu.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ssz.hnxiangtu.top

TS:   // 同上
来源：http://ags.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rts.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ous.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cmm.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://pai.cheryme.top


<!-- 参考信息 -->