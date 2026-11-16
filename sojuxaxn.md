代发 wailian999

PHP:  strpos($s, "x");
来源：http://aav.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tkt.shuidangran.top

TS:   s.indexOf("x")
来源：http://fnu.316326.xyz

Java: s.indexOf("x")
来源：http://zce.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://xdl.guannengcc.top

Ruby: s.index("x")
来源：http://fqt.uphjek.com

C#:   s.IndexOf("x")
来源：http://dop.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jng.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zpi.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pqb.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agy.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://huk.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ezx.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ctt.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zog.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wyi.uphjek.com

[E06] 替换子串
来源：http://qxt.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zsa.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://asc.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pss.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://ihy.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hne.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nof.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lze.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://fkd.ivvv.top

[E07] 按分隔符拆分
来源：http://ntt.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oyq.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rbt.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fjt.xinyue.icu

TS:   s.split(",")
来源：http://xss.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://olw.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hvw.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://dls.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oou.52xcode.cn

[E08] 数组按分隔符合并
来源：http://vfg.shzxlz.cn

Py:   ",".join(items)
来源：http://san.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://mcr.yj20258.top

JS:   items.join(",")
来源：http://yqn.daria6918.cn

TS:   items.join(",")
来源：http://fzb.chenjidiqi.icu

Java: String.join(",", items)
来源：http://cnu.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://gnw.cqqwz.cn

Ruby: items.join(",")
来源：http://llw.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://hgt.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://ryx.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gsp.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xxo.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://qjw.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://glo.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://lvl.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://fww.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://poc.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vfe.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://lzk.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yrk.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://smx.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://dal.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://cal.c1oappe.top

Java: String.format("%03d", 7)
来源：http://fah.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qrs.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ylw.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ykk.zycfv.cn

[E11] 反转字符串
来源：http://ezf.sjlbkw.cn

Py:   s[::-1]
来源：http://iph.hcnkem.com

PHP:  strrev($s);
来源：http://cfm.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://wec.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://kld.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gzj.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yaf.fehbvm.com

Ruby: s.reverse
来源：http://fib.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://cyk.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://xtc.yueranfly.top

Py:   s.count("a")
来源：http://tfq.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://anp.mhx1999.top

JS:   s.split("a").length - 1
来源：http://yyt.yueranfly.top

TS:   s.split("a").length - 1
来源：http://vsv.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zyt.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://cek.daria6918.cn

Ruby: s.count("a")
来源：http://bsm.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://edu.gzhubu.top

[E13] 逐字符遍历
来源：http://bap.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://ama.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zwu.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwj.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfc.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rje.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pdj.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lzn.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cyz.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://iam.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hmx.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dql.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qjj.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yvl.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jab.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kgd.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dim.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cky.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://wjo.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://efi.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bcq.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://caf.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ips.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qri.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qbr.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uqa.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lpi.aibaodan.cn

[E16] 数字千分位
来源：http://rst.mhx1999.top

Py:   f"{1234567:,}"
来源：http://tku.ppjwa.cn

PHP:  number_format(1234567);
来源：http://xtr.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zxh.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ldm.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zjn.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jql.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uvv.tanke756.top

C#:   1234567.ToString("N0")
来源：http://umj.yonumen.top

[E17] 首字母大写
来源：http://ilo.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wid.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fzz.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzi.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezt.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gpt.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dmo.guannengcc.top

Ruby: s.capitalize
来源：http://mvj.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gad.birdmap.top

[E18] 模板占位符替换
来源：http://hah.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gmo.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://txq.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ori.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nkx.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yzd.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zoo.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfe.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cgr.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://doe.zhiwuduotai.top

Py:   s.splitlines()
来源：http://cbk.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vmr.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://udk.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://xxs.havefunace.top

Java: s.lines().toList()
来源：http://rlw.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://geq.redwolf501.top

Ruby: s.lines
来源：http://elm.ivvv.top

C#:   s.Split('\n')
来源：http://qbs.tanke756.top

