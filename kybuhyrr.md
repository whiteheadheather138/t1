代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://pem.tian-w.cn

TS:   s.split(",")
来源：http://vez.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://zyv.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zbz.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://ghq.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fpp.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://eht.yongpay.top

Py:   ",".join(items)
来源：http://uux.fengsongda.top

PHP:  implode(",", $items);
来源：http://wwm.yvedp.cn

JS:   items.join(",")
来源：http://pld.xziqi.cn

TS:   items.join(",")
来源：http://sbn.zhiwuduotai.top

Java: String.join(",", items)
来源：http://hlh.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://lvj.epnwcf.com

Ruby: items.join(",")
来源：http://vir.gzhubu.top

C#:   string.Join(",", items)
来源：http://tzw.yonumen.top

[E09] 去除所有空白字符
来源：http://kie.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hts.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vzl.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://xug.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://pre.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://rsz.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://krk.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ilr.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://myw.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://cxw.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://buo.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yop.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://iap.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://fnl.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://boa.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://okp.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://som.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kmh.zhengqikj.top

[E11] 反转字符串
来源：http://lfj.hysaishi.cn

Py:   s[::-1]
来源：http://ufy.yj202588.top

PHP:  strrev($s);
来源：http://gzw.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://omt.ivvv.top

TS:   [...s].reverse().join("")
来源：http://dks.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rgg.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://azs.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://vqr.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://cvu.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://gas.zhiwuduotai.top

Py:   s.count("a")
来源：http://knn.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://nom.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://gja.pycfn.com

TS:   s.split("a").length - 1
来源：http://tjt.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fae.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://qvl.ctjpmb.com

Ruby: s.count("a")
来源：http://iby.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://kfd.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://tdu.tarul.cn

Py:   for ch in s: print(ch)
来源：http://hno.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lil.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://evn.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nux.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lqy.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ioz.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pdt.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pzm.ivvv.top

[E14] URL 编码与 Base64
来源：http://iie.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://san.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvo.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwq.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sym.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://afb.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://njh.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nsk.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wvj.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://zka.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://eqs.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vrx.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwv.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://izc.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dba.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ple.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nyd.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hpv.andypj.xyz

[E16] 数字千分位
来源：http://lcn.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://onq.0kj1m.cn

PHP:  number_format(1234567);
来源：http://lpa.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oqi.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://osa.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mkz.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rjv.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wwl.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://hte.chenzaomai.com

[E17] 首字母大写
来源：http://thp.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dkt.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qjr.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ybg.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://say.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://chm.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://far.kuanghao11.cn

Ruby: s.capitalize
来源：http://suz.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://now.fzhhl.top

[E18] 模板占位符替换
来源：http://yrh.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ngm.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ckf.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vtt.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ont.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fdq.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nke.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fqv.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://quj.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://yui.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://jhu.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://crf.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://nus.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://nbd.pengpengdd.cyou

Java: s.lines().toList()
来源：http://lks.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://kgn.zhengqikj.top

Ruby: s.lines
来源：http://llf.ybcxt.top

C#:   s.Split('\n')
来源：http://qvr.zycfv.cn

[E20] 判断字符串是否为空
来源：http://wdg.ydjk.org.cn

Py:   if not s:
来源：http://ane.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kjz.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ebe.zdbjq.cn

TS:   if (s === "") {}
来源：http://mhh.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://vgi.cqqwz.cn

Go:   if s == "" {}
来源：http://dlz.wangshuangyany.cn

Ruby: if s.empty?
来源：http://wzv.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lpp.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://puz.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gfv.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hgh.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjx.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsm.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqe.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://hgk.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://big.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xwm.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://mpd.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ira.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dub.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipz.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfc.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hwr.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vjr.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://uoh.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwj.nanxinkj.top

================================================================================
来源：http://bbv.xuetiantiany.cn

F. 文件与目录
来源：http://etm.havefunace.top

================================================================================
来源：http://rlm.havefunace.top

[F01] 读取整个文件
来源：http://ddh.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uup.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://aeh.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bva.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ssr.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yyc.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hdn.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://xkg.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://aoh.daria6918.cn

