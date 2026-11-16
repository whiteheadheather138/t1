代发 wailian999

[E06] 替换子串
来源：http://cov.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yfq.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://hqf.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qqq.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://tqh.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tfg.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hbc.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xgh.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://awg.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://lew.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qzd.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mzy.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://jkd.hammf.cn

TS:   s.split(",")
来源：http://qxw.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://fpb.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ugj.cheryme.top

Ruby: s.split(",");  s.split
来源：http://zkl.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kvo.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://ilc.guannengcc.top

Py:   ",".join(items)
来源：http://ibg.cucudq.cn

PHP:  implode(",", $items);
来源：http://uqv.haohaochexian.top

JS:   items.join(",")
来源：http://cim.yuxming.cn

TS:   items.join(",")
来源：http://dak.yangfankeji.com

Java: String.join(",", items)
来源：http://tkv.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://yog.jqgfzy.top

Ruby: items.join(",")
来源：http://jlr.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://ddn.tian-w.cn

[E09] 去除所有空白字符
来源：http://uhx.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vcg.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qrj.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://yil.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://ovz.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://qnt.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://slj.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://kvj.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yha.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://gaz.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xcd.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://syj.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://kfu.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://yju.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://phx.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wku.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvc.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxv.hongshengwenyu.top

[E11] 反转字符串
来源：http://uoo.svipenyu.cn

Py:   s[::-1]
来源：http://jbl.cqqwz.cn

PHP:  strrev($s);
来源：http://zce.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://ttj.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://nkf.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zia.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://pvt.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://nkp.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lej.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://umb.ydjk.org.cn

Py:   s.count("a")
来源：http://jsk.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://dgy.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://mvv.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://dxu.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fzr.tarul.cn

Go:   strings.Count(s, "a")
来源：http://gna.jianghu66.top

Ruby: s.count("a")
来源：http://sby.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://kbi.yonumen.top

[E13] 逐字符遍历
来源：http://ehp.meibo888.top

Py:   for ch in s: print(ch)
来源：http://pqm.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yew.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uss.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://eoo.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://idb.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ejd.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qnb.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jpi.hesvh.cn

[E14] URL 编码与 Base64
来源：http://iju.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwm.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ayf.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rhi.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nen.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dnk.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ukt.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ixq.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tdb.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://snh.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vew.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fok.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ybe.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gse.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qfy.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://erk.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://deu.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kiz.hysaishi.cn

[E16] 数字千分位
来源：http://nqv.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://yhe.aizwys.cn

PHP:  number_format(1234567);
来源：http://cxp.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ybn.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qkg.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://exw.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jks.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vta.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://uay.yj202588.top

[E17] 首字母大写
来源：http://zgj.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zuw.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bml.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://arz.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://leb.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sdn.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rtt.jyoumei.cn

Ruby: s.capitalize
来源：http://lrv.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ynf.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://ukd.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mmc.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qhy.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ixe.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dqg.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijj.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kkj.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydb.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gof.yj202588.top

[E19] 多行文本按行拆分
来源：http://mvo.tianlin.xyz

Py:   s.splitlines()
来源：http://spl.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tul.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://yik.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://efx.tianlin.xyz

Java: s.lines().toList()
来源：http://ngz.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://rkw.yfazqb.com

Ruby: s.lines
来源：http://klb.zdbjq.cn

C#:   s.Split('\n')
来源：http://lhb.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://itm.wangshuangyany.cn

Py:   if not s:
来源：http://lub.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wbc.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://snz.haohaochexian.top

TS:   if (s === "") {}
来源：http://acg.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://mnm.wangdashe.top

Go:   if s == "" {}
来源：http://ock.nanxuanxn.top

Ruby: if s.empty?
来源：http://xoi.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qhq.svipenyu.cn

[E21] 超长截断加省略号
来源：http://uqy.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wpa.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cfe.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqi.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptl.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ggm.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://fiw.jyoumei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fjb.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vox.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://hmx.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wzp.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bly.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://itp.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yfk.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ide.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zja.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://bol.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xda.redwolf501.top