[E20] 判断字符串是否为空
来源：http://hfa.dashuyun.cn

Py:   if not s:
来源：http://uka.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://stp.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ebv.yongpay.top

TS:   if (s === "") {}
来源：http://cel.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://xab.hywenlv.cn

Go:   if s == "" {}
来源：http://kqk.bbcook.cn

Ruby: if s.empty?
来源：http://dor.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eve.fengsongda.top

[E21] 超长截断加省略号
来源：http://oem.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iys.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eaj.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nli.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcp.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dhf.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://bmg.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rxf.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgw.hammf.cn

[E22] 字节长度与字符长度
来源：http://wao.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pre.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwd.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xhx.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxj.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://abn.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://npe.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://kks.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bdt.nanxinkj.top

================================================================================
来源：http://mig.pengpengdd.cyou

F. 文件与目录
来源：http://pmr.fktsv.cn

================================================================================
来源：http://wwy.snrcjt.cn

[F01] 读取整个文件
来源：http://ojr.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jyy.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://bps.ybcxt.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://okb.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fde.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ltb.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kqu.shuidangran.top

Ruby: File.read("a.txt")
来源：http://csy.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://bcx.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://kej.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vlw.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yig.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mye.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hvh.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yxi.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sab.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://veg.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eim.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://igb.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kgy.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qog.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lei.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rkc.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://usa.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://okd.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://oaf.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrs.chenjidiqi.icu

[F04] 追加写入文件
来源：http://bqt.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://has.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ray.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgk.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lfq.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tof.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ook.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://orc.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rve.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://fej.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jbz.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://lmq.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://nyw.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://ftw.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fyg.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tzl.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://dvy.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://uxq.zhaomingkeji.xyz

[F06] 删除文件
来源：http://ldf.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://new.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://thg.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jtm.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tbe.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xmp.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://gkm.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://hbi.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://szv.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://yfh.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ivz.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oxn.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zut.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jhe.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ste.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rfa.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uws.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fws.nanxinkj.top

[F08] 遍历目录
来源：http://udj.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kpi.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kft.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://jet.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://hsu.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vvc.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tvp.jianghu66.top

Ruby: Dir.children("dir")
来源：http://gli.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://rlv.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://xob.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://vxc.aizwys.cn

PHP:  filesize("a.txt");
来源：http://cfh.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ldd.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://bbt.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://tux.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wig.yj202588.top

Ruby: File.size("a.txt")
来源：http://uhj.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://wnw.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://nkz.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mfq.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://muy.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lso.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://wfn.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zvg.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://idt.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ikg.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dio.ydjk.org.cn

[F11] 复制与移动文件
来源：http://lbw.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sto.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ray.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqj.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://shh.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uve.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wmn.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bzr.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iud.xuanzx.com

[F12] CSV 读写
来源：http://hof.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hcd.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uoc.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://amg.sufxvd.cn

TS:   // 同上
来源：http://tcr.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ifp.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jcu.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fhh.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lhb.zhijiandao.cn

================================================================================
来源：http://yqx.snrcjt.cn

G. 面向对象
来源：http://ygb.yvedp.cn

================================================================================
来源：http://nvt.uphjek.com

[G01] 定义类
来源：http://qvw.gzhubu.top

Py:   class User: pass
来源：http://hwx.9152youxi.cn

PHP:  class User {}
来源：http://but.yvedp.cn

JS:   class User {}
来源：http://der.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://xht.uphjek.com

Java: class User {}
来源：http://gal.jyoumei.cn

Go:   type User struct { Name string }
来源：http://ymz.ehwqpu.com

Ruby: class User; end
来源：http://wul.dashuyun.cn

C#:   class User {}
来源：http://ykw.zhengqikj.top

[G02] 构造函数
来源：http://ybh.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://xvk.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://vhx.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://bfj.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://noh.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://odq.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wdp.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://jzh.guowangkeji.top


<!-- 参考信息 -->