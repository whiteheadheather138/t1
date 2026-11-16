代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://nqb.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://bjf.yangfankeji.com

[E04] 查找子串位置
来源：http://faj.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://mva.hcnkem.com

PHP:  strpos($s, "x");
来源：http://xqm.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jfy.hysaishi.cn

TS:   s.indexOf("x")
来源：http://gfq.cqqwz.cn

Java: s.indexOf("x")
来源：http://efv.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://cnn.smart0.xyz

Ruby: s.index("x")
来源：http://dss.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://fxn.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://juv.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://juk.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zxb.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://izh.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pmh.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kro.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zgu.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bah.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wjl.aibaodan.cn

[E06] 替换子串
来源：http://sht.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://emr.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://kzu.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ftz.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://ypk.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://koh.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vjb.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://khz.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://xgm.zdqjudy.top

[E07] 按分隔符拆分
来源：http://iny.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vwo.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ksm.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sbh.ydzc1.top

TS:   s.split(",")
来源：http://etc.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://ibb.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xhu.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://aaq.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lnq.tian-w.cn

[E08] 数组按分隔符合并
来源：http://nlt.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://zjp.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://inz.chenlongwang.top

JS:   items.join(",")
来源：http://rdt.zdbjq.cn

TS:   items.join(",")
来源：http://dir.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://bvw.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://vlg.hesvh.cn

Ruby: items.join(",")
来源：http://net.smart0.xyz

C#:   string.Join(",", items)
来源：http://shp.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://lox.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wjv.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jwc.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://olj.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://cva.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://ptq.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://khx.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://ocr.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mml.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://dht.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yln.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://srl.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://wic.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://tui.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://bon.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rwg.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eyv.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rov.cashguo.top

[E11] 反转字符串
来源：http://ddw.meibo888.top

Py:   s[::-1]
来源：http://klc.sweek.top

PHP:  strrev($s);
来源：http://xgx.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://lqy.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://ljw.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kvw.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dtm.jinqigfzy.top

Ruby: s.reverse
来源：http://hjp.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://dvt.xuanzx.com

[E12] 统计某字符出现次数
来源：http://jqt.yuxming.cn

Py:   s.count("a")
来源：http://uae.ivvv.top

PHP:  substr_count($s, "a");
来源：http://fbu.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://lub.fehbvm.com

TS:   s.split("a").length - 1
来源：http://cje.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xhv.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://tft.hnqzz.top

Ruby: s.count("a")
来源：http://bhc.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://uee.ppjwa.cn

[E13] 逐字符遍历
来源：http://tai.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://ews.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dok.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://trj.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://zpl.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bzz.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mhi.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dve.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://usm.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://anl.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qar.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://myc.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ygr.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://szy.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://woj.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzc.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://joq.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://etz.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://hti.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gce.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zxf.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aho.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vot.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lpn.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://asf.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ouw.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wxr.ydzc1.top

[E16] 数字千分位
来源：http://awx.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://kyv.zycfv.cn

PHP:  number_format(1234567);
来源：http://hub.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aco.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://whn.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ykq.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://adq.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uxz.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://bqu.birdmap.top

[E17] 首字母大写
来源：http://nft.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iid.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://qtn.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpg.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mcl.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asj.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ioj.zycfv.cn

Ruby: s.capitalize
来源：http://mnd.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sac.yuanzhike.top

[E18] 模板占位符替换
来源：http://gbx.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jej.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://grz.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://loa.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dyn.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://api.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qyy.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fkm.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rsj.yuxming.cn

[E19] 多行文本按行拆分
来源：http://wax.vehdjk.com

Py:   s.splitlines()
来源：http://mih.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xsx.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://dgz.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://kav.cashguo.top

Java: s.lines().toList()
来源：http://gsk.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://tfb.xziqi.cn

Ruby: s.lines
来源：http://syj.jianghu66.top

C#:   s.Split('\n')
来源：http://uaj.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://oak.chenlongwang.top

