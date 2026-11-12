代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://eke.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mdk.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://ufh.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://elc.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://diw.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rxw.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wsm.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://zkc.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://rns.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://bhs.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sas.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ind.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pro.fengsongda.top

[E11] 反转字符串
来源：http://unq.zycfv.cn

Py:   s[::-1]
来源：http://qlf.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://jeu.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://frj.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://gwr.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lxk.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://lnx.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://zrz.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://wfq.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://kcf.hnqzz.top

Py:   s.count("a")
来源：http://txr.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://ysr.yj202588.top

JS:   s.split("a").length - 1
来源：http://jul.nwbrower.top

TS:   s.split("a").length - 1
来源：http://fgi.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cww.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://tgw.iojbl.cn

Ruby: s.count("a")
来源：http://jzh.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://xem.jqgufenzy.top

[E13] 逐字符遍历
来源：http://uwu.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://pck.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yft.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jzg.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://yad.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lss.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aar.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qyr.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://spd.ydzc1.top

[E14] URL 编码与 Base64
来源：http://zgd.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vtc.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ois.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zdu.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ghk.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qhd.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zkj.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hep.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xqn.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://uwp.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tae.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://epe.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gsn.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://dwv.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hdh.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lpo.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gpi.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgp.nwbrower.top

[E16] 数字千分位
来源：http://pro.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://efw.jinqigufen.top

PHP:  number_format(1234567);
来源：http://eiu.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://esx.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ckk.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aax.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zqb.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fam.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://fwo.andypj.xyz

[E17] 首字母大写
来源：http://cft.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cmj.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bxy.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spq.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yen.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mjg.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://meg.havefunace.top

Ruby: s.capitalize
来源：http://jgl.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qmc.mhx1999.top

[E18] 模板占位符替换
来源：http://aic.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iqt.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ets.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hnz.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fde.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cgk.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rln.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://umq.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xxj.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://qcn.xuanzx.com

Py:   s.splitlines()
来源：http://tzf.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fsk.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://pvh.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://vnb.ydzc1.top

Java: s.lines().toList()
来源：http://vag.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://iqq.hfpthk.cn

Ruby: s.lines
来源：http://hfc.hnxiangtu.top

C#:   s.Split('\n')
来源：http://cfz.hcnkem.com

[E20] 判断字符串是否为空
来源：http://wbf.xuanzx.com

Py:   if not s:
来源：http://pdb.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zqg.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dml.yonumen.top

TS:   if (s === "") {}
来源：http://brk.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://wnu.havefunace.top

Go:   if s == "" {}
来源：http://fau.yj20258888.top

Ruby: if s.empty?
来源：http://axo.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nvs.dianchejie.cn

[E21] 超长截断加省略号
来源：http://tla.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wgd.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cky.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eml.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lta.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://htr.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://lef.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbe.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jbj.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://sre.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qvk.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zft.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtn.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gmo.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhf.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qlx.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://ase.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yns.zhongyouzk.top

================================================================================
来源：http://bwb.yonumen.top

F. 文件与目录
来源：http://xah.cucudq.cn

================================================================================
来源：http://vfy.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://kdu.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kti.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://vkp.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rmd.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vic.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pac.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mwv.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://wun.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://qml.yuxming.cn

[F02] 逐行读取文件
来源：http://fcg.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lyq.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://btv.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://suv.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bre.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uhx.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dta.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://twn.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ohz.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://inm.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kvn.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jva.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jae.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osw.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lct.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gts.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://dax.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://grh.316326.xyz

[F04] 追加写入文件
来源：http://gkj.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uzw.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ddk.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xaz.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://edb.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hcl.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lif.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ipq.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xqv.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://cls.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zgh.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://avo.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://xjp.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://etf.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://fnw.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sac.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://baj.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://wyw.ydzc1.top

[F06] 删除文件
来源：http://pcy.smart0.xyz

Py:   os.remove("a.txt")
来源：http://bns.ydzc1.top

PHP:  unlink("a.txt");
来源：http://ydl.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://bxm.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://grp.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jde.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://sgz.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://mbi.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://pmc.redwolf501.top

