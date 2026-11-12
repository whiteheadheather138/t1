代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nrw.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gtg.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ttk.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gfb.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oup.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://srf.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://buo.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wpc.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eim.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fnu.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ghf.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fgf.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tep.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ofx.smart0.xyz

[E16] 数字千分位
来源：http://vyg.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://cyj.52xcode.cn

PHP:  number_format(1234567);
来源：http://pqq.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://yjj.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bji.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hod.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qxc.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lel.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://fkm.yanxiufei.cn

[E17] 首字母大写
来源：http://qzr.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hya.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://frf.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zwd.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hus.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qss.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dlz.cheryme.top

Ruby: s.capitalize
来源：http://ukh.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aal.jqgfzy.top

[E18] 模板占位符替换
来源：http://agi.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://evz.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iyc.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hsf.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qjk.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://adb.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pvh.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txi.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vxh.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://nzg.fktsv.cn

Py:   s.splitlines()
来源：http://mpy.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nwl.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://qfw.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://uak.yonumen.top

Java: s.lines().toList()
来源：http://ysc.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://saa.fzhhl.top

Ruby: s.lines
来源：http://kaj.fengsongda.top

C#:   s.Split('\n')
来源：http://cre.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://pab.yfazqb.com

Py:   if not s:
来源：http://uis.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aeb.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://orp.havefunace.top

TS:   if (s === "") {}
来源：http://hox.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://jpt.pycfn.com

Go:   if s == "" {}
来源：http://ijq.jlsjyb.cn

Ruby: if s.empty?
来源：http://ahm.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uhf.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://koh.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ttp.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://imu.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wiq.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jug.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://whg.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://mli.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dli.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tsi.shuidangran.top

[E22] 字节长度与字符长度
来源：http://pgo.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qtg.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ccx.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://psz.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ayv.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://scd.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iiq.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://jsz.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sxm.iojbl.cn

================================================================================
来源：http://otz.wangshuangyany.cn

F. 文件与目录
来源：http://jar.hysaishi.cn

================================================================================
来源：http://vui.tarul.cn

[F01] 读取整个文件
来源：http://zuu.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://agb.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://ydj.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yln.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://opw.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vuj.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dkz.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://qmu.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://jdv.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://tys.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vws.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uas.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xex.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwz.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwy.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lch.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sqh.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cdi.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://tna.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vlf.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://izl.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwu.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rva.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xmk.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mxk.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://kdh.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uyl.cqqwz.cn

[F04] 追加写入文件
来源：http://tqh.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ust.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gtm.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lsc.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dud.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wpl.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tsj.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xbm.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lxr.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://nug.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ccz.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://lzc.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://vki.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://nii.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ckr.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sww.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://wnv.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://yxi.birdmap.top

[F06] 删除文件
来源：http://rxs.gzhubu.top

Py:   os.remove("a.txt")
来源：http://ygm.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://sss.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jbe.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sdx.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hjo.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://hud.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://dgk.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://huh.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://sto.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rim.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eyf.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gsk.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjp.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qdd.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://apa.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://egp.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://msl.sxryk.cn

[F08] 遍历目录
来源：http://adr.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wrf.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gso.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://xcv.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://rue.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wpe.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yho.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://ekl.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://ggb.fzhhl.top

[F09] 获取文件大小
来源：http://zzy.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://pca.zycfv.cn

PHP:  filesize("a.txt");
来源：http://cyf.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://htt.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://dsd.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xlo.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wkn.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://xbv.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://sqp.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://hht.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sxg.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vix.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qmf.hammf.cn

TS:   path.extname("a.txt")
来源：http://wbv.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hyv.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iqg.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qzf.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vlb.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://oui.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nta.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpp.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qii.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dye.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wlj.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://noz.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hdn.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nnw.quarkkingdee.top

[F12] CSV 读写
来源：http://ils.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zsn.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kdr.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qms.snrcjt.cn

TS:   // 同上
来源：http://smf.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kuv.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eha.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cuy.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cvs.bjfxy.top

================================================================================
来源：http://ddr.yj202588.top

G. 面向对象
来源：http://cig.xingfuxueyuan.xyz

================================================================================
来源：http://rna.ywan-chungtsiang.top

[G01] 定义类
来源：http://vfs.yuxming.cn

Py:   class User: pass
来源：http://ysd.tarul.cn

PHP:  class User {}
来源：http://wpj.zhongyouzk.top

JS:   class User {}
来源：http://yub.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://jpu.xingfuxueyuan.xyz

Java: class User {}
来源：http://lan.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://amm.hesvh.cn

