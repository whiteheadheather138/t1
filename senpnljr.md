代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ofb.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mnt.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyc.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qdm.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhj.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gyh.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dzr.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lju.shangyingyoupin.top

[E06] 替换子串
来源：http://gue.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bro.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://xip.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://exz.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://ouv.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxz.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kiz.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wym.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://buz.fzhhl.top

[E07] 按分隔符拆分
来源：http://odw.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmx.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eud.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yic.xinyue.icu

TS:   s.split(",")
来源：http://shv.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://elr.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fvu.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://kqa.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vzg.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://tmk.yvedp.cn

Py:   ",".join(items)
来源：http://myw.fzhhl.top

PHP:  implode(",", $items);
来源：http://qbh.ybcxt.top

JS:   items.join(",")
来源：http://nbt.sweek.top

TS:   items.join(",")
来源：http://pmc.redwolf501.top

Java: String.join(",", items)
来源：http://qyi.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://dlc.yonumen.top

Ruby: items.join(",")
来源：http://izz.fktsv.cn

C#:   string.Join(",", items)
来源：http://jvn.smart0.xyz

[E09] 去除所有空白字符
来源：http://adu.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hri.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qxy.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://xkc.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://gos.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://vjp.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ydj.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://krp.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mna.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://csg.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://amo.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xyf.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://smg.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://lho.hesvh.cn

Java: String.format("%03d", 7)
来源：http://ygj.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ilg.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fgs.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rkf.jiagoushi.top

[E11] 反转字符串
来源：http://myc.wangshuangyany.cn

Py:   s[::-1]
来源：http://wgf.aibaodan.cn

PHP:  strrev($s);
来源：http://ldz.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://bns.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://lqf.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://boa.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kfa.tianlin.xyz

Ruby: s.reverse
来源：http://ppo.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://rdb.ybcxt.top

[E12] 统计某字符出现次数
来源：http://glk.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://bsr.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://bww.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://wuk.havefunace.top

TS:   s.split("a").length - 1
来源：http://ygc.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kac.yongpay.top

Go:   strings.Count(s, "a")
来源：http://ntx.yongpay.top

Ruby: s.count("a")
来源：http://yhj.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://tla.shuidangran.top

[E13] 逐字符遍历
来源：http://hrp.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://zbf.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pqx.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://axz.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://upn.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nqv.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uwk.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ntq.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pdp.sxryk.cn

[E14] URL 编码与 Base64
来源：http://jxg.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yed.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sqz.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lzi.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yok.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://scl.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uya.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pen.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eic.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://vcv.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://clj.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ldf.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zht.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://may.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gyf.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wgi.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://psz.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ocr.52xcode.cn

[E16] 数字千分位
来源：http://kso.xylfe.cn

Py:   f"{1234567:,}"
来源：http://kzm.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://aoh.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://azf.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://tqz.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gkr.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://way.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://efw.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://qfv.daria6918.cn

[E17] 首字母大写
来源：http://iug.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nrf.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xnp.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://clp.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xhr.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vai.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ftk.havefunace.top

Ruby: s.capitalize
来源：http://ssu.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ghg.hcnkem.com

[E18] 模板占位符替换
来源：http://clr.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wck.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tso.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xsl.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ipd.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fvx.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xud.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cau.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyv.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://zze.redwolf501.top

Py:   s.splitlines()
来源：http://wxw.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oen.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://zts.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://jmt.shuidangran.top

Java: s.lines().toList()
来源：http://wmc.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://nwc.shanyushiyangtech.top

Ruby: s.lines
来源：http://uae.yj20258.top

C#:   s.Split('\n')
来源：http://lxn.xinyue.icu

[E20] 判断字符串是否为空
来源：http://djz.aibaodan.cn

Py:   if not s:
来源：http://kmt.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oeq.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tfs.jinqigfzy.top

TS:   if (s === "") {}
来源：http://ydd.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://cbl.svipenyu.cn

Go:   if s == "" {}
来源：http://mcv.sufxvd.cn

Ruby: if s.empty?
来源：http://lzo.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://soa.havefunace.top

