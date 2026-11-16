代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gbc.yj20258888.top

[E03] 截取子串
来源：http://miy.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dbb.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yho.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hmh.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://rna.iojbl.cn

Java: s.substring(1, 4)
来源：http://ock.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rxd.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://ujc.cheryme.top

C#:   s.Substring(1, 3)
来源：http://ene.pycfn.com

[E04] 查找子串位置
来源：http://aqt.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://xlu.tian-w.cn

PHP:  strpos($s, "x");
来源：http://zyz.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngh.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://ymt.smart0.xyz

Java: s.indexOf("x")
来源：http://vng.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://oat.ehwqpu.com

Ruby: s.index("x")
来源：http://njt.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://opw.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqb.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dqc.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cxs.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lup.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://aal.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kag.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zcn.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gpj.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jik.yuanzhike.top

[E06] 替换子串
来源：http://moi.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sdr.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://kmf.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iey.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://cig.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvt.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sno.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hij.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://ohh.tanke756.top

[E07] 按分隔符拆分
来源：http://raj.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pse.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://esu.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qmz.jqgfzy.top

TS:   s.split(",")
来源：http://pwc.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://qls.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eig.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://dxn.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nwo.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://iyo.guannengcc.top

Py:   ",".join(items)
来源：http://uul.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://dba.xylfe.cn

JS:   items.join(",")
来源：http://cds.mhx1999.top

TS:   items.join(",")
来源：http://ifh.316326.xyz

Java: String.join(",", items)
来源：http://lte.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://gds.xylfe.cn

Ruby: items.join(",")
来源：http://fnp.daria6918.cn

C#:   string.Join(",", items)
来源：http://mxx.hcnkem.com

[E09] 去除所有空白字符
来源：http://wey.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wrv.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uym.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://zcb.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://jhp.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://squ.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://sbd.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://ylj.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uey.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://kcd.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bho.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kby.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://rgk.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://upd.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://gba.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rof.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbj.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gcs.xylfe.cn

[E11] 反转字符串
来源：http://rzu.pengpengdd.cyou

Py:   s[::-1]
来源：http://wdg.xylfe.cn

PHP:  strrev($s);
来源：http://ufh.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://kfi.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://sit.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xjx.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://eym.cashguo.top

Ruby: s.reverse
来源：http://ooi.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rud.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://aig.wangshuangyany.cn

Py:   s.count("a")
来源：http://tpi.ivvv.top

PHP:  substr_count($s, "a");
来源：http://lyo.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://thg.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://wch.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mds.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://zql.hywenlv.cn

Ruby: s.count("a")
来源：http://kcn.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://ubc.haohaochexian.top

[E13] 逐字符遍历
来源：http://ghu.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://nxd.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iat.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ppa.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uto.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xhw.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zal.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://acq.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cxn.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ifw.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ycr.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zuq.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kqz.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xks.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yon.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jee.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://emu.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jgm.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://ups.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zfb.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qkh.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xpg.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hnw.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rxc.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fhc.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rrv.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://peu.bjfxy.top

[E16] 数字千分位
来源：http://pck.yonumen.top

Py:   f"{1234567:,}"
来源：http://lhe.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://ohe.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bqw.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://btn.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pwx.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrv.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cpi.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://nem.bbcook.cn

[E17] 首字母大写
来源：http://kah.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://epg.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qvo.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drg.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dno.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mun.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xqq.pengpengdd.cyou

Ruby: s.capitalize
来源：http://onp.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzi.uphjek.com

[E18] 模板占位符替换
来源：http://qmz.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqw.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umz.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rau.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nav.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybf.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mau.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dnd.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ejp.hesvh.cn

[E19] 多行文本按行拆分
来源：http://leh.zhiwuduotai.top

Py:   s.splitlines()
来源：http://wej.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rdj.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://sdv.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://nak.hnxiangtu.top

Java: s.lines().toList()
来源：http://kiv.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://jdr.yanxiufei.cn

Ruby: s.lines
来源：http://imm.snrcjt.cn

C#:   s.Split('\n')
来源：http://ugj.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://cmg.yonumen.top

Py:   if not s:
来源：http://ikv.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rdu.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mvc.bbcook.cn

TS:   if (s === "") {}
来源：http://oor.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://usb.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://ida.havefunace.top

Ruby: if s.empty?
来源：http://sxl.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pkh.ybcxt.top

[E21] 超长截断加省略号
来源：http://xrs.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://whe.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ubh.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://euk.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlb.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gyw.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://vlg.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xqt.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gdk.nwbrower.top

[E22] 字节长度与字符长度
来源：http://jwi.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dfc.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvy.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzh.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwr.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xot.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgq.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://mve.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pco.52xcode.cn

================================================================================
来源：http://vhi.cucudq.cn

F. 文件与目录
来源：http://tpu.redwolf501.top

================================================================================
来源：http://lsf.jqgufenzy.top

[F01] 读取整个文件
来源：http://kcr.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lpq.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://tnk.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://clj.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nhp.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tts.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eea.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://mci.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://qvg.xuanzx.com

[F02] 逐行读取文件
来源：http://yhv.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bdw.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kna.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spn.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awz.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yhs.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lqa.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wpy.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bgy.316326.xyz

[F03] 写入文件（覆盖）
来源：http://jgo.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mqb.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wic.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kfk.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kgg.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tli.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsy.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://idw.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cdy.zdbjq.cn

[F04] 追加写入文件
来源：http://uku.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://unx.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oat.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nma.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fys.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bjw.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lrf.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gcn.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npo.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://ozm.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kah.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://juv.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://bos.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://qbg.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qok.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vvf.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://dkj.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://qnv.fengsongda.top

[F06] 删除文件
来源：http://mza.hammf.cn

Py:   os.remove("a.txt")
来源：http://chh.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://sqc.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ozz.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://twt.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cuy.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://amq.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://hdr.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://fae.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://clh.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hvb.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqo.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jdp.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://glg.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qvx.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dhq.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gcw.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tci.zdqjudy.top

[F08] 遍历目录
来源：http://xzh.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rls.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rob.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://ylu.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://ljq.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyb.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bwf.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://kyz.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://yqa.cucudq.cn

[F09] 获取文件大小
来源：http://wtm.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://oit.c1oappe.top

PHP:  filesize("a.txt");
来源：http://npv.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://meq.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://ebu.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://hev.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kvj.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://boc.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://mgu.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://upk.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://apd.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qcp.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rzi.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://lnb.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dgf.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zld.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qru.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxn.epnwcf.com

[F11] 复制与移动文件
来源：http://tln.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://djh.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cme.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyp.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wvq.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cms.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rrk.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kph.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lyo.aizwys.cn

[F12] CSV 读写
来源：http://gga.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ulc.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://feh.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pbb.aibaodan.cn

TS:   // 同上
来源：http://nel.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ify.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbb.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aaw.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nxt.shangyingyoupin.top

================================================================================
来源：http://mcm.jianghu66.top

G. 面向对象
来源：http://kvb.zhixingplan.top

================================================================================
来源：http://ahl.ctjpmb.com

[G01] 定义类
来源：http://yma.quarkkingdee.top

Py:   class User: pass
来源：http://gbi.c1oappe.top

PHP:  class User {}
来源：http://kjk.tarul.cn

JS:   class User {}
来源：http://evb.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://kdg.ybcxt.top


<!-- 参考信息 -->