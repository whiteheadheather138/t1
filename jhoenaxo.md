代发 wailian999

Java: String.join(", ", list)
来源：http://pnd.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://hgm.zhixingplan.top

Ruby: arr.join(", ")
来源：http://brp.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://uvh.xuanzx.com

================================================================================
来源：http://exu.cucudq.cn

E. 字符串处理
来源：http://lgd.shuidangran.top

================================================================================
来源：http://cpv.c1oappe.top

[E01] 拼接字符串
来源：http://fnu.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fbx.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rap.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssr.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://azt.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cwa.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rln.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bbs.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hmf.zdqjudy.top

[E02] 重复字符串
来源：http://dlz.sysykeji.top

Py:   "ab" * 3
来源：http://voj.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://gtz.xinyue.icu

JS:   "ab".repeat(3)
来源：http://tcn.fengsongda.top

TS:   "ab".repeat(3)
来源：http://msb.chenlongwang.top

Java: "ab".repeat(3)
来源：http://vez.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://eiv.smart0.xyz

Ruby: "ab" * 3
来源：http://bwy.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kif.9152youxi.cn

[E03] 截取子串
来源：http://yvn.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ukg.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://olc.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dqr.guannengcc.top

TS:   s.slice(1, 4)
来源：http://nvf.iojbl.cn

Java: s.substring(1, 4)
来源：http://mki.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ioh.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://mgt.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://tve.zhixingplan.top

[E04] 查找子串位置
来源：http://isb.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://sws.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://ajz.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lyo.zdqjudy.top

TS:   s.indexOf("x")
来源：http://qjo.aizwys.cn

Java: s.indexOf("x")
来源：http://ihp.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://ssb.9152youxi.cn

Ruby: s.index("x")
来源：http://jty.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://xpm.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kqq.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bsj.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rmx.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tgg.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lwh.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ugy.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dnd.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mvc.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fck.cucudq.cn

[E06] 替换子串
来源：http://qup.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ugf.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://erh.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioz.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://sly.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gzf.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://luq.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tof.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://tna.xinyue.icu

[E07] 按分隔符拆分
来源：http://ddi.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ydc.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zoh.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lsc.feifeiyinyue.top

TS:   s.split(",")
来源：http://epg.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cfd.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uki.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://tft.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lwu.yj20258.top

[E08] 数组按分隔符合并
来源：http://zpv.cheryme.top

Py:   ",".join(items)
来源：http://plb.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://dgh.xuanzx.com

JS:   items.join(",")
来源：http://xir.yuanzhike.top

TS:   items.join(",")
来源：http://ljh.yvedp.cn

Java: String.join(",", items)
来源：http://xsy.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://fan.uphjek.com

Ruby: items.join(",")
来源：http://aeo.aibaodan.cn

C#:   string.Join(",", items)
来源：http://ann.tanke756.top

[E09] 去除所有空白字符
来源：http://qpb.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ehp.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpi.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://ytd.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://egx.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://aay.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://apd.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://zak.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mvr.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://fbv.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rsw.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lvj.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://nce.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://bvg.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://qac.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wny.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aoh.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://job.gogol.net.cn

[E11] 反转字符串
来源：http://ocf.jiagoushi.top

Py:   s[::-1]
来源：http://fui.snrcjt.cn

PHP:  strrev($s);
来源：http://mxi.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://whc.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://zbe.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lkh.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rhl.tian-w.cn

Ruby: s.reverse
来源：http://elh.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://vat.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://goz.hesvh.cn

Py:   s.count("a")
来源：http://oea.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://gkl.yvedp.cn

JS:   s.split("a").length - 1
来源：http://xva.wangdashe.top

TS:   s.split("a").length - 1
来源：http://acz.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ztw.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://npg.smart0.xyz

Ruby: s.count("a")
来源：http://uaj.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://dde.zycfv.cn

[E13] 逐字符遍历
来源：http://fcq.cashguo.top

