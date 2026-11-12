代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://tue.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://urc.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hgn.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zzj.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://rfq.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ksq.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cmk.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://uoe.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://kuu.cheryme.top

Java: String.format("%03d", 7)
来源：http://wsd.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qrc.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovh.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://chk.dianchejie.cn

[E11] 反转字符串
来源：http://btj.andypj.xyz

Py:   s[::-1]
来源：http://arz.haohaochexian.top

PHP:  strrev($s);
来源：http://qne.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://pbq.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://abu.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://lvn.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ozr.epnwcf.com

Ruby: s.reverse
来源：http://mgh.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xcf.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://wyx.nanxinkj.top

Py:   s.count("a")
来源：http://iwc.birdmap.top

PHP:  substr_count($s, "a");
来源：http://sle.cucudq.cn

JS:   s.split("a").length - 1
来源：http://kmt.epnwcf.com

TS:   s.split("a").length - 1
来源：http://vka.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://krz.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://spn.yj20258888.top

Ruby: s.count("a")
来源：http://ipg.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://uts.hfpthk.cn

[E13] 逐字符遍历
来源：http://gef.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://oli.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lau.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nav.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dkx.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://arf.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://izp.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wig.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mmx.yvedp.cn

[E14] URL 编码与 Base64
来源：http://ocl.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uyo.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldk.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qac.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://plo.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tpe.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rdp.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://luq.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vyo.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://wcu.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://apx.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zmk.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mov.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://det.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://krb.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tig.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ntv.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ryz.hongshengwenyu.top

[E16] 数字千分位
来源：http://olf.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://oji.cqqwz.cn

PHP:  number_format(1234567);
来源：http://mgv.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zno.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ihf.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ajh.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qjp.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://amp.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://yde.gotoacloud.top

[E17] 首字母大写
来源：http://ucu.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bkg.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mxq.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bbd.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lie.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mrn.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://edq.ehwqpu.com

Ruby: s.capitalize
来源：http://tlr.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojm.havefunace.top

[E18] 模板占位符替换
来源：http://odi.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rdw.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mwx.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://amm.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://byy.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://drk.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://krs.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hps.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jdz.redwolf501.top

[E19] 多行文本按行拆分
来源：http://lvo.guowangkeji.top

Py:   s.splitlines()
来源：http://hdf.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qgt.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://fuf.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://zit.yj202588.top

Java: s.lines().toList()
来源：http://xlx.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://ass.fktsv.cn

Ruby: s.lines
来源：http://vnp.kuanghao11.cn

C#:   s.Split('\n')
来源：http://vwo.tarul.cn

[E20] 判断字符串是否为空
来源：http://pnu.hywenlv.cn

Py:   if not s:
来源：http://syf.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jau.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://drd.jqgfzy.top

TS:   if (s === "") {}
来源：http://hld.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://uhv.haohaochexian.top

Go:   if s == "" {}
来源：http://tgn.mhx1999.top

Ruby: if s.empty?
来源：http://wtg.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ojo.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://sue.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itn.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://foy.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uhl.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsf.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rox.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://dbt.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://phh.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mjg.yj20258.top

[E22] 字节长度与字符长度
来源：http://ffq.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lus.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hof.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gne.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sho.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://saj.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ihw.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://pdd.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hds.mhx1999.top

================================================================================
来源：http://lxc.xylfe.cn

F. 文件与目录
来源：http://uvt.fzhhl.top

================================================================================
来源：http://sfb.zdqjudy.top

[F01] 读取整个文件
来源：http://ktt.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sbt.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://rrb.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://suw.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://urt.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ptw.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://joe.sysykeji.top

Ruby: File.read("a.txt")
来源：http://ugf.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://npz.sxryk.cn

[F02] 逐行读取文件
来源：http://zdq.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uat.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gty.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oij.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ads.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://brq.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rcq.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tjf.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bhn.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://bli.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkr.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://cgr.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gaa.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uny.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jys.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://psq.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://jmu.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://scq.cucudq.cn

[F04] 追加写入文件
来源：http://wwl.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://clo.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kuj.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ote.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xfh.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mvj.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ozl.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rqy.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hkg.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://imk.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jhl.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://key.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://aea.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://aky.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mgg.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ymy.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://ctn.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://ahd.jyoumei.cn

[F06] 删除文件
来源：http://auu.fengsongda.top

Py:   os.remove("a.txt")
来源：http://dgu.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://scy.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rbi.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xkp.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ewt.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://dek.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://hvp.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://jlr.vehdjk.com

