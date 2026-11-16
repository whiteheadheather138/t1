代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://big.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fjh.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ktt.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kpb.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://pyr.nwbrower.top

[E07] 按分隔符拆分
来源：http://fwd.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://acu.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bug.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://akf.sufxvd.cn

TS:   s.split(",")
来源：http://bzy.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://lad.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dpm.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://yem.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jzx.iojbl.cn

[E08] 数组按分隔符合并
来源：http://kik.hywenlv.cn

Py:   ",".join(items)
来源：http://emd.nwbrower.top

PHP:  implode(",", $items);
来源：http://rxp.zycfv.cn

JS:   items.join(",")
来源：http://sje.hesvh.cn

TS:   items.join(",")
来源：http://tbn.dianchejie.cn

Java: String.join(",", items)
来源：http://fcm.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://ghe.nanxinkj.top

Ruby: items.join(",")
来源：http://xmb.snrcjt.cn

C#:   string.Join(",", items)
来源：http://xqo.sxryk.cn

[E09] 去除所有空白字符
来源：http://idt.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://saw.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vcg.0kj1m.cn

JS:   s.replace(/\s+/g, "")
来源：http://mxq.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://mrx.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://sca.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zwe.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vfa.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pcp.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://iyx.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jar.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xnb.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://ajo.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://pjc.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://pjz.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sfp.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yke.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yoy.guannengcc.top

[E11] 反转字符串
来源：http://fez.tanke756.top

Py:   s[::-1]
来源：http://irc.jqgfzy.top

PHP:  strrev($s);
来源：http://khd.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://nmf.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://wzu.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lyz.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gxo.ydzc1.top

Ruby: s.reverse
来源：http://auc.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://mxx.52xcode.cn

[E12] 统计某字符出现次数
来源：http://jgh.hongshengwenyu.top

Py:   s.count("a")
来源：http://mqp.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://uqo.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://rog.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://etf.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lei.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://yib.daria6918.cn

Ruby: s.count("a")
来源：http://vzf.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://dmf.yfazqb.com

[E13] 逐字符遍历
来源：http://rct.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://eqp.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vbl.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gda.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zvg.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cme.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qzi.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://knh.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qkc.cucudq.cn

[E14] URL 编码与 Base64
来源：http://qhr.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wee.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eta.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zrq.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gqb.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://svh.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dho.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vdt.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rvc.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://ekx.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://odi.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nav.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://trz.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xtp.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rsc.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sps.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lay.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vjt.hfpthk.cn

[E16] 数字千分位
来源：http://fmk.andypj.xyz

Py:   f"{1234567:,}"
来源：http://weh.yonumen.top

PHP:  number_format(1234567);
来源：http://smx.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://obw.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hvi.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lum.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ocg.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jwj.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://cqc.kuanghao11.cn

[E17] 首字母大写
来源：http://abv.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mkq.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jjq.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ffz.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iig.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://etl.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qir.xinyue.icu

Ruby: s.capitalize
来源：http://iro.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mro.hesvh.cn

[E18] 模板占位符替换
来源：http://tom.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hbz.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hzf.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vbm.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fpj.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vjl.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cew.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bgr.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fzd.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://gpo.jianghu66.top

Py:   s.splitlines()
来源：http://yde.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gti.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://xti.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://wbm.gzhubu.top

Java: s.lines().toList()
来源：http://hkr.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://tkz.ydzc1.top

Ruby: s.lines
来源：http://uni.meibo888.top

C#:   s.Split('\n')
来源：http://syj.nwbrower.top

[E20] 判断字符串是否为空
来源：http://ipk.gotoacloud.top

Py:   if not s:
来源：http://eyg.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ots.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://khp.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://ewp.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://cgf.chenlongwang.top

Go:   if s == "" {}
来源：http://pcn.shuidangran.top

Ruby: if s.empty?
来源：http://joc.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vkb.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://kzc.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfj.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tpj.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jii.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gnh.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qzt.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://qgm.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vqp.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://igp.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://gqz.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qva.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qje.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mmf.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nuu.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rxv.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bmj.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://tjh.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iyl.gaohongyu789.top

================================================================================
来源：http://anj.daxiang520.top

