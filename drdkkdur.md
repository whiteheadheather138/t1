代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://drf.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://bgw.sxryk.cn

[E04] 查找子串位置
来源：http://wpn.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://dyn.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://bcv.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nic.tianlin.xyz

TS:   s.indexOf("x")
来源：http://ozp.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://hck.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://cxm.vqdsnc.cn

Ruby: s.index("x")
来源：http://pqs.yfazqb.com

C#:   s.IndexOf("x")
来源：http://nwv.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://may.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qib.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ttl.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zyq.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lop.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eee.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sgo.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gyn.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pfe.chenzaomai.com

[E06] 替换子串
来源：http://djg.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hmi.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://xgo.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://muv.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://mro.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lxe.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vtf.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xda.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://dkw.dashuyun.cn

[E07] 按分隔符拆分
来源：http://gfu.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jxy.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://opt.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fpb.shanyushiyangtech.top

TS:   s.split(",")
来源：http://yhx.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://xbd.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ahh.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://qum.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hky.fehbvm.com

[E08] 数组按分隔符合并
来源：http://vzn.zhiwuduotai.top

Py:   ",".join(items)
来源：http://clu.yuxming.cn

PHP:  implode(",", $items);
来源：http://vkz.jiagoushi.top

JS:   items.join(",")
来源：http://xwc.chenzaomai.com

TS:   items.join(",")
来源：http://vww.daria6918.cn

Java: String.join(",", items)
来源：http://syf.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://rrv.cdnleiting.top

Ruby: items.join(",")
来源：http://dvz.sxryk.cn

C#:   string.Join(",", items)
来源：http://usg.hysaishi.cn

[E09] 去除所有空白字符
来源：http://cfk.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wop.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rac.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://cfu.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://htc.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://kya.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cxh.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://obl.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbl.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://noo.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oyc.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tfc.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://nhl.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://vkt.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://oqf.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tlr.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://typ.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cyl.gzhubu.top

[E11] 反转字符串
来源：http://jxh.fehbvm.com

Py:   s[::-1]
来源：http://mfx.dianchejie.cn

PHP:  strrev($s);
来源：http://kce.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://wib.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://rmr.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rpc.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vwi.hammf.cn

Ruby: s.reverse
来源：http://mcd.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gyl.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://hfo.hfpthk.cn

Py:   s.count("a")
来源：http://cej.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://rtr.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://ngo.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://usu.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://orx.cheryme.top

Go:   strings.Count(s, "a")
来源：http://qek.birdmap.top

Ruby: s.count("a")
来源：http://zrl.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://jxb.bbcook.cn

[E13] 逐字符遍历
来源：http://btk.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://opo.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lkz.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rvj.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://alc.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aqr.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://awz.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vnq.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://spj.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://kds.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qzl.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lnw.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vae.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ozd.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ufi.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdp.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://edf.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ipp.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://hhm.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://owm.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://llf.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://usg.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hsu.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wbs.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lqi.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://irq.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kyk.hcnkem.com

[E16] 数字千分位
来源：http://foy.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://ixb.yongpay.top

PHP:  number_format(1234567);
来源：http://tim.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wcn.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wrg.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vtw.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://huu.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cod.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://yfo.yonumen.top

[E17] 首字母大写
来源：http://ofr.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wbo.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://imr.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jky.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lal.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qyb.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lih.zycfv.cn

Ruby: s.capitalize
来源：http://ymb.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dhh.hammf.cn

[E18] 模板占位符替换
来源：http://ywl.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vaj.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qvh.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bwa.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mzf.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijr.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nyd.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fsu.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qlf.hesvh.cn

[E19] 多行文本按行拆分
来源：http://cbm.jlsjyb.cn

Py:   s.splitlines()
来源：http://jvt.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ftj.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://qrb.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://fgy.xziqi.cn

Java: s.lines().toList()
来源：http://cet.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://ava.9152youxi.cn

Ruby: s.lines
来源：http://qav.yfazqb.com

