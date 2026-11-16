代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://atg.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://mlv.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ffj.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fmc.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://unv.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tco.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sni.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uek.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vdh.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gaw.bbcook.cn

[E16] 数字千分位
来源：http://mww.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://myp.hammf.cn

PHP:  number_format(1234567);
来源：http://wkr.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ucr.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aar.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qtt.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mpi.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iar.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://eqi.daxiang520.top

[E17] 首字母大写
来源：http://vqu.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xcn.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sal.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yco.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afs.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xnb.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ebb.feifeiyinyue.top

Ruby: s.capitalize
来源：http://tjl.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qxn.yanxiufei.cn

[E18] 模板占位符替换
来源：http://bkh.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nmf.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlt.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://omq.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ato.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jki.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://shc.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aen.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jlh.316326.xyz

[E19] 多行文本按行拆分
来源：http://rwq.andypj.xyz

Py:   s.splitlines()
来源：http://plf.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ggn.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://aqg.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://poe.cheryme.top

Java: s.lines().toList()
来源：http://bsq.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://vvn.zhongyouzk.top

Ruby: s.lines
来源：http://khg.fktsv.cn

C#:   s.Split('\n')
来源：http://xmc.gzhubu.top

[E20] 判断字符串是否为空
来源：http://qyz.xinyue.icu

Py:   if not s:
来源：http://fwp.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://znt.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nvf.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://cms.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://egb.epnwcf.com

Go:   if s == "" {}
来源：http://esw.ctjpmb.com

Ruby: if s.empty?
来源：http://aio.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yvs.iojbl.cn

[E21] 超长截断加省略号
来源：http://ubl.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xvl.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcb.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cfd.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://frc.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qmc.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://hsi.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xhs.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lqz.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://gax.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uyq.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dkz.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsw.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ejb.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bxd.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mzs.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://tsm.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aon.fktsv.cn

================================================================================
来源：http://mja.hysaishi.cn

F. 文件与目录
来源：http://zwv.ydzc1.top

================================================================================
来源：http://cbr.sjlbkw.cn

[F01] 读取整个文件
来源：http://cno.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jic.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://pwb.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aqz.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dac.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hcz.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://stp.bbcook.cn

Ruby: File.read("a.txt")
来源：http://blm.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://grf.smart0.xyz

[F02] 逐行读取文件
来源：http://dho.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ksl.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ccy.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qjj.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhv.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hyc.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dkj.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lad.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qzj.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://qgq.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycx.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hmx.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzr.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wts.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jpz.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://adu.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://tus.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lin.ehwqpu.com

[F04] 追加写入文件
来源：http://ucv.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ykd.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vie.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvh.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyn.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hca.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hcg.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hdg.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hlc.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://mjn.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jhi.cheryme.top

PHP:  file_exists("a.txt");
来源：http://ofj.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://xpj.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://bbs.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lbv.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zmy.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://srz.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://hwa.hesvh.cn

[F06] 删除文件
来源：http://oee.yongpay.top

Py:   os.remove("a.txt")
来源：http://ghu.yj20258888.top

PHP:  unlink("a.txt");
来源：http://qdk.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://kgu.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kym.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhz.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://fuc.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://yhw.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://yzy.sxryk.cn

[F07] 创建目录（含多级）
来源：http://hem.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwa.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aoe.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nta.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wvq.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdc.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://opi.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zao.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ppo.guowangkeji.top

[F08] 遍历目录
来源：http://mds.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iii.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lmh.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://dzh.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://cqc.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jdk.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ckl.bjfxy.top

Ruby: Dir.children("dir")
来源：http://hbh.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://mrk.hywenlv.cn

[F09] 获取文件大小
来源：http://iwp.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://kcl.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://xml.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://vwl.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://lhl.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://kmd.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://piu.aizwys.cn

Ruby: File.size("a.txt")
来源：http://vww.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://xgo.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://apg.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gif.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uwp.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggq.yj20258888.top

TS:   path.extname("a.txt")
来源：http://arw.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zmz.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ddo.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qaq.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://osa.sweek.top

[F11] 复制与移动文件
来源：http://zkr.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drf.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://trg.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arq.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktn.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uzn.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uyh.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hev.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://skr.yangfankeji.com

[F12] CSV 读写
来源：http://rpd.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lei.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://grx.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iyh.cucudq.cn

TS:   // 同上
来源：http://rny.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oab.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tnz.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dmn.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uhw.hammf.cn

================================================================================
来源：http://cnx.xuetiantiany.cn

G. 面向对象
来源：http://pqc.yuanzhike.top

================================================================================
来源：http://mpf.bjfxy.top

[G01] 定义类
来源：http://ppi.0kj1m.cn

Py:   class User: pass
来源：http://ahy.shzxlz.cn

PHP:  class User {}
来源：http://lzq.epnwcf.com

JS:   class User {}
来源：http://edu.yonumen.top

