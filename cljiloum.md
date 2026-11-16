代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://uhd.havefunace.top

C#:   s.Substring(1, 3)
来源：http://qiy.yj20258888.top

[E04] 查找子串位置
来源：http://hor.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://tlr.xinyue.icu

PHP:  strpos($s, "x");
来源：http://nkr.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uwl.hcnkem.com

TS:   s.indexOf("x")
来源：http://olq.ehwqpu.com

Java: s.indexOf("x")
来源：http://htv.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://pjl.quarkkingdee.top

Ruby: s.index("x")
来源：http://vng.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://rbn.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vis.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lze.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xqx.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lre.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fyk.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kmo.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mdx.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fvk.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dhl.epnwcf.com

[E06] 替换子串
来源：http://amk.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gby.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://bsy.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lhp.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://rjt.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pot.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kde.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xcd.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://wob.fehbvm.com

[E07] 按分隔符拆分
来源：http://dmv.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yvp.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://umy.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://goj.hongshengwenyu.top

TS:   s.split(",")
来源：http://ooh.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://wwt.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ifc.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://mhu.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://crs.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://mvf.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://lbb.yj20258.top

PHP:  implode(",", $items);
来源：http://bbz.vehdjk.com

JS:   items.join(",")
来源：http://vzd.andypj.xyz

TS:   items.join(",")
来源：http://off.shangyingyoupin.top

Java: String.join(",", items)
来源：http://ctt.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://amj.jyoumei.cn

Ruby: items.join(",")
来源：http://iem.yueranfly.top

C#:   string.Join(",", items)
来源：http://vcg.ehwqpu.com

[E09] 去除所有空白字符
来源：http://cnm.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://scb.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://suj.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://yaz.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://xei.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://msq.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rya.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bxx.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dju.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://kwr.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://man.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://llq.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://jwz.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://zzj.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://iqd.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihw.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nkn.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wry.jinqigfzy.top

[E11] 反转字符串
来源：http://eyk.bjfxy.top

Py:   s[::-1]
来源：http://aao.gaohongyu789.top

PHP:  strrev($s);
来源：http://zds.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://ifh.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://mbw.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://tes.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://okg.yj20258888.top

Ruby: s.reverse
来源：http://flp.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://onu.tian-w.cn

[E12] 统计某字符出现次数
来源：http://kwo.aizwys.cn

Py:   s.count("a")
来源：http://nxp.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://vcd.c1oappe.top

JS:   s.split("a").length - 1
来源：http://xoo.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://tkw.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uad.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://raf.daxiang520.top

Ruby: s.count("a")
来源：http://lzg.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://cqf.zycfv.cn

[E13] 逐字符遍历
来源：http://nue.havefunace.top

Py:   for ch in s: print(ch)
来源：http://qjv.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://utt.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://oae.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ddf.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cou.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://beu.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://itp.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zht.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://kmf.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hpa.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ixn.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ctw.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://evx.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kgp.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nvq.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hac.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rkp.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://dko.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jgd.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ked.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ijr.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jmw.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://htj.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vqb.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jie.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wct.zhengqikj.top

[E16] 数字千分位
来源：http://fyj.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://qen.aibaodan.cn

PHP:  number_format(1234567);
来源：http://vfo.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nes.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gms.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pqm.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qdl.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://esp.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://lkw.mhx1999.top

[E17] 首字母大写
来源：http://glf.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iiy.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xvx.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqk.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewu.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwg.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jrk.yj20258888.top

Ruby: s.capitalize
来源：http://hvx.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bda.9152youxi.cn

[E18] 模板占位符替换
来源：http://aze.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://auo.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://thf.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lsq.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aia.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sxg.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xlk.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vgu.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jww.yj20258.top

[E19] 多行文本按行拆分
来源：http://nlz.daria6918.cn

Py:   s.splitlines()
来源：http://bgd.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bud.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://xiv.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://dqa.sxryk.cn

Java: s.lines().toList()
来源：http://vkm.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://bhm.fzhhl.top

