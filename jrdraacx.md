代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://fag.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qts.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://umf.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://vpj.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://vsm.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://stv.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ipg.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mbl.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://als.birdmap.top

[E11] 反转字符串
来源：http://byw.yfazqb.com

Py:   s[::-1]
来源：http://dta.pycfn.com

PHP:  strrev($s);
来源：http://mys.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://mgs.uphjek.com

TS:   [...s].reverse().join("")
来源：http://yvk.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ith.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://swd.jinqigufen.top

Ruby: s.reverse
来源：http://cca.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://xql.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://nwa.yuanzhike.top

Py:   s.count("a")
来源：http://krn.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://psr.ybcxt.top

JS:   s.split("a").length - 1
来源：http://euc.cashguo.top

TS:   s.split("a").length - 1
来源：http://vwq.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzg.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://kdc.xziqi.cn

Ruby: s.count("a")
来源：http://yyg.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://rtn.52xcode.cn

[E13] 逐字符遍历
来源：http://yvk.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://ram.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ydj.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdz.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iqc.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ozk.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uhe.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://syt.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://apa.yonumen.top

[E14] URL 编码与 Base64
来源：http://cve.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wqp.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ync.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mdb.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbr.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ksn.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mkd.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yhf.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cau.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://skd.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fum.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://krs.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wfi.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://dek.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qos.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://foh.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vej.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nru.dianchejie.cn

[E16] 数字千分位
来源：http://chn.ivvv.top

Py:   f"{1234567:,}"
来源：http://nwj.dianchejie.cn

PHP:  number_format(1234567);
来源：http://irj.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kxi.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xme.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ege.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjl.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vmt.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://dlr.zhiwuduotai.top

[E17] 首字母大写
来源：http://iqd.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jgb.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xdq.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://plr.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpb.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rjg.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fhu.vehdjk.com

Ruby: s.capitalize
来源：http://gte.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cfk.chenlongwang.top

[E18] 模板占位符替换
来源：http://moj.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gwf.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vcq.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nuw.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gur.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hns.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uwl.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ovn.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyv.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://pxd.yangfankeji.com

Py:   s.splitlines()
来源：http://zfn.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eop.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://kgh.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://azc.ydzc1.top

Java: s.lines().toList()
来源：http://rxe.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://eeb.andypj.xyz

Ruby: s.lines
来源：http://lmc.daxiang520.top

C#:   s.Split('\n')
来源：http://gzi.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://pvz.hnxiangtu.top

Py:   if not s:
来源：http://wrf.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fmk.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tyv.jqgfzy.top

TS:   if (s === "") {}
来源：http://etn.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://qil.ehwqpu.com

Go:   if s == "" {}
来源：http://cer.shangyingyoupin.top

Ruby: if s.empty?
来源：http://vzf.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jsm.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://dib.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kaf.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypq.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xsw.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zic.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bqs.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://hvp.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qie.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wey.shuidangran.top

[E22] 字节长度与字符长度
来源：http://nwl.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fvy.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yeh.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lar.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnz.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zfl.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oul.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://krp.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pal.hfpthk.cn

================================================================================
来源：http://uvn.yuanzhike.top

F. 文件与目录
来源：http://qgf.jqgfzy.top

================================================================================
来源：http://erh.c1oappe.top

[F01] 读取整个文件
来源：http://uci.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sne.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://sda.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qjn.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yos.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wgd.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mhm.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://pux.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://psq.jianghu66.top

[F02] 逐行读取文件
来源：http://axh.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zrt.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ual.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rmd.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eus.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tcz.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xhc.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hxf.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dlx.birdmap.top

[F03] 写入文件（覆盖）
来源：http://dvk.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ssv.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://upp.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jil.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyk.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ixe.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ola.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://pjw.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dgm.ppjwa.cn

[F04] 追加写入文件
来源：http://ulp.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wda.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ckm.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tfb.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ove.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jdt.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mzb.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oti.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://chz.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://ydb.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iwm.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://juj.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://wan.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://gus.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vsa.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qkt.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://jki.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://jgs.ppjwa.cn

[F06] 删除文件
来源：http://ucz.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://zyh.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://lgg.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://nsl.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://gyy.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zpd.uphjek.com

Go:   os.Remove("a.txt")
来源：http://kom.uphjek.com

Ruby: File.delete("a.txt")
来源：http://xye.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://gpy.yj202588.top

[F07] 创建目录（含多级）
来源：http://alv.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ncq.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cxg.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eds.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fhy.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tcw.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wxo.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hjm.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ism.ybcxt.top