[F07] 创建目录（含多级）
来源：http://rsb.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hoe.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ewx.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pxq.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jsi.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uej.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iyl.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ljs.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://glp.uphjek.com

[F08] 遍历目录
来源：http://zeb.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ccw.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oil.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://awz.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://goe.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sge.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qfk.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://xbk.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://ylm.daria6918.cn

[F09] 获取文件大小
来源：http://whc.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://zui.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://cma.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://kub.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://kif.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://obq.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xtt.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://oie.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://wqz.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://sln.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twl.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eks.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ppx.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://dzz.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kby.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tnq.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lwq.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zrr.dianchejie.cn

[F11] 复制与移动文件
来源：http://lpv.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cbo.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yqq.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkp.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nnd.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kpe.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mro.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mqs.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kiz.cashguo.top

[F12] CSV 读写
来源：http://wmq.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tiu.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xtz.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fom.hnxiangtu.top

TS:   // 同上
来源：http://xmn.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gsa.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oqk.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wdt.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://onf.hfpthk.cn

================================================================================
来源：http://qzf.zdqjudy.top

G. 面向对象
来源：http://xgh.jlsjyb.cn

================================================================================
来源：http://iio.havefunace.top

[G01] 定义类
来源：http://fvw.hfpthk.cn

Py:   class User: pass
来源：http://ejj.haohaochexian.top

PHP:  class User {}
来源：http://vhz.hfpthk.cn

JS:   class User {}
来源：http://pxl.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://bdf.yonumen.top

Java: class User {}
来源：http://zrd.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://lco.cucudq.cn

Ruby: class User; end
来源：http://rqa.hammf.cn

C#:   class User {}
来源：http://xkt.tarul.cn

[G02] 构造函数
来源：http://nba.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://fep.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://hiw.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://kqh.316326.xyz

TS:   constructor(public name: string) {}
来源：http://vxt.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://ptt.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ohp.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://xck.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://who.yj20258888.top

[G03] 实例属性
来源：http://lfq.nanxinkj.top

Py:   self.name = "x"
来源：http://kgj.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://icq.andypj.xyz

JS:   this.name = "x";
来源：http://lru.jinqigfzy.top

TS:   name: string = "x";
来源：http://hyj.yangfankeji.com

Java: private String name;
来源：http://jzd.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lpf.xinyue.icu

Ruby: @name = "x"
来源：http://vwv.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://jcq.guowangkeji.top

[G04] 定义方法
来源：http://oad.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://ivm.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sut.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://hjw.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://oac.hnqzz.top

Java: String greet() { return name; }
来源：http://tva.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vlg.c1oappe.top

Ruby: def greet; @name; end
来源：http://jhi.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://gjb.snrcjt.cn

[G05] 继承
来源：http://pyr.ehwqpu.com

Py:   class Admin(User): pass
来源：http://oit.yj20258.top

PHP:  class Admin extends User {}
来源：http://bda.cqqwz.cn

JS:   class Admin extends User {}
来源：http://mwc.hesvh.cn

TS:   class Admin extends User {}
来源：http://fai.yj20258888.top

Java: class Admin extends User {}
来源：http://sjf.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gdc.uphjek.com

Ruby: class Admin < User; end
来源：http://hjc.hesvh.cn

C#:   class Admin : User {}
来源：http://zqs.hcnkem.com

[G06] 重写方法
来源：http://jam.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://mgh.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wpg.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://vyd.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://gmt.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://yig.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://boa.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://qgf.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://txs.sufxvd.cn

[G07] 调用父类方法
来源：http://lsk.jqgufenzy.top

Py:   super().greet()
来源：http://jco.yangfankeji.com

PHP:  parent::greet();
来源：http://nvy.shzxlz.cn

JS:   super.greet();
来源：http://uhs.ivvv.top

TS:   super.greet();
来源：http://cen.wangdashe.top

Java: super.greet();
来源：http://goj.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mun.wangshuangyany.cn

Ruby: super
来源：http://xmi.chenjidiqi.icu

C#:   base.Greet();
来源：http://lpp.hfpthk.cn

[G08] 静态方法与属性
来源：http://fat.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nca.hywenlv.cn


<!-- 参考信息 -->