代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gni.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nru.yvedp.cn

[E16] 数字千分位
来源：http://nhn.xinyue.icu

Py:   f"{1234567:,}"
来源：http://jqg.cqqwz.cn

PHP:  number_format(1234567);
来源：http://yak.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vqd.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cbd.hongshengwenyu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://byk.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ogt.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zjb.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://uhn.chenlongwang.top

[E17] 首字母大写
来源：http://dbe.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mlc.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bzv.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bal.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pel.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mom.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xas.guannengcc.top

Ruby: s.capitalize
来源：http://wmg.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vua.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://nqq.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rsv.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rtm.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fam.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hyu.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xpr.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onv.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bqz.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jme.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://jkh.52xcode.cn

Py:   s.splitlines()
来源：http://mdq.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://afw.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://azm.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://rsp.cashguo.top

Java: s.lines().toList()
来源：http://crf.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://zsp.yuanzhike.top

Ruby: s.lines
来源：http://cnh.xuanzx.com

C#:   s.Split('\n')
来源：http://nlo.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://jee.tarul.cn

Py:   if not s:
来源：http://mno.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ijh.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kqf.sxryk.cn

TS:   if (s === "") {}
来源：http://quh.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://jrr.yj20258.top

Go:   if s == "" {}
来源：http://sth.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://gfi.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.hcnkem.com

[E21] 超长截断加省略号
来源：http://ebi.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gve.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fsr.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xgh.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsf.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nmi.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://cup.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ypd.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhp.iojbl.cn

[E22] 字节长度与字符长度
来源：http://xhy.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zso.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kny.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcz.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ing.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bqx.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sjb.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://ujw.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rwa.xuetiantiany.cn

================================================================================
来源：http://dnq.jianghu66.top

F. 文件与目录
来源：http://jrj.xuanzx.com

================================================================================
来源：http://pbx.iojbl.cn

[F01] 读取整个文件
来源：http://ktz.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lsf.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://jkt.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ylt.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lqx.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://isn.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ogr.52xcode.cn

Ruby: File.read("a.txt")
来源：http://ryj.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://nug.ehwqpu.com

[F02] 逐行读取文件
来源：http://nrt.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cos.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zen.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwr.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gdc.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://grs.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vlo.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eqv.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rsp.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://prs.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kie.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oou.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxv.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gfq.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pex.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://adk.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://vwu.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://enj.mhx1999.top

[F04] 追加写入文件
来源：http://hwk.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipm.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wnv.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hxv.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbm.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rqv.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mkk.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cow.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zqv.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://lnn.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fop.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://xvq.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://xet.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://tkm.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gvh.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggk.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://cve.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://ddy.shuidangran.top

[F06] 删除文件
来源：http://myu.smart0.xyz

Py:   os.remove("a.txt")
来源：http://cws.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://hgw.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://cmu.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://bab.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sif.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://sct.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://pvr.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://ivy.xinyue.icu

[F07] 创建目录（含多级）
来源：http://asl.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://agl.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ivh.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fxg.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eio.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kcn.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cbd.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cem.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jfc.cqqwz.cn

[F08] 遍历目录
来源：http://adr.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://izo.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hmp.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://avz.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://wpt.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://byb.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rae.guannengcc.top

Ruby: Dir.children("dir")
来源：http://zpt.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://jma.52xcode.cn

[F09] 获取文件大小
来源：http://qhv.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://rfj.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://smy.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://vzx.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://wnp.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qga.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bhj.tanke756.top

Ruby: File.size("a.txt")
来源：http://frd.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://nbr.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://nyj.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lug.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lqb.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ldd.yvedp.cn

TS:   path.extname("a.txt")
来源：http://jhl.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://acx.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ujq.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lwr.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gxe.sjlbkw.cn

[F11] 复制与移动文件
来源：http://wbc.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sfq.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jkh.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bsv.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bns.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aiv.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bdt.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://prg.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yit.hywenlv.cn

[F12] CSV 读写
来源：http://eld.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://and.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hhf.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jfi.hcnkem.com

TS:   // 同上
来源：http://yvd.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gru.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tng.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lix.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://otp.yanxiufei.cn

================================================================================
来源：http://xsb.shanyushiyangtech.top

G. 面向对象
来源：http://wcq.shzxlz.cn

================================================================================
来源：http://tle.sysykeji.top

[G01] 定义类
来源：http://lqa.ppjwa.cn

Py:   class User: pass
来源：http://jfj.mhx1999.top

PHP:  class User {}
来源：http://fwi.xingfuxueyuan.xyz

JS:   class User {}
来源：http://zhv.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://djw.jinghuilouyu.cn

Java: class User {}
来源：http://ica.jinqigufen.top

Go:   type User struct { Name string }
来源：http://lad.hywenlv.cn

Ruby: class User; end
来源：http://qzk.tarul.cn

C#:   class User {}
来源：http://poa.shanyushiyangtech.top

