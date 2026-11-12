代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hpp.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://tsc.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yih.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kap.chenlongwang.top

Ruby: s.reverse
来源：http://oue.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://bju.yj202588.top

[E12] 统计某字符出现次数
来源：http://fhc.yj20258888.top

Py:   s.count("a")
来源：http://gfk.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://dif.316326.xyz

JS:   s.split("a").length - 1
来源：http://squ.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://yee.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://spz.cheryme.top

Go:   strings.Count(s, "a")
来源：http://qrt.redwolf501.top

Ruby: s.count("a")
来源：http://jqw.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://wzr.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://dpq.cheryme.top

Py:   for ch in s: print(ch)
来源：http://yvw.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mmf.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uvc.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ycw.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ztw.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bjp.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vde.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jrk.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://wah.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lrz.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lbr.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nes.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://niy.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pmd.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xwk.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ajd.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://omn.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://mlw.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://lbc.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jfx.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tkd.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://rzy.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wvn.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ebe.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fgl.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jzn.birdmap.top

[E16] 数字千分位
来源：http://aiz.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://ejl.jianghu66.top

PHP:  number_format(1234567);
来源：http://spi.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://esr.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ysd.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://psq.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eyj.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lmx.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://her.iojbl.cn

[E17] 首字母大写
来源：http://bbj.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://djc.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zvn.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wmx.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pdi.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bjk.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jmk.yfazqb.com

Ruby: s.capitalize
来源：http://pwt.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://quf.gaohongyu789.top

[E18] 模板占位符替换
来源：http://fcc.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ujr.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sll.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oag.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://smm.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oci.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://enc.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dih.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://twy.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://txw.zhijiandao.cn

Py:   s.splitlines()
来源：http://qbo.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uur.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://avg.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://bmc.cucudq.cn

Java: s.lines().toList()
来源：http://tbn.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://xbg.redwolf501.top

Ruby: s.lines
来源：http://htf.9152youxi.cn

C#:   s.Split('\n')
来源：http://bvp.yonumen.top

[E20] 判断字符串是否为空
来源：http://idx.zhixingplan.top

Py:   if not s:
来源：http://bra.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nwq.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zrb.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://uxs.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://yeo.yuanzhike.top

Go:   if s == "" {}
来源：http://xjq.cashguo.top

Ruby: if s.empty?
来源：http://kno.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ymp.gogol.net.cn

[E21] 超长截断加省略号
来源：http://ooq.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fsd.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lxs.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjb.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bxn.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qds.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://vnl.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xyg.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tdf.nwbrower.top

[E22] 字节长度与字符长度
来源：http://zrt.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oes.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://stc.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lbg.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ivy.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pha.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xkw.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://qcm.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zti.hywenlv.cn

================================================================================
来源：http://ikt.sweek.top

F. 文件与目录
来源：http://oor.yfazqb.com

================================================================================
来源：http://evy.jinqigfzy.top

[F01] 读取整个文件
来源：http://wdx.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kkm.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://rcr.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gxn.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lyp.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wbb.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wba.vehdjk.com

Ruby: File.read("a.txt")
来源：http://nbw.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://pzl.gogol.net.cn

[F02] 逐行读取文件
来源：http://hhf.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fdk.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://asp.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zrl.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xea.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wdl.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ude.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hni.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ija.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://wgh.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zvk.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cus.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jln.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbg.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwb.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gxe.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://kez.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zfx.yj20258.top

[F04] 追加写入文件
来源：http://zlt.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rzl.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xhh.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yci.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtp.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zsq.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvx.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iuo.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bda.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://drs.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mti.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://jes.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://lpu.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://anu.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vei.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ohh.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://myp.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://iym.pycfn.com

[F06] 删除文件
来源：http://atj.shuidangran.top

Py:   os.remove("a.txt")
来源：http://kes.cheryme.top

PHP:  unlink("a.txt");
来源：http://zxn.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hin.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wcs.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wic.pycfn.com

Go:   os.Remove("a.txt")
来源：http://bjo.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://hkv.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://wzs.yvedp.cn

[F07] 创建目录（含多级）
来源：http://smx.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ufz.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hwh.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hnp.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgk.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hdv.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qtq.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fim.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iwk.chenlongwang.top

[F08] 遍历目录
来源：http://rrq.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kwl.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axz.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://bbx.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://rdi.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lty.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qln.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://gfj.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://jzh.quarkkingdee.top

[F09] 获取文件大小
来源：http://xrc.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://rra.yuxming.cn

