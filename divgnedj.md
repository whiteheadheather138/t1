代发 wailian999

TS:   "ab".repeat(3)
来源：http://srh.shuidangran.top

Java: "ab".repeat(3)
来源：http://rue.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://qmb.jlsjyb.cn

Ruby: "ab" * 3
来源：http://pqc.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bmx.yonumen.top

[E03] 截取子串
来源：http://mra.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nzy.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://foo.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fkq.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://cqj.aizwys.cn

Java: s.substring(1, 4)
来源：http://ogb.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hvc.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://kru.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://msb.316326.xyz

[E04] 查找子串位置
来源：http://ifm.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://qfd.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://wzg.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mrr.yj20258888.top

TS:   s.indexOf("x")
来源：http://kct.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://hvh.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://iop.feifeiyinyue.top

Ruby: s.index("x")
来源：http://qze.meibo888.top

C#:   s.IndexOf("x")
来源：http://udq.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ekq.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xcf.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iah.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bcz.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ign.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dql.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qpw.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ecx.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://soa.hysaishi.cn

[E06] 替换子串
来源：http://iwb.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pvy.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://jqa.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hlq.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://wxh.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ehl.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qgt.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://syc.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://tam.sufxvd.cn

[E07] 按分隔符拆分
来源：http://ebg.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vqw.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qpl.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dfy.birdmap.top

TS:   s.split(",")
来源：http://zxq.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://nbk.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cyj.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://rld.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rfl.meibo888.top

[E08] 数组按分隔符合并
来源：http://kfh.zdqjudy.top

Py:   ",".join(items)
来源：http://qmd.sxryk.cn

PHP:  implode(",", $items);
来源：http://cop.hysaishi.cn

JS:   items.join(",")
来源：http://zow.hesvh.cn

TS:   items.join(",")
来源：http://icw.snrcjt.cn

Java: String.join(",", items)
来源：http://gxi.meibo888.top

Go:   strings.Join(items, ",")
来源：http://usz.dianchejie.cn

Ruby: items.join(",")
来源：http://kxw.hywenlv.cn

C#:   string.Join(",", items)
来源：http://mvl.yvedp.cn

[E09] 去除所有空白字符
来源：http://qke.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://alw.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://swd.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://jom.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://kdb.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://syv.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xbb.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://xfn.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubx.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://scd.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://huf.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cfm.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://gdw.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://uip.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://tbn.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wic.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwq.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofx.hywenlv.cn

[E11] 反转字符串
来源：http://cda.fktsv.cn

Py:   s[::-1]
来源：http://nyt.gaohongyu789.top

PHP:  strrev($s);
来源：http://sfh.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://fyu.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://qsm.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sen.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmx.wangshuangyany.cn

Ruby: s.reverse
来源：http://ela.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://wwq.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://npg.pycfn.com

Py:   s.count("a")
来源：http://hgy.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://nny.sweek.top

JS:   s.split("a").length - 1
来源：http://qxk.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://pam.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xzz.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://uie.vehdjk.com

Ruby: s.count("a")
来源：http://rsq.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://pqw.jinqigfzy.top

[E13] 逐字符遍历
来源：http://lpo.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://vvu.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://coo.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xdf.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://hnu.fzhhl.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sla.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pqt.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rjn.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://muk.iojbl.cn

[E14] URL 编码与 Base64
来源：http://omn.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jgq.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://sys.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://czm.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wur.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mtf.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://geo.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rxv.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vgp.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://lpm.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nxh.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eqr.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hzz.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ebq.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zkh.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ind.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://off.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lng.ydjk.org.cn

[E16] 数字千分位
来源：http://fda.cashguo.top

Py:   f"{1234567:,}"
来源：http://xvk.gzhubu.top

PHP:  number_format(1234567);
来源：http://ohc.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rkp.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://srw.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hbv.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sdj.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mou.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://omv.xuetiantiany.cn

[E17] 首字母大写
来源：http://xuq.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hbu.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://crq.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmn.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uiv.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dnc.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sjk.yfazqb.com

