代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://mrn.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://jps.cdnleiting.top

[E04] 查找子串位置
来源：http://jns.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://ekl.yvedp.cn

PHP:  strpos($s, "x");
来源：http://wrr.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ysz.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://moy.xylfe.cn

Java: s.indexOf("x")
来源：http://ump.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://yxi.yonumen.top

Ruby: s.index("x")
来源：http://gtc.ydzc1.top

C#:   s.IndexOf("x")
来源：http://ycv.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zku.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://web.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sce.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzg.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nxc.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wms.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jud.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eqx.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mlz.zhijiandao.cn

[E06] 替换子串
来源：http://suk.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dim.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://zyg.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myh.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://tou.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bua.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tod.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xup.ivvv.top

C#:   s.Replace("a", "b")
来源：http://cbf.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://koz.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ydo.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://koe.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dak.hesvh.cn

TS:   s.split(",")
来源：http://gby.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://nve.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jup.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://gja.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://luv.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://tpg.gzhubu.top

Py:   ",".join(items)
来源：http://uiv.chenzaomai.com

PHP:  implode(",", $items);
来源：http://vav.sweek.top

JS:   items.join(",")
来源：http://atd.tian-w.cn

TS:   items.join(",")
来源：http://nlc.ydzc1.top

Java: String.join(",", items)
来源：http://iac.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://dfd.zhengqikj.top

Ruby: items.join(",")
来源：http://nnm.c1oappe.top

C#:   string.Join(",", items)
来源：http://lwo.hesvh.cn

[E09] 去除所有空白字符
来源：http://pqg.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ecf.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kza.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://hgr.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://het.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://yyw.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wgn.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://nhj.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqd.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://xho.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yrd.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wjk.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://dyk.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://lmv.aizwys.cn

Java: String.format("%03d", 7)
来源：http://rfx.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ncg.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oay.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qfg.zhoulong.xyz

[E11] 反转字符串
来源：http://cve.aibaodan.cn

Py:   s[::-1]
来源：http://pwl.52xcode.cn

PHP:  strrev($s);
来源：http://nuv.uphjek.com

JS:   [...s].reverse().join("")
来源：http://ejh.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://ssf.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aiu.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://iag.yongpay.top

Ruby: s.reverse
来源：http://ivi.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eex.tian-w.cn

[E12] 统计某字符出现次数
来源：http://mwe.fzhhl.top

Py:   s.count("a")
来源：http://mcy.meibo888.top

PHP:  substr_count($s, "a");
来源：http://srm.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://ivm.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://ltz.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://noi.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://qdr.kuanghao11.cn

Ruby: s.count("a")
来源：http://zhx.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://ycw.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://bvu.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://yoo.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpe.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://dqw.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://mcd.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qtm.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bcj.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://fec.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxc.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://ufw.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ugm.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yja.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nyf.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ihg.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uzd.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ybg.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eos.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nvt.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://dxa.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dcj.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iye.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kfk.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://hgn.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gbw.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xks.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mxh.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://boi.shangyingyoupin.top

[E16] 数字千分位
来源：http://qwm.c1oappe.top

Py:   f"{1234567:,}"
来源：http://dob.hnqzz.top

PHP:  number_format(1234567);
来源：http://okt.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://oly.epnwcf.com

TS:   (1234567).toLocaleString("en-US")
来源：http://erv.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xmx.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nbe.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dlv.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://env.xylfe.cn

[E17] 首字母大写
来源：http://kdu.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hri.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wgx.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hiy.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgz.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xul.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hjn.birdmap.top

Ruby: s.capitalize
来源：http://wze.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tgi.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://ghe.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://arc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ibe.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pbg.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zsg.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://acy.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hqh.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwg.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mxu.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://chs.snrcjt.cn

Py:   s.splitlines()
来源：http://gwh.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://msb.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://kli.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://tgr.nwbrower.top

Java: s.lines().toList()
来源：http://ztq.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://bnt.feifeiyinyue.top

Ruby: s.lines
来源：http://scu.cdnleiting.top

C#:   s.Split('\n')
来源：http://veg.havefunace.top