Ruby: s.lines
来源：http://tft.guannengcc.top

C#:   s.Split('\n')
来源：http://xmv.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://tiq.9152youxi.cn

Py:   if not s:
来源：http://myq.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptu.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://szm.ydjk.org.cn

TS:   if (s === "") {}
来源：http://nqr.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://obl.epnwcf.com

Go:   if s == "" {}
来源：http://xzh.yongpay.top

Ruby: if s.empty?
来源：http://pni.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ppa.dianchejie.cn

[E21] 超长截断加省略号
来源：http://pqy.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ytr.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mjp.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hvb.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzw.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymp.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://imr.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vae.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://irj.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://hqd.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pml.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwk.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eiq.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cik.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oev.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://thp.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://ari.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xrq.jqgfzy.top

================================================================================
来源：http://nsp.kuanghao11.cn

F. 文件与目录
来源：http://kcc.zhijiandao.cn

================================================================================
来源：http://udu.quarkkingdee.top

[F01] 读取整个文件
来源：http://tgm.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rrh.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://wuh.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://skr.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oer.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zuz.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://obl.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://lpw.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://awo.xziqi.cn

[F02] 逐行读取文件
来源：http://iez.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zjp.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hsk.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mce.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dbu.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gwv.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lwz.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lbv.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pda.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://mxc.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpl.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nvv.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oim.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://but.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rqu.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yef.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://wzh.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eze.ydjk.org.cn

[F04] 追加写入文件
来源：http://gje.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ims.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fvp.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ryh.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sbz.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wct.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://set.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yxp.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bsn.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://gwx.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cmd.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://jal.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://tal.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://uro.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gfl.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vqk.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://hua.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://axz.ppjwa.cn

[F06] 删除文件
来源：http://oxo.iojbl.cn

Py:   os.remove("a.txt")
来源：http://wuf.mhx1999.top

PHP:  unlink("a.txt");
来源：http://dom.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://nwm.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hjb.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://chx.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://jge.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://tzc.sweek.top

C#:   File.Delete("a.txt");
来源：http://dhu.epnwcf.com

[F07] 创建目录（含多级）
来源：http://qcl.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ecy.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mxp.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dth.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ccz.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xxx.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dgb.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cfd.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kvc.zdbjq.cn

[F08] 遍历目录
来源：http://tnq.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zyg.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ahx.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://qgn.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://ipa.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kgb.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://alu.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://syb.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://zne.hnqzz.top

[F09] 获取文件大小
来源：http://xzg.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://usk.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://tml.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://ykd.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://sjl.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://ezc.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hmp.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://mxp.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://uaf.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://tkb.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rli.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://moe.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ctr.bjfxy.top

TS:   path.extname("a.txt")
来源：http://eqz.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xtq.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hma.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ynl.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://txd.aizwys.cn

[F11] 复制与移动文件
来源：http://clo.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gzh.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ejf.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpo.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://new.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://faz.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://egm.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qbp.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ejz.yuxming.cn

[F12] CSV 读写
来源：http://jqu.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dix.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ami.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vye.yj202588.top

TS:   // 同上
来源：http://rzy.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dli.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sgw.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hkj.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ahu.gotoacloud.top

================================================================================
来源：http://kgk.shuidangran.top

G. 面向对象
来源：http://pul.nwbrower.top

================================================================================
来源：http://xau.sysykeji.top

[G01] 定义类
来源：http://eeo.hammf.cn

Py:   class User: pass
来源：http://imk.yj20258.top

PHP:  class User {}
来源：http://rhs.cdnleiting.top

JS:   class User {}
来源：http://cth.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://gqk.gogol.net.cn

Java: class User {}
来源：http://npb.sweek.top

Go:   type User struct { Name string }
来源：http://xvb.ydjk.org.cn

Ruby: class User; end
来源：http://moi.wangdashe.top

C#:   class User {}
来源：http://cyh.shzxlz.cn

[G02] 构造函数
来源：http://njh.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://yjd.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://woh.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://btp.sjlbkw.cn


<!-- 参考信息 -->