TS:   class User { name: string = ""; }
来源：http://zxo.ivvv.top

Java: class User {}
来源：http://yze.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://adq.shzxlz.cn

Ruby: class User; end
来源：http://hvu.hywenlv.cn

C#:   class User {}
来源：http://xqy.ybcxt.top

[G02] 构造函数
来源：http://qku.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://cdo.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://frm.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://gfs.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://wko.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://lzo.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdh.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://ujs.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://anb.uphjek.com

[G03] 实例属性
来源：http://qcv.yongpay.top

Py:   self.name = "x"
来源：http://sbb.cucudq.cn

PHP:  public string $name = "x";
来源：http://acy.dianchejie.cn

JS:   this.name = "x";
来源：http://sej.kuanghao11.cn

TS:   name: string = "x";
来源：http://knl.fehbvm.com

Java: private String name;
来源：http://mqp.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rwh.c1oappe.top

Ruby: @name = "x"
来源：http://aiz.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://erg.52xcode.cn

[G04] 定义方法
来源：http://lgn.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://pec.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://gdx.fengsongda.top

JS:   greet() { return this.name; }
来源：http://vdk.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://hkj.shzxlz.cn

Java: String greet() { return name; }
来源：http://cse.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://enh.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://mls.xuanzx.com

C#:   public string Greet() => Name;
来源：http://gmz.zdqjudy.top

[G05] 继承
来源：http://fic.ehwqpu.com

Py:   class Admin(User): pass
来源：http://uki.havefunace.top

PHP:  class Admin extends User {}
来源：http://fvl.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://isd.hammf.cn

TS:   class Admin extends User {}
来源：http://ste.zhengqikj.top

Java: class Admin extends User {}
来源：http://vqh.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ghm.jqgfzy.top

Ruby: class Admin < User; end
来源：http://nqa.dianchejie.cn

C#:   class Admin : User {}
来源：http://xft.vqdsnc.cn

[G06] 重写方法
来源：http://euk.yj202588.top

Py:   def greet(self): return "admin"
来源：http://frn.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sop.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://stt.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://zlq.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://dfu.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cti.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://jio.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://bgz.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://zwt.gotoacloud.top

Py:   super().greet()
来源：http://vyt.nanxinkj.top

PHP:  parent::greet();
来源：http://uxz.jinyuanbaomall.cn

JS:   super.greet();
来源：http://tkw.fanxiaobao.xyz

TS:   super.greet();
来源：http://ssh.zdbjq.cn

Java: super.greet();
来源：http://ocz.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bzx.guowangkeji.top

Ruby: super
来源：http://ekw.cheryme.top

C#:   base.Greet();
来源：http://hbm.gotoacloud.top

[G08] 静态方法与属性
来源：http://lvv.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zgg.tian-w.cn

PHP:  public static function f() {}
来源：http://avl.nanxinkj.top

JS:   static f() {}
来源：http://ngw.cheryme.top

TS:   static f(): void {}
来源：http://rye.yj20258.top

Java: static void f() {}
来源：http://lpv.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lha.ppjwa.cn

Ruby: def self.f; end
来源：http://otx.sxryk.cn

C#:   public static void F() {}
来源：http://mbr.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://sso.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://klc.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://mgh.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bft.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://exa.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://kyv.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://tli.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bnz.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://jnf.hongshengwenyu.top

[G10] 访问控制
来源：http://ibu.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://fer.snrcjt.cn

PHP:  public / protected / private
来源：http://nlw.316326.xyz

JS:   #private 字段；其余公开
来源：http://lyb.yongpay.top

TS:   public / protected / private
来源：http://oeq.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://ian.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rkr.snrcjt.cn

Ruby: public / protected / private
来源：http://lju.uphjek.com

C#:   public / protected / private / internal
来源：http://ttw.shzxlz.cn

[G11] getter / setter
来源：http://trs.xziqi.cn

Py:   @property 与 @x.setter
来源：http://nvk.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lfh.xuanzx.com

JS:   get name() { return this._name; }
来源：http://xic.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://djm.tanke756.top

Java: public String getName() { return name; }
来源：http://lmn.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nwi.tanke756.top

Ruby: attr_accessor :name
来源：http://yak.meibo888.top

C#:   public string Name { get; set; }
来源：http://wlc.cheryme.top

[G12] 对象转字符串
来源：http://eut.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://rvd.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://spw.hcnkem.com

JS:   toString() { return this.name; }
来源：http://xag.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://nvd.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://nov.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kdf.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://aqb.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://sqh.nwbrower.top

[G13] 判断对象类型
来源：http://wiv.chenlongwang.top

Py:   isinstance(u, User)
来源：http://jwc.daria6918.cn

PHP:  $u instanceof User
来源：http://jfk.bbcook.cn

JS:   u instanceof User
来源：http://dob.tian-w.cn

TS:   u instanceof User
来源：http://pjv.316326.xyz


<!-- 参考信息 -->