F. 文件与目录
来源：http://nlc.hysaishi.cn

================================================================================
来源：http://ymk.ybcxt.top

[F01] 读取整个文件
来源：http://dij.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eio.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://eat.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pqd.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gsq.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cld.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zfr.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://rkt.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://sfw.hnqzz.top

[F02] 逐行读取文件
来源：http://cfx.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hkt.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gwz.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofa.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vui.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qvz.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nev.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qmw.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yet.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://zzo.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qug.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fyi.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hvh.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lnb.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cgp.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://czb.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://kpr.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://usd.shuidangran.top

[F04] 追加写入文件
来源：http://wsi.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jqc.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sdz.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gpk.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eih.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pgk.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uyi.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hki.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzt.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://ejj.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zie.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://esp.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://eaw.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://uvt.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tiv.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wtx.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://koj.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://wtu.yuxming.cn

[F06] 删除文件
来源：http://dwj.cucudq.cn

Py:   os.remove("a.txt")
来源：http://evy.fehbvm.com

PHP:  unlink("a.txt");
来源：http://mid.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://mql.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hak.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://edd.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://fzk.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://ald.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://xeu.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://kof.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zsd.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sos.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xik.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yci.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lqo.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mmz.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jkz.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vaf.tianlin.xyz

[F08] 遍历目录
来源：http://diq.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vzs.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cwv.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://abb.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://ooc.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpg.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xrb.bbcook.cn

Ruby: Dir.children("dir")
来源：http://xsb.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://jfu.cheryme.top

[F09] 获取文件大小
来源：http://dzr.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://vre.jianghu66.top

PHP:  filesize("a.txt");
来源：http://cvf.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://wib.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://ccw.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://skz.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://atv.tanke756.top

Ruby: File.size("a.txt")
来源：http://mzt.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://yzq.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://ort.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfk.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uth.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pof.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://mzq.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afj.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uqq.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gvu.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lqa.chenzaomai.com

[F11] 复制与移动文件
来源：http://dwg.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zwd.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qcw.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://owb.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qwk.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qfj.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pzo.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nkv.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://apa.ydzc1.top

[F12] CSV 读写
来源：http://daj.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://joy.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qji.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivk.cdnleiting.top

TS:   // 同上
来源：http://egb.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wip.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xgq.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://erq.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://bfh.jqgufenzy.top

================================================================================
来源：http://kfb.ctjpmb.com

G. 面向对象
来源：http://gpy.andypj.xyz

================================================================================
来源：http://xzr.yj20258.top

[G01] 定义类
来源：http://tyx.smart0.xyz

Py:   class User: pass
来源：http://ncg.zhaomingkeji.xyz

PHP:  class User {}
来源：http://uyv.shanyushiyangtech.top

JS:   class User {}
来源：http://ecg.meibo888.top

TS:   class User { name: string = ""; }
来源：http://jlm.cheryme.top

Java: class User {}
来源：http://ras.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://aef.yueranfly.top

Ruby: class User; end
来源：http://gtd.zhoulong.xyz

C#:   class User {}
来源：http://cbb.fengsongda.top

[G02] 构造函数
来源：http://nom.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://zcz.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://rlu.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://cph.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://nbs.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://ppt.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vop.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://zty.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://ivn.fktsv.cn

[G03] 实例属性
来源：http://ccd.cashguo.top

Py:   self.name = "x"
来源：http://exs.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://efa.cheryme.top

JS:   this.name = "x";
来源：http://qfa.xziqi.cn

TS:   name: string = "x";
来源：http://ilz.svipenyu.cn

Java: private String name;
来源：http://dlm.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zcb.gotoacloud.top

Ruby: @name = "x"
来源：http://xlj.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://zsv.bbcook.cn

[G04] 定义方法
来源：http://fep.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://jrg.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ywq.cucudq.cn

JS:   greet() { return this.name; }
来源：http://fyr.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://qrb.tarul.cn

Java: String greet() { return name; }
来源：http://ewb.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qew.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://aej.gzhubu.top

C#:   public string Greet() => Name;
来源：http://vho.xuanzx.com

[G05] 继承
来源：http://itq.birdmap.top


<!-- 参考信息 -->