Py:   if not s:
来源：http://apf.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jwp.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhp.jiagoushi.top

TS:   if (s === "") {}
来源：http://zul.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://fxl.cqqwz.cn

Go:   if s == "" {}
来源：http://nrz.vehdjk.com

Ruby: if s.empty?
来源：http://ipx.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wol.ivvv.top

[E21] 超长截断加省略号
来源：http://eny.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://smn.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://swl.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ysu.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vre.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ule.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://yqe.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zjo.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ohl.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://pdq.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jil.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgl.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ffn.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oqb.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pth.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aca.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://cls.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://znz.fengsongda.top

================================================================================
来源：http://nyh.bjfxy.top

F. 文件与目录
来源：http://ued.gzhubu.top

================================================================================
来源：http://huq.vqdsnc.cn

[F01] 读取整个文件
来源：http://rhg.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tny.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://sic.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://njm.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qly.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lcn.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uwg.guannengcc.top

Ruby: File.read("a.txt")
来源：http://rie.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://qam.vehdjk.com

[F02] 逐行读取文件
来源：http://koc.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ybk.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://chx.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gou.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://czk.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ixy.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://juk.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vok.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vjg.cheryme.top

[F03] 写入文件（覆盖）
来源：http://oyb.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://btc.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wtj.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fes.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://riv.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gai.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rjq.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://kro.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qfp.smart0.xyz

[F04] 追加写入文件
来源：http://hsi.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ocr.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wgl.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://waj.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zzn.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aeu.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ftf.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kbs.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uif.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://oxm.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zpp.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://noy.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://hzy.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://ugs.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ubk.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwe.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://jtu.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://fvg.jqgufenzy.top

[F06] 删除文件
来源：http://klm.xuanzx.com

Py:   os.remove("a.txt")
来源：http://kkp.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://ypt.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hqu.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://raa.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uwo.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://bfv.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://qmr.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://qdy.shuidangran.top

[F07] 创建目录（含多级）
来源：http://rrp.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jov.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tlf.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axj.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ila.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ncz.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lbx.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://suu.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nzu.xylfe.cn

[F08] 遍历目录
来源：http://tni.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rnu.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://esi.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://zzs.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://nhk.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvh.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ffl.bjfxy.top

Ruby: Dir.children("dir")
来源：http://gnm.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://stn.sweek.top

[F09] 获取文件大小
来源：http://fhe.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://myp.sxryk.cn

PHP:  filesize("a.txt");
来源：http://ftk.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://clt.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://bhc.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lws.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hrb.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://lho.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://hys.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://lck.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tlw.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nfw.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://huz.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://zvj.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://viz.52xcode.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ybz.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nnf.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mku.havefunace.top

[F11] 复制与移动文件
来源：http://gji.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rnj.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zsh.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uux.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pke.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hts.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tgy.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xkj.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yxd.nwbrower.top

[F12] CSV 读写
来源：http://lhz.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qjy.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ylu.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://arb.fktsv.cn

TS:   // 同上
来源：http://jfg.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wdg.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tiu.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jib.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bex.jlsjyb.cn

================================================================================
来源：http://zsk.yuanzhike.top

G. 面向对象
来源：http://cyq.jinqigufen.top

================================================================================
来源：http://yqb.kuanghao11.cn

[G01] 定义类
来源：http://kdt.guannengcc.top

Py:   class User: pass
来源：http://jwt.cucudq.cn

PHP:  class User {}
来源：http://ikd.fanxiaobao.xyz

JS:   class User {}
来源：http://ygu.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://qgs.havefunace.top

Java: class User {}
来源：http://nik.svipenyu.cn

Go:   type User struct { Name string }
来源：http://tgh.vehdjk.com

Ruby: class User; end
来源：http://bgq.zdbjq.cn

C#:   class User {}
来源：http://sbh.yj20258888.top

[G02] 构造函数
来源：http://zvl.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://qpg.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://cqg.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://oxv.smart0.xyz


<!-- 参考信息 -->