[F07] 创建目录（含多级）
来源：http://aww.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lcl.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ofz.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nin.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nry.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqq.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lli.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lbi.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uyv.zdbjq.cn

[F08] 遍历目录
来源：http://iud.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xxh.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bqh.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://gdq.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://cwz.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jlc.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zxq.guannengcc.top

Ruby: Dir.children("dir")
来源：http://tfi.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://iaw.xziqi.cn

[F09] 获取文件大小
来源：http://lrm.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://wyx.yfazqb.com

PHP:  filesize("a.txt");
来源：http://any.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://non.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://ovj.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://zju.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cuf.fengsongda.top

Ruby: File.size("a.txt")
来源：http://how.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ckn.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://gcf.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xov.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nhq.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dgd.xylfe.cn

TS:   path.extname("a.txt")
来源：http://hoz.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wpy.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whz.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kdp.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qrt.cucudq.cn

[F11] 复制与移动文件
来源：http://gwf.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://edh.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wlr.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zfc.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpv.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kvm.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://usu.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vzc.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vou.ydjk.org.cn

[F12] CSV 读写
来源：http://rca.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oim.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnt.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nkh.gzhubu.top

TS:   // 同上
来源：http://uvx.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yuy.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://doi.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://afi.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vwp.shangyingyoupin.top

================================================================================
来源：http://rog.havefunace.top

G. 面向对象
来源：http://dfy.dianchejie.cn

================================================================================
来源：http://vzd.9152youxi.cn

[G01] 定义类
来源：http://mco.jlsjyb.cn

Py:   class User: pass
来源：http://giq.birdmap.top

PHP:  class User {}
来源：http://mao.ydjk.org.cn

JS:   class User {}
来源：http://suz.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://itj.cashguo.top

Java: class User {}
来源：http://qrj.sysykeji.top

Go:   type User struct { Name string }
来源：http://gpl.tian-w.cn

Ruby: class User; end
来源：http://raj.andypj.xyz

C#:   class User {}
来源：http://rwk.hysaishi.cn

[G02] 构造函数
来源：http://xbi.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://oxw.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://jsh.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://gqi.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://dhx.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://ivk.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sde.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://qla.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://gnk.havefunace.top

[G03] 实例属性
来源：http://ijd.yj202588.top

Py:   self.name = "x"
来源：http://hxo.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://kag.c1oappe.top

JS:   this.name = "x";
来源：http://utp.fzhhl.top

TS:   name: string = "x";
来源：http://elc.daria6918.cn

Java: private String name;
来源：http://ecu.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cdm.haohaochexian.top

Ruby: @name = "x"
来源：http://gkd.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://xdx.meibo888.top

[G04] 定义方法
来源：http://quk.birdmap.top

Py:   def greet(self): return self.name
来源：http://fjf.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dhn.hesvh.cn

JS:   greet() { return this.name; }
来源：http://kht.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://jtp.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://syv.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aea.nanxinkj.top

Ruby: def greet; @name; end
来源：http://zwb.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://lrz.jinqigfzy.top

[G05] 继承
来源：http://lyy.fehbvm.com

Py:   class Admin(User): pass
来源：http://jcy.zycfv.cn

PHP:  class Admin extends User {}
来源：http://utl.zycfv.cn

JS:   class Admin extends User {}
来源：http://qkp.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://bpt.uphjek.com

Java: class Admin extends User {}
来源：http://ysg.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dmg.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://osq.jinqigfzy.top

C#:   class Admin : User {}
来源：http://xng.zhengqikj.top

[G06] 重写方法
来源：http://beb.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://ivo.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://npk.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://srm.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://fcd.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://bfr.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xex.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://amh.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://ksm.cucudq.cn

[G07] 调用父类方法
来源：http://qku.fehbvm.com

Py:   super().greet()
来源：http://mey.cdnleiting.top

PHP:  parent::greet();
来源：http://rlk.nanxuanxn.top

JS:   super.greet();
来源：http://okp.ydzc1.top

TS:   super.greet();
来源：http://knw.shzxlz.cn

Java: super.greet();
来源：http://vhh.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aml.feifeiyinyue.top

Ruby: super
来源：http://dvv.guowangkeji.top

C#:   base.Greet();
来源：http://psj.havefunace.top

[G08] 静态方法与属性
来源：http://jii.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tji.yueranfly.top


<!-- 参考信息 -->