[E21] 超长截断加省略号
来源：http://doo.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qmx.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bxy.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rmk.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afo.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://flj.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://eif.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jvz.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cav.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://ejd.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rzj.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zlg.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmj.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lim.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://otk.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cbq.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://yxy.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qzq.ctjpmb.com

================================================================================
来源：http://aqs.cucudq.cn

F. 文件与目录
来源：http://ick.epnwcf.com

================================================================================
来源：http://ebh.jianghu66.top

[F01] 读取整个文件
来源：http://gyg.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aip.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://kvr.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qsp.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywg.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://nnf.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sse.cucudq.cn

Ruby: File.read("a.txt")
来源：http://wws.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yyq.kuanghao11.cn

[F02] 逐行读取文件
来源：http://rat.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gkf.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbq.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pea.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://axg.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sls.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ysx.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uvp.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vmh.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://hed.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://naw.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://exi.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ull.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aaz.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kzr.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vtp.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://fir.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awj.mhx1999.top

[F04] 追加写入文件
来源：http://qpx.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qyr.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://isv.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ioo.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fhl.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://klg.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://guo.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bqj.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wyr.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://bza.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://emb.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://zkv.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://dkd.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://cbu.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zlm.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jnv.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://poe.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://jif.ctjpmb.com

[F06] 删除文件
来源：http://mtt.yueranfly.top

Py:   os.remove("a.txt")
来源：http://sui.zycfv.cn

PHP:  unlink("a.txt");
来源：http://hrm.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://hua.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://zry.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qhx.cashguo.top

Go:   os.Remove("a.txt")
来源：http://egz.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://tae.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://ahb.yfazqb.com

[F07] 创建目录（含多级）
来源：http://dvz.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rtm.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jvi.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aig.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lyl.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vpn.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://huo.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ned.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://knm.bjfxy.top

[F08] 遍历目录
来源：http://kwv.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://azc.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ehz.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://lgf.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://adg.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oug.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gnh.tian-w.cn

Ruby: Dir.children("dir")
来源：http://yzu.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://ujk.ybcxt.top

[F09] 获取文件大小
来源：http://jiq.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://fns.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://igi.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://opp.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://kmp.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pmk.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mud.hcnkem.com

Ruby: File.size("a.txt")
来源：http://dfr.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://isw.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://fvt.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iwy.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hnc.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://viv.tian-w.cn

TS:   path.extname("a.txt")
来源：http://vyu.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lao.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xgm.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnk.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ixi.ehwqpu.com

[F11] 复制与移动文件
来源：http://eqe.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vek.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ytp.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upg.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gjj.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ahf.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kkf.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jqo.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jln.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://wqe.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cyd.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dmy.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iiy.daxiang520.top

TS:   // 同上
来源：http://mkb.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cvq.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mlj.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nwc.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ytm.zhoulong.xyz

================================================================================
来源：http://tfc.xziqi.cn

G. 面向对象
来源：http://gkx.tanke756.top

================================================================================
来源：http://fyi.xuetiantiany.cn

[G01] 定义类
来源：http://fkd.zhoulong.xyz

Py:   class User: pass
来源：http://ikh.daria6918.cn

PHP:  class User {}
来源：http://xhf.xuetiantiany.cn

JS:   class User {}
来源：http://nbc.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://bgs.cucudq.cn

Java: class User {}
来源：http://wge.ybcxt.top

Go:   type User struct { Name string }
来源：http://mlp.hongshengwenyu.top

Ruby: class User; end
来源：http://mxh.tian-w.cn

C#:   class User {}
来源：http://pvs.jinqigufen.top

[G02] 构造函数
来源：http://hlo.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://yue.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://jjt.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://vms.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://efn.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://nai.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wwp.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://okr.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://you.aibaodan.cn

[G03] 实例属性
来源：http://xpq.yj20258.top

Py:   self.name = "x"
来源：http://ewt.dashuyun.cn

PHP:  public string $name = "x";
来源：http://fus.nanxuanxn.top

JS:   this.name = "x";
来源：http://zqc.tarul.cn

TS:   name: string = "x";
来源：http://jmi.pengpengdd.cyou

Java: private String name;
来源：http://nol.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wmw.gzhubu.top


<!-- 参考信息 -->