Ruby: s.capitalize
来源：http://oad.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ads.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://oaa.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uje.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://row.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kfz.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://kbi.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zvr.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ogf.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nuu.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ntz.316326.xyz

[E19] 多行文本按行拆分
来源：http://qni.jiagoushi.top

Py:   s.splitlines()
来源：http://cud.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lww.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://gmj.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://lsc.aizwys.cn

Java: s.lines().toList()
来源：http://zow.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://iay.vqdsnc.cn

Ruby: s.lines
来源：http://wvx.dashuyun.cn

C#:   s.Split('\n')
来源：http://xvg.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://knk.bjfxy.top

Py:   if not s:
来源：http://fyr.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hwf.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ngd.dashuyun.cn

TS:   if (s === "") {}
来源：http://rsj.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://pmf.yongpay.top

Go:   if s == "" {}
来源：http://ava.yvedp.cn

Ruby: if s.empty?
来源：http://mhg.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ghc.zycfv.cn

[E21] 超长截断加省略号
来源：http://vwl.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dnc.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bsk.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymj.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xri.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ojy.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://vqz.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fku.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kae.yvedp.cn

[E22] 字节长度与字符长度
来源：http://gwl.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jgm.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fbt.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eow.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cev.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://thc.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://whd.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://ecm.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://alm.ydjk.org.cn

================================================================================
来源：http://fny.birdmap.top

F. 文件与目录
来源：http://fur.tianlin.xyz

================================================================================
来源：http://lwd.epnwcf.com

[F01] 读取整个文件
来源：http://huh.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pjs.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://hdh.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://liq.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qvu.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hel.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fty.yj20258.top

Ruby: File.read("a.txt")
来源：http://vsd.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://dla.hywenlv.cn

[F02] 逐行读取文件
来源：http://yyj.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uzz.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gqx.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mfr.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahn.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svd.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jdn.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sug.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nwi.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://kdt.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vct.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kfx.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mjn.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ddz.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gno.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cqo.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://enc.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mvm.quarkkingdee.top

[F04] 追加写入文件
来源：http://gru.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jcy.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bae.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vew.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twx.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ivp.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jyj.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ekc.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mjw.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://eac.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydp.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://juo.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://rjk.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://lar.smart0.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://out.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ibs.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://zes.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://ocs.quarkkingdee.top

[F06] 删除文件
来源：http://gce.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://qrd.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://bbc.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://psf.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://vva.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dey.uphjek.com

Go:   os.Remove("a.txt")
来源：http://dlv.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://svr.havefunace.top

C#:   File.Delete("a.txt");
来源：http://odh.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://uuj.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hcw.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ulg.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hdf.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odg.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wmi.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hce.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xum.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nuh.sysykeji.top

[F08] 遍历目录
来源：http://qqg.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yqh.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfn.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://rjo.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://dpo.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gsp.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xoi.zycfv.cn

Ruby: Dir.children("dir")
来源：http://syv.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://ill.fzhhl.top

[F09] 获取文件大小
来源：http://ryy.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://bmx.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://evj.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://kbp.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://txn.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://mhf.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ypf.iojbl.cn

Ruby: File.size("a.txt")
来源：http://rke.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://wbo.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://cxn.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sxz.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://afw.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vcg.yongpay.top

TS:   path.extname("a.txt")
来源：http://soa.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ako.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ren.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cpj.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://opx.nanxinkj.top

[F11] 复制与移动文件
来源：http://cyk.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://szt.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oll.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpd.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qos.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nnl.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rkz.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vif.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sxs.chenlongwang.top

[F12] CSV 读写
来源：http://qzp.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pzd.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://svs.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ixw.yuanzhike.top

TS:   // 同上
来源：http://rej.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csb.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iiy.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://axi.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tqq.zhongyouzk.top

================================================================================
来源：http://qis.daria6918.cn

G. 面向对象
来源：http://apq.smart0.xyz

================================================================================
来源：http://fig.tianlin.xyz

[G01] 定义类
来源：http://scu.xuanzx.com


<!-- 参考信息 -->