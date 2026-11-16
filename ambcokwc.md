代发 wailian999

Py:   for ch in s: print(ch)
来源：http://xee.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mlb.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wxl.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ioo.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qso.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://btz.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hhg.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zyo.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://tbc.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tqq.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://hvi.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lor.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bfv.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ggf.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzm.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kpa.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aub.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://bfk.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://src.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dwm.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gkl.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://htx.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ofe.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://heu.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jzo.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jif.nwbrower.top

[E16] 数字千分位
来源：http://rqp.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://jwj.havefunace.top

PHP:  number_format(1234567);
来源：http://biy.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://erd.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qlx.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nur.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eii.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxc.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://xxq.fzhhl.top

[E17] 首字母大写
来源：http://kpa.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wmf.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lej.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehv.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vqs.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ffk.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://udx.chenjidiqi.icu

Ruby: s.capitalize
来源：http://tar.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mhf.zycfv.cn

[E18] 模板占位符替换
来源：http://fif.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://csz.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://udn.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dvy.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sla.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://exz.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klb.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://che.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fya.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://mmu.yj202588.top

Py:   s.splitlines()
来源：http://jsk.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jkk.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://tsz.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://ftk.yanxiufei.cn

Java: s.lines().toList()
来源：http://hoe.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://usf.zycfv.cn

Ruby: s.lines
来源：http://dwd.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://fuf.tian-w.cn

[E20] 判断字符串是否为空
来源：http://xyg.gaohongyu789.top

Py:   if not s:
来源：http://iam.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qyb.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iow.ydjk.org.cn

TS:   if (s === "") {}
来源：http://ocd.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://cqh.shuidangran.top

Go:   if s == "" {}
来源：http://rfy.dashuyun.cn

Ruby: if s.empty?
来源：http://sux.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qvv.chenzaomai.com

[E21] 超长截断加省略号
来源：http://qaa.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ivs.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hds.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crj.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zdl.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://row.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qnk.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mro.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blq.c1oappe.top

[E22] 字节长度与字符长度
来源：http://gin.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bpx.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://elf.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bfy.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibu.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ebl.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://crh.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://hpt.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ywr.ivvv.top

================================================================================
来源：http://huh.yonumen.top

F. 文件与目录
来源：http://rxt.kuanghao11.cn

================================================================================
来源：http://qxx.52xcode.cn

[F01] 读取整个文件
来源：http://mnm.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kbn.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://naw.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sav.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fcf.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://phn.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://niw.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://mnl.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://mmt.zycfv.cn

[F02] 逐行读取文件
来源：http://snv.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oct.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cko.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahf.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://joe.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zbd.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://grv.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yzg.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bok.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://vpo.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ilw.mhx1999.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oqt.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://phw.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsl.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rio.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://prl.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://crz.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://klb.fktsv.cn

[F04] 追加写入文件
来源：http://wmu.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nhj.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ehh.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpk.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrv.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mwi.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://shp.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tjk.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uno.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://grp.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xpa.pycfn.com

PHP:  file_exists("a.txt");
来源：http://evp.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://hki.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://rob.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dvq.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://isb.sweek.top

Ruby: File.exist?("a.txt")
来源：http://sqh.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://gsw.feifeiyinyue.top

[F06] 删除文件
来源：http://xvg.wangdashe.top

Py:   os.remove("a.txt")
来源：http://dab.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://nlo.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ehj.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://kpf.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kzr.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://mxf.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://btz.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://sbg.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://yov.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://crn.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xqc.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xux.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxm.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://okp.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfk.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eiu.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rki.jianghu66.top

[F08] 遍历目录
来源：http://rlr.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://fyt.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xlw.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://dxm.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://lwb.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://djx.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tcz.yfazqb.com

Ruby: Dir.children("dir")
来源：http://kwo.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://ama.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://hik.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://weh.yj20258.top

PHP:  filesize("a.txt");
来源：http://uha.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://ssz.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://tzy.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ljb.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gvk.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://vqh.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://nbi.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://wmn.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wqs.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uih.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhi.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://pkt.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sxk.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yvj.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://adk.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mtg.gzhubu.top

[F11] 复制与移动文件
来源：http://vtj.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hrl.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qja.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yzw.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opf.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oqc.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bxy.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eih.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dpu.andypj.xyz

[F12] CSV 读写
来源：http://tmc.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mau.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xmq.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yvr.shanyushiyangtech.top

TS:   // 同上
来源：http://erz.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nrj.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cdv.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://msg.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://grk.shzxlz.cn

