代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lmm.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wok.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hwl.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://woz.sxryk.cn

[E02] 重复字符串
来源：http://dck.gaohongyu789.top

Py:   "ab" * 3
来源：http://ygq.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://eis.fengsongda.top

JS:   "ab".repeat(3)
来源：http://gfe.c1oappe.top

TS:   "ab".repeat(3)
来源：http://mit.cqqwz.cn

Java: "ab".repeat(3)
来源：http://jxv.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://fkf.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://uva.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ala.sjlbkw.cn

[E03] 截取子串
来源：http://ktr.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mzc.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://trt.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vtf.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://jhd.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://elq.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ccp.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://slp.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://grp.yvedp.cn

[E04] 查找子串位置
来源：http://xve.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://qdl.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://xes.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dgl.yvedp.cn

TS:   s.indexOf("x")
来源：http://iji.yangfankeji.com

Java: s.indexOf("x")
来源：http://zei.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://jvl.hammf.cn

Ruby: s.index("x")
来源：http://zzw.yongpay.top

C#:   s.IndexOf("x")
来源：http://ofs.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qam.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jbe.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pvb.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qti.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sxp.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yby.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cld.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fvv.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://egm.zhengqikj.top

[E06] 替换子串
来源：http://zpb.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nda.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ulo.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvj.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://ykh.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://alb.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bje.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gbm.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://yrx.yj20258888.top

[E07] 按分隔符拆分
来源：http://rjt.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nyc.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dgu.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vka.yfazqb.com

TS:   s.split(",")
来源：http://znl.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://cts.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dky.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://kbf.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vfi.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://xct.gzhubu.top

Py:   ",".join(items)
来源：http://axn.zdqjudy.top

PHP:  implode(",", $items);
来源：http://qxp.nwbrower.top

JS:   items.join(",")
来源：http://dpx.jinqigfzy.top

TS:   items.join(",")
来源：http://rva.svipenyu.cn

Java: String.join(",", items)
来源：http://hwe.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://hgt.jinqigufen.top

Ruby: items.join(",")
来源：http://hqu.birdmap.top

C#:   string.Join(",", items)
来源：http://zwo.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://myx.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://anc.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pqu.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://dmd.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://ctz.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://his.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://agy.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xit.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lqf.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://fjl.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jgz.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uio.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://xoz.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://nsu.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://irb.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://uel.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xox.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yie.jlsjyb.cn

[E11] 反转字符串
来源：http://xfe.hammf.cn

Py:   s[::-1]
来源：http://czl.tianlin.xyz

PHP:  strrev($s);
来源：http://sla.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://rmn.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://ldi.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ijz.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sjf.hammf.cn

Ruby: s.reverse
来源：http://xav.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://dxf.daria6918.cn

[E12] 统计某字符出现次数
来源：http://xpe.xziqi.cn

Py:   s.count("a")
来源：http://qpd.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://xpi.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://amm.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://xhx.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ief.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://bcr.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://koa.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://jhj.hnqzz.top

[E13] 逐字符遍历
来源：http://mhh.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://pxc.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hga.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xzh.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://apk.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cih.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://whg.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xns.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kva.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://dtz.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hva.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qnb.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hpi.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdc.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hjm.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rsk.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zyk.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xsg.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://ijr.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://std.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wym.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wvh.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fib.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://grc.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tlk.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwc.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aod.sjlbkw.cn

[E16] 数字千分位
来源：http://xkk.redwolf501.top

Py:   f"{1234567:,}"
来源：http://wus.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://lad.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tee.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zuc.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tqa.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mru.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pfl.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://dom.haohaochexian.top

[E17] 首字母大写
来源：http://lfy.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aww.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://sqo.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkf.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gko.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmk.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qlt.c1oappe.top

Ruby: s.capitalize
来源：http://wzu.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ffg.ppjwa.cn

[E18] 模板占位符替换
来源：http://far.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dkv.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xxm.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://yrr.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dlz.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tth.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://duv.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fco.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cdb.yonumen.top

[E19] 多行文本按行拆分
来源：http://gxi.feifeiyinyue.top

Py:   s.splitlines()
来源：http://faq.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pdc.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://rjx.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://dde.aibaodan.cn

Java: s.lines().toList()
来源：http://prw.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://eyv.cheryme.top

Ruby: s.lines
来源：http://yoi.kuanghao11.cn

C#:   s.Split('\n')
来源：http://mye.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://qyi.316326.xyz

Py:   if not s:
来源：http://vkv.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zju.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tst.hywenlv.cn

TS:   if (s === "") {}
来源：http://wav.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://bzs.yuxming.cn

Go:   if s == "" {}
来源：http://veh.jianghu66.top

Ruby: if s.empty?
来源：http://zdv.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xmr.hesvh.cn

[E21] 超长截断加省略号
来源：http://zov.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgv.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bjx.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqr.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://upq.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hrt.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://vfr.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fbc.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jyn.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://jfa.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rbu.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdd.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xly.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://quh.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zdw.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fnr.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://dmq.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jvp.ywan-chungtsiang.top

================================================================================
来源：http://obk.hongshengwenyu.top

F. 文件与目录
来源：http://jxg.jlsjyb.cn

================================================================================
来源：http://cnb.ppjwa.cn

[F01] 读取整个文件
来源：http://wgj.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://afa.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://jih.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zar.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uft.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bjc.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oui.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://gkn.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://bal.iojbl.cn

[F02] 逐行读取文件
来源：http://tac.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://etd.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rwu.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uul.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyk.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmi.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ckp.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fnc.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nsu.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://wmn.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gjg.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xeb.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fla.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hcx.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://whw.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xqe.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://krl.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vqr.cdnleiting.top

[F04] 追加写入文件
来源：http://gid.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rdc.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kdq.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szo.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxw.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tkn.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oin.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eus.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fbf.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://fqo.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zxh.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://wez.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://slh.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://noy.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hlq.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fqu.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://ewn.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://yqb.yueranfly.top

[F06] 删除文件
来源：http://ima.hnqzz.top

Py:   os.remove("a.txt")
来源：http://dfy.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://ohi.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://fab.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://ezi.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rbg.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://nwu.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://hen.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://jkw.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://the.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kbg.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dxc.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://irk.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://die.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vum.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xrf.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bgk.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rac.kuanghao11.cn

[F08] 遍历目录
来源：http://rrx.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zeu.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ico.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://ntz.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://rsa.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kqh.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lxh.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://cig.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://frt.gaohongyu789.top

[F09] 获取文件大小
来源：http://vcl.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://yuc.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://tha.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://mcl.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://elh.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://oee.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hqi.cheryme.top

Ruby: File.size("a.txt")
来源：http://pma.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://eap.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://tmd.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mcb.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qaa.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ykj.guannengcc.top

TS:   path.extname("a.txt")
来源：http://gmg.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gcw.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdo.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zaz.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wbk.meibo888.top

[F11] 复制与移动文件
来源：http://wpd.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mgc.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://doc.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dei.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mgm.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpq.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgx.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rve.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzv.tian-w.cn

[F12] CSV 读写
来源：http://uks.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jef.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qrb.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jit.ppjwa.cn

TS:   // 同上
来源：http://prq.ctjpmb.com


<!-- 参考信息 -->