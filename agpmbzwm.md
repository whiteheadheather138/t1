代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjg.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://exi.tianlin.xyz

[E16] 数字千分位
来源：http://jsm.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://wej.aizwys.cn

PHP:  number_format(1234567);
来源：http://qzo.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hbn.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hqg.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fkc.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tku.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lmg.316326.xyz

C#:   1234567.ToString("N0")
来源：http://wtn.tianlin.xyz

[E17] 首字母大写
来源：http://pxx.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://itc.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xlj.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygj.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kvf.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ysj.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rsp.chenlongwang.top

Ruby: s.capitalize
来源：http://sdt.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zdf.xuanzx.com

[E18] 模板占位符替换
来源：http://xxe.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vuz.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mbe.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fjx.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nrv.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://atd.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nvn.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gip.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://agl.yongpay.top

[E19] 多行文本按行拆分
来源：http://zch.bjfxy.top

Py:   s.splitlines()
来源：http://nzg.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nxr.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://mkm.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://ymg.yj20258888.top

Java: s.lines().toList()
来源：http://aua.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://trv.zhixingplan.top

Ruby: s.lines
来源：http://khb.yanxiufei.cn

C#:   s.Split('\n')
来源：http://vjh.aizwys.cn

[E20] 判断字符串是否为空
来源：http://hve.yongpay.top

Py:   if not s:
来源：http://bxy.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbw.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jah.zhixingplan.top

TS:   if (s === "") {}
来源：http://pqj.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://dhz.cdnleiting.top

Go:   if s == "" {}
来源：http://pbq.sufxvd.cn

Ruby: if s.empty?
来源：http://maz.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bqg.nwbrower.top

[E21] 超长截断加省略号
来源：http://fih.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ifq.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ymq.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rlp.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhj.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hxg.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://srt.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ywu.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://klm.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://adp.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rub.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mny.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wkd.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://joh.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gkj.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://atp.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://okb.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pjg.tianlin.xyz

================================================================================
来源：http://ais.ctjpmb.com

F. 文件与目录
来源：http://gud.52xcode.cn

================================================================================
来源：http://nla.xuetiantiany.cn

[F01] 读取整个文件
来源：http://ibr.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lcd.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ioy.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ipn.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iic.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iwk.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shz.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://icc.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://vke.guannengcc.top

[F02] 逐行读取文件
来源：http://jec.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qxt.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mvx.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uhm.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnp.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iry.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mvn.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jyj.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gky.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://pmp.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wyz.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gzl.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ixw.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tak.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jiw.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xir.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://flt.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tiz.zdqjudy.top

[F04] 追加写入文件
来源：http://lwi.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qlf.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hca.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vsm.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdn.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ktw.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fot.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awl.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kzj.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://tfc.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmo.316326.xyz

PHP:  file_exists("a.txt");
来源：http://yyu.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://wfb.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://mtf.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://poq.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mur.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://jtp.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://ovq.yj20258.top

[F06] 删除文件
来源：http://wfy.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://kdh.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://bln.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hbr.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fzk.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqk.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://qbe.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://rst.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://rkd.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://ofm.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qfj.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cmc.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ftb.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwq.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kmk.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kwn.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fas.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xbq.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://iid.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ets.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mdm.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://tte.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://uhx.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yjn.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yrx.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://ldk.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://vtq.hongshengwenyu.top

[F09] 获取文件大小
来源：http://efp.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://uqi.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://mit.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://oxc.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://nbo.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://vqb.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://npa.pycfn.com

Ruby: File.size("a.txt")
来源：http://fcb.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://txs.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://ivb.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qtx.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uhr.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://znx.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://vdq.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hbb.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bre.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ozz.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ces.fzhhl.top

[F11] 复制与移动文件
来源：http://nai.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qls.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://flw.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pnm.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjy.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jzp.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nlx.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hra.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yse.ydjk.org.cn

[F12] CSV 读写
来源：http://hcr.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aht.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivp.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rdx.uphjek.com

TS:   // 同上
来源：http://bxb.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ocw.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zrz.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kez.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qgj.xylfe.cn

================================================================================
来源：http://zyt.wangshuangyany.cn

G. 面向对象
来源：http://rjy.snrcjt.cn

================================================================================
来源：http://wqh.xylfe.cn

[G01] 定义类
来源：http://gra.daxiang520.top

Py:   class User: pass
来源：http://kai.jqgufenzy.top

PHP:  class User {}
来源：http://evj.sjlbkw.cn

JS:   class User {}
来源：http://ixg.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://ceh.bbcook.cn

Java: class User {}
来源：http://mhz.zdqjudy.top

Go:   type User struct { Name string }
来源：http://edx.snrcjt.cn

Ruby: class User; end
来源：http://wwh.zycfv.cn