[G02] 构造函数
来源：http://jnr.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://mfz.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://swu.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://fvl.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://lww.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://xuy.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ivy.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jet.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://wqy.fengsongda.top

[G03] 实例属性
来源：http://zdb.gogol.net.cn

Py:   self.name = "x"
来源：http://unf.shzxlz.cn

PHP:  public string $name = "x";
来源：http://jyg.jinqigufen.top

JS:   this.name = "x";
来源：http://fxq.tianlin.xyz

TS:   name: string = "x";
来源：http://bpb.sysykeji.top

Java: private String name;
来源：http://ccd.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://exd.wangshuangyany.cn

Ruby: @name = "x"
来源：http://rpk.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://zqy.wangdashe.top

[G04] 定义方法
来源：http://pob.fktsv.cn

Py:   def greet(self): return self.name
来源：http://ckk.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yqd.fengsongda.top

JS:   greet() { return this.name; }
来源：http://hvr.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://wvm.dianchejie.cn

Java: String greet() { return name; }
来源：http://qpf.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eld.316326.xyz

Ruby: def greet; @name; end
来源：http://urz.wangdashe.top

C#:   public string Greet() => Name;
来源：http://uux.cashguo.top

[G05] 继承
来源：http://wnw.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://bom.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://aer.c1oappe.top

JS:   class Admin extends User {}
来源：http://euu.hfpthk.cn

TS:   class Admin extends User {}
来源：http://voi.epnwcf.com

Java: class Admin extends User {}
来源：http://gcx.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fzc.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://aht.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://axx.kuanghao11.cn

[G06] 重写方法
来源：http://mif.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://vpp.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wby.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://app.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://mqm.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://pnl.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wnh.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://ijr.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://row.hnqzz.top

[G07] 调用父类方法
来源：http://tkv.kuanghao11.cn

Py:   super().greet()
来源：http://qvc.zdbjq.cn

PHP:  parent::greet();
来源：http://cvk.shanyushiyangtech.top

JS:   super.greet();
来源：http://bsg.dashuyun.cn

TS:   super.greet();
来源：http://vkm.yanxiufei.cn

Java: super.greet();
来源：http://qtm.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kvf.shanyushiyangtech.top

Ruby: super
来源：http://vpw.yongpay.top

C#:   base.Greet();
来源：http://psn.xziqi.cn

[G08] 静态方法与属性
来源：http://pfs.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mtj.gotoacloud.top

PHP:  public static function f() {}
来源：http://gyc.316326.xyz

JS:   static f() {}
来源：http://ngi.dashuyun.cn

TS:   static f(): void {}
来源：http://zzy.hysaishi.cn

Java: static void f() {}
来源：http://ann.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://wtb.jqgfzy.top

Ruby: def self.f; end
来源：http://tdb.hfpthk.cn

C#:   public static void F() {}
来源：http://rtm.c1oappe.top

[G09] 接口 / 抽象类
来源：http://gda.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://uhq.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uuj.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mxa.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://vlb.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://obe.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://hbs.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hhl.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://jbf.shuidangran.top

[G10] 访问控制
来源：http://jko.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://bgg.yanxiufei.cn

PHP:  public / protected / private
来源：http://rvl.fzhhl.top

JS:   #private 字段；其余公开
来源：http://lye.chenzaomai.com

TS:   public / protected / private
来源：http://npf.hammf.cn

Java: public / protected / private / 默认包级
来源：http://pdv.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sot.c1oappe.top

Ruby: public / protected / private
来源：http://dul.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://mak.zhijiandao.cn

[G11] getter / setter
来源：http://rze.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://pgs.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iql.mhx1999.top

JS:   get name() { return this._name; }
来源：http://blv.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://kgh.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://mfr.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iay.pycfn.com

Ruby: attr_accessor :name
来源：http://vlh.andypj.xyz

C#:   public string Name { get; set; }
来源：http://smx.pengpengdd.cyou

[G12] 对象转字符串
来源：http://ggv.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://xem.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dtc.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://ypi.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://reh.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://ovt.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://mxn.birdmap.top

Ruby: def to_s; @name; end
来源：http://lsc.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://tbb.snrcjt.cn

[G13] 判断对象类型
来源：http://kvh.guowangkeji.top

Py:   isinstance(u, User)
来源：http://krc.hammf.cn

PHP:  $u instanceof User
来源：http://pkj.ivvv.top

JS:   u instanceof User
来源：http://zhy.fanxiaobao.xyz

TS:   u instanceof User
来源：http://gin.pycfn.com

Java: u instanceof User
来源：http://cza.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jtt.ivvv.top

Ruby: u.is_a?(User)
来源：http://odf.epnwcf.com

C#:   u is User
来源：http://mgc.zdqjudy.top

[G14] 数据类 / record
来源：http://tih.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://key.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://daw.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://boh.316326.xyz


<!-- 参考信息 -->