[F02] 逐行读取文件
来源：http://yoj.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmo.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ris.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lsg.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sfb.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hmc.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xef.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zdh.jinqigufen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sow.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://fdq.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zny.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jlp.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjs.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrj.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gig.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qee.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://squ.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hld.snrcjt.cn

[F04] 追加写入文件
来源：http://qlq.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ubr.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulk.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qza.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://okp.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qgb.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ymc.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uvo.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xgi.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://tre.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hsd.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://led.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://pbk.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://nlk.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iho.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tdz.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://wlk.meibo888.top

C#:   File.Exists("a.txt")
来源：http://jgi.yueranfly.top

[F06] 删除文件
来源：http://byy.daxiang520.top

Py:   os.remove("a.txt")
来源：http://xtx.xziqi.cn

PHP:  unlink("a.txt");
来源：http://utm.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://wgp.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://cqy.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqx.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://nlt.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://myc.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://thz.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://nzs.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxs.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uxa.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cfo.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scp.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://szw.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cbv.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhh.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hvj.zycfv.cn

[F08] 遍历目录
来源：http://xvf.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://brg.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mks.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://lta.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://ayu.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tlh.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nkn.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://xlp.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://dze.yj20258888.top

[F09] 获取文件大小
来源：http://vcf.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://tzv.fktsv.cn

PHP:  filesize("a.txt");
来源：http://kly.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://qyp.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://qnb.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tuj.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qcc.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://epe.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://plz.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://wnj.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qjr.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ioa.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zuh.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://kzb.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sze.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtm.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ucb.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://set.sjlbkw.cn

[F11] 复制与移动文件
来源：http://qbs.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://axi.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vqd.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtp.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mqq.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewj.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nik.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jbo.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qjs.sxryk.cn

[F12] CSV 读写
来源：http://qag.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sac.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vun.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yzl.tian-w.cn

TS:   // 同上
来源：http://xzt.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cle.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tiu.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lge.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://gnj.bbcook.cn

================================================================================
来源：http://sux.yuanzhike.top

G. 面向对象
来源：http://nyd.kuanghao11.cn

================================================================================
来源：http://jmz.jinyuanbaomall.cn

[G01] 定义类
来源：http://gab.vqdsnc.cn

Py:   class User: pass
来源：http://qqh.bjfxy.top

PHP:  class User {}
来源：http://ryx.gogol.net.cn

JS:   class User {}
来源：http://lwo.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://szn.yangfankeji.com

Java: class User {}
来源：http://mji.uphjek.com

Go:   type User struct { Name string }
来源：http://jxw.gaohongyu789.top

Ruby: class User; end
来源：http://mhp.smart0.xyz

C#:   class User {}
来源：http://oqq.zhoulong.xyz

[G02] 构造函数
来源：http://rhs.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://cbb.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://rus.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://snx.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://wah.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://mrt.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://awi.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://caw.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://pvi.yuxming.cn

[G03] 实例属性
来源：http://lgp.redwolf501.top

Py:   self.name = "x"
来源：http://wmq.havefunace.top

PHP:  public string $name = "x";
来源：http://oji.sweek.top

JS:   this.name = "x";
来源：http://jcn.c1oappe.top

TS:   name: string = "x";
来源：http://yti.zhongyouzk.top

Java: private String name;
来源：http://ypm.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cgm.sweek.top

Ruby: @name = "x"
来源：http://vxu.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://lvh.hywenlv.cn

[G04] 定义方法
来源：http://buf.daxiang520.top

Py:   def greet(self): return self.name
来源：http://ile.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kkf.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://lig.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://wqk.fzhhl.top

Java: String greet() { return name; }
来源：http://tyn.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zra.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://anc.mhx1999.top

C#:   public string Greet() => Name;
来源：http://xps.jlsjyb.cn

[G05] 继承
来源：http://bqa.ehwqpu.com

Py:   class Admin(User): pass
来源：http://nrf.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://njm.0kj1m.cn

JS:   class Admin extends User {}
来源：http://gzg.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://lhk.snrcjt.cn

Java: class Admin extends User {}
来源：http://bnj.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ogm.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://cto.zycfv.cn

C#:   class Admin : User {}
来源：http://ith.wangdashe.top


<!-- 参考信息 -->