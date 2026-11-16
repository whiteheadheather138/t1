代发 wailian999

Go:   strings.Index(s, "x")
来源：http://bnq.zhoulong.xyz

Ruby: s.index("x")
来源：http://pxl.cucudq.cn

C#:   s.IndexOf("x")
来源：http://dkt.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkw.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://guy.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knj.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://okj.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lcm.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhs.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ilf.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hux.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rmo.c1oappe.top

[E06] 替换子串
来源：http://kae.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tzk.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ucu.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mgi.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://cps.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjn.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://not.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zyo.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://jhg.yongpay.top

[E07] 按分隔符拆分
来源：http://dna.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://chk.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hxf.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://trj.xziqi.cn

TS:   s.split(",")
来源：http://ywn.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://qis.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fod.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://tkj.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wxh.c1oappe.top

[E08] 数组按分隔符合并
来源：http://ycz.daria6918.cn

Py:   ",".join(items)
来源：http://jrv.tanke756.top

PHP:  implode(",", $items);
来源：http://gmq.daria6918.cn

JS:   items.join(",")
来源：http://gqb.fzhhl.top

TS:   items.join(",")
来源：http://mcg.c1oappe.top

Java: String.join(",", items)
来源：http://mqn.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://ovw.0kj1m.cn

Ruby: items.join(",")
来源：http://kip.zhengqikj.top

C#:   string.Join(",", items)
来源：http://wlw.dianchejie.cn

[E09] 去除所有空白字符
来源：http://oss.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xrx.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lsj.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://zjm.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://nbq.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://qjp.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oyk.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://qyb.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xyk.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://ghh.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gba.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bde.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://qwf.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://agq.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://par.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://inh.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wwk.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jjp.ybcxt.top

[E11] 反转字符串
来源：http://wes.shuidangran.top

Py:   s[::-1]
来源：http://cso.zhijiandao.cn

PHP:  strrev($s);
来源：http://fgr.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://huh.meibo888.top

TS:   [...s].reverse().join("")
来源：http://lku.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://umy.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://evx.xuanzx.com

Ruby: s.reverse
来源：http://dgu.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zip.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://gek.hesvh.cn

Py:   s.count("a")
来源：http://nob.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://del.nwbrower.top

JS:   s.split("a").length - 1
来源：http://lnk.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://vnr.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yev.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://wwp.hesvh.cn

Ruby: s.count("a")
来源：http://hly.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://kum.jqgufenzy.top

[E13] 逐字符遍历
来源：http://bha.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://ssl.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bns.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vsi.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dvc.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gpa.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sxe.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://ghy.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pgl.birdmap.top

[E14] URL 编码与 Base64
来源：http://mwq.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jrw.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ayv.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://txy.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ogh.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uvj.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dxb.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ylp.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mon.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://axx.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mxh.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xlo.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fgd.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wjz.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jas.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bjl.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ata.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aan.shuidangran.top

[E16] 数字千分位
来源：http://oyi.ivvv.top

Py:   f"{1234567:,}"
来源：http://edh.havefunace.top

PHP:  number_format(1234567);
来源：http://ncw.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://etd.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ohg.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nim.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://leb.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sqh.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://lpl.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://qpg.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://caq.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zvg.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gli.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guo.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rar.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sbr.ydjk.org.cn

Ruby: s.capitalize
来源：http://lis.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jjp.tian-w.cn

[E18] 模板占位符替换
来源：http://osc.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sta.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nrw.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wnt.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://eyl.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://elo.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eps.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zbt.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bpi.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://bkm.yonumen.top

Py:   s.splitlines()
来源：http://api.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://las.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://upk.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://vbr.zhijiandao.cn

Java: s.lines().toList()
来源：http://vmz.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://odp.xuetiantiany.cn

Ruby: s.lines
来源：http://cpk.sufxvd.cn

C#:   s.Split('\n')
来源：http://yfo.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://rqn.cucudq.cn

Py:   if not s:
来源：http://jqq.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cpv.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://khf.9152youxi.cn

