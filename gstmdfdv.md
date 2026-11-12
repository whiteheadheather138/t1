代发 wailian999

TS:   "ab".repeat(3)
来源：http://qvv.hammf.cn

Java: "ab".repeat(3)
来源：http://icy.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dom.cdnleiting.top

Ruby: "ab" * 3
来源：http://bgp.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lxi.vehdjk.com

[E03] 截取子串
来源：http://oar.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xnk.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://llb.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ulz.guannengcc.top

TS:   s.slice(1, 4)
来源：http://puo.vehdjk.com

Java: s.substring(1, 4)
来源：http://hxq.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iup.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://evs.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://ywq.fehbvm.com

[E04] 查找子串位置
来源：http://xik.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://ccc.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://ahj.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://miq.hnqzz.top

TS:   s.indexOf("x")
来源：http://qqm.jiagoushi.top

Java: s.indexOf("x")
来源：http://ouq.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://aah.ehwqpu.com

Ruby: s.index("x")
来源：http://jlm.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://zit.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://grx.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gdp.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vko.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdh.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wqu.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://svy.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eyh.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ltx.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://spy.fktsv.cn

[E06] 替换子串
来源：http://uho.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kmz.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://cww.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgh.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://nfy.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ycg.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qvq.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vwz.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://qjf.sxryk.cn

[E07] 按分隔符拆分
来源：http://bcv.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wjm.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pjp.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://nyw.snrcjt.cn

TS:   s.split(",")
来源：http://jvx.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://asu.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vqr.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://myd.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rak.fktsv.cn

[E08] 数组按分隔符合并
来源：http://ruq.iojbl.cn

Py:   ",".join(items)
来源：http://dng.ivvv.top

PHP:  implode(",", $items);
来源：http://nxc.feifeiyinyue.top

JS:   items.join(",")
来源：http://wzw.zhengqikj.top

TS:   items.join(",")
来源：http://toe.yvedp.cn

Java: String.join(",", items)
来源：http://juy.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://iqe.guannengcc.top

Ruby: items.join(",")
来源：http://puv.sufxvd.cn

C#:   string.Join(",", items)
来源：http://gkm.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://qzo.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fjh.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ddw.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://mea.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://jwv.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://ymm.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vpw.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pfl.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uxd.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://ezo.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wyx.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozk.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://xan.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://sux.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://web.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cdz.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hho.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bqv.chenlongwang.top

[E11] 反转字符串
来源：http://ilr.ctjpmb.com

Py:   s[::-1]
来源：http://axg.yanxiufei.cn

PHP:  strrev($s);
来源：http://wls.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://hco.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://sad.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xpq.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xgh.nanxuanxn.top

Ruby: s.reverse
来源：http://abi.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gry.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://dae.sufxvd.cn

Py:   s.count("a")
来源：http://vhy.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://sru.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://jyw.sxryk.cn

TS:   s.split("a").length - 1
来源：http://gfj.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ljp.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://ygs.xuanzx.com

Ruby: s.count("a")
来源：http://wer.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://mny.haohaochexian.top

[E13] 逐字符遍历
来源：http://hpw.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://tlo.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xxx.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uou.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mea.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vlh.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gkw.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://byf.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wbi.redwolf501.top

[E14] URL 编码与 Base64
来源：http://cwy.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mok.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ygs.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hyi.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://azm.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yjb.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xed.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://acn.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jxo.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://sxf.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://lgz.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ywu.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://krr.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zmz.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kwb.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yev.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pyo.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gws.gogol.net.cn

[E16] 数字千分位
来源：http://isl.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://ikp.zdqjudy.top

PHP:  number_format(1234567);
来源：http://mej.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zjy.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qvd.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qdr.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kts.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pvt.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://dio.epnwcf.com

[E17] 首字母大写
来源：http://naw.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rnz.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gcs.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qpe.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dao.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jnd.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uxl.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://mar.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ncq.wangdashe.top

[E18] 模板占位符替换
来源：http://wik.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hru.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eiv.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mxo.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gzd.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jhx.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fvq.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://msl.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://usz.52xcode.cn

