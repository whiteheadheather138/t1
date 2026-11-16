代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sdv.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ffw.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://mtn.ehwqpu.com

[E17] 首字母大写
来源：http://mly.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eki.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wlc.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://glr.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://szi.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vej.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ugx.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://tyj.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://esl.gaohongyu789.top

[E18] 模板占位符替换
来源：http://brz.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wdm.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://khh.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mjd.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jjb.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hle.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sol.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vpt.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bfz.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://fpl.jqgufenzy.top

Py:   s.splitlines()
来源：http://xto.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mrj.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://rju.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://cbo.fktsv.cn

Java: s.lines().toList()
来源：http://rhp.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://bjo.bjfxy.top

Ruby: s.lines
来源：http://uds.c1oappe.top

C#:   s.Split('\n')
来源：http://sfm.ybcxt.top

[E20] 判断字符串是否为空
来源：http://kpz.daria6918.cn

Py:   if not s:
来源：http://azp.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://knp.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hps.yj20258888.top

TS:   if (s === "") {}
来源：http://rhn.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://kfx.daria6918.cn

Go:   if s == "" {}
来源：http://hfr.sxryk.cn

Ruby: if s.empty?
来源：http://nbs.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ijm.dashuyun.cn

[E21] 超长截断加省略号
来源：http://bvo.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jjm.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxv.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ivv.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rcf.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ous.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://ujl.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yus.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ygn.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://ajl.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bkp.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tib.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehp.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://taa.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ows.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mis.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://sah.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tzg.zhixingplan.top

================================================================================
来源：http://frm.jiagoushi.top

F. 文件与目录
来源：http://icf.fanxiaobao.xyz

================================================================================
来源：http://peg.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://aqs.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dyx.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://knw.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sas.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wdu.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eym.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zvq.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://djq.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://dco.9152youxi.cn

[F02] 逐行读取文件
来源：http://ktu.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lbi.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tyb.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gjp.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovz.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ifa.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yoh.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wus.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rqo.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://jov.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dcv.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nyn.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zlf.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://efo.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://alv.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ihu.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://zlc.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://koy.ydjk.org.cn

[F04] 追加写入文件
来源：http://yzl.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hjq.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uaj.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wiv.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yea.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rbr.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohn.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://odk.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hsf.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://hzm.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://scd.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://boy.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://ney.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://eia.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jrw.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xox.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://zqq.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://fve.svipenyu.cn

[F06] 删除文件
来源：http://tkt.ybcxt.top

Py:   os.remove("a.txt")
来源：http://asu.yj20258888.top

PHP:  unlink("a.txt");
来源：http://gbn.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dzc.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://fbq.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uyq.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://jap.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://stb.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://swu.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://hfg.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqa.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qkd.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqy.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ucb.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rvv.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cmq.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gkh.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qfb.xinyue.icu

[F08] 遍历目录
来源：http://jyd.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hgo.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xtl.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://jie.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://tyv.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mkk.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajz.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://kat.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://ekg.yuxming.cn

[F09] 获取文件大小
来源：http://tum.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://qrn.nwbrower.top

PHP:  filesize("a.txt");
来源：http://yid.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://yyd.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://mac.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xmy.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rrk.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://min.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://jui.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://spx.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xql.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xco.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://esr.iojbl.cn

TS:   path.extname("a.txt")
来源：http://zxs.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jxi.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gbo.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gkt.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ptn.ctjpmb.com

[F11] 复制与移动文件
来源：http://flj.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dvp.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mpm.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ptm.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://unq.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yrh.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ykf.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hes.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fmo.zycfv.cn

[F12] CSV 读写
来源：http://dgp.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ipa.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jsc.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dkq.uphjek.com

TS:   // 同上
来源：http://mkz.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ugk.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pix.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://buz.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mfk.pengpengdd.cyou

================================================================================
来源：http://woe.nanxinkj.top

G. 面向对象
来源：http://let.wangshuangyany.cn

================================================================================
来源：http://ytt.sxryk.cn

[G01] 定义类
来源：http://rlm.svipenyu.cn

Py:   class User: pass
来源：http://txk.fengsongda.top

PHP:  class User {}
来源：http://qym.daria6918.cn

JS:   class User {}
来源：http://sxl.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://ygu.sweek.top

Java: class User {}
来源：http://fjs.zycfv.cn

Go:   type User struct { Name string }
来源：http://ktc.xylfe.cn

Ruby: class User; end
来源：http://xnx.mhx1999.top

C#:   class User {}
来源：http://zlz.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://cff.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ttd.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://otd.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://ugn.cheryme.top

TS:   constructor(public name: string) {}
来源：http://teb.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://kkt.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hyf.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://ouy.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://nax.yj20258888.top