TS:   if (s === "") {}
来源：http://ene.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://bxi.zhongyouzk.top

Go:   if s == "" {}
来源：http://zny.ybcxt.top

Ruby: if s.empty?
来源：http://ams.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bsk.uphjek.com

[E21] 超长截断加省略号
来源：http://jml.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wyf.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kyg.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbc.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pwg.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gwk.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://nve.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oah.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fbp.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://wsg.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://osg.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lgj.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hsp.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://irl.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ezy.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xwy.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://bug.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jky.jlsjyb.cn

================================================================================
来源：http://rka.pengpengdd.cyou

F. 文件与目录
来源：http://ocb.zhaomingkeji.xyz

================================================================================
来源：http://fmm.gogol.net.cn

[F01] 读取整个文件
来源：http://zti.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qrh.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://fzd.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ibr.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gzf.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dtk.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qhs.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://nap.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://fga.ppjwa.cn

[F02] 逐行读取文件
来源：http://nxu.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ite.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cxt.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://btv.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sdh.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://joo.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yfn.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nex.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hec.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://lso.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uar.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pih.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://itz.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://caa.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uzz.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://icx.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://srn.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twt.gaohongyu789.top

[F04] 追加写入文件
来源：http://mae.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://glx.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mnh.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sqq.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdu.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jod.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wef.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://txl.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rbh.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://imk.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bzt.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://cci.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://iwi.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://xan.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://onp.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djs.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://kgy.yj20258.top

C#:   File.Exists("a.txt")
来源：http://xqx.mhx1999.top

[F06] 删除文件
来源：http://seg.sweek.top

Py:   os.remove("a.txt")
来源：http://rks.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://bgg.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hah.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://tzv.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ksp.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://zxw.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://tkl.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://fqv.sysykeji.top

[F07] 创建目录（含多级）
来源：http://bvm.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gaw.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lvg.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jww.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://obc.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tlq.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ggy.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tfh.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://alb.cdnleiting.top

[F08] 遍历目录
来源：http://cxa.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bbr.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uin.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://jho.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://diy.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jpn.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gfa.fzhhl.top

Ruby: Dir.children("dir")
来源：http://ons.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://uer.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://sjg.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://pef.yfazqb.com

PHP:  filesize("a.txt");
来源：http://qqi.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://gyt.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://ccp.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jps.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pfi.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://avo.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://wig.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://rfq.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mql.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwm.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vsh.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://auj.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://utv.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ern.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqw.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://irj.c1oappe.top

[F11] 复制与移动文件
来源：http://sso.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jwe.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bjo.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fmv.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rhh.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hds.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nyg.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uih.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vow.zhongyouzk.top

[F12] CSV 读写
来源：http://wjf.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rho.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://idl.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fnn.sxryk.cn

TS:   // 同上
来源：http://gqn.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmm.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lms.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fdw.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dxu.shangyingyoupin.top

================================================================================
来源：http://obe.hesvh.cn

G. 面向对象
来源：http://hul.hongshengwenyu.top

================================================================================
来源：http://lzk.mhx1999.top

[G01] 定义类
来源：http://ydw.fktsv.cn

Py:   class User: pass
来源：http://beh.ydzc1.top

PHP:  class User {}
来源：http://ngz.xinyue.icu

JS:   class User {}
来源：http://rle.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://gsn.chenjidiqi.icu

Java: class User {}
来源：http://avj.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://glc.havefunace.top

Ruby: class User; end
来源：http://uqq.birdmap.top

C#:   class User {}
来源：http://qbb.svipenyu.cn

[G02] 构造函数
来源：http://jez.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://fun.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://lak.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://ral.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://grx.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://ing.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dwq.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://hoj.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://ghi.jqgfzy.top

[G03] 实例属性
来源：http://yae.smart0.xyz

Py:   self.name = "x"
来源：http://phv.sweek.top

PHP:  public string $name = "x";
来源：http://puc.tian-w.cn


<!-- 参考信息 -->