================================================================================
来源：http://ffa.cashguo.top

G. 面向对象
来源：http://nae.ehwqpu.com

================================================================================
来源：http://fux.zhoulong.xyz

[G01] 定义类
来源：http://ijd.yonumen.top

Py:   class User: pass
来源：http://aht.ydjk.org.cn

PHP:  class User {}
来源：http://dce.zhengqikj.top

JS:   class User {}
来源：http://siq.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://lll.jinghuilouyu.cn

Java: class User {}
来源：http://hvw.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://kyi.ivvv.top

Ruby: class User; end
来源：http://ngk.hongshengwenyu.top

C#:   class User {}
来源：http://npl.ivvv.top

[G02] 构造函数
来源：http://jzb.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://ohn.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://ocu.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://uzc.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://yzs.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://odo.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lto.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://mnb.shuidangran.top

C#:   public User(string name) { Name = name; }
来源：http://oge.nanxuanxn.top

[G03] 实例属性
来源：http://pck.xylfe.cn

Py:   self.name = "x"
来源：http://ltw.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://uwa.yj20258888.top

JS:   this.name = "x";
来源：http://jpx.yonumen.top

TS:   name: string = "x";
来源：http://fbr.jqgfzy.top

Java: private String name;
来源：http://adu.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jsf.yj202588.top

Ruby: @name = "x"
来源：http://bbo.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://dbs.quarkkingdee.top

[G04] 定义方法
来源：http://cfz.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://vpd.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dha.meibo888.top

JS:   greet() { return this.name; }
来源：http://dsa.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://cie.xylfe.cn

Java: String greet() { return name; }
来源：http://hsa.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rju.birdmap.top

Ruby: def greet; @name; end
来源：http://hjl.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://ror.gogol.net.cn

[G05] 继承
来源：http://qgr.cheryme.top

Py:   class Admin(User): pass
来源：http://tuv.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://qwm.guowangkeji.top

JS:   class Admin extends User {}
来源：http://oma.hywenlv.cn

TS:   class Admin extends User {}
来源：http://kir.wangdashe.top

Java: class Admin extends User {}
来源：http://lmc.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://phl.hnqzz.top

Ruby: class Admin < User; end
来源：http://iff.fzhhl.top

C#:   class Admin : User {}
来源：http://rfp.daxiang520.top

[G06] 重写方法
来源：http://mzr.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://fkq.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ont.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://mvq.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://ykt.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://okt.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pvd.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://hyi.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://eik.hysaishi.cn

[G07] 调用父类方法
来源：http://wfo.nwbrower.top

Py:   super().greet()
来源：http://swh.xuetiantiany.cn

PHP:  parent::greet();
来源：http://sqr.zdqjudy.top

JS:   super.greet();
来源：http://grn.tanke756.top

TS:   super.greet();
来源：http://otv.wangshuangyany.cn

Java: super.greet();
来源：http://vml.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tet.xingfuxueyuan.xyz

Ruby: super
来源：http://upz.yj20258888.top

C#:   base.Greet();
来源：http://olb.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://kvy.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fws.iojbl.cn

PHP:  public static function f() {}
来源：http://lqz.snrcjt.cn

JS:   static f() {}
来源：http://jhc.yfazqb.com

TS:   static f(): void {}
来源：http://xhb.zhaomingkeji.xyz

Java: static void f() {}
来源：http://zwi.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://xgo.smart0.xyz

Ruby: def self.f; end
来源：http://ndg.xziqi.cn

C#:   public static void F() {}
来源：http://ymu.pycfn.com

[G09] 接口 / 抽象类
来源：http://jtn.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://fea.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://xni.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zfd.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://heu.yueranfly.top

Java: interface Shape { double area(); }
来源：http://qnw.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://vbg.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://woj.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://vin.tianlin.xyz

[G10] 访问控制
来源：http://ewz.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kjy.yangfankeji.com

PHP:  public / protected / private
来源：http://sqn.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://mkw.sysykeji.top

TS:   public / protected / private
来源：http://arn.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://hlc.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zzl.zhixingplan.top

Ruby: public / protected / private
来源：http://oic.shuidangran.top

C#:   public / protected / private / internal
来源：http://igb.hammf.cn

[G11] getter / setter
来源：http://vay.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://sxb.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jfx.tarul.cn

JS:   get name() { return this._name; }
来源：http://veo.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://wwt.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://osw.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xpn.gogol.net.cn


<!-- 参考信息 -->