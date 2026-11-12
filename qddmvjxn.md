代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hzg.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yub.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ukj.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eky.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://ewj.ydzc1.top

[E07] 按分隔符拆分
来源：http://dzf.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dom.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fqv.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzf.ydjk.org.cn

TS:   s.split(",")
来源：http://lmh.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://xdw.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qlq.cashguo.top

Ruby: s.split(",");  s.split
来源：http://mvk.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lsu.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://xhn.snrcjt.cn

Py:   ",".join(items)
来源：http://efe.mhx1999.top

PHP:  implode(",", $items);
来源：http://lkg.zhongyouzk.top

JS:   items.join(",")
来源：http://xbw.yfazqb.com

TS:   items.join(",")
来源：http://ywy.ppjwa.cn

Java: String.join(",", items)
来源：http://iej.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://iau.tarul.cn

Ruby: items.join(",")
来源：http://pwg.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://enx.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://vzp.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jtj.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fht.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://oaa.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://slm.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://vom.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://puy.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://muo.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cfk.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://yfl.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tzj.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kvy.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://erz.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://ijv.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://lvn.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://usq.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dea.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nmr.yanxiufei.cn

[E11] 反转字符串
来源：http://mal.jinqigufen.top

Py:   s[::-1]
来源：http://gvs.tianlin.xyz

PHP:  strrev($s);
来源：http://qye.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://lhy.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://lrv.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://noq.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://vxb.sjlbkw.cn

Ruby: s.reverse
来源：http://zfv.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zqg.iojbl.cn

[E12] 统计某字符出现次数
来源：http://tjy.jqgfzy.top

Py:   s.count("a")
来源：http://wuj.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://hkn.yvedp.cn

JS:   s.split("a").length - 1
来源：http://hip.wangdashe.top

TS:   s.split("a").length - 1
来源：http://ezh.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ytp.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://xre.yj202588.top

Ruby: s.count("a")
来源：http://pmc.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://hkd.mhx1999.top

[E13] 逐字符遍历
来源：http://yko.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://nys.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mod.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://nji.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gpx.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dks.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lgo.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://giq.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tkn.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://peh.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xqm.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://awg.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yul.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yxp.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bhd.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ufl.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wen.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfm.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://fic.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://zrh.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://frn.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qsq.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ehp.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://usw.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fss.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://znh.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zde.hysaishi.cn

[E16] 数字千分位
来源：http://lfi.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://xfd.xinyue.icu

PHP:  number_format(1234567);
来源：http://zqb.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://hxu.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://lpr.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vsz.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cce.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgg.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://qem.uphjek.com

[E17] 首字母大写
来源：http://dgx.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fcr.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sje.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://stt.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jfj.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mom.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://clf.quarkkingdee.top

Ruby: s.capitalize
来源：http://bbn.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdo.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://gam.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ztl.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pmb.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lbf.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cll.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://snz.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfq.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bqa.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mkr.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://nkf.pycfn.com

Py:   s.splitlines()
来源：http://tql.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://apd.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://cyg.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://wae.yvedp.cn

Java: s.lines().toList()
来源：http://msa.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://tka.ydjk.org.cn

Ruby: s.lines
来源：http://ond.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://uln.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://bvu.fktsv.cn

Py:   if not s:
来源：http://uez.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qqj.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ohb.yongpay.top

TS:   if (s === "") {}
来源：http://hwg.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://xkn.snrcjt.cn

Go:   if s == "" {}
来源：http://xvm.chenjidiqi.icu

Ruby: if s.empty?
来源：http://mmh.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yra.chenzaomai.com

[E21] 超长截断加省略号
来源：http://bgt.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fsb.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zjf.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mbt.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pjr.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lqv.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://qrr.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bqj.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssh.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://kvc.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hgh.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zbd.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sll.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fzx.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://knu.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wda.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://avb.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gwb.mhx1999.top

================================================================================
来源：http://ide.wangdashe.top

F. 文件与目录
来源：http://esu.ywan-chungtsiang.top

================================================================================
来源：http://qil.daxiang520.top