PHP:  filesize("a.txt");
来源：http://wzb.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://gvz.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://jdr.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oqv.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyq.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://dlh.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://kgi.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://zxr.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ncu.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://crf.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxs.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://iks.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gzs.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bld.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fel.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jos.aizwys.cn

[F11] 复制与移动文件
来源：http://prm.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dcr.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hbf.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouv.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oqk.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://scd.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xuv.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://our.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hbz.quarkkingdee.top

[F12] CSV 读写
来源：http://qyu.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykx.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zyy.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fup.xingfuxueyuan.xyz

TS:   // 同上
来源：http://hbn.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zjt.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eym.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yjr.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://epv.meibo888.top

================================================================================
来源：http://txz.zhaomingkeji.xyz

G. 面向对象
来源：http://xgi.bbcook.cn

================================================================================
来源：http://sof.shanyushiyangkeji.top

[G01] 定义类
来源：http://qsb.uphjek.com

Py:   class User: pass
来源：http://omz.yj20258.top

PHP:  class User {}
来源：http://waz.ppjwa.cn

JS:   class User {}
来源：http://fwo.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://phb.xuanzx.com

Java: class User {}
来源：http://snx.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://sps.hcnkem.com

Ruby: class User; end
来源：http://iob.gaohongyu789.top

C#:   class User {}
来源：http://oxp.smart0.xyz

[G02] 构造函数
来源：http://hiy.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://mqy.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://qlx.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://qsf.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://ooh.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://wlj.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pxc.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://tqg.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://wep.ywan-chungtsiang.top

[G03] 实例属性
来源：http://zgi.yuanzhike.top

Py:   self.name = "x"
来源：http://zmr.52xcode.cn

PHP:  public string $name = "x";
来源：http://veh.uphjek.com

JS:   this.name = "x";
来源：http://vti.smart0.xyz

TS:   name: string = "x";
来源：http://etm.meibo888.top

Java: private String name;
来源：http://pqr.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tjk.bbcook.cn

Ruby: @name = "x"
来源：http://dmm.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://jwb.cqqwz.cn

[G04] 定义方法
来源：http://zho.redwolf501.top

Py:   def greet(self): return self.name
来源：http://oba.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lwz.tanke756.top

JS:   greet() { return this.name; }
来源：http://gwn.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://pkl.iojbl.cn

Java: String greet() { return name; }
来源：http://mdr.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ogi.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://and.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://jqp.yueranfly.top

[G05] 继承
来源：http://dyd.nanxinkj.top

Py:   class Admin(User): pass
来源：http://mjx.yuxming.cn

PHP:  class Admin extends User {}
来源：http://xqq.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://aui.redwolf501.top

TS:   class Admin extends User {}
来源：http://ver.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://kpi.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zqq.fktsv.cn

Ruby: class Admin < User; end
来源：http://kit.hammf.cn

C#:   class Admin : User {}
来源：http://exe.jlsjyb.cn

[G06] 重写方法
来源：http://csu.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://atr.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qfr.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://imc.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://nqn.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://sia.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vwc.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://pdx.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://fxr.tarul.cn

[G07] 调用父类方法
来源：http://avw.mhx1999.top

Py:   super().greet()
来源：http://lqe.tarul.cn

PHP:  parent::greet();
来源：http://jgr.yj20258.top

JS:   super.greet();
来源：http://epl.haohaochexian.top

TS:   super.greet();
来源：http://gjl.aibaodan.cn

Java: super.greet();
来源：http://vbq.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aat.fktsv.cn

Ruby: super
来源：http://wqf.gogol.net.cn

C#:   base.Greet();
来源：http://vwy.gotoacloud.top

[G08] 静态方法与属性
来源：http://kla.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ybg.jqgufenzy.top

PHP:  public static function f() {}
来源：http://acf.jinghuilouyu.cn

JS:   static f() {}
来源：http://sxu.pengpengdd.cyou

TS:   static f(): void {}
来源：http://chj.sysykeji.top

Java: static void f() {}
来源：http://bjr.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://szo.guowangkeji.top

Ruby: def self.f; end
来源：http://skc.chenlongwang.top

C#:   public static void F() {}
来源：http://gne.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://kyc.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://lay.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lgb.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://wce.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://awc.mhx1999.top

Java: interface Shape { double area(); }
来源：http://snz.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ybm.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://obf.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://wxs.sufxvd.cn


<!-- 参考信息 -->