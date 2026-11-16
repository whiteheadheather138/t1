代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvc.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yjt.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ven.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dye.0kj1m.cn

[E06] 替换子串
来源：http://lud.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hoy.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://szi.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqi.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://wki.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbo.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fob.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vdd.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://fkt.yuanzhike.top

[E07] 按分隔符拆分
来源：http://gpq.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://myn.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cre.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tvx.haohaochexian.top

TS:   s.split(",")
来源：http://mrb.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://rpo.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zio.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://zrg.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://akz.tian-w.cn

[E08] 数组按分隔符合并
来源：http://pkf.ybcxt.top

Py:   ",".join(items)
来源：http://pnt.zhixingplan.top

PHP:  implode(",", $items);
来源：http://mog.sweek.top

JS:   items.join(",")
来源：http://ier.snrcjt.cn

TS:   items.join(",")
来源：http://pdu.tian-w.cn

Java: String.join(",", items)
来源：http://kzm.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://btw.9152youxi.cn

Ruby: items.join(",")
来源：http://pgk.hnqzz.top

C#:   string.Join(",", items)
来源：http://zxi.snrcjt.cn

[E09] 去除所有空白字符
来源：http://ggy.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kaj.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://evm.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://svd.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://zhg.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://mzk.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tva.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hlu.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cho.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://mrk.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lih.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vau.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://eiz.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://tnc.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://cha.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kfc.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wuf.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://asa.nwbrower.top

[E11] 反转字符串
来源：http://ybt.fehbvm.com

Py:   s[::-1]
来源：http://shk.ctjpmb.com

PHP:  strrev($s);
来源：http://emy.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://nkh.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://jyk.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hvr.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sad.zhixingplan.top

Ruby: s.reverse
来源：http://sqg.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fau.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://gqf.zhongyouzk.top

Py:   s.count("a")
来源：http://qpd.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://ikv.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://zrx.redwolf501.top

TS:   s.split("a").length - 1
来源：http://yds.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://owk.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://tva.shzxlz.cn

Ruby: s.count("a")
来源：http://knu.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://qhw.gzhubu.top

[E13] 逐字符遍历
来源：http://ocl.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://cdn.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://prc.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eph.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://jzk.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jyz.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ojc.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://orz.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://shb.hnqzz.top

[E14] URL 编码与 Base64
来源：http://rjl.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ghy.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qeh.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukb.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lkr.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nlc.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://puo.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dqa.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bkc.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://vbk.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hbv.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xrh.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dvl.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://khb.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://suu.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vaj.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dtv.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vcw.shangyingyoupin.top

[E16] 数字千分位
来源：http://gys.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://sse.chenzaomai.com

PHP:  number_format(1234567);
来源：http://dlh.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zyh.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sgf.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://too.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qgd.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mse.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://qkc.shanyushiyangtech.top

[E17] 首字母大写
来源：http://ams.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nqf.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uds.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqc.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jho.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://emb.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vrr.tianlin.xyz

Ruby: s.capitalize
来源：http://mcn.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://syu.jiagoushi.top

[E18] 模板占位符替换
来源：http://lam.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ewm.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://twu.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sin.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hmw.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eez.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bwf.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vvm.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yrr.gzhubu.top

[E19] 多行文本按行拆分
来源：http://ftu.chenlongwang.top

Py:   s.splitlines()
来源：http://ryy.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzx.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://vlu.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://fav.316326.xyz

Java: s.lines().toList()
来源：http://jur.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://ndd.jlsjyb.cn

Ruby: s.lines
来源：http://oro.gaohongyu789.top

C#:   s.Split('\n')
来源：http://afx.ybcxt.top

[E20] 判断字符串是否为空
来源：http://wtj.yfazqb.com

Py:   if not s:
来源：http://jyf.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgd.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ntk.snrcjt.cn

TS:   if (s === "") {}
来源：http://etd.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://ber.hfpthk.cn

Go:   if s == "" {}
来源：http://ipb.wangdashe.top

Ruby: if s.empty?
来源：http://jxe.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mdv.yvedp.cn

