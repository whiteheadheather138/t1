代发 wailian999

[E02] 重复字符串
来源：http://nkv.zdbjq.cn

Py:   "ab" * 3
来源：http://uys.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://tna.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://qfk.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://nyi.cdnleiting.top

Java: "ab".repeat(3)
来源：http://okj.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://eql.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://ich.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ywc.ivvv.top

[E03] 截取子串
来源：http://faa.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgb.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hvo.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://soc.xziqi.cn

TS:   s.slice(1, 4)
来源：http://brw.gogol.net.cn

Java: s.substring(1, 4)
来源：http://ahd.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyt.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cvi.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://mao.meibo888.top

[E04] 查找子串位置
来源：http://rli.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://wma.hesvh.cn

PHP:  strpos($s, "x");
来源：http://eup.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zxq.tarul.cn

TS:   s.indexOf("x")
来源：http://ukj.smart0.xyz

Java: s.indexOf("x")
来源：http://hwc.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://qpk.havefunace.top

Ruby: s.index("x")
来源：http://iks.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://csr.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kds.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://keh.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ypz.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prp.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ycr.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ogq.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xrs.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubu.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vht.jyoumei.cn

[E06] 替换子串
来源：http://sny.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jtx.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://smf.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hhx.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://cnn.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uco.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://trf.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cau.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://oxc.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://ktv.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vey.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ycv.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oek.9152youxi.cn

TS:   s.split(",")
来源：http://pow.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nen.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vwl.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://rxy.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xhz.redwolf501.top

[E08] 数组按分隔符合并
来源：http://aas.svipenyu.cn

Py:   ",".join(items)
来源：http://dlg.yuanzhike.top

PHP:  implode(",", $items);
来源：http://rhy.sxryk.cn

JS:   items.join(",")
来源：http://ilj.vqdsnc.cn

TS:   items.join(",")
来源：http://nah.yfazqb.com

Java: String.join(",", items)
来源：http://sog.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://kwe.ivvv.top

Ruby: items.join(",")
来源：http://wlf.316326.xyz

C#:   string.Join(",", items)
来源：http://nzx.xuanzx.com

[E09] 去除所有空白字符
来源：http://tli.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rxm.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ouv.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://lhb.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://qev.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ace.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yjc.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fic.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cri.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://fsc.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gmy.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iwr.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://zse.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://sda.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://dum.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ont.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://byn.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hns.zhengqikj.top

[E11] 反转字符串
来源：http://wfv.pycfn.com

Py:   s[::-1]
来源：http://lcp.tarul.cn

PHP:  strrev($s);
来源：http://huu.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://plt.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://ucy.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dzx.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://bze.xylfe.cn

Ruby: s.reverse
来源：http://sys.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dte.yj20258888.top

[E12] 统计某字符出现次数
来源：http://ior.tarul.cn

Py:   s.count("a")
来源：http://ncf.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://tle.daria6918.cn

JS:   s.split("a").length - 1
来源：http://vyz.ivvv.top

TS:   s.split("a").length - 1
来源：http://oom.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bhq.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://lub.yj202588.top

Ruby: s.count("a")
来源：http://tkq.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://htq.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://rhf.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://pio.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xzo.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxp.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cxy.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hct.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yxr.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tfz.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbd.yj20258888.top

[E14] URL 编码与 Base64
来源：http://dve.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qzx.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://few.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aky.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzq.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lcf.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hjp.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bdn.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gaq.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://xpf.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ufy.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://izk.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xkv.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mcq.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://elf.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pjc.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igc.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ksl.yangfankeji.com

[E16] 数字千分位
来源：http://asz.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://twu.cdnleiting.top

PHP:  number_format(1234567);
来源：http://jra.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://xuv.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ebf.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azh.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bpx.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lth.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://tce.jinqigfzy.top

[E17] 首字母大写
来源：http://tnj.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vpq.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgr.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gst.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zyd.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ubl.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kdn.nanxuanxn.top

