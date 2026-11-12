代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vas.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://skd.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vdk.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jkd.birdmap.top

[E14] URL 编码与 Base64
来源：http://gmg.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://udt.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pnp.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bqd.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://snp.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hug.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xcr.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tdx.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yss.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://orq.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wks.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ahd.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nfl.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fmn.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mls.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qof.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xbw.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jeq.xylfe.cn

[E16] 数字千分位
来源：http://cbm.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://ltu.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://pup.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aku.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nfh.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nwg.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mwp.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tak.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://kmm.dianchejie.cn

[E17] 首字母大写
来源：http://luz.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://azn.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ukp.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kxv.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rct.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knz.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bjy.xziqi.cn

Ruby: s.capitalize
来源：http://kvr.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://clv.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://lgk.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rzn.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uen.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cyo.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ogc.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bqs.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://awz.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lyk.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fwi.yueranfly.top

[E19] 多行文本按行拆分
来源：http://aqr.hfpthk.cn

Py:   s.splitlines()
来源：http://cyt.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mxr.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://vkt.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://drl.zhoulong.xyz

Java: s.lines().toList()
来源：http://oxf.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://xjz.dashuyun.cn

Ruby: s.lines
来源：http://laf.yongpay.top

C#:   s.Split('\n')
来源：http://eei.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://buj.hysaishi.cn

Py:   if not s:
来源：http://cgh.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lby.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dse.ydjk.org.cn

TS:   if (s === "") {}
来源：http://kem.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://lns.pengpengdd.cyou

Go:   if s == "" {}
来源：http://fjx.ydzc1.top

Ruby: if s.empty?
来源：http://uty.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://och.yvedp.cn

[E21] 超长截断加省略号
来源：http://dcc.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mxv.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bel.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uuj.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yow.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tss.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://wth.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fbt.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vsh.xylfe.cn

[E22] 字节长度与字符长度
来源：http://nmw.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://joz.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygn.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mov.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uwr.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yya.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rmm.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://zbk.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qfi.ydzc1.top

================================================================================
来源：http://ejz.uphjek.com

F. 文件与目录
来源：http://yoi.guannengcc.top

================================================================================
来源：http://khc.yanxiufei.cn

[F01] 读取整个文件
来源：http://vyp.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bko.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://hbr.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xfo.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tcn.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cez.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rct.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://fby.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://hxw.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://ego.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvd.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bra.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vyl.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ske.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kdf.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dfu.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wqg.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gmm.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://xsw.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mvl.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://unz.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvu.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysd.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rrv.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgh.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://gix.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://upw.xinyue.icu

[F04] 追加写入文件
来源：http://jvs.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fjs.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dxg.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yyj.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpz.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blr.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rfr.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xow.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pjo.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://jxf.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdd.sweek.top

PHP:  file_exists("a.txt");
来源：http://lxm.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://rgw.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://acn.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pny.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://azs.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://yot.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://myn.chenzaomai.com

[F06] 删除文件
来源：http://fwm.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://byt.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://qiy.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://xol.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://tin.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bbw.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://ybl.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://tkb.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://sua.ybcxt.top

[F07] 创建目录（含多级）
来源：http://drn.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://diz.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://utw.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhg.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjf.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wbw.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ehx.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fps.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://opq.ydzc1.top

[F08] 遍历目录
来源：http://srv.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wcs.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qds.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://hhn.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://jci.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hud.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://idm.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://gjd.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://pgp.dashuyun.cn

[F09] 获取文件大小
来源：http://fcg.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://tdu.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://ahq.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://jut.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://nlg.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://alq.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://asy.sweek.top

Ruby: File.size("a.txt")
来源：http://qqx.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://jps.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://pab.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://snv.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnf.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qlw.tarul.cn

TS:   path.extname("a.txt")
来源：http://usc.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ahx.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fhy.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vus.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kus.yangfankeji.com

[F11] 复制与移动文件
来源：http://xmk.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yqc.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xix.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmv.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrv.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hhy.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vzj.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pmz.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iwp.mhx1999.top

[F12] CSV 读写
来源：http://lct.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dee.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eet.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pzf.zhongyouzk.top

TS:   // 同上
来源：http://oob.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pup.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugt.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pxd.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rtp.gotoacloud.top

================================================================================
来源：http://qfx.yvedp.cn

G. 面向对象
来源：http://dkr.chenlongwang.top

================================================================================
来源：http://lfs.ydzc1.top

