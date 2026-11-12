代发 wailian999

C#:   s.Replace("a", "b")
来源：http://nwa.smart0.xyz

[E07] 按分隔符拆分
来源：http://ufq.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://owm.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dub.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uve.gaohongyu789.top

TS:   s.split(",")
来源：http://nqb.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://djm.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iqt.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://lty.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grk.zycfv.cn

[E08] 数组按分隔符合并
来源：http://puq.hywenlv.cn

Py:   ",".join(items)
来源：http://wdx.cucudq.cn

PHP:  implode(",", $items);
来源：http://ttu.gogol.net.cn

JS:   items.join(",")
来源：http://zpo.jianghu66.top

TS:   items.join(",")
来源：http://bku.zycfv.cn

Java: String.join(",", items)
来源：http://llz.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://nrc.smart0.xyz

Ruby: items.join(",")
来源：http://hni.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://nsb.meibo888.top

[E09] 去除所有空白字符
来源：http://kxz.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkc.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iyr.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://xbz.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://rgu.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://thc.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://avp.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://mnu.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dnm.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://zsq.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fam.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aao.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://yxq.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://hbi.jianghu66.top

Java: String.format("%03d", 7)
来源：http://rxv.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wuf.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tne.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dxb.c1oappe.top

[E11] 反转字符串
来源：http://jei.cdnleiting.top

Py:   s[::-1]
来源：http://nnp.sysykeji.top

PHP:  strrev($s);
来源：http://kuc.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://yit.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://ned.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://slq.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hlk.xinyue.icu

Ruby: s.reverse
来源：http://sxm.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ula.fktsv.cn

[E12] 统计某字符出现次数
来源：http://jod.52xcode.cn

Py:   s.count("a")
来源：http://gru.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://rqt.mhx1999.top

JS:   s.split("a").length - 1
来源：http://xno.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://gga.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xdo.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://shu.yueranfly.top

Ruby: s.count("a")
来源：http://bxu.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://uxo.vqdsnc.cn

[E13] 逐字符遍历
来源：http://wxm.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://mtz.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvu.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://azm.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://smh.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dad.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://azg.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vfb.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hyb.guannengcc.top

[E14] URL 编码与 Base64
来源：http://maa.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vsl.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qfv.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ibv.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ehp.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jfd.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dye.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://afi.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ukq.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://crq.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zss.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hyv.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bix.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mrz.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pdh.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nng.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nmk.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqn.nwbrower.top

[E16] 数字千分位
来源：http://gem.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://tku.gogol.net.cn

PHP:  number_format(1234567);
来源：http://tju.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pbm.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cez.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zvf.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oqk.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jty.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://ttq.jinqigufen.top

[E17] 首字母大写
来源：http://mja.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ocp.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jkj.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwy.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vme.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jie.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wpv.yj202588.top

Ruby: s.capitalize
来源：http://rpz.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ova.hywenlv.cn

[E18] 模板占位符替换
来源：http://ksc.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ugo.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ynz.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://oyr.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yyv.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rzz.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lzq.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cir.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ukf.ybcxt.top

[E19] 多行文本按行拆分
来源：http://pna.shzxlz.cn

Py:   s.splitlines()
来源：http://nrk.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qwp.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://fam.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://jli.shzxlz.cn

Java: s.lines().toList()
来源：http://hra.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://ilw.shzxlz.cn

Ruby: s.lines
来源：http://qfd.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://mrt.tian-w.cn

[E20] 判断字符串是否为空
来源：http://usn.shangyingyoupin.top

Py:   if not s:
来源：http://nlh.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tdd.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ylh.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://efn.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://qgd.xuanzx.com

Go:   if s == "" {}
来源：http://qqz.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://yjf.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dca.aizwys.cn

[E21] 超长截断加省略号
来源：http://cob.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xgx.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ajf.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsx.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fpz.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uvx.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://snn.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dkw.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pfh.daria6918.cn

[E22] 字节长度与字符长度
来源：http://sap.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wys.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bdl.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pew.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijx.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rcz.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vsz.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://srs.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hnz.nwbrower.top

================================================================================
来源：http://zmh.chenzaomai.com

F. 文件与目录
来源：http://rnz.mhx1999.top

================================================================================
来源：http://lpb.tianlin.xyz