Ruby: class User; end
来源：http://hun.ppjwa.cn

C#:   class User {}
来源：http://gyl.jinqigufen.top

[G02] 构造函数
来源：http://aep.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wdb.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://erd.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://rba.316326.xyz

TS:   constructor(public name: string) {}
来源：http://ncy.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://stw.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mek.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://xqj.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://rdz.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://xmb.sufxvd.cn

Py:   self.name = "x"
来源：http://vgv.epnwcf.com

PHP:  public string $name = "x";
来源：http://aar.ydjk.org.cn

JS:   this.name = "x";
来源：http://fqo.jyoumei.cn

TS:   name: string = "x";
来源：http://kbf.zhiwuduotai.top

Java: private String name;
来源：http://xva.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gpe.dianchejie.cn

Ruby: @name = "x"
来源：http://lch.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://dtg.yongpay.top

[G04] 定义方法
来源：http://mji.yueranfly.top

Py:   def greet(self): return self.name
来源：http://qeq.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ddl.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://nnn.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://kfc.nanxuanxn.top

Java: String greet() { return name; }
来源：http://yon.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fas.0kj1m.cn

Ruby: def greet; @name; end
来源：http://sit.yj202588.top

C#:   public string Greet() => Name;
来源：http://iow.yonumen.top

[G05] 继承
来源：http://sxw.haohaochexian.top

Py:   class Admin(User): pass
来源：http://aix.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://bnw.nwbrower.top

JS:   class Admin extends User {}
来源：http://ahy.yangfankeji.com

TS:   class Admin extends User {}
来源：http://dwx.yj20258.top

Java: class Admin extends User {}
来源：http://apx.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ece.havefunace.top

Ruby: class Admin < User; end
来源：http://tnv.dashuyun.cn

C#:   class Admin : User {}
来源：http://man.vehdjk.com

[G06] 重写方法
来源：http://iqg.sweek.top

Py:   def greet(self): return "admin"
来源：http://knz.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sus.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://iqq.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://tcq.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://gcb.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vdq.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://mhm.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://wjh.shzxlz.cn

[G07] 调用父类方法
来源：http://nzk.mhx1999.top

Py:   super().greet()
来源：http://lbd.cucudq.cn

PHP:  parent::greet();
来源：http://rpx.chenzaomai.com

JS:   super.greet();
来源：http://trw.c1oappe.top

TS:   super.greet();
来源：http://vra.cqqwz.cn

Java: super.greet();
来源：http://pbk.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ydb.9152youxi.cn

Ruby: super
来源：http://ykc.pengpengdd.cyou

C#:   base.Greet();
来源：http://bup.jlsjyb.cn

[G08] 静态方法与属性
来源：http://juk.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://adu.guowangkeji.top

PHP:  public static function f() {}
来源：http://mwj.ydjk.org.cn

JS:   static f() {}
来源：http://ogo.jianghu66.top

TS:   static f(): void {}
来源：http://ahx.jinghuilouyu.cn

Java: static void f() {}
来源：http://ahh.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xjj.ydjk.org.cn

Ruby: def self.f; end
来源：http://fgk.dashuyun.cn

C#:   public static void F() {}
来源：http://xyd.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://uho.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://tjc.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://xms.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qra.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://mhe.hnqzz.top

Java: interface Shape { double area(); }
来源：http://jpt.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://oyg.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xed.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://eha.yj20258.top

[G10] 访问控制
来源：http://ndl.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://ciy.fengsongda.top

PHP:  public / protected / private
来源：http://xod.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://jtg.ydzc1.top

TS:   public / protected / private
来源：http://dlz.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://chr.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://mxz.hammf.cn

Ruby: public / protected / private
来源：http://pqu.ydzc1.top

C#:   public / protected / private / internal
来源：http://ubr.hammf.cn

[G11] getter / setter
来源：http://jqi.uphjek.com

Py:   @property 与 @x.setter
来源：http://xyq.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ptq.birdmap.top

JS:   get name() { return this._name; }
来源：http://jyd.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://odw.316326.xyz

Java: public String getName() { return name; }
来源：http://vlf.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://nxj.chenlongwang.top

Ruby: attr_accessor :name
来源：http://fyi.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://rvk.yonumen.top

[G12] 对象转字符串
来源：http://nzq.yj202588.top

Py:   def __str__(self): return self.name
来源：http://mlo.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://abw.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://zgq.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://dpc.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://uku.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://vcm.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://chr.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://ffy.yonumen.top

[G13] 判断对象类型
来源：http://fog.zhengqikj.top


<!-- 参考信息 -->