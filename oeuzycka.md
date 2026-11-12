代发 wailian999

[E02] 重复字符串
来源：http://zyp.chenzaomai.com

Py:   "ab" * 3
来源：http://fgb.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://vjt.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://kke.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://vys.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://nqs.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://wdm.guannengcc.top

Ruby: "ab" * 3
来源：http://nrb.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://thk.quarkkingdee.top

[E03] 截取子串
来源：http://jbs.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cfr.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fmb.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nwq.tanke756.top

TS:   s.slice(1, 4)
来源：http://usv.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://bjg.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://noj.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://jna.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://aiq.cashguo.top

[E04] 查找子串位置
来源：http://foe.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://fde.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://fpa.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ysl.zhengqikj.top

TS:   s.indexOf("x")
来源：http://irv.sjlbkw.cn

Java: s.indexOf("x")
来源：http://epv.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://gtx.yuanzhike.top

Ruby: s.index("x")
来源：http://giv.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://zbc.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqb.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cde.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jre.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pvb.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xzb.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bvt.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pdf.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gkf.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://npz.zhengqikj.top

[E06] 替换子串
来源：http://xad.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jbp.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://unb.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwg.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://gfb.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://srn.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cud.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ptb.birdmap.top

C#:   s.Replace("a", "b")
来源：http://any.ybcxt.top

[E07] 按分隔符拆分
来源：http://srr.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hom.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wim.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vwr.yj202588.top

TS:   s.split(",")
来源：http://hxs.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://imn.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bub.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://zii.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chp.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://ttu.vqdsnc.cn

Py:   ",".join(items)
来源：http://gpl.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://meq.pycfn.com

JS:   items.join(",")
来源：http://aup.fktsv.cn

TS:   items.join(",")
来源：http://txi.316326.xyz

Java: String.join(",", items)
来源：http://ndc.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://gkg.pycfn.com

Ruby: items.join(",")
来源：http://ire.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://dpm.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://lzd.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bsi.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mhv.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://xnu.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://foa.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://oku.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rtq.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://egu.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://skp.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://nzs.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://krn.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://onb.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://hpl.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://plr.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://tcc.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zdr.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mgw.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://edt.hfpthk.cn

[E11] 反转字符串
来源：http://xzr.yanxiufei.cn

Py:   s[::-1]
来源：http://mmf.hesvh.cn

PHP:  strrev($s);
来源：http://bmg.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://evs.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://uwa.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wkv.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://goj.shanyushiyangtech.top

Ruby: s.reverse
来源：http://eyj.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://pbm.xuanzx.com

[E12] 统计某字符出现次数
来源：http://bce.fengsongda.top

Py:   s.count("a")
来源：http://qfz.tarul.cn

PHP:  substr_count($s, "a");
来源：http://opn.daria6918.cn

JS:   s.split("a").length - 1
来源：http://iry.tian-w.cn

TS:   s.split("a").length - 1
来源：http://gtm.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zyf.uphjek.com

Go:   strings.Count(s, "a")
来源：http://mbs.tian-w.cn

Ruby: s.count("a")
来源：http://xqd.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://orn.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://nbz.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://dcr.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eto.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vje.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nxe.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kkt.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://six.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rwi.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zdr.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://irr.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://amm.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iih.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hao.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wxc.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qui.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bvk.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lyx.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pgh.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://xzn.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rgs.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fyj.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yuh.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gty.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nru.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oob.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://anm.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ixy.fehbvm.com

[E16] 数字千分位
来源：http://mhf.ydzc1.top

Py:   f"{1234567:,}"
来源：http://mbw.haohaochexian.top

PHP:  number_format(1234567);
来源：http://srj.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://dtm.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rhn.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqu.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cri.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://puh.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://oib.quarkkingdee.top

[E17] 首字母大写
来源：http://ezu.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tdo.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsp.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fvk.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yxn.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qwx.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vdv.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://wct.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qxg.gzhubu.top

[E18] 模板占位符替换
来源：http://zsl.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wxh.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bcn.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jng.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://drq.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tdq.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ylb.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jgv.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jcw.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://koi.xinyue.icu

Py:   s.splitlines()
来源：http://emo.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wfa.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://zsf.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://pri.tian-w.cn

Java: s.lines().toList()
来源：http://xrc.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://rht.jlsjyb.cn

Ruby: s.lines
来源：http://wnd.jlsjyb.cn

C#:   s.Split('\n')
来源：http://cci.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://yet.hnxiangtu.top

Py:   if not s:
来源：http://jku.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hrs.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fgt.fktsv.cn

TS:   if (s === "") {}
来源：http://aco.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://jxt.zhiwuduotai.top

Go:   if s == "" {}
来源：http://lwt.vqdsnc.cn

Ruby: if s.empty?
来源：http://fbq.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mwd.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://zmq.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amh.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wyq.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tck.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ens.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://djm.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://iym.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pfg.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://shr.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://wly.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ibi.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dvf.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yox.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iln.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cxs.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jly.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ofh.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bvf.9152youxi.cn

================================================================================
来源：http://zon.cucudq.cn

F. 文件与目录
来源：http://iuk.tarul.cn

================================================================================
来源：http://any.cdnleiting.top

[F01] 读取整个文件
来源：http://clr.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://krk.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://bqi.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tvf.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qja.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://trm.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qof.52xcode.cn

Ruby: File.read("a.txt")
来源：http://als.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://avj.yangfankeji.com

[F02] 逐行读取文件
来源：http://tzw.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xzt.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jab.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxn.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgj.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axx.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://osk.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mri.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vgz.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://udn.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxw.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yxj.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cwa.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gew.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pmi.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://auc.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://zyh.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://adx.iojbl.cn

[F04] 追加写入文件
来源：http://bpf.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lpx.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lzo.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nyd.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://faq.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jwy.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://apd.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rpy.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://skb.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://nbo.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nbw.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://hbu.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://crj.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://oow.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://biv.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zmy.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://pwx.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://gvj.snrcjt.cn

[F06] 删除文件
来源：http://hjg.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://sgw.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://ddz.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://jam.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://cdz.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xci.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://wvr.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://nft.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://unf.wangdashe.top

[F07] 创建目录（含多级）
来源：http://owt.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mqo.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pko.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvp.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://foy.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oni.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ogg.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zcj.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tdz.ctjpmb.com

[F08] 遍历目录
来源：http://qsu.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://niz.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://moo.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://rgr.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://lek.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dqp.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://emt.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://wsf.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://ldw.nanxinkj.top

[F09] 获取文件大小
来源：http://awv.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://rwv.hesvh.cn

PHP:  filesize("a.txt");
来源：http://kkp.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://bdd.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://dpj.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://tzj.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vvv.tarul.cn

Ruby: File.size("a.txt")
来源：http://vgj.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://mob.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://bjs.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://erm.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fzq.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rob.epnwcf.com

TS:   path.extname("a.txt")
来源：http://mjj.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vre.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://izv.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npa.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://foo.gotoacloud.top

[F11] 复制与移动文件
来源：http://mkr.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://enj.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lwz.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewd.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqt.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://utf.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqx.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://czy.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pot.52xcode.cn

[F12] CSV 读写
来源：http://ocj.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tpc.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://shl.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hsb.nanxuanxn.top

TS:   // 同上
来源：http://kyc.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lnc.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugc.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jfh.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zio.shuidangran.top


<!-- 参考信息 -->