[G01] 定义类
来源：http://trz.meibo888.top

Py:   class User: pass
来源：http://sks.yuxming.cn

PHP:  class User {}
来源：http://gby.ydjk.org.cn

JS:   class User {}
来源：http://qlg.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://dlv.svipenyu.cn

Java: class User {}
来源：http://meb.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://xuo.sjlbkw.cn

Ruby: class User; end
来源：http://bds.hywenlv.cn

C#:   class User {}
来源：http://rzv.tanke756.top

[G02] 构造函数
来源：http://bwf.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://qhh.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://qhv.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mzf.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://cnd.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://jay.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mtp.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://dxr.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://wrb.guowangkeji.top

[G03] 实例属性
来源：http://owr.jinqigfzy.top

Py:   self.name = "x"
来源：http://uln.chenzaomai.com

PHP:  public string $name = "x";
来源：http://cco.xylfe.cn

JS:   this.name = "x";
来源：http://ofq.jinqigufen.top

TS:   name: string = "x";
来源：http://dla.fengsongda.top

Java: private String name;
来源：http://aav.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nkc.dashuyun.cn

Ruby: @name = "x"
来源：http://pry.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://map.xziqi.cn

[G04] 定义方法
来源：http://jro.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://ioy.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fcc.zycfv.cn

JS:   greet() { return this.name; }
来源：http://khi.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://rww.vqdsnc.cn

Java: String greet() { return name; }
来源：http://luc.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gtv.cheryme.top

Ruby: def greet; @name; end
来源：http://obz.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://ggg.aizwys.cn

[G05] 继承
来源：http://rgr.zycfv.cn

Py:   class Admin(User): pass
来源：http://jay.nwbrower.top

PHP:  class Admin extends User {}
来源：http://jjz.wangdashe.top

JS:   class Admin extends User {}
来源：http://dsf.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://nbk.hesvh.cn

Java: class Admin extends User {}
来源：http://viy.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xei.zdqjudy.top

Ruby: class Admin < User; end
来源：http://wel.daria6918.cn

C#:   class Admin : User {}
来源：http://iov.hnqzz.top

[G06] 重写方法
来源：http://bnr.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://lxj.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://llo.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://ttm.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://dce.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://uyb.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bnn.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://nhr.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://cjw.gotoacloud.top

[G07] 调用父类方法
来源：http://kpf.shzxlz.cn

Py:   super().greet()
来源：http://jhv.hywenlv.cn

PHP:  parent::greet();
来源：http://ckg.yangfankeji.com

JS:   super.greet();
来源：http://bex.nwbrower.top

TS:   super.greet();
来源：http://dhv.hammf.cn

Java: super.greet();
来源：http://ndx.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gin.0kj1m.cn

Ruby: super
来源：http://htj.hnxiangtu.top

C#:   base.Greet();
来源：http://lxr.zhengqikj.top

[G08] 静态方法与属性
来源：http://fdn.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nni.shzxlz.cn

PHP:  public static function f() {}
来源：http://yhn.zycfv.cn

JS:   static f() {}
来源：http://ldp.0kj1m.cn

TS:   static f(): void {}
来源：http://yqo.yfazqb.com

Java: static void f() {}
来源：http://ujl.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://sjt.dashuyun.cn

Ruby: def self.f; end
来源：http://xlf.meibo888.top

C#:   public static void F() {}
来源：http://hok.birdmap.top

[G09] 接口 / 抽象类
来源：http://ghy.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://eht.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://djf.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zsa.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://iis.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://sps.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://ybm.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ioh.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://qga.52xcode.cn

[G10] 访问控制
来源：http://aln.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://fuh.aibaodan.cn

PHP:  public / protected / private
来源：http://oqv.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://kcn.jinqigufen.top

TS:   public / protected / private
来源：http://mva.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://dci.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ucx.meibo888.top

Ruby: public / protected / private
来源：http://jtk.cucudq.cn

C#:   public / protected / private / internal
来源：http://jyc.smart0.xyz

[G11] getter / setter
来源：http://anp.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://iuv.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jbr.daria6918.cn

JS:   get name() { return this._name; }
来源：http://hhc.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://frp.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://bre.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ejk.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://lsg.vehdjk.com

C#:   public string Name { get; set; }
来源：http://yys.pycfn.com

[G12] 对象转字符串
来源：http://adj.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://nwj.fengsongda.top


<!-- 参考信息 -->