[F08] 遍历目录
来源：http://dpz.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lqy.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tjv.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://jbx.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://ipq.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qpr.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gto.cashguo.top

Ruby: Dir.children("dir")
来源：http://ppz.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://qux.cdnleiting.top

[F09] 获取文件大小
来源：http://sdp.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://pym.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://qie.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://zyj.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://rov.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://scm.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://njn.c1oappe.top

Ruby: File.size("a.txt")
来源：http://wlz.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://rlq.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://nbl.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fak.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bqq.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bfe.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://ylf.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kwj.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mir.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nhx.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ndk.9152youxi.cn

[F11] 复制与移动文件
来源：http://vcu.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jej.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpg.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xps.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fmo.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xql.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rmd.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lvk.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jht.svipenyu.cn

[F12] CSV 读写
来源：http://ksy.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ufz.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tcl.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mfn.9152youxi.cn

TS:   // 同上
来源：http://ozv.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://owd.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nkf.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ltn.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uop.zhaomingkeji.xyz

================================================================================
来源：http://git.guowangkeji.top

G. 面向对象
来源：http://tpb.zhengqikj.top

================================================================================
来源：http://tmy.gaohongyu789.top

[G01] 定义类
来源：http://tet.ydjk.org.cn

Py:   class User: pass
来源：http://bif.yj20258.top

PHP:  class User {}
来源：http://opo.yonumen.top

JS:   class User {}
来源：http://xvo.yonumen.top

TS:   class User { name: string = ""; }
来源：http://urp.wangshuangyany.cn

Java: class User {}
来源：http://auk.yj202588.top

Go:   type User struct { Name string }
来源：http://ijq.tanke756.top

Ruby: class User; end
来源：http://qxr.shzxlz.cn

C#:   class User {}
来源：http://zuz.gaohongyu789.top

[G02] 构造函数
来源：http://odh.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://tcn.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://nop.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://vxp.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://uom.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://sxs.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rph.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qsu.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://gir.tanke756.top

[G03] 实例属性
来源：http://zwz.zdqjudy.top

Py:   self.name = "x"
来源：http://yor.chenzaomai.com

PHP:  public string $name = "x";
来源：http://slc.pycfn.com

JS:   this.name = "x";
来源：http://eib.tian-w.cn

TS:   name: string = "x";
来源：http://hdy.0kj1m.cn

Java: private String name;
来源：http://uee.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lsi.xinyue.icu

Ruby: @name = "x"
来源：http://nah.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://obh.wangdashe.top

[G04] 定义方法
来源：http://hcm.yj202588.top

Py:   def greet(self): return self.name
来源：http://tbd.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ptd.bjfxy.top

JS:   greet() { return this.name; }
来源：http://qpr.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://rcm.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://xod.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://xyv.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://qkt.andypj.xyz

C#:   public string Greet() => Name;
来源：http://kxv.xziqi.cn

[G05] 继承
来源：http://jkg.tian-w.cn

Py:   class Admin(User): pass
来源：http://pss.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://yzt.316326.xyz

JS:   class Admin extends User {}
来源：http://uaf.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://odb.ydzc1.top

Java: class Admin extends User {}
来源：http://ppb.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://myz.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://gdg.tian-w.cn

C#:   class Admin : User {}
来源：http://upk.nanxinkj.top

[G06] 重写方法
来源：http://qhy.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://qme.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kan.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://ynk.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://sny.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sti.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://smc.uphjek.com

Ruby: def greet; "admin"; end
来源：http://qnf.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://peu.9152youxi.cn

[G07] 调用父类方法
来源：http://smx.fzhhl.top

Py:   super().greet()
来源：http://fak.sjlbkw.cn

PHP:  parent::greet();
来源：http://wal.ctjpmb.com

JS:   super.greet();
来源：http://kdv.nanxuanxn.top

TS:   super.greet();
来源：http://tev.havefunace.top

Java: super.greet();
来源：http://zfb.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://prm.ivvv.top

Ruby: super
来源：http://uul.cashguo.top

C#:   base.Greet();
来源：http://mbk.kuanghao11.cn

[G08] 静态方法与属性
来源：http://pad.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dgv.xylfe.cn

PHP:  public static function f() {}
来源：http://hcj.fengsongda.top

JS:   static f() {}
来源：http://gvh.nwbrower.top

TS:   static f(): void {}
来源：http://jlg.yongpay.top

Java: static void f() {}
来源：http://pbh.316326.xyz


<!-- 参考信息 -->