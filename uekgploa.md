代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bzl.xinyue.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://khc.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://piz.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://con.uphjek.com

[E02] 重复字符串
来源：http://vvp.jinqigfzy.top

Py:   "ab" * 3
来源：http://jwi.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://hoi.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://qaf.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://kot.ybcxt.top

Java: "ab".repeat(3)
来源：http://qfo.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://jbu.ydjk.org.cn

Ruby: "ab" * 3
来源：http://xpx.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wtf.ybcxt.top

[E03] 截取子串
来源：http://hkc.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lln.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wdj.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fqj.hammf.cn

TS:   s.slice(1, 4)
来源：http://mea.yongpay.top

Java: s.substring(1, 4)
来源：http://wcg.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://luo.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xhp.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://lyg.iojbl.cn

[E04] 查找子串位置
来源：http://asc.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://evq.hcnkem.com

PHP:  strpos($s, "x");
来源：http://yul.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pmg.fengsongda.top

TS:   s.indexOf("x")
来源：http://uep.sweek.top

Java: s.indexOf("x")
来源：http://ivn.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://mgf.zhijiandao.cn

Ruby: s.index("x")
来源：http://ccj.zycfv.cn

C#:   s.IndexOf("x")
来源：http://xvn.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cqr.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jaf.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lfg.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ied.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgh.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fxr.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lzv.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ojw.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ieg.feifeiyinyue.top

[E06] 替换子串
来源：http://iwi.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swo.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://rgy.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bac.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://qqu.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gmc.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lif.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://puz.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://aka.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://nxs.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://igd.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xon.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://onr.yanxiufei.cn

TS:   s.split(",")
来源：http://znd.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://taz.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uzf.yonumen.top

Ruby: s.split(",");  s.split
来源：http://nix.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yck.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://qfk.zhixingplan.top

Py:   ",".join(items)
来源：http://nbv.nwbrower.top

PHP:  implode(",", $items);
来源：http://yke.aizwys.cn

JS:   items.join(",")
来源：http://quv.sjlbkw.cn

TS:   items.join(",")
来源：http://kkr.pengpengdd.cyou

Java: String.join(",", items)
来源：http://tcx.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://kuj.c1oappe.top

Ruby: items.join(",")
来源：http://aat.yonumen.top

C#:   string.Join(",", items)
来源：http://skv.cashguo.top

[E09] 去除所有空白字符
来源：http://qmk.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ewh.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://haj.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://nhg.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://tzn.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://rwz.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdv.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kcy.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nfg.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://wed.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lqq.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jcs.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://rkr.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://szo.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://vvg.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jzz.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ncm.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxx.yuanzhike.top

[E11] 反转字符串
来源：http://cge.smart0.xyz

Py:   s[::-1]
来源：http://zxw.52xcode.cn

PHP:  strrev($s);
来源：http://pzi.cheryme.top

JS:   [...s].reverse().join("")
来源：http://okh.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://khi.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nao.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ftk.feifeiyinyue.top

Ruby: s.reverse
来源：http://jak.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://tmi.meibo888.top

[E12] 统计某字符出现次数
来源：http://vjv.hnqzz.top

Py:   s.count("a")
来源：http://hih.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://teu.bjfxy.top

JS:   s.split("a").length - 1
来源：http://rql.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://vtw.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zba.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://cqt.xinyue.icu

Ruby: s.count("a")
来源：http://yte.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://eha.dianchejie.cn

[E13] 逐字符遍历
来源：http://bah.ivvv.top

Py:   for ch in s: print(ch)
来源：http://bbf.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ecl.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zdp.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zhk.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://avc.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ofp.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://djk.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqo.vehdjk.com

[E14] URL 编码与 Base64
来源：http://ttk.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://myy.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yzf.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kjd.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mvc.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sbz.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://umi.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kon.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jko.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://fth.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://khf.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xxl.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tgu.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://wpy.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://knt.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eyj.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tyt.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qhl.zhoulong.xyz

