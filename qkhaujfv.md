代发 wailian999

[E02] 重复字符串
来源：http://jvt.yuxming.cn

Py:   "ab" * 3
来源：http://ooe.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://mrw.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://law.cheryme.top

TS:   "ab".repeat(3)
来源：http://uuv.zhixingplan.top

Java: "ab".repeat(3)
来源：http://tbl.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://tao.yuanzhike.top

Ruby: "ab" * 3
来源：http://wwi.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ldc.yj202588.top

[E03] 截取子串
来源：http://ras.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqe.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://paf.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://esn.wangdashe.top

TS:   s.slice(1, 4)
来源：http://psu.snrcjt.cn

Java: s.substring(1, 4)
来源：http://dxe.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://irf.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://spq.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://wpb.hysaishi.cn

[E04] 查找子串位置
来源：http://zqs.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://igt.jianghu66.top

PHP:  strpos($s, "x");
来源：http://ntz.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wus.yvedp.cn

TS:   s.indexOf("x")
来源：http://eww.yanxiufei.cn

Java: s.indexOf("x")
来源：http://kpb.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://lwu.sjlbkw.cn

Ruby: s.index("x")
来源：http://mwa.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://hjo.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ccn.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xkq.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://csl.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yfc.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sif.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mda.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oid.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uzc.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ctm.kuanghao11.cn

[E06] 替换子串
来源：http://ifl.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eja.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://qpp.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fop.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://bsx.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhi.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pce.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cmf.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://zbb.snrcjt.cn

[E07] 按分隔符拆分
来源：http://bua.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://huf.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qya.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gni.nwbrower.top

TS:   s.split(",")
来源：http://lgn.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gtm.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://org.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://vxv.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mrq.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://gbk.jinqigfzy.top

Py:   ",".join(items)
来源：http://jwr.c1oappe.top

PHP:  implode(",", $items);
来源：http://vyz.hnxiangtu.top

JS:   items.join(",")
来源：http://atg.jinqigufen.top

TS:   items.join(",")
来源：http://ovp.hywenlv.cn

Java: String.join(",", items)
来源：http://soj.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://ngd.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://bnd.sxryk.cn

C#:   string.Join(",", items)
来源：http://vka.zhixingplan.top

[E09] 去除所有空白字符
来源：http://wyy.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dss.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vsl.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://csx.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://sha.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://pjn.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hmm.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yax.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vle.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://zis.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zqp.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nnd.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://wbq.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://egs.xuanzx.com

Java: String.format("%03d", 7)
来源：http://axj.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jzy.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xbm.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rhs.ybcxt.top

[E11] 反转字符串
来源：http://uzk.tian-w.cn

Py:   s[::-1]
来源：http://eds.fehbvm.com

PHP:  strrev($s);
来源：http://dbh.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://sdz.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://dge.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://znl.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ydm.xuanzx.com

Ruby: s.reverse
来源：http://vta.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://dlr.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://hft.zdqjudy.top

Py:   s.count("a")
来源：http://ddb.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://pyv.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://cdh.cucudq.cn

TS:   s.split("a").length - 1
来源：http://ftc.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://whw.hammf.cn

Go:   strings.Count(s, "a")
来源：http://lsg.yfazqb.com

Ruby: s.count("a")
来源：http://uzj.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://sbx.hnxiangtu.top

[E13] 逐字符遍历
来源：http://knl.havefunace.top

Py:   for ch in s: print(ch)
来源：http://lvn.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bkj.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jyj.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zlz.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://squ.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://asz.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cvb.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ywg.yvedp.cn

[E14] URL 编码与 Base64
来源：http://ejd.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ior.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jeh.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xaf.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ncd.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rie.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gxy.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ekf.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zgx.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://pxp.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bvv.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xou.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sav.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://aps.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://icg.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ops.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewn.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hct.hesvh.cn

[E16] 数字千分位
来源：http://ihf.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://dxv.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://bql.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cwg.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ewp.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hdn.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fcy.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jmd.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://grz.cheryme.top

