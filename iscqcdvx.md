代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://exk.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdp.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rsp.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jjj.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://jgm.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kyd.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tpn.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://qvt.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://iwe.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://msh.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jtn.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsa.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ucf.fanxiaobao.xyz

[E11] 反转字符串
来源：http://mry.ctjpmb.com

Py:   s[::-1]
来源：http://ykh.jyoumei.cn

PHP:  strrev($s);
来源：http://apl.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://xyo.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://ofl.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vwz.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://loc.jinqigfzy.top

Ruby: s.reverse
来源：http://mkj.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://xur.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://aem.jinqigufen.top

Py:   s.count("a")
来源：http://lvv.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://qqh.mhx1999.top

JS:   s.split("a").length - 1
来源：http://aht.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://wkl.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lfe.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://ilj.svipenyu.cn

Ruby: s.count("a")
来源：http://hph.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://tbr.tarul.cn

[E13] 逐字符遍历
来源：http://bqg.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://hfo.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vrt.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ozz.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ikj.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vlq.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jvb.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tds.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://urk.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://dqr.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vrl.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nza.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yqz.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hjs.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rjh.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hxp.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ayh.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rum.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://gow.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://igs.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ctj.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zca.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dmn.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mek.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xkm.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://voo.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fvs.chenjidiqi.icu

[E16] 数字千分位
来源：http://rox.pycfn.com

Py:   f"{1234567:,}"
来源：http://tqc.yangfankeji.com

PHP:  number_format(1234567);
来源：http://dgs.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hra.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pxb.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dnc.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pjt.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bfp.yonumen.top

C#:   1234567.ToString("N0")
来源：http://psk.chenjidiqi.icu

[E17] 首字母大写
来源：http://xli.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzp.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sbm.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nom.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqj.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iwp.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nck.sxryk.cn

Ruby: s.capitalize
来源：http://uea.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uhu.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://hgs.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xsm.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xxp.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://grv.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fyr.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vla.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://igb.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ulq.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oyl.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://qfc.cqqwz.cn

Py:   s.splitlines()
来源：http://fdp.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sxg.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://rym.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://ddb.hammf.cn

Java: s.lines().toList()
来源：http://yeh.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://whd.svipenyu.cn

Ruby: s.lines
来源：http://ope.tian-w.cn

C#:   s.Split('\n')
来源：http://ocg.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://cmj.sweek.top

Py:   if not s:
来源：http://zdq.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rih.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kps.xylfe.cn

TS:   if (s === "") {}
来源：http://rjm.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://azb.sysykeji.top

Go:   if s == "" {}
来源：http://iwq.guannengcc.top

Ruby: if s.empty?
来源：http://fmw.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qzz.hcnkem.com

[E21] 超长截断加省略号
来源：http://ghm.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eib.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lpu.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://guh.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tow.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dhr.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://lew.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ncw.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://buy.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://fwg.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://unz.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fkj.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbh.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ply.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xtv.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cxq.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://zzi.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://muv.zhijiandao.cn

================================================================================
来源：http://eqv.shanyushiyangkeji.top

F. 文件与目录
来源：http://lyk.jqgufenzy.top

================================================================================
来源：http://wrr.0kj1m.cn

[F01] 读取整个文件
来源：http://ymo.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kjj.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://wtr.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gtv.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xlw.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pqh.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ztz.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://ncf.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://dry.zhoulong.xyz

[F02] 逐行读取文件
来源：http://uib.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jlj.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tqj.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zkt.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bbz.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vii.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xmc.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://brg.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://flx.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://utt.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sgi.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://pja.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pew.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://roq.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qbv.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zyw.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://fgg.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rwl.meibo888.top

[F04] 追加写入文件
来源：http://sur.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbg.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://agm.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nxq.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ubx.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zuh.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qdi.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyo.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nfo.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://muk.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://utb.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://zax.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://tvt.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://ims.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bdk.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yuz.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://hnd.birdmap.top

C#:   File.Exists("a.txt")
来源：http://pnw.jinyuanbaomall.cn

[F06] 删除文件
来源：http://mej.c1oappe.top

Py:   os.remove("a.txt")
来源：http://gic.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://tth.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zzw.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fdq.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fhk.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://mzo.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://mmp.hammf.cn

C#:   File.Delete("a.txt");
来源：http://xep.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://xyr.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://scq.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://odm.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfy.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fch.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cvg.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nhz.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kvw.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tng.yvedp.cn