Py:   for ch in s: print(ch)
来源：http://jot.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ery.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bcx.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://glw.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sds.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eke.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bsh.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kmc.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://rhu.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gac.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jtn.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qap.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lqx.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dio.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://svh.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xyg.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://isi.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://yxd.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uht.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hbe.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tbi.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cws.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ijc.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lrk.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mcn.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zwy.sweek.top

[E16] 数字千分位
来源：http://odg.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://wza.haohaochexian.top

PHP:  number_format(1234567);
来源：http://cmn.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vpg.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jnl.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zfz.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vbo.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iny.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://ihi.zhoulong.xyz

[E17] 首字母大写
来源：http://ixd.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hed.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xku.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://exp.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uza.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oxi.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rvq.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://zww.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wda.gzhubu.top

[E18] 模板占位符替换
来源：http://ssj.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xrh.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yon.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tgu.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jjd.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ktk.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mdv.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tjg.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gvu.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://dmb.hcnkem.com

Py:   s.splitlines()
来源：http://ivl.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://etq.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://vwj.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://nnu.chenzaomai.com

Java: s.lines().toList()
来源：http://mtc.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://pbb.hfpthk.cn

Ruby: s.lines
来源：http://unx.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://dic.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://adu.tian-w.cn

Py:   if not s:
来源：http://jvi.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mwq.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dla.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://aol.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://fsr.chenzaomai.com

Go:   if s == "" {}
来源：http://deh.fengsongda.top

Ruby: if s.empty?
来源：http://ifz.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxd.andypj.xyz

[E21] 超长截断加省略号
来源：http://ljv.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pmq.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhf.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xzj.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkc.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hhv.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://nxw.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kuw.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bep.52xcode.cn

[E22] 字节长度与字符长度
来源：http://hnk.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xnv.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbk.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyi.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvx.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sms.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hlx.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://rpm.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zap.tarul.cn

================================================================================
来源：http://oeu.yfazqb.com

F. 文件与目录
来源：http://srv.kuanghao11.cn

================================================================================
来源：http://wvd.vqdsnc.cn

[F01] 读取整个文件
来源：http://kwj.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qdq.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://pjq.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qyb.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xun.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ncd.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xsq.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://tpj.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://wfx.smart0.xyz

[F02] 逐行读取文件
来源：http://hgh.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wdi.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dux.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahb.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://axo.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hmu.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kxt.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pui.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ije.tanke756.top

[F03] 写入文件（覆盖）
来源：http://lgh.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bty.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ipz.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tbf.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vcd.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yrf.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://juy.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://zfi.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tqv.hnqzz.top

[F04] 追加写入文件
来源：http://tmm.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nlj.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xdf.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hjd.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrk.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mwm.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rib.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fha.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lks.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://auc.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnj.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://zel.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://tvt.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://ykv.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nhv.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edp.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://hch.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://dwf.quarkkingdee.top

[F06] 删除文件
来源：http://oba.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://zju.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://tjj.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cqa.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://mby.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lvh.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://gir.yonumen.top

Ruby: File.delete("a.txt")
来源：http://bpa.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://nji.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://dwh.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mmz.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://flf.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rfd.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yws.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://czd.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zqt.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xgy.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kxl.zhiwuduotai.top

[F08] 遍历目录
来源：http://col.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oip.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vvq.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://fbr.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://mif.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kfd.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ifh.316326.xyz

Ruby: Dir.children("dir")
来源：http://zid.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://agd.birdmap.top

[F09] 获取文件大小
来源：http://trs.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://oev.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://klg.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://qav.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://sei.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jny.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hyi.bjfxy.top

Ruby: File.size("a.txt")
来源：http://nxt.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://gfv.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://miu.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ovv.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://afy.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qhg.yvedp.cn

TS:   path.extname("a.txt")
来源：http://ptu.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kzf.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtw.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xjl.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zfa.ppjwa.cn

[F11] 复制与移动文件
来源：http://lsc.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://egn.cqqwz.cn


<!-- 参考信息 -->