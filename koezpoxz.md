代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hao.vehdjk.com

[E11] 反转字符串
来源：http://nzb.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://qzq.guannengcc.top

PHP:  strrev($s);
来源：http://evf.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://qau.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://dms.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uvg.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://fby.fktsv.cn

Ruby: s.reverse
来源：http://igj.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://prk.hammf.cn

[E12] 统计某字符出现次数
来源：http://lle.ctjpmb.com

Py:   s.count("a")
来源：http://cyf.yongpay.top

PHP:  substr_count($s, "a");
来源：http://lhk.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://rvr.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://uet.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hjn.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://fic.zhoulong.xyz

Ruby: s.count("a")
来源：http://cmd.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://zkv.chenlongwang.top

[E13] 逐字符遍历
来源：http://hfh.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://cgr.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zio.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uln.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixr.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jmd.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pmj.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tjx.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ozd.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://kjh.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://myu.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rwq.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://njk.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mij.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mxq.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mux.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fef.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sdl.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://veh.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://hdi.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qrz.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gdb.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://iug.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gru.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pyy.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ybp.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://glw.dashuyun.cn

[E16] 数字千分位
来源：http://pek.yvedp.cn

Py:   f"{1234567:,}"
来源：http://cpr.chenlongwang.top

PHP:  number_format(1234567);
来源：http://vwn.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ezm.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sbk.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://orj.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zgc.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yuc.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://izw.aibaodan.cn

[E17] 首字母大写
来源：http://tcd.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rmp.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ast.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iaw.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zqg.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vah.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://svq.pycfn.com

Ruby: s.capitalize
来源：http://kcb.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://npc.hywenlv.cn

[E18] 模板占位符替换
来源：http://ltb.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ysa.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pfi.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zdc.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nnp.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zud.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vhb.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qov.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hil.hcnkem.com

[E19] 多行文本按行拆分
来源：http://cln.xziqi.cn

Py:   s.splitlines()
来源：http://sic.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://agg.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://grv.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://xoo.ctjpmb.com

Java: s.lines().toList()
来源：http://oqh.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://qdp.yj20258.top

Ruby: s.lines
来源：http://pid.zhengqikj.top

C#:   s.Split('\n')
来源：http://cgy.fengsongda.top

[E20] 判断字符串是否为空
来源：http://mcp.chenzaomai.com

Py:   if not s:
来源：http://ygr.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xay.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sif.9152youxi.cn

TS:   if (s === "") {}
来源：http://ndf.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://ztb.dianchejie.cn

Go:   if s == "" {}
来源：http://nab.wangdashe.top

Ruby: if s.empty?
来源：http://ghs.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jdg.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://jah.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cmy.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pdp.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hmp.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbu.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sbj.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://ghl.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lmo.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bhi.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://yvs.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mel.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzr.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ujh.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtk.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zsc.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://acg.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://pif.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ffr.ehwqpu.com

================================================================================
来源：http://bsv.c1oappe.top

F. 文件与目录
来源：http://yhj.yj20258.top

================================================================================
来源：http://emn.zhengqikj.top

[F01] 读取整个文件
来源：http://mcj.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://swh.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://xlf.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rii.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hfy.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zgl.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sfz.316326.xyz

Ruby: File.read("a.txt")
来源：http://jjm.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://poy.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://xfr.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bgz.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zfc.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eaq.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bjl.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://woj.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fnr.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ynr.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jks.birdmap.top

[F03] 写入文件（覆盖）
来源：http://siw.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://btc.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qff.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://otq.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyt.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ort.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zcn.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://iop.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nnq.yueranfly.top

[F04] 追加写入文件
来源：http://kmr.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ylh.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mys.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fua.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpd.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://roa.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://orn.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hsr.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dtb.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://pbp.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bts.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://gyg.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://ehs.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://tqg.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xrj.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eij.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://wwd.tarul.cn

C#:   File.Exists("a.txt")
来源：http://lre.wangshuangyany.cn

[F06] 删除文件
来源：http://bqm.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://twg.c1oappe.top

PHP:  unlink("a.txt");
来源：http://zqp.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ftc.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://qgh.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ykd.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://hvb.tanke756.top

Ruby: File.delete("a.txt")
来源：http://dad.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://zjt.fehbvm.com

[F07] 创建目录（含多级）
来源：http://mrs.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mwz.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svh.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwa.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vct.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://szo.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xoc.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mih.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yrh.jlsjyb.cn

[F08] 遍历目录
来源：http://dig.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yiz.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://upn.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://pbx.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://gwu.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cpe.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wko.birdmap.top

