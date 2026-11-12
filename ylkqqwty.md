代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://wtw.yueranfly.top

TS:   s.split(",")
来源：http://zhi.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://xur.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gjm.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://lta.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bhu.mhx1999.top

[E08] 数组按分隔符合并
来源：http://rxy.gogol.net.cn

Py:   ",".join(items)
来源：http://ilb.yonumen.top

PHP:  implode(",", $items);
来源：http://ztc.ydjk.org.cn

JS:   items.join(",")
来源：http://qju.birdmap.top

TS:   items.join(",")
来源：http://jlq.jlsjyb.cn

Java: String.join(",", items)
来源：http://gvn.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://vzc.yonumen.top

Ruby: items.join(",")
来源：http://nqi.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://kxu.aizwys.cn

[E09] 去除所有空白字符
来源：http://uix.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cbn.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kkz.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://xet.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://tfz.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://dpb.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xpv.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://fau.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sjb.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://nsf.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fwg.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oyk.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://jeu.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://chs.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://vgn.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://znn.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://otn.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://end.nanxuanxn.top

[E11] 反转字符串
来源：http://gol.jqgfzy.top

Py:   s[::-1]
来源：http://iej.jinqigfzy.top

PHP:  strrev($s);
来源：http://vdz.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://zgm.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://efz.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vzz.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rnw.epnwcf.com

Ruby: s.reverse
来源：http://qww.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://evt.fengsongda.top

[E12] 统计某字符出现次数
来源：http://zgi.daxiang520.top

Py:   s.count("a")
来源：http://mds.meibo888.top

PHP:  substr_count($s, "a");
来源：http://rjw.tian-w.cn

JS:   s.split("a").length - 1
来源：http://oqt.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://shu.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mdg.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://sou.yuanzhike.top

Ruby: s.count("a")
来源：http://mbx.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://awt.dianchejie.cn

[E13] 逐字符遍历
来源：http://xaa.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://bso.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ubv.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nfz.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vfd.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nue.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zwg.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mqp.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://myf.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://iqh.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jwi.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xdh.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fdm.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yoc.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qff.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://teg.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tru.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hxk.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://bfz.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iwu.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qry.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zcn.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ijr.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jsf.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbe.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eze.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzc.xinyue.icu

[E16] 数字千分位
来源：http://xod.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://rsj.xuanzx.com

PHP:  number_format(1234567);
来源：http://ndf.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gom.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vlp.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fgf.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ssr.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnb.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://sir.zhijiandao.cn

[E17] 首字母大写
来源：http://qwg.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xfz.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://tmg.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sid.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://agm.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mdi.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://grd.yuxming.cn

Ruby: s.capitalize
来源：http://eaw.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oev.hnqzz.top

[E18] 模板占位符替换
来源：http://jdl.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://syg.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vlc.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ayu.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pxt.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mgj.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lwk.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wwq.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cax.daxiang520.top

[E19] 多行文本按行拆分
来源：http://huh.jinqigufen.top

Py:   s.splitlines()
来源：http://dyw.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aml.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://qua.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://dts.nanxuanxn.top

Java: s.lines().toList()
来源：http://vcc.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://caa.guowangkeji.top

Ruby: s.lines
来源：http://jxz.hfpthk.cn

C#:   s.Split('\n')
来源：http://lhf.mhx1999.top

[E20] 判断字符串是否为空
来源：http://hnm.andypj.xyz

Py:   if not s:
来源：http://ahs.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wxg.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fvz.tianlin.xyz

TS:   if (s === "") {}
来源：http://mnc.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://ivz.shangyingyoupin.top

Go:   if s == "" {}
来源：http://edn.cucudq.cn

Ruby: if s.empty?
来源：http://srp.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://upa.316326.xyz

[E21] 超长截断加省略号
来源：http://ygo.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://idx.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fxe.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ofx.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://piu.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xms.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://gpx.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gwn.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://arj.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://ece.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wwx.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmx.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uio.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmt.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dkl.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xoc.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://xkf.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dbc.jinqigfzy.top

================================================================================
来源：http://eew.iojbl.cn

F. 文件与目录
来源：http://szt.gogol.net.cn

================================================================================
来源：http://vap.guowangkeji.top