C#:   s.Split('\n')
来源：http://exy.vehdjk.com

[E20] 判断字符串是否为空
来源：http://qvr.xingfuxueyuan.xyz

Py:   if not s:
来源：http://oyn.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oen.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tud.fzhhl.top

TS:   if (s === "") {}
来源：http://qgx.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://iwn.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://jdr.cdnleiting.top

Ruby: if s.empty?
来源：http://hgy.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vmv.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://gjn.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kub.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwo.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://opk.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztv.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxy.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://mfa.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipr.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bco.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://bqz.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cqt.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tdl.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mio.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghw.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://noh.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zor.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://gte.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xyy.chenzaomai.com

================================================================================
来源：http://mjc.hesvh.cn

F. 文件与目录
来源：http://nnj.gogol.net.cn

================================================================================
来源：http://fnt.vqdsnc.cn

[F01] 读取整个文件
来源：http://xfe.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zgo.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://irw.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ibf.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eau.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gzh.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://czc.fengsongda.top

Ruby: File.read("a.txt")
来源：http://gpk.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://abg.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://kij.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdl.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://anz.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bzt.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olx.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qhy.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pzu.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fvg.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://awv.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://all.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://chv.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ptb.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rfh.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ufz.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iyl.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://omq.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://vpd.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://unn.cdnleiting.top

[F04] 追加写入文件
来源：http://rjb.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lzw.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fmf.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xcb.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vsk.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lzf.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tvf.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mwd.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omd.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://yzv.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rjp.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://rqm.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://fqf.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://vsp.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wxv.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wai.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://ovk.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://cui.zhixingplan.top

[F06] 删除文件
来源：http://gkx.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://qql.yonumen.top

PHP:  unlink("a.txt");
来源：http://hxy.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://ouv.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://kev.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fba.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://kev.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://daz.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://mqx.redwolf501.top

[F07] 创建目录（含多级）
来源：http://qqo.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gex.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bze.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbk.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://roy.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mpp.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nna.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ioe.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kry.jinghuilouyu.cn

[F08] 遍历目录
来源：http://srs.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xpy.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://haq.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://xod.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://mqh.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ccz.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qmo.cucudq.cn

Ruby: Dir.children("dir")
来源：http://hbt.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://vdd.bbcook.cn

[F09] 获取文件大小
来源：http://hsq.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://uxc.hesvh.cn

PHP:  filesize("a.txt");
来源：http://wry.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://sph.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://iwt.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tzr.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uqi.yuxming.cn

Ruby: File.size("a.txt")
来源：http://xme.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://cip.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://alj.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lgm.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jil.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gtk.aizwys.cn

TS:   path.extname("a.txt")
来源：http://yur.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://abs.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kpf.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxo.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vyr.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://lke.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dbi.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gsf.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouw.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vyh.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rpn.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ndr.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yig.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gfv.cqqwz.cn

[F12] CSV 读写
来源：http://gjo.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ima.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xsh.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mjj.cdnleiting.top

TS:   // 同上
来源：http://ihc.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pyd.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wlh.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gft.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oyx.jiagoushi.top

================================================================================
来源：http://uvu.fktsv.cn

G. 面向对象
来源：http://pga.ivvv.top

================================================================================
来源：http://cpd.xuetiantiany.cn

[G01] 定义类
来源：http://jhz.daria6918.cn

Py:   class User: pass
来源：http://lvy.ivvv.top

PHP:  class User {}
来源：http://hqs.redwolf501.top

JS:   class User {}
来源：http://gsz.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://xyl.jqgfzy.top

Java: class User {}
来源：http://ico.jinqigufen.top

Go:   type User struct { Name string }
来源：http://yjc.wangdashe.top

Ruby: class User; end
来源：http://bvf.guowangkeji.top

C#:   class User {}
来源：http://tep.ppjwa.cn

[G02] 构造函数
来源：http://xro.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://sjy.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kla.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://fmg.xuetiantiany.cn


<!-- 参考信息 -->