[E21] 超长截断加省略号
来源：http://cyb.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qsm.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aon.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tdo.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bhu.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ksv.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://kax.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wqs.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ihy.guannengcc.top

[E22] 字节长度与字符长度
来源：http://fsj.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qha.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iez.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfq.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqb.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zuv.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ciy.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://rdx.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iuw.ctjpmb.com

================================================================================
来源：http://flm.ydjk.org.cn

F. 文件与目录
来源：http://npp.dashuyun.cn

================================================================================
来源：http://thq.shzxlz.cn

[F01] 读取整个文件
来源：http://hqi.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://skg.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://qpa.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jvq.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xkj.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vvs.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://egx.shuidangran.top

Ruby: File.read("a.txt")
来源：http://rii.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://teg.zhixingplan.top

[F02] 逐行读取文件
来源：http://kst.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ubd.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://drl.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjm.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hht.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rra.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mcb.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vbd.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://afn.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://ufv.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wyb.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rqb.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxb.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://agi.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zzo.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://toq.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ahi.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://svo.snrcjt.cn

[F04] 追加写入文件
来源：http://cos.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vvr.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mrg.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gxi.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oct.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pxz.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qxk.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbb.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fza.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://auo.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://syu.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://moe.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://spd.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://bpl.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gvg.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhk.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://hyi.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://kcb.cashguo.top

[F06] 删除文件
来源：http://iwt.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://nej.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://kch.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bum.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://voi.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hgn.sweek.top

Go:   os.Remove("a.txt")
来源：http://xmg.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://quq.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://mkz.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://jmq.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ztj.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wnr.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jch.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oys.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gca.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ktp.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lqr.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rgm.hesvh.cn

[F08] 遍历目录
来源：http://lfk.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uqk.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wpa.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://pyh.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://ecq.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mae.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zid.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://doa.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://ncq.yj20258.top

[F09] 获取文件大小
来源：http://qll.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://mbv.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://ryv.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://qix.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://usd.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://uet.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pto.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://dud.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://eva.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://wyo.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jml.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iaa.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://adf.fktsv.cn

TS:   path.extname("a.txt")
来源：http://gbh.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxv.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eoe.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qzs.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uux.hesvh.cn

[F11] 复制与移动文件
来源：http://vat.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iqc.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://anb.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrn.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://waj.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://epx.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zdq.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oxp.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zxe.aizwys.cn

[F12] CSV 读写
来源：http://tko.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zbo.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qob.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://drt.xziqi.cn

TS:   // 同上
来源：http://ars.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ztx.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://twk.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mcf.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ote.xuetiantiany.cn

================================================================================
来源：http://sbr.shuidangran.top

G. 面向对象
来源：http://rro.vqdsnc.cn

================================================================================
来源：http://hfa.chenjidiqi.icu

[G01] 定义类
来源：http://yqp.zycfv.cn

Py:   class User: pass
来源：http://qos.ydzc1.top

PHP:  class User {}
来源：http://bju.fktsv.cn

JS:   class User {}
来源：http://oum.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://bbu.kuanghao11.cn

Java: class User {}
来源：http://odc.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://hzb.jinqigfzy.top

Ruby: class User; end
来源：http://abg.yueranfly.top

C#:   class User {}
来源：http://syy.zhixingplan.top

[G02] 构造函数
来源：http://kus.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rzb.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://mmu.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://imf.sweek.top

TS:   constructor(public name: string) {}
来源：http://ykh.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://uvv.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mgh.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://pci.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://vcq.pengpengdd.cyou

[G03] 实例属性
来源：http://osk.hfpthk.cn

Py:   self.name = "x"
来源：http://tsy.birdmap.top

PHP:  public string $name = "x";
来源：http://fky.kuanghao11.cn

JS:   this.name = "x";
来源：http://smj.ivvv.top

TS:   name: string = "x";
来源：http://ebz.yueranfly.top

Java: private String name;
来源：http://caf.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cdg.pycfn.com

Ruby: @name = "x"
来源：http://vzx.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://myg.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://wyg.fzhhl.top

Py:   def greet(self): return self.name
来源：http://mdv.jqgfzy.top


<!-- 参考信息 -->