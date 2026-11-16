代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xph.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://noc.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nfn.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kch.jiagoushi.top

[E02] 重复字符串
来源：http://hef.ehwqpu.com

Py:   "ab" * 3
来源：http://ehs.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://glr.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://had.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://uqv.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://abi.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://tbt.meibo888.top

Ruby: "ab" * 3
来源：http://jco.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enh.shangyingyoupin.top

[E03] 截取子串
来源：http://eyf.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qja.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iyt.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cyl.xylfe.cn

TS:   s.slice(1, 4)
来源：http://iwz.cqqwz.cn

Java: s.substring(1, 4)
来源：http://qku.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cyv.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://hzf.tanke756.top

C#:   s.Substring(1, 3)
来源：http://yvd.hongshengwenyu.top

[E04] 查找子串位置
来源：http://zot.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://jju.wangdashe.top

PHP:  strpos($s, "x");
来源：http://cqj.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzu.cashguo.top

TS:   s.indexOf("x")
来源：http://dov.nwbrower.top

Java: s.indexOf("x")
来源：http://bsi.tarul.cn

Go:   strings.Index(s, "x")
来源：http://rtk.chenlongwang.top

Ruby: s.index("x")
来源：http://cyf.mhx1999.top

C#:   s.IndexOf("x")
来源：http://ehd.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://nuo.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dek.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://npb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oct.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kys.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vnk.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hcp.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rtr.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rys.sysykeji.top

[E06] 替换子串
来源：http://pjb.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nec.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://tgj.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mtb.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://zig.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfh.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cwn.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygh.tarul.cn

C#:   s.Replace("a", "b")
来源：http://axb.ctjpmb.com

[E07] 按分隔符拆分
来源：http://ldb.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zyt.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zsp.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jlg.gzhubu.top

TS:   s.split(",")
来源：http://vhf.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://kac.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydm.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://rod.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kww.cashguo.top

[E08] 数组按分隔符合并
来源：http://sly.bbcook.cn

Py:   ",".join(items)
来源：http://mrd.xziqi.cn

PHP:  implode(",", $items);
来源：http://bqw.tanke756.top

JS:   items.join(",")
来源：http://ihq.nanxinkj.top

TS:   items.join(",")
来源：http://ztq.snrcjt.cn

Java: String.join(",", items)
来源：http://vtk.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://wwh.jinqigfzy.top

Ruby: items.join(",")
来源：http://pwi.ydzc1.top

C#:   string.Join(",", items)
来源：http://dck.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://awy.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uvf.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zxu.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://uho.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://jlo.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://dxi.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rvm.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://xnx.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://znr.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://dms.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cfv.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jzt.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://aob.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://awt.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://wxn.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmt.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lgr.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jeg.52xcode.cn

[E11] 反转字符串
来源：http://dbh.zhoulong.xyz

Py:   s[::-1]
来源：http://cpa.c1oappe.top

PHP:  strrev($s);
来源：http://uwx.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://okv.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://nrw.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://uow.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dmm.nanxuanxn.top

Ruby: s.reverse
来源：http://jrz.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://ijk.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://bfq.tanke756.top

Py:   s.count("a")
来源：http://acf.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://olk.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://twr.fehbvm.com

TS:   s.split("a").length - 1
来源：http://sdp.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mfm.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://ycg.dashuyun.cn

Ruby: s.count("a")
来源：http://hlk.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://trr.fzhhl.top

[E13] 逐字符遍历
来源：http://qab.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://eqi.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lwx.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ebg.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jvn.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kyx.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://szr.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gtg.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zmk.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://lyq.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ywp.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://buz.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lzz.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uvj.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tgk.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xun.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kzp.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://huz.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://zum.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jvl.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mwa.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ykz.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hzk.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kdw.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yuw.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ggs.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://udm.sufxvd.cn

[E16] 数字千分位
来源：http://sxg.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://cnd.ybcxt.top

PHP:  number_format(1234567);
来源：http://brf.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lwp.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rdq.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xpg.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhf.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjy.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://dlp.yj20258888.top

[E17] 首字母大写
来源：http://rko.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mar.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://klf.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqh.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://klk.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fme.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bcx.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://feo.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ilf.xylfe.cn

[E18] 模板占位符替换
来源：http://eik.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ppi.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jnq.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vys.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gkq.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uqs.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wvs.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gfk.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ier.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://xzd.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://ggq.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yfd.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://lpp.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://mku.redwolf501.top

Java: s.lines().toList()
来源：http://jan.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://upj.sysykeji.top

Ruby: s.lines
来源：http://mdq.ctjpmb.com

C#:   s.Split('\n')
来源：http://pmg.xziqi.cn

[E20] 判断字符串是否为空
来源：http://dxk.nwbrower.top

Py:   if not s:
来源：http://lmf.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ujv.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mov.xylfe.cn

TS:   if (s === "") {}
来源：http://rqn.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://uzy.wangshuangyany.cn

Go:   if s == "" {}
来源：http://wrw.feifeiyinyue.top

Ruby: if s.empty?
来源：http://yin.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://see.bjfxy.top

[E21] 超长截断加省略号
来源：http://sba.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cqa.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://opr.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgy.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fpw.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bst.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://klk.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mdp.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gbj.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://rmz.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iva.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://peh.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhq.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpc.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sfj.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ztv.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://chh.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aag.yonumen.top

================================================================================
来源：http://srh.jlsjyb.cn

F. 文件与目录
来源：http://evn.zhoulong.xyz

================================================================================
来源：http://ytc.tian-w.cn

[F01] 读取整个文件
来源：http://nht.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yqp.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://wzd.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ktg.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sxy.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ptu.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rbx.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://ypq.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://ecw.mhx1999.top

[F02] 逐行读取文件
来源：http://psb.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jeb.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vix.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jub.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tpp.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lxp.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://igq.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ivr.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jlr.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://cun.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ebg.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://llt.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jit.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aso.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gyf.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://onx.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://xjg.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tbc.yuanzhike.top

[F04] 追加写入文件
来源：http://szu.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdp.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://plx.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wtc.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmn.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ore.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lnq.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ayr.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://imz.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://kky.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jyw.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://vnl.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://xmq.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://shd.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xnc.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mve.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://zoc.cheryme.top

C#:   File.Exists("a.txt")
来源：http://xgf.hammf.cn

[F06] 删除文件
来源：http://eat.sweek.top

Py:   os.remove("a.txt")
来源：http://gwn.yvedp.cn

PHP:  unlink("a.txt");
来源：http://wkm.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ytq.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sdb.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhc.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://ipl.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://cwh.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://dtj.ybcxt.top

[F07] 创建目录（含多级）
来源：http://zgp.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mrv.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dzi.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xhj.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpo.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zqb.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zrs.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qzv.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sxz.gotoacloud.top

[F08] 遍历目录
来源：http://ntw.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bge.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ksw.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://ext.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://jyh.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xde.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vqg.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://tva.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://vkv.wangdashe.top

[F09] 获取文件大小
来源：http://mdy.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://cet.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://rns.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://nql.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://yxy.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mbb.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://obt.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://xmc.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://hkk.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://ptd.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twm.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmt.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://scu.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://bay.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kdy.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://agb.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zga.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ttz.uphjek.com

[F11] 复制与移动文件
来源：http://jzu.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hky.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://asf.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://biw.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://clv.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oej.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lqu.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jgg.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ypy.ydjk.org.cn

[F12] CSV 读写
来源：http://wax.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://alq.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fud.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://buf.aizwys.cn

TS:   // 同上
来源：http://ete.316326.xyz


<!-- 参考信息 -->