[E17] 首字母大写
来源：http://hcw.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zfm.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ouh.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eak.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tro.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nmc.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hsg.hywenlv.cn

Ruby: s.capitalize
来源：http://umk.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qfe.yj20258888.top

[E18] 模板占位符替换
来源：http://zwz.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kml.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gqc.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://frh.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oac.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yml.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvo.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rxe.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://thn.yj20258.top

[E19] 多行文本按行拆分
来源：http://bzg.chenlongwang.top

Py:   s.splitlines()
来源：http://rir.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ovk.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://wxf.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://dfq.nanxuanxn.top

Java: s.lines().toList()
来源：http://szi.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://nea.nanxinkj.top

Ruby: s.lines
来源：http://fji.yanxiufei.cn

C#:   s.Split('\n')
来源：http://scj.hesvh.cn

[E20] 判断字符串是否为空
来源：http://wrs.hysaishi.cn

Py:   if not s:
来源：http://gxg.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvp.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ghe.fktsv.cn

TS:   if (s === "") {}
来源：http://lch.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://kfl.guowangkeji.top

Go:   if s == "" {}
来源：http://rbi.ivvv.top

Ruby: if s.empty?
来源：http://xrx.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ats.tarul.cn

[E21] 超长截断加省略号
来源：http://njx.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qgf.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://skp.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kxt.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://imh.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wca.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://pqm.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ket.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kbg.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://ukz.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uuw.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evn.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://afy.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnz.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sgl.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ymp.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://fjl.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bwc.cqqwz.cn

================================================================================
来源：http://rli.shuidangran.top

F. 文件与目录
来源：http://uqs.jqgfzy.top

================================================================================
来源：http://ksv.chenzaomai.com

[F01] 读取整个文件
来源：http://ouy.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aly.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://cbc.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cqp.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hzs.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oxy.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://laz.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://uwx.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://dnf.bjfxy.top

[F02] 逐行读取文件
来源：http://zec.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zmh.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zjh.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apx.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llx.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqt.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bmb.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://okc.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cxf.hammf.cn

[F03] 写入文件（覆盖）
来源：http://pru.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ega.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://abc.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mjn.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnf.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ygv.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cjb.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://wzx.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pau.ctjpmb.com

[F04] 追加写入文件
来源：http://ash.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdb.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kag.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gdl.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyt.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eic.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ldy.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yds.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eof.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://wuc.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vgi.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://fek.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://osp.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://vzm.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wyc.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cpp.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://ldt.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://snf.fktsv.cn

[F06] 删除文件
来源：http://vza.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://dfb.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://vmj.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ygd.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dgt.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fpn.havefunace.top

Go:   os.Remove("a.txt")
来源：http://xaw.havefunace.top

Ruby: File.delete("a.txt")
来源：http://dgc.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://asy.cashguo.top

[F07] 创建目录（含多级）
来源：http://joh.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qxj.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lar.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jvp.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dnu.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://akz.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dkr.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sqb.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kpz.fanxiaobao.xyz

[F08] 遍历目录
来源：http://scp.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://dqo.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://umv.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://bgw.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://tnf.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vlu.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://omq.ydzc1.top

Ruby: Dir.children("dir")
来源：http://edl.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://wnz.gotoacloud.top

[F09] 获取文件大小
来源：http://sjs.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://aux.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://alw.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://cgo.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://scc.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://mpl.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nnq.c1oappe.top

Ruby: File.size("a.txt")
来源：http://dej.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://skg.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://fdd.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lje.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wkc.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://odo.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://nsi.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cvb.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gtv.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iua.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dpr.guowangkeji.top

[F11] 复制与移动文件
来源：http://scv.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://chs.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xdl.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzn.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgb.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eey.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxx.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bwz.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mbt.xuanzx.com

[F12] CSV 读写
来源：http://dme.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nly.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cud.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dcg.yvedp.cn

TS:   // 同上
来源：http://gev.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jko.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qle.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uzw.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gbh.zycfv.cn


<!-- 参考信息 -->