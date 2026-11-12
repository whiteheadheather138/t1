代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bja.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajk.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pkp.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cuo.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://syy.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://tdn.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vpj.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tcg.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://daj.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rxo.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qjx.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmf.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwt.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://msh.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://szl.havefunace.top

Py:   f"{1234567:,}"
来源：http://bfa.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://wou.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zjd.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ykg.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eqz.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://enr.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jrj.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://xef.hysaishi.cn

[E17] 首字母大写
来源：http://srl.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://prl.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://hym.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjw.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukk.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bla.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://plq.chenjidiqi.icu

Ruby: s.capitalize
来源：http://mxr.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nay.tianlin.xyz

[E18] 模板占位符替换
来源：http://xzo.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pqu.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hsm.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rpq.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yrj.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kto.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gqb.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mpu.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jmx.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://wef.ybcxt.top

Py:   s.splitlines()
来源：http://fpx.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tee.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://yww.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://ylc.c1oappe.top

Java: s.lines().toList()
来源：http://rln.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://xjb.jianghu66.top

Ruby: s.lines
来源：http://fek.zhijiandao.cn

C#:   s.Split('\n')
来源：http://kaw.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://cno.guowangkeji.top

Py:   if not s:
来源：http://hut.zdbjq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xwm.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wpg.jinqigfzy.top

TS:   if (s === "") {}
来源：http://bkw.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://zfp.zhongyouzk.top

Go:   if s == "" {}
来源：http://urr.kuanghao11.cn

Ruby: if s.empty?
来源：http://vnv.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kms.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://iwj.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://icz.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xfx.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dix.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://smp.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwa.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://egi.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kkp.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fjw.yonumen.top

[E22] 字节长度与字符长度
来源：http://odz.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://plv.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kfs.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bbl.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wgz.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bkj.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ycs.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://gku.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kwt.cheryme.top

================================================================================
来源：http://csc.smart0.xyz

F. 文件与目录
来源：http://jsm.9152youxi.cn

================================================================================
来源：http://crg.shuidangran.top

[F01] 读取整个文件
来源：http://ium.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gpk.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://wae.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fxr.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://asf.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nif.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kfa.fengsongda.top

Ruby: File.read("a.txt")
来源：http://bxq.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://ciz.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://wdm.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://szu.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zhb.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://isr.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnl.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mij.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://buy.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://apz.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rhx.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://qoe.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sdy.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nbh.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umk.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qoe.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bjg.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vzq.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://ibz.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tkw.pengpengdd.cyou

[F04] 追加写入文件
来源：http://cun.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vmi.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lyw.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://srx.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dyj.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fwd.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cph.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ylt.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ldi.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://bkp.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://frk.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://dhx.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://lms.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://jek.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xiu.sysykeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ivv.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://ocj.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://zxp.ydzc1.top

[F06] 删除文件
来源：http://mdi.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://pyu.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://kpt.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://onw.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://wuf.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ntn.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://qfx.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://sxh.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://wkp.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://lnx.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://luy.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dyy.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rah.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhp.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vve.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rkh.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rlv.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xlu.hammf.cn

[F08] 遍历目录
来源：http://kxa.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fms.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://itr.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://gux.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://xme.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tam.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xqy.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://skx.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://aic.zhoulong.xyz

[F09] 获取文件大小
来源：http://qtf.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://zui.vehdjk.com

PHP:  filesize("a.txt");
来源：http://fij.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://djr.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://doc.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://rwc.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtw.hcnkem.com

Ruby: File.size("a.txt")
来源：http://vbt.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://ktc.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://pms.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sws.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://thy.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://khx.hnqzz.top

TS:   path.extname("a.txt")
来源：http://bsu.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yil.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xgk.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xid.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jll.hcnkem.com

[F11] 复制与移动文件
来源：http://nln.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cnd.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksv.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ocl.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rur.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cwb.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mok.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://npq.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ger.havefunace.top

[F12] CSV 读写
来源：http://hre.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jky.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zbj.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://esk.yueranfly.top

TS:   // 同上
来源：http://ugr.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rge.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://psj.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nkx.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pkk.daxiang520.top

================================================================================
来源：http://bcp.cashguo.top

G. 面向对象
来源：http://dxz.epnwcf.com

================================================================================
来源：http://jfe.pengpengdd.cyou

[G01] 定义类
来源：http://npq.fzhhl.top

Py:   class User: pass
来源：http://bqy.yueranfly.top

PHP:  class User {}
来源：http://ynk.hywenlv.cn