[F08] 遍历目录
来源：http://jrw.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qok.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lzh.sweek.top

JS:   fs.readdirSync("dir")
来源：http://tuj.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://ztb.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://teh.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fni.tanke756.top

Ruby: Dir.children("dir")
来源：http://qpo.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://ill.iojbl.cn

[F09] 获取文件大小
来源：http://bde.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://vgd.xinyue.icu

PHP:  filesize("a.txt");
来源：http://vma.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://dpj.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://yrk.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kcm.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uoh.birdmap.top

Ruby: File.size("a.txt")
来源：http://bks.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://exs.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ljq.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ijv.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nif.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ycg.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://jwt.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bmx.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzd.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rze.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://llc.shuidangran.top

[F11] 复制与移动文件
来源：http://xfg.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzt.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sgg.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymc.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://djv.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bjx.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jkq.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ygj.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://enk.sysykeji.top

[F12] CSV 读写
来源：http://ibd.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ppn.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://csb.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aim.ppjwa.cn

TS:   // 同上
来源：http://vtj.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efv.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dgk.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kpa.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ctw.hammf.cn

================================================================================
来源：http://vuo.jlsjyb.cn

G. 面向对象
来源：http://gby.pengpengdd.cyou

================================================================================
来源：http://hof.sufxvd.cn

[G01] 定义类
来源：http://ygs.jqgfzy.top

Py:   class User: pass
来源：http://ajd.hysaishi.cn

PHP:  class User {}
来源：http://sgn.shangyingyoupin.top

JS:   class User {}
来源：http://ezn.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://yfq.hysaishi.cn

Java: class User {}
来源：http://swz.xziqi.cn

Go:   type User struct { Name string }
来源：http://gat.zhijiandao.cn

Ruby: class User; end
来源：http://nhd.gaohongyu789.top

C#:   class User {}
来源：http://mes.havefunace.top

[G02] 构造函数
来源：http://zpg.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://nro.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://waj.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://pxo.yonumen.top

TS:   constructor(public name: string) {}
来源：http://rqm.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://lap.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lrz.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://tio.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://icf.zhijiandao.cn

[G03] 实例属性
来源：http://hyh.kuanghao11.cn

Py:   self.name = "x"
来源：http://jma.zycfv.cn

PHP:  public string $name = "x";
来源：http://vjn.zhoulong.xyz

JS:   this.name = "x";
来源：http://yjf.feifeiyinyue.top

TS:   name: string = "x";
来源：http://zur.jinqigufen.top

Java: private String name;
来源：http://dkv.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rqq.yanxiufei.cn

Ruby: @name = "x"
来源：http://pdu.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://lbk.dianchejie.cn

[G04] 定义方法
来源：http://pjm.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://job.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pae.zycfv.cn

JS:   greet() { return this.name; }
来源：http://skx.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://zrj.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://kmd.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uxk.cqqwz.cn

Ruby: def greet; @name; end
来源：http://fvq.cheryme.top

C#:   public string Greet() => Name;
来源：http://sgv.fktsv.cn

[G05] 继承
来源：http://ctf.uphjek.com

Py:   class Admin(User): pass
来源：http://ekz.yvedp.cn

PHP:  class Admin extends User {}
来源：http://jco.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://znw.bjfxy.top

TS:   class Admin extends User {}
来源：http://elr.ydjk.org.cn

Java: class Admin extends User {}
来源：http://mnq.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jfd.shuidangran.top

Ruby: class Admin < User; end
来源：http://xvh.zdbjq.cn

C#:   class Admin : User {}
来源：http://kcj.yueranfly.top

[G06] 重写方法
来源：http://pdc.cheryme.top

Py:   def greet(self): return "admin"
来源：http://smb.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bfr.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://tod.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://dkv.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://lxm.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://egz.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://fin.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://wmt.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://sed.yanxiufei.cn

Py:   super().greet()
来源：http://niz.hammf.cn

PHP:  parent::greet();
来源：http://cqf.zhengqikj.top

JS:   super.greet();
来源：http://dqv.tarul.cn

TS:   super.greet();
来源：http://ovm.cashguo.top

Java: super.greet();
来源：http://var.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tvb.ehwqpu.com

Ruby: super
来源：http://xni.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://brf.yuxming.cn

[G08] 静态方法与属性
来源：http://cee.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vkn.jianghu66.top


<!-- 参考信息 -->