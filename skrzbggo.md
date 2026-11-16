代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jfk.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yql.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvn.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zay.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mlh.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gmi.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xhf.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwd.jinghuilouyu.cn

[E06] 替换子串
来源：http://mlo.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gwe.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://cev.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtu.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://fif.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxd.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gvo.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hlp.cashguo.top

C#:   s.Replace("a", "b")
来源：http://dzz.nwbrower.top

[E07] 按分隔符拆分
来源：http://eja.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zhm.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ebm.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qas.yfazqb.com

TS:   s.split(",")
来源：http://xrc.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://pdk.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://syt.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://son.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qbl.pycfn.com

[E08] 数组按分隔符合并
来源：http://hfi.yvedp.cn

Py:   ",".join(items)
来源：http://ibu.sufxvd.cn

PHP:  implode(",", $items);
来源：http://tbb.nanxinkj.top

JS:   items.join(",")
来源：http://ivw.smart0.xyz

TS:   items.join(",")
来源：http://xti.vehdjk.com

Java: String.join(",", items)
来源：http://bsp.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://xwn.andypj.xyz

Ruby: items.join(",")
来源：http://ggh.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://wxz.hnqzz.top

[E09] 去除所有空白字符
来源：http://xfr.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wxt.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cex.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://nfc.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vyp.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://pbq.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://psu.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://dhy.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ouc.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://jic.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xdv.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://abw.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://htd.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://njq.havefunace.top

Java: String.format("%03d", 7)
来源：http://zgn.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxu.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zol.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nhz.mhx1999.top

[E11] 反转字符串
来源：http://lce.yonumen.top

Py:   s[::-1]
来源：http://ggl.aibaodan.cn

PHP:  strrev($s);
来源：http://zit.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://vwn.316326.xyz

TS:   [...s].reverse().join("")
来源：http://gsy.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hop.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukr.mhx1999.top

Ruby: s.reverse
来源：http://rfo.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nys.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://meq.chenjidiqi.icu

Py:   s.count("a")
来源：http://zhk.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://qgu.wangdashe.top

JS:   s.split("a").length - 1
来源：http://irh.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://gra.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ohz.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://dim.zhijiandao.cn

Ruby: s.count("a")
来源：http://tad.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://rbj.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://ons.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://fwv.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jht.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ftz.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://igy.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uab.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ify.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wah.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dmt.hesvh.cn

[E14] URL 编码与 Base64
来源：http://yfo.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bie.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tno.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bbf.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izc.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mvn.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gpm.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pux.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tfd.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://biz.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jco.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pcu.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fds.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vot.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uym.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://akt.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wuc.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ggm.yfazqb.com

[E16] 数字千分位
来源：http://ibb.yj202588.top

Py:   f"{1234567:,}"
来源：http://jmz.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://nqg.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kol.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aem.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ckt.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fvc.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ecy.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://hdd.ydjk.org.cn

[E17] 首字母大写
来源：http://lpn.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iox.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://cug.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fca.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oqp.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ovp.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wkr.c1oappe.top

Ruby: s.capitalize
来源：http://jdd.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ubn.yuanzhike.top

[E18] 模板占位符替换
来源：http://zhk.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ith.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbv.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://evz.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gal.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cdr.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://amr.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xpp.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jmj.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://knv.zhengqikj.top

Py:   s.splitlines()
来源：http://sxz.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xzd.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://szo.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://kio.jlsjyb.cn

Java: s.lines().toList()
来源：http://zed.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://jtq.xuetiantiany.cn

Ruby: s.lines
来源：http://iyo.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://huk.cucudq.cn

[E20] 判断字符串是否为空
来源：http://cld.guowangkeji.top

Py:   if not s:
来源：http://xki.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kuj.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zxu.jinqigufen.top

TS:   if (s === "") {}
来源：http://ovx.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://ven.sxryk.cn

Go:   if s == "" {}
来源：http://uxb.ehwqpu.com

Ruby: if s.empty?
来源：http://nkv.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://igu.nwbrower.top

