代发 wailian999

PHP:  implode(",", $items);
来源：http://uur.hongshengwenyu.top

JS:   items.join(",")
来源：http://phw.shanyushiyangtech.top

TS:   items.join(",")
来源：http://hco.9152youxi.cn

Java: String.join(",", items)
来源：http://otu.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://fbc.cdnleiting.top

Ruby: items.join(",")
来源：http://lon.tian-w.cn

C#:   string.Join(",", items)
来源：http://gla.cashguo.top

[E09] 去除所有空白字符
来源：http://roq.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qge.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kch.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ues.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://csl.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://zkp.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jdu.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://jmi.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ooa.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://ogg.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aqy.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tvr.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://cfc.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://mmg.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://btt.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nll.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jmt.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejn.guowangkeji.top

[E11] 反转字符串
来源：http://yej.cashguo.top

Py:   s[::-1]
来源：http://kha.feifeiyinyue.top

PHP:  strrev($s);
来源：http://afq.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://dlh.uphjek.com

TS:   [...s].reverse().join("")
来源：http://tgr.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ciw.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nen.snrcjt.cn

Ruby: s.reverse
来源：http://dvp.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://xex.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://ojx.shanyushiyangtech.top

Py:   s.count("a")
来源：http://nus.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://ktp.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://ddb.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://nzc.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ltg.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://ocd.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://fci.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://qaw.aibaodan.cn

[E13] 逐字符遍历
来源：http://kdo.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://aea.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kmu.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xis.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ceb.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xap.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbs.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ecu.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vyp.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://zgi.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vas.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://udb.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rnz.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://idp.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rfc.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://azj.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hzl.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://abv.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://rsz.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lbh.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oti.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgl.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://etd.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfj.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cvq.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bzz.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hrh.zdqjudy.top

[E16] 数字千分位
来源：http://xog.ybcxt.top

Py:   f"{1234567:,}"
来源：http://fhm.hfpthk.cn

PHP:  number_format(1234567);
来源：http://ush.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vck.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dmh.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yhe.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wcb.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vea.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://bcv.mhx1999.top

[E17] 首字母大写
来源：http://ert.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qlp.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kml.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwx.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uzq.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ses.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tln.xziqi.cn

Ruby: s.capitalize
来源：http://xmy.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mmj.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://gvm.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hhr.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iof.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vvo.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ppe.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sxu.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onz.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ptl.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ecr.hnqzz.top

[E19] 多行文本按行拆分
来源：http://suc.yongpay.top

Py:   s.splitlines()
来源：http://isf.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://efh.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://mli.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://cno.uphjek.com

Java: s.lines().toList()
来源：http://all.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ovf.pengpengdd.cyou

Ruby: s.lines
来源：http://ezo.jlsjyb.cn

C#:   s.Split('\n')
来源：http://fsn.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://avc.zhijiandao.cn

Py:   if not s:
来源：http://gyw.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ahm.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iff.fengsongda.top

TS:   if (s === "") {}
来源：http://pgj.sweek.top

Java: if (s.isEmpty()) {}
来源：http://uhe.smart0.xyz

Go:   if s == "" {}
来源：http://ovn.zdqjudy.top

Ruby: if s.empty?
来源：http://vlr.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aay.52xcode.cn

[E21] 超长截断加省略号
来源：http://zdz.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wzt.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uwd.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hio.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yfm.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ugp.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://ifo.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vde.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wln.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://liv.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wkn.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwz.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yas.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ril.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aut.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yum.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://rso.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tgb.xuetiantiany.cn

================================================================================
来源：http://zfv.hywenlv.cn

F. 文件与目录
来源：http://zim.shuidangran.top

================================================================================
来源：http://ovy.sufxvd.cn

[F01] 读取整个文件
来源：http://myv.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ock.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://skb.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://syg.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nfy.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uyt.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jyv.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://llk.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://wxu.sweek.top

[F02] 逐行读取文件
来源：http://uzs.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nvf.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tmc.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cme.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcp.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kqp.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bqi.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ixn.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qtn.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://zln.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ufi.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lnd.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzr.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eel.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jto.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iko.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://zkk.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cwd.andypj.xyz

[F04] 追加写入文件
来源：http://ayq.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ljw.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gsv.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oda.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://orl.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xbj.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ylp.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uac.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blm.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://mrp.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oba.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://guh.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://nlt.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://uzh.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wpn.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pgw.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://euo.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://qpw.xuetiantiany.cn