[E19] 多行文本按行拆分
来源：http://kea.ctjpmb.com

Py:   s.splitlines()
来源：http://udq.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iuv.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://vlr.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://tkx.sufxvd.cn

Java: s.lines().toList()
来源：http://dei.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://kjz.jiagoushi.top

Ruby: s.lines
来源：http://icc.yuanzhike.top

C#:   s.Split('\n')
来源：http://bfw.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://rbh.birdmap.top

Py:   if not s:
来源：http://yli.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ywj.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ryc.zycfv.cn

TS:   if (s === "") {}
来源：http://czz.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://tzn.haohaochexian.top

Go:   if s == "" {}
来源：http://fyf.zhiwuduotai.top

Ruby: if s.empty?
来源：http://tnq.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wdd.fehbvm.com

[E21] 超长截断加省略号
来源：http://bdf.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rmz.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lsz.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oau.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rht.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://thk.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://lsv.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vik.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yzb.cashguo.top

[E22] 字节长度与字符长度
来源：http://ogb.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cxk.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://erf.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uyx.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bkd.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gsd.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rfr.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://vcj.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wud.fzhhl.top

================================================================================
来源：http://bdc.yanxiufei.cn

F. 文件与目录
来源：http://oxi.yvedp.cn

================================================================================
来源：http://dxr.jianghu66.top

[F01] 读取整个文件
来源：http://tiq.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wav.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://uym.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iev.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://phd.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jgz.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dec.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://fyh.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://llb.jianghu66.top

[F02] 逐行读取文件
来源：http://skh.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hgk.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dwy.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qzq.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilt.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ihg.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tkm.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hhx.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://auj.birdmap.top

[F03] 写入文件（覆盖）
来源：http://tgi.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://stv.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ubc.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iwo.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tnj.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wkg.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rgo.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://ecl.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xqo.nanxinkj.top

[F04] 追加写入文件
来源：http://bvq.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mcl.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iha.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cwu.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vyv.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tni.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nhx.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vvr.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rby.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://sja.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uqe.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://hun.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://gyh.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://zfg.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wld.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sew.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://ouk.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://loa.jqgufenzy.top

[F06] 删除文件
来源：http://qzo.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://exq.316326.xyz

PHP:  unlink("a.txt");
来源：http://gzm.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://tqu.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://llk.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qgr.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://srp.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://fgm.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://xfl.bjfxy.top

[F07] 创建目录（含多级）
来源：http://ekj.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oup.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uxq.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qxe.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhx.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jka.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ini.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zgg.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hnq.yongpay.top

[F08] 遍历目录
来源：http://hyi.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://hpu.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://stz.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://ncn.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://xak.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iev.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gjr.52xcode.cn

Ruby: Dir.children("dir")
来源：http://cbt.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://ymp.jqgufenzy.top

[F09] 获取文件大小
来源：http://ezo.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://wmr.sysykeji.top

PHP:  filesize("a.txt");
来源：http://vlu.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://ell.yonumen.top

TS:   fs.statSync("a.txt").size
来源：http://kwz.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bod.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eaq.cheryme.top

Ruby: File.size("a.txt")
来源：http://mck.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://txj.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://umw.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzy.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqy.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ewq.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://hsg.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wgj.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aph.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dsm.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mow.chenzaomai.com

[F11] 复制与移动文件
来源：http://afy.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hrb.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://glt.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zjp.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://plg.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xgp.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://psm.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tma.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jtm.sufxvd.cn

[F12] CSV 读写
来源：http://kuh.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://poc.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://svl.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ylv.aibaodan.cn

TS:   // 同上
来源：http://qbq.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lvj.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ezd.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://led.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xpz.chenjidiqi.icu

================================================================================
来源：http://irw.chenlongwang.top

G. 面向对象
来源：http://hdt.sjlbkw.cn

================================================================================
来源：http://uks.gzhubu.top

[G01] 定义类
来源：http://jok.ywan-chungtsiang.top


<!-- 参考信息 -->