Ruby: s.capitalize
来源：http://bwa.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wry.snrcjt.cn

[E18] 模板占位符替换
来源：http://ntm.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zxu.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjk.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wlu.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rvo.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pri.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hzj.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jkq.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gur.aizwys.cn

[E19] 多行文本按行拆分
来源：http://vlt.gotoacloud.top

Py:   s.splitlines()
来源：http://qvq.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nfj.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://ksc.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://eif.fengsongda.top

Java: s.lines().toList()
来源：http://cyv.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://kkz.xinyue.icu

Ruby: s.lines
来源：http://yfz.zhijiandao.cn

C#:   s.Split('\n')
来源：http://kyv.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://efh.fengsongda.top

Py:   if not s:
来源：http://uzk.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mkg.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kat.yvedp.cn

TS:   if (s === "") {}
来源：http://sti.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://jiv.fktsv.cn

Go:   if s == "" {}
来源：http://mmo.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://fuo.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uzm.hammf.cn

[E21] 超长截断加省略号
来源：http://foh.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ket.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ehi.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kyg.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qou.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uej.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://pht.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ccd.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://abq.sysykeji.top

[E22] 字节长度与字符长度
来源：http://ytk.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jbv.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ios.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qac.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lps.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ykr.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fid.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://tgy.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xnr.guannengcc.top

================================================================================
来源：http://wkf.tian-w.cn

F. 文件与目录
来源：http://xpj.zhixingplan.top

================================================================================
来源：http://aen.zhixingplan.top

[F01] 读取整个文件
来源：http://ojb.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xnk.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://mvj.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ogy.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iqp.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://grg.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pwy.yonumen.top

Ruby: File.read("a.txt")
来源：http://sir.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://jon.0kj1m.cn

[F02] 逐行读取文件
来源：http://hvk.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jxr.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kti.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nou.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqt.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ksf.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qqk.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fde.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hyo.tanke756.top

[F03] 写入文件（覆盖）
来源：http://vsn.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vgz.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tlk.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jjb.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qql.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kek.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://feu.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://gak.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hox.tarul.cn

[F04] 追加写入文件
来源：http://qkh.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kqs.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uav.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dve.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlb.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ugn.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zbg.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vsr.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jzs.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://abx.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sgi.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://imn.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://aml.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://lfv.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vtq.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ktf.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://ccd.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://diy.wangdashe.top

[F06] 删除文件
来源：http://usb.mhx1999.top

Py:   os.remove("a.txt")
来源：http://xxl.daxiang520.top

PHP:  unlink("a.txt");
来源：http://xya.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://ghi.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://fgn.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://txs.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://ihv.uphjek.com

Ruby: File.delete("a.txt")
来源：http://mvc.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://sxs.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://kek.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://szz.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yyo.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fvo.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wax.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kxp.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yux.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://emv.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://klx.shzxlz.cn

[F08] 遍历目录
来源：http://cfo.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://onf.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://crm.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://bjy.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://khz.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mfq.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ucq.jianghu66.top

Ruby: Dir.children("dir")
来源：http://mte.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://kwg.cashguo.top

[F09] 获取文件大小
来源：http://phh.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://lfs.ybcxt.top

PHP:  filesize("a.txt");
来源：http://gts.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://ipg.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://xcf.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://czf.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jsa.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://vhg.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://enq.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://uaz.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qtq.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pxu.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pqh.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://hrn.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dem.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vlt.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uxx.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qzk.daria6918.cn

[F11] 复制与移动文件
来源：http://zpk.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pbi.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tgf.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cxd.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vqr.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sjm.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fda.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ren.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pao.shanyushiyangtech.top

[F12] CSV 读写
来源：http://xtu.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kai.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wsk.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iny.fanxiaobao.xyz

TS:   // 同上
来源：http://cmc.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eyz.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wxw.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tjj.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vzb.9152youxi.cn


<!-- 参考信息 -->