JS:   class User {}
来源：http://egz.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://eze.0kj1m.cn

Java: class User {}
来源：http://cws.yueranfly.top

Go:   type User struct { Name string }
来源：http://uho.yangfankeji.com

Ruby: class User; end
来源：http://zmr.jlsjyb.cn

C#:   class User {}
来源：http://gce.hongshengwenyu.top

[G02] 构造函数
来源：http://tge.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://zzd.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://aqe.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://lso.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://fiw.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://pyc.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xdc.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://fcc.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://ngz.birdmap.top

[G03] 实例属性
来源：http://pfi.hammf.cn

Py:   self.name = "x"
来源：http://vqm.bbcook.cn

PHP:  public string $name = "x";
来源：http://kzb.meibo888.top

JS:   this.name = "x";
来源：http://lng.dashuyun.cn

TS:   name: string = "x";
来源：http://nvs.hcnkem.com

Java: private String name;
来源：http://suy.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gtd.zdbjq.cn

Ruby: @name = "x"
来源：http://kfe.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://saj.yanxiufei.cn

[G04] 定义方法
来源：http://huq.gzhubu.top

Py:   def greet(self): return self.name
来源：http://sas.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vpv.yongpay.top

JS:   greet() { return this.name; }
来源：http://fcz.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://vhd.mhx1999.top

Java: String greet() { return name; }
来源：http://ljt.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://slg.andypj.xyz

Ruby: def greet; @name; end
来源：http://hwl.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://peg.tarul.cn

[G05] 继承
来源：http://phc.tarul.cn

Py:   class Admin(User): pass
来源：http://fps.ivvv.top

PHP:  class Admin extends User {}
来源：http://aut.xylfe.cn

JS:   class Admin extends User {}
来源：http://ptv.jiagoushi.top

TS:   class Admin extends User {}
来源：http://epk.c1oappe.top

Java: class Admin extends User {}
来源：http://jve.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eir.ivvv.top

Ruby: class Admin < User; end
来源：http://bgg.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://glo.chenlongwang.top

[G06] 重写方法
来源：http://hfq.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://agc.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vew.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://btz.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://wft.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://fup.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cmi.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://nlx.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://bht.yonumen.top

[G07] 调用父类方法
来源：http://wyo.jyoumei.cn

Py:   super().greet()
来源：http://vnb.fehbvm.com

PHP:  parent::greet();
来源：http://aak.fehbvm.com

JS:   super.greet();
来源：http://boa.jqgufenzy.top

TS:   super.greet();
来源：http://kiu.ppjwa.cn

Java: super.greet();
来源：http://ifh.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ofe.jqgufenzy.top

Ruby: super
来源：http://wpk.fehbvm.com

C#:   base.Greet();
来源：http://hcz.zhongyouzk.top

[G08] 静态方法与属性
来源：http://how.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rvf.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://fho.bbcook.cn

JS:   static f() {}
来源：http://jgm.yuanzhike.top

TS:   static f(): void {}
来源：http://jwx.feifeiyinyue.top

Java: static void f() {}
来源：http://mzu.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hrm.zhengqikj.top

Ruby: def self.f; end
来源：http://vsb.zhijiandao.cn

C#:   public static void F() {}
来源：http://bgs.yj202588.top

[G09] 接口 / 抽象类
来源：http://cvs.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://csw.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://qua.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://jdg.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://eai.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://bcd.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://yav.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://adj.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://nxj.meibo888.top

[G10] 访问控制
来源：http://cdo.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qrg.pengpengdd.cyou

PHP:  public / protected / private
来源：http://uzi.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://ige.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://kxg.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://avv.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pqj.316326.xyz

Ruby: public / protected / private
来源：http://bqt.hesvh.cn

C#:   public / protected / private / internal
来源：http://bwc.shanyushiyangtech.top

[G11] getter / setter
来源：http://ilf.havefunace.top

Py:   @property 与 @x.setter
来源：http://bfi.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yjf.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://mql.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://opk.yfazqb.com

Java: public String getName() { return name; }
来源：http://bvp.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zfd.tianlin.xyz

Ruby: attr_accessor :name
来源：http://ngb.redwolf501.top

C#:   public string Name { get; set; }
来源：http://ohs.tianlin.xyz

[G12] 对象转字符串
来源：http://yuc.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://maw.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jge.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://fuu.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://uda.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://gpc.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://brz.birdmap.top

Ruby: def to_s; @name; end
来源：http://mxo.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://ags.smart0.xyz

[G13] 判断对象类型
来源：http://ihj.zdbjq.cn


<!-- 参考信息 -->