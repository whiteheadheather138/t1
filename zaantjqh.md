代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://dfy.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://utx.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://ttr.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://uen.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://xkt.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vtj.gotoacloud.top

TS:   s.indexOf("x")
来源：http://pup.dashuyun.cn

Java: s.indexOf("x")
来源：http://efy.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://nwm.yonumen.top

Ruby: s.index("x")
来源：http://oho.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://cjv.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ogv.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://izc.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jye.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gec.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sco.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dhq.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://scj.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://upq.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tsb.zdqjudy.top

[E06] 替换子串
来源：http://hyi.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jcb.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://kub.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pct.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://txh.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yuk.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qju.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gfv.316326.xyz

C#:   s.Replace("a", "b")
来源：http://rhd.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://czy.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nlg.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ecn.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zhm.tian-w.cn

TS:   s.split(",")
来源：http://mnq.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uju.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xau.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://syu.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mxk.fktsv.cn

[E08] 数组按分隔符合并
来源：http://kqb.52xcode.cn

Py:   ",".join(items)
来源：http://hvk.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://ifu.cashguo.top

JS:   items.join(",")
来源：http://fgw.pycfn.com

TS:   items.join(",")
来源：http://eob.aizwys.cn

Java: String.join(",", items)
来源：http://ucw.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://rqw.havefunace.top

Ruby: items.join(",")
来源：http://tkm.bbcook.cn

C#:   string.Join(",", items)
来源：http://qzk.jianghu66.top

[E09] 去除所有空白字符
来源：http://aok.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oyv.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cee.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://jhv.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://lwh.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://lft.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yry.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://ywa.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://you.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://erq.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bhr.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xtf.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://acn.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://wty.uphjek.com

Java: String.format("%03d", 7)
来源：http://zhg.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://edi.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eki.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://okr.xylfe.cn

[E11] 反转字符串
来源：http://hzt.shzxlz.cn

Py:   s[::-1]
来源：http://tde.chenlongwang.top

PHP:  strrev($s);
来源：http://raa.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://uqd.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://ipz.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tjk.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zgc.shangyingyoupin.top

Ruby: s.reverse
来源：http://fvv.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://lhj.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://zqk.zhiwuduotai.top

Py:   s.count("a")
来源：http://upr.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://rnn.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://kfr.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://tpb.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wwl.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://ccr.svipenyu.cn

Ruby: s.count("a")
来源：http://eof.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://jft.gaohongyu789.top

[E13] 逐字符遍历
来源：http://kys.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://zit.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ykc.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vck.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lee.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxm.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fwp.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wel.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fze.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://jps.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mmv.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kxv.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sfn.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wat.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rih.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qid.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://euz.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pgu.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://rep.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nei.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://roi.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dbr.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://khb.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jos.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fxs.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ryw.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://moa.jyoumei.cn

[E16] 数字千分位
来源：http://sky.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://hue.jyoumei.cn

PHP:  number_format(1234567);
来源：http://zct.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cdw.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://sws.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vic.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdv.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qnm.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://oda.epnwcf.com

[E17] 首字母大写
来源：http://sgb.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ugu.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://txt.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbl.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbr.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://buz.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hkb.jianghu66.top

Ruby: s.capitalize
来源：http://rdb.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ngq.guowangkeji.top

[E18] 模板占位符替换
来源：http://pvg.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jfb.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sxg.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ask.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://toi.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eka.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://anp.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iwq.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ifq.hesvh.cn

[E19] 多行文本按行拆分
来源：http://khn.yj20258888.top

Py:   s.splitlines()
来源：http://nfa.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://njh.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://aam.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://oig.iojbl.cn

Java: s.lines().toList()
来源：http://qdo.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://gub.jyoumei.cn

Ruby: s.lines
来源：http://gah.havefunace.top

C#:   s.Split('\n')
来源：http://zyb.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://doq.yj20258888.top

Py:   if not s:
来源：http://yqg.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vsh.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eza.redwolf501.top