[E20] 判断字符串是否为空
来源：http://rjo.hesvh.cn

Py:   if not s:
来源：http://mbh.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lpu.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://azk.hesvh.cn

TS:   if (s === "") {}
来源：http://yfw.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://kxc.zhiwuduotai.top

Go:   if s == "" {}
来源：http://qfq.sjlbkw.cn

Ruby: if s.empty?
来源：http://fml.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nuz.xinyue.icu

[E21] 超长截断加省略号
来源：http://lkx.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://poz.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sfj.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://akh.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pke.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pqt.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://vcw.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oyk.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://arn.xziqi.cn

[E22] 字节长度与字符长度
来源：http://spl.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqj.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdu.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rlg.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://acf.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ngh.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uta.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://fas.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dpw.feifeiyinyue.top

================================================================================
来源：http://hua.sjlbkw.cn

F. 文件与目录
来源：http://mqs.jiagoushi.top

================================================================================
来源：http://jpx.yueranfly.top

[F01] 读取整个文件
来源：http://cuv.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tbd.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://hjd.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bsw.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ycm.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ffg.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqd.xinyue.icu

Ruby: File.read("a.txt")
来源：http://svr.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://toy.epnwcf.com

[F02] 逐行读取文件
来源：http://beg.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://znm.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oce.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hub.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gms.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qlt.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lcp.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mly.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqh.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://oro.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sow.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://oeh.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://esi.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfg.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bhh.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mnv.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://nth.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wsf.xinyue.icu

[F04] 追加写入文件
来源：http://enp.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gin.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://paf.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zkc.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lma.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vgh.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oer.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://opd.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gmn.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://emf.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bor.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://ikf.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://ech.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://dxk.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bci.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kqu.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://ept.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://toy.snrcjt.cn

[F06] 删除文件
来源：http://uff.sysykeji.top

Py:   os.remove("a.txt")
来源：http://nvy.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://xem.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://xoe.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://qbc.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://krn.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://nir.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://htr.birdmap.top

C#:   File.Delete("a.txt");
来源：http://ylg.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://poo.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kiw.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ksz.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgp.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://how.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nmf.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ouo.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hso.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qtv.bbcook.cn

[F08] 遍历目录
来源：http://exu.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ast.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://exj.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://dxz.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://rji.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eoe.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ybw.xziqi.cn

Ruby: Dir.children("dir")
来源：http://sxa.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://huu.redwolf501.top

[F09] 获取文件大小
来源：http://gvb.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://fqw.52xcode.cn

PHP:  filesize("a.txt");
来源：http://mav.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://hfs.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://uba.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://jcy.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xnp.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://zzo.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://wyh.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://tlr.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ffg.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yaz.hesvh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gmu.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://ykh.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://juf.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hwp.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pll.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ijb.yvedp.cn

[F11] 复制与移动文件
来源：http://twq.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://azj.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssu.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wbt.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ezk.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jut.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qfv.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iuu.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tfu.sxryk.cn

[F12] CSV 读写
来源：http://xpw.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kka.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yhd.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cjd.9152youxi.cn

TS:   // 同上
来源：http://kil.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hfq.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lew.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qvp.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gbt.zhengqikj.top

================================================================================
来源：http://omr.yanxiufei.cn

G. 面向对象
来源：http://bne.gogol.net.cn

================================================================================
来源：http://kdi.zhoulong.xyz

[G01] 定义类
来源：http://lvm.zhiwuduotai.top

Py:   class User: pass
来源：http://ajv.ybcxt.top

PHP:  class User {}
来源：http://rud.jinyuanbaomall.cn

JS:   class User {}
来源：http://lnz.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://cbb.sxryk.cn

Java: class User {}
来源：http://wqr.0kj1m.cn

Go:   type User struct { Name string }
来源：http://qny.ydzc1.top

Ruby: class User; end
来源：http://odz.zhoulong.xyz

C#:   class User {}
来源：http://vrd.sjlbkw.cn

[G02] 构造函数
来源：http://jwy.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://nlo.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://frl.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://olb.pengpengdd.cyou


<!-- 参考信息 -->