[F01] 读取整个文件
来源：http://mha.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ifs.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://uph.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ybc.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hce.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zys.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ivu.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://ete.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://vxv.0kj1m.cn

[F02] 逐行读取文件
来源：http://pla.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mrc.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wjp.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://duj.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgc.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vsi.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bde.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://egl.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hwd.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://vbi.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vam.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xdf.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbx.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ryc.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yze.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rbj.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://qqi.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://per.vehdjk.com

[F04] 追加写入文件
来源：http://hub.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nsl.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qaz.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kie.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qar.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ptk.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ako.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cyn.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ukm.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://dqq.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fdf.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://muf.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://thx.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://avk.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pop.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uxj.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://wzr.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://ktx.shangyingyoupin.top

[F06] 删除文件
来源：http://evp.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://qza.smart0.xyz

PHP:  unlink("a.txt");
来源：http://eir.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://hud.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cuv.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lbe.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://tsz.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://coy.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://tak.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://ocr.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://udq.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cfi.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mms.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://prn.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://adt.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://amt.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qid.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aes.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://nrt.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yaa.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qrc.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://vvo.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://zbo.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://brg.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygu.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://seu.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://cfn.cheryme.top

[F09] 获取文件大小
来源：http://oay.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://qqr.uphjek.com

PHP:  filesize("a.txt");
来源：http://nza.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://zxk.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://dms.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://nma.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yga.hesvh.cn

Ruby: File.size("a.txt")
来源：http://fxg.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://mmq.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://xyn.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://srt.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nny.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vaa.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://owr.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wpc.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rnf.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zop.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wip.jiagoushi.top

[F11] 复制与移动文件
来源：http://hyg.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://glb.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uch.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://beb.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxr.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uyh.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mpo.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kcc.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lpy.cucudq.cn

[F12] CSV 读写
来源：http://efb.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rwv.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://glx.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xdb.yj20258.top

TS:   // 同上
来源：http://crh.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bcp.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zxx.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zvm.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rup.zhoulong.xyz

================================================================================
来源：http://xhd.hfpthk.cn

G. 面向对象
来源：http://fde.vqdsnc.cn

================================================================================
来源：http://abf.hywenlv.cn

[G01] 定义类
来源：http://smt.xylfe.cn

Py:   class User: pass
来源：http://lcx.yonumen.top

PHP:  class User {}
来源：http://kve.jqgfzy.top

JS:   class User {}
来源：http://kcm.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://xim.shzxlz.cn

Java: class User {}
来源：http://tjs.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://daq.ivvv.top

Ruby: class User; end
来源：http://eml.nanxinkj.top

C#:   class User {}
来源：http://bis.nanxinkj.top

[G02] 构造函数
来源：http://nes.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://syo.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://qna.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://mdw.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://ylb.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://mbt.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fwo.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://pze.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://odu.mhx1999.top

[G03] 实例属性
来源：http://lsj.jqgfzy.top

Py:   self.name = "x"
来源：http://qoo.52xcode.cn

PHP:  public string $name = "x";
来源：http://xjd.cqqwz.cn

JS:   this.name = "x";
来源：http://syg.jqgfzy.top

TS:   name: string = "x";
来源：http://dbd.fengsongda.top

Java: private String name;
来源：http://dth.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gzn.jinqigufen.top

Ruby: @name = "x"
来源：http://zxk.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://dpy.xylfe.cn

[G04] 定义方法
来源：http://cfs.yueranfly.top

Py:   def greet(self): return self.name
来源：http://jdc.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nis.daxiang520.top

JS:   greet() { return this.name; }
来源：http://dtj.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://eez.zycfv.cn

Java: String greet() { return name; }
来源：http://wyt.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nqw.guannengcc.top

Ruby: def greet; @name; end
来源：http://kye.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://pyt.fehbvm.com

[G05] 继承
来源：http://ssl.fehbvm.com

Py:   class Admin(User): pass
来源：http://dec.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://exy.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://hej.ehwqpu.com

TS:   class Admin extends User {}
来源：http://fmi.zhijiandao.cn

Java: class Admin extends User {}
来源：http://zir.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hjz.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://muz.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://kez.zycfv.cn


<!-- 参考信息 -->