================================================================================
来源：http://vta.hongshengwenyu.top

F. 文件与目录
来源：http://ihc.uphjek.com

================================================================================
来源：http://lhn.aizwys.cn

[F01] 读取整个文件
来源：http://ivw.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lgp.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://swe.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gsr.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mxr.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://yie.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ldu.cashguo.top

Ruby: File.read("a.txt")
来源：http://hll.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://xxv.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://uwo.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blr.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ziu.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vgm.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mtw.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zcy.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://izd.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eol.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ogl.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://vlg.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oug.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tlk.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hgw.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnv.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://buk.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nbt.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://pvz.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://omd.xylfe.cn

[F04] 追加写入文件
来源：http://zfd.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cst.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dlm.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ods.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwz.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iwk.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://roo.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rrx.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omm.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://bpc.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iix.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://tng.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://rar.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://rdw.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nst.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cgh.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://fwh.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://dhd.hywenlv.cn

[F06] 删除文件
来源：http://kxh.hesvh.cn

Py:   os.remove("a.txt")
来源：http://ywd.hesvh.cn

PHP:  unlink("a.txt");
来源：http://prg.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://yex.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://olv.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pvj.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://zps.yonumen.top

Ruby: File.delete("a.txt")
来源：http://yjo.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://qgd.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://egh.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hty.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sbq.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uah.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enw.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xxh.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ggw.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ruq.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rav.uphjek.com

[F08] 遍历目录
来源：http://reb.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://rgb.svipenyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tur.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://euj.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://hnh.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jpz.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hae.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://akr.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://edr.jyoumei.cn

[F09] 获取文件大小
来源：http://wua.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://huv.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://tls.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://vlw.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://mpa.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ucg.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tzb.hcnkem.com

Ruby: File.size("a.txt")
来源：http://mkh.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://okm.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://zrc.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zhg.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rlu.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ygh.havefunace.top

TS:   path.extname("a.txt")
来源：http://bls.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mls.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hre.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bmg.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jxt.mhx1999.top

[F11] 复制与移动文件
来源：http://dlb.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://goe.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qyh.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhs.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nif.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpt.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wue.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nkz.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ytq.cucudq.cn

[F12] CSV 读写
来源：http://gkc.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vxg.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://crt.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://odo.hongshengwenyu.top

TS:   // 同上
来源：http://paj.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qju.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nug.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wvv.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iyl.316326.xyz

================================================================================
来源：http://nyx.uphjek.com

G. 面向对象
来源：http://imp.chenjidiqi.icu

================================================================================
来源：http://rkg.chenzaomai.com

[G01] 定义类
来源：http://vyt.yongpay.top

Py:   class User: pass
来源：http://ntk.jianghu66.top

PHP:  class User {}
来源：http://jhx.meibo888.top

JS:   class User {}
来源：http://zdb.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://kab.jinyuanbaomall.cn

Java: class User {}
来源：http://jsv.52xcode.cn

Go:   type User struct { Name string }
来源：http://rng.hcnkem.com

Ruby: class User; end
来源：http://eik.bbcook.cn

C#:   class User {}
来源：http://gwx.yvedp.cn

[G02] 构造函数
来源：http://tnd.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://lyy.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://oif.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://rjv.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://fwq.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://bag.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://izl.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://jex.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://gbj.epnwcf.com

[G03] 实例属性
来源：http://uis.sweek.top

Py:   self.name = "x"
来源：http://rre.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://iem.zhiwuduotai.top

JS:   this.name = "x";
来源：http://mll.chenlongwang.top

TS:   name: string = "x";
来源：http://jeu.ehwqpu.com

Java: private String name;
来源：http://vte.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nlx.fzhhl.top

Ruby: @name = "x"
来源：http://obu.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://iem.daria6918.cn

[G04] 定义方法
来源：http://gqa.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://wvh.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wjp.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://qnj.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://hxz.yangfankeji.com

Java: String greet() { return name; }
来源：http://mjt.gogol.net.cn


<!-- 参考信息 -->