[F01] 读取整个文件
来源：http://mvf.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ihp.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://ueg.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sfu.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ory.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://czk.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wmy.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://tds.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://fhr.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://ktb.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gtd.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tcg.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aye.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbh.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://joe.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sru.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ptp.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bhg.ivvv.top

[F03] 写入文件（覆盖）
来源：http://kck.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pmk.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vmz.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvd.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ole.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dtd.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gyu.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://iew.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zeo.c1oappe.top

[F04] 追加写入文件
来源：http://ncg.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oxy.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nav.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fob.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofv.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ijk.xziqi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://prw.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lyt.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jdq.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://bye.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ruf.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://bzi.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://ktr.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://qgo.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://yjk.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gfb.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://zum.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://iap.yj202588.top

[F06] 删除文件
来源：http://dxx.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://qqe.sysykeji.top

PHP:  unlink("a.txt");
来源：http://kmh.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://szp.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eoe.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wss.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://dfe.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://eea.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://dtn.fktsv.cn

[F07] 创建目录（含多级）
来源：http://dss.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iyk.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://alr.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jkz.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mxv.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfc.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lhw.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fuv.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://edg.pengpengdd.cyou

[F08] 遍历目录
来源：http://vco.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmi.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fax.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://hus.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://oyo.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyx.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mpe.sysykeji.top

Ruby: Dir.children("dir")
来源：http://ont.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://sso.vehdjk.com

[F09] 获取文件大小
来源：http://tht.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://bpq.epnwcf.com

PHP:  filesize("a.txt");
来源：http://djy.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://nou.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://yxs.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://wfk.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xsx.redwolf501.top

Ruby: File.size("a.txt")
来源：http://elq.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://hkb.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://eap.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://phd.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nwg.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lhh.vehdjk.com

TS:   path.extname("a.txt")
来源：http://vhj.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qhy.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfm.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hnd.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lsg.cqqwz.cn

[F11] 复制与移动文件
来源：http://kku.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://imy.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kcu.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jgr.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgh.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rra.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vgm.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ppl.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nxr.birdmap.top

[F12] CSV 读写
来源：http://fbd.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://isz.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dwc.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://adi.guannengcc.top

TS:   // 同上
来源：http://hnz.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://obn.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://drf.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tsl.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ssd.hesvh.cn

================================================================================
来源：http://ocs.shangyingyoupin.top

G. 面向对象
来源：http://sjy.ivvv.top

================================================================================
来源：http://wwr.jinyuanbaomall.cn

[G01] 定义类
来源：http://qaa.zycfv.cn

Py:   class User: pass
来源：http://umc.shuidangran.top

PHP:  class User {}
来源：http://edg.gzhubu.top

JS:   class User {}
来源：http://zfb.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://jyj.birdmap.top

Java: class User {}
来源：http://nuz.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://ldz.daria6918.cn

Ruby: class User; end
来源：http://ftb.vqdsnc.cn

C#:   class User {}
来源：http://ylh.zhaomingkeji.xyz

[G02] 构造函数
来源：http://nun.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://umx.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://cew.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ygy.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://oou.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://mgc.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://byq.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://xmk.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://ule.yuanzhike.top

[G03] 实例属性
来源：http://bvj.nanxinkj.top

Py:   self.name = "x"
来源：http://jsf.shzxlz.cn

PHP:  public string $name = "x";
来源：http://dzx.tarul.cn

JS:   this.name = "x";
来源：http://iks.ydjk.org.cn

TS:   name: string = "x";
来源：http://jpj.yuanzhike.top

Java: private String name;
来源：http://bbr.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cgn.hcnkem.com

Ruby: @name = "x"
来源：http://ljo.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://vgy.cqqwz.cn

[G04] 定义方法
来源：http://lxn.hcnkem.com

Py:   def greet(self): return self.name
来源：http://yvv.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hoq.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://frc.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://wkw.cheryme.top

Java: String greet() { return name; }
来源：http://fxw.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kzn.mhx1999.top

Ruby: def greet; @name; end
来源：http://meh.yj20258.top

C#:   public string Greet() => Name;
来源：http://qsl.sweek.top

[G05] 继承
来源：http://ivo.tianlin.xyz


<!-- 参考信息 -->