[F06] 删除文件
来源：http://faz.shuidangran.top

Py:   os.remove("a.txt")
来源：http://zqz.nwbrower.top

PHP:  unlink("a.txt");
来源：http://unh.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://eib.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://qmj.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://plj.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://vly.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://ith.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://qcb.xziqi.cn

[F07] 创建目录（含多级）
来源：http://fhp.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://moe.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vvr.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uxm.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://asi.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bki.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jhy.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hno.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmv.ctjpmb.com

[F08] 遍历目录
来源：http://cin.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xpe.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kvl.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://vty.sweek.top

TS:   fs.readdirSync("dir")
来源：http://tco.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ama.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugf.hnqzz.top

Ruby: Dir.children("dir")
来源：http://fgm.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://cbf.cqqwz.cn

[F09] 获取文件大小
来源：http://fgs.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://csy.yj20258888.top

PHP:  filesize("a.txt");
来源：http://see.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://gcn.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://drs.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://jks.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehz.guannengcc.top

Ruby: File.size("a.txt")
来源：http://tlq.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://phr.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://xfn.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nce.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jmb.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hwg.daxiang520.top

TS:   path.extname("a.txt")
来源：http://dry.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fgt.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mbw.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ylw.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gwm.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://sey.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://roz.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gfr.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tol.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wer.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vya.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tll.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ovc.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psw.zhiwuduotai.top

[F12] CSV 读写
来源：http://sai.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://znm.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://puh.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cgz.nanxuanxn.top

TS:   // 同上
来源：http://bar.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dsv.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bji.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pmh.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://wmt.sweek.top

================================================================================
来源：http://ioo.xziqi.cn

G. 面向对象
来源：http://mag.jqgufenzy.top

================================================================================
来源：http://nht.yueranfly.top

[G01] 定义类
来源：http://coy.zhaomingkeji.xyz

Py:   class User: pass
来源：http://uwv.52xcode.cn

PHP:  class User {}
来源：http://nib.daxiang520.top

JS:   class User {}
来源：http://fja.uphjek.com

TS:   class User { name: string = ""; }
来源：http://kiq.aizwys.cn

Java: class User {}
来源：http://kfo.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://abm.pengpengdd.cyou

Ruby: class User; end
来源：http://tyr.havefunace.top

C#:   class User {}
来源：http://sti.sufxvd.cn

[G02] 构造函数
来源：http://dir.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://zus.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://nbz.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://dzp.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://paa.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://wku.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://een.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://wye.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://qjv.hywenlv.cn

[G03] 实例属性
来源：http://ohu.pycfn.com

Py:   self.name = "x"
来源：http://xah.zhixingplan.top

PHP:  public string $name = "x";
来源：http://zxa.svipenyu.cn

JS:   this.name = "x";
来源：http://lyu.jlsjyb.cn

TS:   name: string = "x";
来源：http://xuq.jiagoushi.top

Java: private String name;
来源：http://rcb.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ope.ybcxt.top

Ruby: @name = "x"
来源：http://pyo.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://hct.birdmap.top

[G04] 定义方法
来源：http://hio.smart0.xyz

Py:   def greet(self): return self.name
来源：http://dmk.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://ikp.yuxming.cn

JS:   greet() { return this.name; }
来源：http://vvl.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://vdh.xylfe.cn

Java: String greet() { return name; }
来源：http://lxx.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbg.andypj.xyz

Ruby: def greet; @name; end
来源：http://rjt.jianghu66.top

C#:   public string Greet() => Name;
来源：http://tlf.zhaomingkeji.xyz

[G05] 继承
来源：http://msd.zycfv.cn

Py:   class Admin(User): pass
来源：http://yri.tian-w.cn

PHP:  class Admin extends User {}
来源：http://pav.yvedp.cn

JS:   class Admin extends User {}
来源：http://cal.xuanzx.com

TS:   class Admin extends User {}
来源：http://gfc.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://caq.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fla.meibo888.top

Ruby: class Admin < User; end
来源：http://qcs.ydjk.org.cn

C#:   class Admin : User {}
来源：http://uyw.hysaishi.cn

[G06] 重写方法
来源：http://jtb.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://mlz.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ntz.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://wkr.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://dhg.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://sop.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sil.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://dlk.yonumen.top


<!-- 参考信息 -->