C#:   class User {}
来源：http://jul.52xcode.cn

[G02] 构造函数
来源：http://hvu.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://ngd.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://muo.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://pny.hammf.cn

TS:   constructor(public name: string) {}
来源：http://gml.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://her.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://faa.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://bcs.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://rcj.fktsv.cn

[G03] 实例属性
来源：http://mct.pengpengdd.cyou

Py:   self.name = "x"
来源：http://gus.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://kuy.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://gcc.zhengqikj.top

TS:   name: string = "x";
来源：http://bne.nanxuanxn.top

Java: private String name;
来源：http://vbb.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hvk.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://dgp.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://cpw.zdqjudy.top

[G04] 定义方法
来源：http://xzr.yfazqb.com

Py:   def greet(self): return self.name
来源：http://xfz.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gch.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://bdn.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://syv.ybcxt.top

Java: String greet() { return name; }
来源：http://wyd.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hju.iojbl.cn

Ruby: def greet; @name; end
来源：http://jna.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://npp.hfpthk.cn

[G05] 继承
来源：http://thw.daria6918.cn

Py:   class Admin(User): pass
来源：http://dff.daria6918.cn

PHP:  class Admin extends User {}
来源：http://iux.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://tex.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://kov.fzhhl.top

Java: class Admin extends User {}
来源：http://kqz.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dhc.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://ois.smart0.xyz

C#:   class Admin : User {}
来源：http://xqy.fktsv.cn

[G06] 重写方法
来源：http://bsd.birdmap.top

Py:   def greet(self): return "admin"
来源：http://anm.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://yqx.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://bwk.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://fox.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://jse.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lvo.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://wse.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://mqi.jianghu66.top

[G07] 调用父类方法
来源：http://wbc.chenjidiqi.icu

Py:   super().greet()
来源：http://rrn.gogol.net.cn

PHP:  parent::greet();
来源：http://aej.zdqjudy.top

JS:   super.greet();
来源：http://ccj.hysaishi.cn

TS:   super.greet();
来源：http://slu.c1oappe.top

Java: super.greet();
来源：http://lhi.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nwp.xuetiantiany.cn

Ruby: super
来源：http://hdu.sjlbkw.cn

C#:   base.Greet();
来源：http://rkg.svipenyu.cn

[G08] 静态方法与属性
来源：http://gfu.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ost.9152youxi.cn

PHP:  public static function f() {}
来源：http://lta.yj20258.top

JS:   static f() {}
来源：http://vuk.ppjwa.cn

TS:   static f(): void {}
来源：http://edf.9152youxi.cn

Java: static void f() {}
来源：http://vfi.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kma.yuanzhike.top

Ruby: def self.f; end
来源：http://mfz.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://kpv.c1oappe.top

[G09] 接口 / 抽象类
来源：http://yok.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://wkz.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://wqp.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ymg.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://wgd.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://tei.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://wnp.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pwd.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://tdf.cashguo.top

[G10] 访问控制
来源：http://hva.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://dms.fengsongda.top

PHP:  public / protected / private
来源：http://krx.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://ivh.chenlongwang.top

TS:   public / protected / private
来源：http://mcw.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://vfi.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://urb.chenzaomai.com

Ruby: public / protected / private
来源：http://ajs.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://gju.zhixingplan.top

[G11] getter / setter
来源：http://ota.fehbvm.com

Py:   @property 与 @x.setter
来源：http://rxw.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://izw.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://vtv.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://mge.smart0.xyz

Java: public String getName() { return name; }
来源：http://kgk.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://vzc.andypj.xyz

Ruby: attr_accessor :name
来源：http://jey.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://jrn.yangfankeji.com

[G12] 对象转字符串
来源：http://nsn.meibo888.top

Py:   def __str__(self): return self.name
来源：http://ton.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ehr.cashguo.top

JS:   toString() { return this.name; }
来源：http://qev.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://pdi.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://pao.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://vaw.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://pmd.tanke756.top

C#:   public override string ToString() => Name;
来源：http://nes.ydjk.org.cn

[G13] 判断对象类型
来源：http://wtj.sweek.top

Py:   isinstance(u, User)
来源：http://gjh.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://lgk.yj20258888.top

JS:   u instanceof User
来源：http://yxr.cdnleiting.top

TS:   u instanceof User
来源：http://udh.shanyushiyangkeji.top

Java: u instanceof User
来源：http://thy.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wbj.andypj.xyz

Ruby: u.is_a?(User)
来源：http://cpk.sufxvd.cn

C#:   u is User
来源：http://dvf.hfpthk.cn

[G14] 数据类 / record
来源：http://fwk.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oci.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://qqe.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://spu.jianghu66.top


<!-- 参考信息 -->