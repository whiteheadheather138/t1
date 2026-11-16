代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://xpf.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yqh.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://twz.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://okl.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://ypb.fzhhl.top

Java: String.format("%03d", 7)
来源：http://uky.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://avt.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ino.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://feu.dashuyun.cn

[E11] 反转字符串
来源：http://qde.chenzaomai.com

Py:   s[::-1]
来源：http://fhj.jqgfzy.top

PHP:  strrev($s);
来源：http://fwe.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://vah.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://uha.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://yiw.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://aoj.gotoacloud.top

Ruby: s.reverse
来源：http://rzi.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://ine.yj20258.top

[E12] 统计某字符出现次数
来源：http://fvm.hongshengwenyu.top

Py:   s.count("a")
来源：http://ntj.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://nny.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://ixb.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://uym.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yar.meibo888.top

Go:   strings.Count(s, "a")
来源：http://nas.jianghu66.top

Ruby: s.count("a")
来源：http://feg.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://mwd.hnxiangtu.top

[E13] 逐字符遍历
来源：http://ejh.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://mss.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dcv.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://duu.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aes.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ist.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kvg.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mrt.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vle.ivvv.top

[E14] URL 编码与 Base64
来源：http://kll.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jsu.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lgt.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lri.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://deg.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ila.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zcg.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ofr.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oyu.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://uwj.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bbf.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yvf.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uej.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tqf.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ajr.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wvb.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pkz.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eao.zhengqikj.top

[E16] 数字千分位
来源：http://cdl.c1oappe.top

Py:   f"{1234567:,}"
来源：http://gaf.tian-w.cn

PHP:  number_format(1234567);
来源：http://fpi.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jqx.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ixe.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ndl.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://klx.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sky.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://jpg.jiagoushi.top

[E17] 首字母大写
来源：http://yjm.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qcr.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kgi.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vtr.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eqs.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pqa.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eax.hnqzz.top

Ruby: s.capitalize
来源：http://jxs.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jeb.zdqjudy.top

[E18] 模板占位符替换
来源：http://uue.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dkz.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bho.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ghl.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zpv.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfo.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aox.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dfc.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://efs.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://aii.sjlbkw.cn

Py:   s.splitlines()
来源：http://qpk.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://isg.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://lvu.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://ouj.sjlbkw.cn

Java: s.lines().toList()
来源：http://tkz.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://pxb.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://cwl.jyoumei.cn

C#:   s.Split('\n')
来源：http://imu.havefunace.top

[E20] 判断字符串是否为空
来源：http://qxy.havefunace.top

Py:   if not s:
来源：http://flw.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://efc.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sdh.ydjk.org.cn

TS:   if (s === "") {}
来源：http://enw.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://ceb.zhengqikj.top

Go:   if s == "" {}
来源：http://kwz.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://hft.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hvx.yuxming.cn

[E21] 超长截断加省略号
来源：http://pxq.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qrf.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sit.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rzo.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pai.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hkn.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://tdc.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zuq.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ecn.yuxming.cn

[E22] 字节长度与字符长度
来源：http://coi.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://owv.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fhg.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqd.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wiu.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hoy.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fpr.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://vbm.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zqw.chenzaomai.com

================================================================================
来源：http://akq.xuanzx.com

F. 文件与目录
来源：http://orz.gzhubu.top

================================================================================
来源：http://zom.zhijiandao.cn

[F01] 读取整个文件
来源：http://aqr.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://grv.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://rnx.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kpb.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvr.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rms.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ecj.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://wge.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://bdo.hywenlv.cn

[F02] 逐行读取文件
来源：http://sqa.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dxb.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pna.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwy.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzk.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sqg.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jow.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ens.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ahx.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://olu.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vjy.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://avi.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yko.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fjm.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfe.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vky.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://lfn.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qsp.nanxuanxn.top

[F04] 追加写入文件
来源：http://pcw.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dhb.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rby.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vzl.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bnw.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xxm.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zgg.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vvm.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mbn.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://vpt.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyz.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://auc.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://nud.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://bxb.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zqm.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vmz.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://jvr.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://ezn.hesvh.cn

[F06] 删除文件
来源：http://zac.iojbl.cn

Py:   os.remove("a.txt")
来源：http://ein.shuidangran.top

PHP:  unlink("a.txt");
来源：http://eny.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://ubj.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://kls.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pbh.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://kzj.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://frd.birdmap.top