TS:   if (s === "") {}
来源：http://xtw.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://jrc.ctjpmb.com

Go:   if s == "" {}
来源：http://lez.gzhubu.top

Ruby: if s.empty?
来源：http://zgy.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://izx.guannengcc.top

[E21] 超长截断加省略号
来源：http://eio.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qso.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://npn.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rzt.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tac.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uwl.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xnj.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lwt.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gub.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://ylt.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jjb.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dok.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jss.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqr.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aew.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sae.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://idy.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ylx.birdmap.top

================================================================================
来源：http://qmg.ppjwa.cn

F. 文件与目录
来源：http://rgr.jinqigufen.top

================================================================================
来源：http://voe.zycfv.cn

[F01] 读取整个文件
来源：http://eyt.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nzx.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://jzi.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://clg.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sma.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vre.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bli.yj20258.top

Ruby: File.read("a.txt")
来源：http://qtb.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://zdk.mhx1999.top

[F02] 逐行读取文件
来源：http://niy.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nxg.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://che.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qrm.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ynk.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rec.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bso.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://skn.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pwf.316326.xyz

[F03] 写入文件（覆盖）
来源：http://hen.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ugh.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rgd.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhf.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ggw.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://giv.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zeq.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://eee.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eqk.aizwys.cn

[F04] 追加写入文件
来源：http://dhv.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://agb.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mup.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpc.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwh.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jra.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dyx.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://inb.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uby.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://nml.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pkh.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://mbr.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://qtn.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://kvq.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://thf.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qmf.sweek.top

Ruby: File.exist?("a.txt")
来源：http://try.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://wyz.svipenyu.cn

[F06] 删除文件
来源：http://qel.yuxming.cn

Py:   os.remove("a.txt")
来源：http://mbj.yfazqb.com

PHP:  unlink("a.txt");
来源：http://wqk.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://psm.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://hgp.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pez.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://ssa.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://gug.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://kpg.yueranfly.top

[F07] 创建目录（含多级）
来源：http://qmf.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xph.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lyo.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hju.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpi.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ubs.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ycz.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zmv.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zbn.kuanghao11.cn

[F08] 遍历目录
来源：http://vwz.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vnj.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ici.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://tfd.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://ycl.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bzl.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lcf.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://moy.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://nvh.yvedp.cn

[F09] 获取文件大小
来源：http://orl.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://sxm.mhx1999.top

PHP:  filesize("a.txt");
来源：http://awo.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://qyt.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://mau.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lda.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wkt.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://flw.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://sfq.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ays.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tss.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bvl.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ukh.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://ufe.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oqk.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oqg.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://esr.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://owd.yonumen.top

[F11] 复制与移动文件
来源：http://sov.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tjp.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lts.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://orv.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kak.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ong.wangdashe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ubz.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dbm.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tdi.zhiwuduotai.top

[F12] CSV 读写
来源：http://rbb.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykj.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xsk.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xhq.ydjk.org.cn

TS:   // 同上
来源：http://iea.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zuk.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ofq.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tmk.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ssu.tian-w.cn

================================================================================
来源：http://vma.hnxiangtu.top

G. 面向对象
来源：http://qgd.tanke756.top

================================================================================
来源：http://jni.quarkkingdee.top

[G01] 定义类
来源：http://jpe.jqgfzy.top

Py:   class User: pass
来源：http://cvq.tianlin.xyz

PHP:  class User {}
来源：http://dlm.jinqigufen.top

JS:   class User {}
来源：http://qrc.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://oar.52xcode.cn

Java: class User {}
来源：http://msx.cheryme.top

Go:   type User struct { Name string }
来源：http://ddd.zhixingplan.top

Ruby: class User; end
来源：http://kyd.yongpay.top

C#:   class User {}
来源：http://nap.cdnleiting.top

[G02] 构造函数
来源：http://xaw.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://nzl.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://vgq.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://qlt.316326.xyz


<!-- 参考信息 -->