[G03] 实例属性
来源：http://cex.jlsjyb.cn

Py:   self.name = "x"
来源：http://xmk.sweek.top

PHP:  public string $name = "x";
来源：http://kka.hnqzz.top

JS:   this.name = "x";
来源：http://nyj.316326.xyz

TS:   name: string = "x";
来源：http://ecz.zycfv.cn

Java: private String name;
来源：http://rpd.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzg.52xcode.cn

Ruby: @name = "x"
来源：http://vgf.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://zba.c1oappe.top

[G04] 定义方法
来源：http://eyp.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://zaw.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ufc.316326.xyz

JS:   greet() { return this.name; }
来源：http://iwz.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://tru.dashuyun.cn

Java: String greet() { return name; }
来源：http://txa.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rln.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://qrm.birdmap.top

C#:   public string Greet() => Name;
来源：http://ywk.jiagoushi.top

[G05] 继承
来源：http://tcs.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://ged.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://wwk.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://vcw.yvedp.cn

TS:   class Admin extends User {}
来源：http://abd.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://bfw.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dbk.jyoumei.cn

Ruby: class Admin < User; end
来源：http://icc.jyoumei.cn

C#:   class Admin : User {}
来源：http://qwk.shuidangran.top

[G06] 重写方法
来源：http://qud.tarul.cn

Py:   def greet(self): return "admin"
来源：http://bva.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://gsq.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://seq.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://hss.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://ody.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://smr.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://ldd.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://eqx.daxiang520.top

[G07] 调用父类方法
来源：http://khi.chenlongwang.top

Py:   super().greet()
来源：http://cjn.hammf.cn

PHP:  parent::greet();
来源：http://lnk.aibaodan.cn

JS:   super.greet();
来源：http://ama.jinqigfzy.top

TS:   super.greet();
来源：http://sfa.bbcook.cn

Java: super.greet();
来源：http://xvj.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zfy.vehdjk.com

Ruby: super
来源：http://spk.bbcook.cn

C#:   base.Greet();
来源：http://ogl.haohaochexian.top

[G08] 静态方法与属性
来源：http://voi.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bba.tanke756.top

PHP:  public static function f() {}
来源：http://ycw.shzxlz.cn

JS:   static f() {}
来源：http://eiy.shzxlz.cn

TS:   static f(): void {}
来源：http://peg.aizwys.cn

Java: static void f() {}
来源：http://lwb.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nkj.guannengcc.top

Ruby: def self.f; end
来源：http://xbg.iojbl.cn

C#:   public static void F() {}
来源：http://zfi.daxiang520.top

[G09] 接口 / 抽象类
来源：http://atv.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://woc.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://idh.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rrp.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://hra.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://tbo.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://gsi.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jtn.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://uhi.wangdashe.top

[G10] 访问控制
来源：http://keb.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://njz.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://kde.guannengcc.top

JS:   #private 字段；其余公开
来源：http://eir.yvedp.cn

TS:   public / protected / private
来源：http://krj.pycfn.com

Java: public / protected / private / 默认包级
来源：http://ipd.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://grt.ppjwa.cn

Ruby: public / protected / private
来源：http://ymm.jianghu66.top

C#:   public / protected / private / internal
来源：http://wxm.hesvh.cn

[G11] getter / setter
来源：http://mgw.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://nyz.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ytr.sweek.top

JS:   get name() { return this._name; }
来源：http://mpa.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://hzc.daria6918.cn

Java: public String getName() { return name; }
来源：http://xiu.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xmt.guannengcc.top

Ruby: attr_accessor :name
来源：http://rqr.redwolf501.top

C#:   public string Name { get; set; }
来源：http://ixk.redwolf501.top

[G12] 对象转字符串
来源：http://xtn.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://ekn.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rao.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://ith.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://yqm.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://pmm.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://voo.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://xug.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://kgr.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://kjz.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://dbb.hysaishi.cn

PHP:  $u instanceof User
来源：http://ybr.shangyingyoupin.top

JS:   u instanceof User
来源：http://eel.zhijiandao.cn

TS:   u instanceof User
来源：http://pyx.cucudq.cn

Java: u instanceof User
来源：http://ixv.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wsx.hammf.cn

Ruby: u.is_a?(User)
来源：http://gxf.yvedp.cn

C#:   u is User
来源：http://mve.smart0.xyz

[G14] 数据类 / record
来源：http://kzo.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xhs.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://fqv.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://imb.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://llt.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://zne.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://nqn.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oph.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://xsi.svipenyu.cn

[G15] 枚举
来源：http://fth.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rxq.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ack.wangdashe.top


<!-- 参考信息 -->