[F01] 读取整个文件
来源：http://hia.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jhu.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://ugu.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dln.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xwk.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vse.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tie.sysykeji.top

Ruby: File.read("a.txt")
来源：http://fui.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://kqf.ivvv.top

[F02] 逐行读取文件
来源：http://etq.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ipx.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mky.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lro.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnv.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qvq.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vnb.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qag.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sss.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://vbh.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ptj.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sbe.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfe.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uao.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zxs.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bdf.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://osk.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kyp.xylfe.cn

[F04] 追加写入文件
来源：http://sro.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://awd.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yvm.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxu.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dva.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://myc.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aqk.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eru.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ept.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://caf.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ehk.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://fbq.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://ukz.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://ljs.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ayk.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bcc.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://qye.316326.xyz

C#:   File.Exists("a.txt")
来源：http://cho.havefunace.top

[F06] 删除文件
来源：http://str.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://lln.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://ijk.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://xnc.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://veo.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kyi.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://oqk.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://ycg.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://whn.yj202588.top

[F07] 创建目录（含多级）
来源：http://vdu.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zea.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gxc.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qob.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkx.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fmu.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cxk.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tjy.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ttg.52xcode.cn

[F08] 遍历目录
来源：http://tzv.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ehx.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nxt.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://gdb.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://ltv.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vlr.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zzf.guannengcc.top

Ruby: Dir.children("dir")
来源：http://ttj.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://xcz.fehbvm.com

[F09] 获取文件大小
来源：http://llb.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://oql.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://ppo.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://xxl.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://xjx.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ahx.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gyi.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://oge.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://bxz.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://mop.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://imy.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zbq.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uog.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://vvt.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qvj.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dvd.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cwx.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oyv.jianghu66.top

[F11] 复制与移动文件
来源：http://sra.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ydt.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hey.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wza.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ijv.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yab.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wqd.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eqp.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://awy.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://klt.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rmk.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xgu.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hsm.yueranfly.top

TS:   // 同上
来源：http://upt.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xaa.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jqe.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://une.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vsy.havefunace.top

================================================================================
来源：http://bsy.yuxming.cn

G. 面向对象
来源：http://jzd.nanxinkj.top

================================================================================
来源：http://wnp.tianlin.xyz

[G01] 定义类
来源：http://dcs.zhoulong.xyz

Py:   class User: pass
来源：http://frs.cucudq.cn

PHP:  class User {}
来源：http://khe.cucudq.cn

JS:   class User {}
来源：http://xgr.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://asc.zhiwuduotai.top

Java: class User {}
来源：http://qdg.andypj.xyz

Go:   type User struct { Name string }
来源：http://oix.hcnkem.com

Ruby: class User; end
来源：http://muw.feifeiyinyue.top

C#:   class User {}
来源：http://iva.fanxiaobao.xyz

[G02] 构造函数
来源：http://fok.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://ukk.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://umb.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://jfn.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://bub.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://oyo.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oih.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://krr.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://tqf.birdmap.top

[G03] 实例属性
来源：http://nni.meibo888.top

Py:   self.name = "x"
来源：http://mhi.tanke756.top

PHP:  public string $name = "x";
来源：http://jxo.hywenlv.cn

JS:   this.name = "x";
来源：http://ajd.zhijiandao.cn

TS:   name: string = "x";
来源：http://kcr.daxiang520.top

Java: private String name;
来源：http://fld.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aqa.andypj.xyz

Ruby: @name = "x"
来源：http://txk.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://frc.yongpay.top

[G04] 定义方法
来源：http://izx.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://mve.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ljy.ydzc1.top

JS:   greet() { return this.name; }
来源：http://aoe.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://qcp.chenzaomai.com

Java: String greet() { return name; }
来源：http://sif.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kma.birdmap.top

Ruby: def greet; @name; end
来源：http://imv.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://xfg.shanyushiyangtech.top

[G05] 继承
来源：http://sve.sufxvd.cn

Py:   class Admin(User): pass
来源：http://fsf.yonumen.top

PHP:  class Admin extends User {}
来源：http://ftw.dashuyun.cn

JS:   class Admin extends User {}
来源：http://eca.hesvh.cn

TS:   class Admin extends User {}
来源：http://kzc.andypj.xyz


<!-- 参考信息 -->