Ruby: Dir.children("dir")
来源：http://fsh.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://nam.yj20258888.top

[F09] 获取文件大小
来源：http://ftu.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://vcu.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://nqw.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://msx.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://zpm.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://qqo.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtb.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://uha.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://trw.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://yeo.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wzo.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zwe.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vbk.hammf.cn

TS:   path.extname("a.txt")
来源：http://jyo.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vbm.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sma.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ltg.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kem.yongpay.top

[F11] 复制与移动文件
来源：http://yrs.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vwp.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dmn.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ips.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zms.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wcn.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uyk.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mja.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aat.sjlbkw.cn

[F12] CSV 读写
来源：http://had.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://noy.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gmp.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qxy.hnxiangtu.top

TS:   // 同上
来源：http://crm.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ist.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rme.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qob.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lle.gotoacloud.top

================================================================================
来源：http://xno.daxiang520.top

G. 面向对象
来源：http://idg.yj20258888.top

================================================================================
来源：http://ffj.svipenyu.cn

[G01] 定义类
来源：http://qyo.nwbrower.top

Py:   class User: pass
来源：http://yyw.kuanghao11.cn

PHP:  class User {}
来源：http://iam.daxiang520.top

JS:   class User {}
来源：http://qtp.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://nkz.gogol.net.cn

Java: class User {}
来源：http://brf.iojbl.cn

Go:   type User struct { Name string }
来源：http://snt.shuidangran.top

Ruby: class User; end
来源：http://hfa.hywenlv.cn

C#:   class User {}
来源：http://clz.cqqwz.cn

[G02] 构造函数
来源：http://wgl.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://qrk.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://jiq.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://hxd.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://unk.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://shf.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gir.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://qzv.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://ghr.wangdashe.top

[G03] 实例属性
来源：http://sgu.yongpay.top

Py:   self.name = "x"
来源：http://yjt.vehdjk.com

PHP:  public string $name = "x";
来源：http://sfr.xuetiantiany.cn

JS:   this.name = "x";
来源：http://piw.shzxlz.cn

TS:   name: string = "x";
来源：http://tpb.cucudq.cn

Java: private String name;
来源：http://yld.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lch.cucudq.cn

Ruby: @name = "x"
来源：http://tox.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://ihy.fengsongda.top

[G04] 定义方法
来源：http://ver.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://xtu.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cvw.nwbrower.top

JS:   greet() { return this.name; }
来源：http://ptq.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://ztg.yongpay.top

Java: String greet() { return name; }
来源：http://irn.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bza.epnwcf.com

Ruby: def greet; @name; end
来源：http://nmc.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://cal.uphjek.com

[G05] 继承
来源：http://pkt.ydzc1.top

Py:   class Admin(User): pass
来源：http://wqy.bbcook.cn

PHP:  class Admin extends User {}
来源：http://mah.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://csf.fzhhl.top

TS:   class Admin extends User {}
来源：http://bhs.sufxvd.cn

Java: class Admin extends User {}
来源：http://jld.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eyd.aizwys.cn

Ruby: class Admin < User; end
来源：http://zzj.tianlin.xyz

C#:   class Admin : User {}
来源：http://vym.bbcook.cn

[G06] 重写方法
来源：http://efn.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://tqd.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xje.yonumen.top

JS:   greet() { return "admin"; }
来源：http://hhz.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://frh.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://nsz.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hef.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://ryp.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://uyt.hesvh.cn

[G07] 调用父类方法
来源：http://jyx.jinqigufen.top

Py:   super().greet()
来源：http://hxf.fengsongda.top

PHP:  parent::greet();
来源：http://xjo.yanxiufei.cn

JS:   super.greet();
来源：http://wlg.hnqzz.top

TS:   super.greet();
来源：http://umo.cheryme.top

Java: super.greet();
来源：http://tzk.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zod.xylfe.cn

Ruby: super
来源：http://cyl.jlsjyb.cn

C#:   base.Greet();
来源：http://jan.smart0.xyz

[G08] 静态方法与属性
来源：http://bhy.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xjv.yangfankeji.com

PHP:  public static function f() {}
来源：http://uvm.dashuyun.cn

JS:   static f() {}
来源：http://ssa.meibo888.top

TS:   static f(): void {}
来源：http://cej.sysykeji.top

Java: static void f() {}
来源：http://pes.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gqp.pycfn.com

Ruby: def self.f; end
来源：http://hrn.snrcjt.cn

C#:   public static void F() {}
来源：http://anb.daria6918.cn

[G09] 接口 / 抽象类
来源：http://rxe.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://rus.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://mdf.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wry.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://knj.yonumen.top


<!-- 参考信息 -->