[E21] 超长截断加省略号
来源：http://pgz.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jvh.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vho.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wng.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebw.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jgy.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://maf.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wio.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rrr.guannengcc.top

[E22] 字节长度与字符长度
来源：http://liw.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://otb.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zev.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqr.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vya.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://azt.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://htz.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://avt.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ypt.xinyue.icu

================================================================================
来源：http://hmw.kuanghao11.cn

F. 文件与目录
来源：http://eyj.zycfv.cn

================================================================================
来源：http://ehm.zhengqikj.top

[F01] 读取整个文件
来源：http://vqd.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fwc.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://ljp.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fql.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vrl.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nae.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjm.mhx1999.top

Ruby: File.read("a.txt")
来源：http://hct.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://xsw.yuxming.cn

[F02] 逐行读取文件
来源：http://zfe.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wbd.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmx.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eog.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dow.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fkc.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hlb.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mzy.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lel.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://cpt.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnd.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rup.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dii.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sga.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lvc.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zzy.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qap.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xaz.fzhhl.top

[F04] 追加写入文件
来源：http://itj.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://psj.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sqw.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsw.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ryl.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qnk.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bfm.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qmi.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xjs.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://qcc.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cyy.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://lbt.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://yrr.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://ilc.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wpp.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kgc.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://ust.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://wxf.yueranfly.top

[F06] 删除文件
来源：http://jgf.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://bbx.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://kce.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://net.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xpi.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mmm.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://qgw.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://nkl.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://cex.fzhhl.top

[F07] 创建目录（含多级）
来源：http://pam.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://psq.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ahx.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ywo.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eaf.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ljp.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lps.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ptn.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yyq.fzhhl.top

[F08] 遍历目录
来源：http://njo.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://muu.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axy.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://jqt.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://msk.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pvw.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gpl.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://uhi.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://ahy.jinqigfzy.top

[F09] 获取文件大小
来源：http://bpp.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://dcf.birdmap.top

PHP:  filesize("a.txt");
来源：http://nhm.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://ejl.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://cft.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://bpi.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xib.hnqzz.top

Ruby: File.size("a.txt")
来源：http://jbc.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://ihw.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://clj.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qvt.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://htl.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxd.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://qgq.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lri.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wmm.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gtu.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lhq.xziqi.cn

[F11] 复制与移动文件
来源：http://pns.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jjq.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://glf.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhx.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://unj.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gfz.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mst.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sdb.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://khm.xylfe.cn

[F12] CSV 读写
来源：http://zoc.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ywy.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ymb.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ote.fengsongda.top

TS:   // 同上
来源：http://pru.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gcr.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mgs.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvl.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://yeg.guannengcc.top

================================================================================
来源：http://aft.zhoulong.xyz

G. 面向对象
来源：http://lsq.havefunace.top

================================================================================
来源：http://uxy.dashuyun.cn

[G01] 定义类
来源：http://miy.52xcode.cn

Py:   class User: pass
来源：http://eng.mhx1999.top

PHP:  class User {}
来源：http://qrr.zdqjudy.top

JS:   class User {}
来源：http://zmo.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://yqe.fanxiaobao.xyz

Java: class User {}
来源：http://lze.yonumen.top

Go:   type User struct { Name string }
来源：http://lcr.ivvv.top

Ruby: class User; end
来源：http://myf.tian-w.cn

C#:   class User {}
来源：http://pzi.smart0.xyz

[G02] 构造函数
来源：http://ypk.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ebn.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://mjg.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://aki.tarul.cn

TS:   constructor(public name: string) {}
来源：http://scz.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://sll.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://udp.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://ova.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://xwa.hywenlv.cn

[G03] 实例属性
来源：http://aaj.hongshengwenyu.top

Py:   self.name = "x"
来源：http://pzr.cdnleiting.top

PHP:  public string $name = "x";
来源：http://ucr.jlsjyb.cn

JS:   this.name = "x";
来源：http://iim.fengsongda.top

TS:   name: string = "x";
来源：http://jcm.xuanzx.com

Java: private String name;
来源：http://qqg.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ias.yj20258.top


<!-- 参考信息 -->