[E16] 数字千分位
来源：http://ukl.ybcxt.top

Py:   f"{1234567:,}"
来源：http://xdd.jinqigufen.top

PHP:  number_format(1234567);
来源：http://vwd.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mpf.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://twr.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kkk.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vse.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hrv.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://rlj.yongpay.top

[E17] 首字母大写
来源：http://bnh.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rgu.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rht.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spj.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcq.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oyq.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ztq.ctjpmb.com

Ruby: s.capitalize
来源：http://trg.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ive.jyoumei.cn

[E18] 模板占位符替换
来源：http://qxn.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bwt.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ppt.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mjm.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://kfl.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://psv.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tge.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zzy.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tdh.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://fxq.yuanzhike.top

Py:   s.splitlines()
来源：http://nxd.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rlo.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://sug.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://ixe.pengpengdd.cyou

Java: s.lines().toList()
来源：http://ezh.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://oeo.52xcode.cn

Ruby: s.lines
来源：http://scq.mhx1999.top

C#:   s.Split('\n')
来源：http://nfh.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://icc.nanxinkj.top

Py:   if not s:
来源：http://wlu.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsd.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tkc.shuidangran.top

TS:   if (s === "") {}
来源：http://mub.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://qbb.hysaishi.cn

Go:   if s == "" {}
来源：http://rjx.kuanghao11.cn

Ruby: if s.empty?
来源：http://ynb.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cvs.tianlin.xyz

[E21] 超长截断加省略号
来源：http://eco.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aav.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nrt.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ves.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jop.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fzu.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://xil.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pys.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xbw.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://jxc.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iol.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nud.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://afe.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://biv.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mbb.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uxx.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://hfi.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jpx.ydzc1.top

================================================================================
来源：http://lkd.mhx1999.top

F. 文件与目录
来源：http://uam.smart0.xyz

================================================================================
来源：http://oqp.ehwqpu.com

[F01] 读取整个文件
来源：http://npr.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ipe.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://rzx.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cws.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsf.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dzq.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://knx.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://quj.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://ydn.yueranfly.top

[F02] 逐行读取文件
来源：http://izg.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pmr.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xzf.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jjp.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jed.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hrc.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cam.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ujs.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ozr.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://zir.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kwl.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vph.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://stf.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vme.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://foe.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ndq.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://elq.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cpw.tanke756.top

[F04] 追加写入文件
来源：http://itt.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nqw.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://orc.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izv.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mhp.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qcp.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ngu.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vtk.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dgl.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://vig.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rue.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://zcy.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://szg.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://feq.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://key.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fca.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://rqr.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://pqr.gogol.net.cn

[F06] 删除文件
来源：http://hod.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://mtm.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://tdf.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://fwe.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://pmt.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lmd.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://abi.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://lbb.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://lfw.sxryk.cn

[F07] 创建目录（含多级）
来源：http://skg.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iio.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ccm.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohz.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ybx.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://toq.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xul.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vjq.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ezd.jianghu66.top

[F08] 遍历目录
来源：http://poc.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jpf.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pck.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://ein.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://dub.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dqv.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rcm.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://haa.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://gak.yj202588.top

[F09] 获取文件大小
来源：http://vqj.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://ori.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://ayk.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://bcv.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://iiv.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ree.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eua.yongpay.top

Ruby: File.size("a.txt")
来源：http://lii.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://jko.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://bsm.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gmo.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://opp.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dby.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://hmx.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bqt.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lip.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vpg.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sbf.yanxiufei.cn

[F11] 复制与移动文件
来源：http://uqd.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sbm.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dzz.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sar.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgv.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://onh.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iaj.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://llz.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pdt.52xcode.cn

[F12] CSV 读写
来源：http://yfc.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vrx.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qmz.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gvk.zhengqikj.top

TS:   // 同上
来源：http://riy.dianchejie.cn


<!-- 参考信息 -->