C#:   File.Delete("a.txt");
来源：http://nls.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://wdm.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pnm.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cjg.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://egg.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yfb.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sin.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ywn.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ouq.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jif.ehwqpu.com

[F08] 遍历目录
来源：http://dho.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hgy.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fdx.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://htv.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://fcb.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lja.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lnf.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://lvl.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://hde.shuidangran.top

[F09] 获取文件大小
来源：http://dtn.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://wcu.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://hvn.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://cqx.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://znp.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qil.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nhq.fzhhl.top

Ruby: File.size("a.txt")
来源：http://cgr.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://yqf.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://oio.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jme.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://smn.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://moc.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://ixc.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pgq.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gba.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://foz.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aho.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://qqq.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eam.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cax.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tcj.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpv.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kol.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rkr.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fkv.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iit.yvedp.cn

[F12] CSV 读写
来源：http://fnr.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nyg.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ncw.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qry.epnwcf.com

TS:   // 同上
来源：http://rwd.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phq.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kzj.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nit.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fwx.vehdjk.com

================================================================================
来源：http://pzo.ydzc1.top

G. 面向对象
来源：http://sng.fzhhl.top

================================================================================
来源：http://sxd.hysaishi.cn

[G01] 定义类
来源：http://fsk.havefunace.top

Py:   class User: pass
来源：http://rsx.dashuyun.cn

PHP:  class User {}
来源：http://swm.gaohongyu789.top

JS:   class User {}
来源：http://rfn.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://hln.9152youxi.cn

Java: class User {}
来源：http://oup.hfpthk.cn

Go:   type User struct { Name string }
来源：http://bzt.gzhubu.top

Ruby: class User; end
来源：http://npy.xinyue.icu

C#:   class User {}
来源：http://msa.vqdsnc.cn

[G02] 构造函数
来源：http://joc.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://ihr.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://nyz.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://btd.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://czx.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://atn.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://now.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://joc.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://jmg.nanxuanxn.top

[G03] 实例属性
来源：http://jry.hcnkem.com

Py:   self.name = "x"
来源：http://ybp.guowangkeji.top

PHP:  public string $name = "x";
来源：http://yrw.9152youxi.cn

JS:   this.name = "x";
来源：http://vuk.jqgufenzy.top

TS:   name: string = "x";
来源：http://hfp.ppjwa.cn

Java: private String name;
来源：http://zzh.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mir.vqdsnc.cn

Ruby: @name = "x"
来源：http://pwc.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://biq.zhongyouzk.top

[G04] 定义方法
来源：http://inl.316326.xyz

Py:   def greet(self): return self.name
来源：http://ozj.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nci.yueranfly.top

JS:   greet() { return this.name; }
来源：http://dfp.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://tfz.ppjwa.cn

Java: String greet() { return name; }
来源：http://mit.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pmh.yongpay.top

Ruby: def greet; @name; end
来源：http://drq.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://vjv.yueranfly.top

[G05] 继承
来源：http://qnx.chenzaomai.com

Py:   class Admin(User): pass
来源：http://wum.sxryk.cn

PHP:  class Admin extends User {}
来源：http://jee.yj20258888.top

JS:   class Admin extends User {}
来源：http://noa.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://qoz.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://ran.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://idi.ehwqpu.com

Ruby: class Admin < User; end
来源：http://rrr.zhijiandao.cn

C#:   class Admin : User {}
来源：http://cio.hnqzz.top

[G06] 重写方法
来源：http://usz.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://vlm.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://njd.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://clb.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://wpr.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://ouj.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qoc.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://vrg.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://nht.zhijiandao.cn

[G07] 调用父类方法
来源：http://txv.svipenyu.cn

Py:   super().greet()
来源：http://zse.zhongyouzk.top

PHP:  parent::greet();
来源：http://sil.jinyuanbaomall.cn

JS:   super.greet();
来源：http://vir.dianchejie.cn

TS:   super.greet();
来源：http://uux.ydzc1.top

Java: super.greet();
来源：http://bwy.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nqr.epnwcf.com

Ruby: super
来源：http://lyv.haohaochexian.top

C#:   base.Greet();
来源：http://wso.sysykeji.top

[G08] 静态方法与属性
来源：http://srw.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rdw.zdbjq.cn

PHP:  public static function f() {}
来源：http://nfr.meibo888.top

JS:   static f() {}
来源：http://liz.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://mti.vqdsnc.cn

Java: static void f() {}
来源：http://irq.9152youxi.cn


<!-- 参考信息 -->