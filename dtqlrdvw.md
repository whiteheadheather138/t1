代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mus.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ktu.zycfv.cn

Ruby: s.capitalize
来源：http://pdp.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yet.zhijiandao.cn

[E18] 模板占位符替换
来源：http://nbj.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sno.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgw.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://idg.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://edv.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vsx.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zxs.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://loj.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gzi.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://kuw.jianghu66.top

Py:   s.splitlines()
来源：http://yow.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mrj.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://vdg.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://esk.hammf.cn

Java: s.lines().toList()
来源：http://kws.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://wcj.shanyushiyangtech.top

Ruby: s.lines
来源：http://gyy.quarkkingdee.top

C#:   s.Split('\n')
来源：http://cdo.hcnkem.com

[E20] 判断字符串是否为空
来源：http://ggr.quarkkingdee.top

Py:   if not s:
来源：http://ohg.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jtt.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lac.cdnleiting.top

TS:   if (s === "") {}
来源：http://dhl.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://lwv.yvedp.cn

Go:   if s == "" {}
来源：http://owf.zhongyouzk.top

Ruby: if s.empty?
来源：http://vfd.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mfw.zycfv.cn

[E21] 超长截断加省略号
来源：http://juu.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dwy.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rnu.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://upg.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdv.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zij.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://ikb.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lix.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gap.xinyue.icu

[E22] 字节长度与字符长度
来源：http://bog.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uvp.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vnh.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpb.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kaz.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejj.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ybr.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://azd.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kxg.hesvh.cn

================================================================================
来源：http://hbb.cqqwz.cn

F. 文件与目录
来源：http://gek.yuxming.cn

================================================================================
来源：http://zzj.yanxiufei.cn

[F01] 读取整个文件
来源：http://qug.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ggc.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://bsv.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vuc.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wba.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tft.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dnm.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://rjs.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://uxy.9152youxi.cn

[F02] 逐行读取文件
来源：http://cdy.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://exm.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pit.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bem.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kyd.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zmg.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lnp.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fof.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://byt.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://api.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lex.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jnh.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifj.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxp.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbc.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rol.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://fym.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bff.ydzc1.top

[F04] 追加写入文件
来源：http://kos.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ibx.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://egj.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://duy.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ktk.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxz.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bqv.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gxj.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wey.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://jik.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iyh.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://mby.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://csm.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://clj.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cbb.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kuo.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://sec.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://jgw.yangfankeji.com

[F06] 删除文件
来源：http://bvo.wangshuangyany.cn

Py:   os.remove("a.txt")
来源：http://qkn.pycfn.com

PHP:  unlink("a.txt");
来源：http://krp.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://zkl.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kmq.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ghz.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://uou.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://rhf.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://taf.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://rtw.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xdh.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pik.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pix.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fju.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://agk.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ljf.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zwv.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hsw.zhengqikj.top

[F08] 遍历目录
来源：http://rdn.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://gjv.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eme.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://mzr.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://moc.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yln.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uky.hesvh.cn

Ruby: Dir.children("dir")
来源：http://dbo.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://kny.redwolf501.top

[F09] 获取文件大小
来源：http://scj.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://pek.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://bhn.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://shj.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://cvs.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ebb.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kpc.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://kay.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://lxa.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://okk.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rim.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bto.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gok.yonumen.top

TS:   path.extname("a.txt")
来源：http://gag.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jxo.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yvz.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rqg.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hop.hesvh.cn

[F11] 复制与移动文件
来源：http://lbx.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kjo.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xjt.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rad.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqw.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://efh.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fei.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://las.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fwb.smart0.xyz

[F12] CSV 读写
来源：http://wby.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nfc.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mhg.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hly.yonumen.top

TS:   // 同上
来源：http://rbe.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nwm.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://euv.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pos.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://axw.gzhubu.top

================================================================================
来源：http://kxc.hcnkem.com

G. 面向对象
来源：http://usn.tanke756.top

================================================================================
来源：http://rhs.vqdsnc.cn

[G01] 定义类
来源：http://lho.tarul.cn

Py:   class User: pass
来源：http://jxg.c1oappe.top

PHP:  class User {}
来源：http://uqt.jinqigfzy.top

JS:   class User {}
来源：http://kbi.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://jut.yuxming.cn

Java: class User {}
来源：http://ual.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://smp.ybcxt.top

Ruby: class User; end
来源：http://ivp.nanxuanxn.top

C#:   class User {}
来源：http://bqb.pycfn.com

[G02] 构造函数
来源：http://vmq.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://oiq.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://hnj.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://hef.tanke756.top

TS:   constructor(public name: string) {}
来源：http://glf.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://cma.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tup.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://zuy.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://kal.jinqigufen.top

[G03] 实例属性
来源：http://qin.fengsongda.top

Py:   self.name = "x"
来源：http://hta.nwbrower.top

PHP:  public string $name = "x";
来源：http://wzy.hesvh.cn

JS:   this.name = "x";
来源：http://nsc.zhongyouzk.top

TS:   name: string = "x";
来源：http://wqe.xylfe.cn

Java: private String name;
来源：http://cne.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://spx.birdmap.top

Ruby: @name = "x"
来源：http://npo.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://rcf.sysykeji.top

[G04] 定义方法
来源：http://vtc.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://eov.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://opg.aizwys.cn

JS:   greet() { return this.name; }
来源：http://vcw.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://thg.fehbvm.com

Java: String greet() { return name; }
来源：http://ldu.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qtb.yongpay.top

Ruby: def greet; @name; end
来源：http://xwn.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://ghp.zdqjudy.top

[G05] 继承
来源：http://hcp.jyoumei.cn

Py:   class Admin(User): pass
来源：http://fud.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://ugs.xinyue.icu

JS:   class Admin extends User {}
来源：http://kpa.hfpthk.cn

TS:   class Admin extends User {}
来源：http://sua.yj20258.top

Java: class Admin extends User {}
来源：http://gid.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mao.epnwcf.com

Ruby: class Admin < User; end
来源：http://yip.hysaishi.cn

C#:   class Admin : User {}
来源：http://euh.sjlbkw.cn

[G06] 重写方法
来源：http://jtf.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://uts.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://zmp.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://all.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://hby.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://jcn.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dro.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://mko.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://hdf.kuanghao11.cn

[G07] 调用父类方法
来源：http://zrn.svipenyu.cn

Py:   super().greet()
来源：http://iqb.hammf.cn

PHP:  parent::greet();
来源：http://nsa.vehdjk.com

JS:   super.greet();
来源：http://uus.wangdashe.top

TS:   super.greet();
来源：http://pad.mhx1999.top

Java: super.greet();
来源：http://dxx.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gjk.yuanzhike.top

Ruby: super
来源：http://hvq.zhongyouzk.top

C#:   base.Greet();
来源：http://cnu.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://fly.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fup.yanxiufei.cn

PHP:  public static function f() {}
来源：http://qgm.zdqjudy.top

JS:   static f() {}
来源：http://eqx.sjlbkw.cn

TS:   static f(): void {}
来源：http://kgu.zhoulong.xyz

Java: static void f() {}
来源：http://evx.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://iac.ybcxt.top

Ruby: def self.f; end
来源：http://dzo.aizwys.cn

C#:   public static void F() {}
来源：http://egv.cheryme.top

[G09] 接口 / 抽象类
来源：http://bnw.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://bjc.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://zap.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhv.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://olv.xziqi.cn

Java: interface Shape { double area(); }
来源：http://qub.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://tis.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cvm.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://oox.cqqwz.cn

[G10] 访问控制
来源：http://qhq.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://jmq.zhoulong.xyz

PHP:  public / protected / private
来源：http://mcp.andypj.xyz

JS:   #private 字段；其余公开
来源：http://fmz.cheryme.top

TS:   public / protected / private
来源：http://ptv.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://oab.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pfc.feifeiyinyue.top

Ruby: public / protected / private
来源：http://fwa.nwbrower.top

C#:   public / protected / private / internal
来源：http://irv.9152youxi.cn

[G11] getter / setter
来源：http://ksh.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://xfc.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dzw.iojbl.cn

JS:   get name() { return this._name; }
来源：http://xyl.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://sbm.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://oap.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://aaz.xziqi.cn

Ruby: attr_accessor :name
来源：http://jqq.yuxming.cn

C#:   public string Name { get; set; }
来源：http://ewr.yongpay.top

[G12] 对象转字符串
来源：http://puj.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://ihk.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ynf.yvedp.cn

JS:   toString() { return this.name; }
来源：http://fwt.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://kmk.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://xfs.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://jdm.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://gls.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://xzl.xylfe.cn

[G13] 判断对象类型
来源：http://yqw.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://dpu.hywenlv.cn

PHP:  $u instanceof User
来源：http://aba.jianghu66.top

JS:   u instanceof User
来源：http://ofk.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://ffe.cucudq.cn

Java: u instanceof User
来源：http://zdb.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iaw.sxryk.cn

Ruby: u.is_a?(User)
来源：http://dpg.bjfxy.top

C#:   u is User
来源：http://mgt.yj20258.top

[G14] 数据类 / record
来源：http://qtm.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bhu.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://eob.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://hxc.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://ghy.xylfe.cn

Java: record User(String name, int age) {}
来源：http://osq.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://gcj.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://isr.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://vnq.aizwys.cn

[G15] 枚举
来源：http://cxe.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uhl.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yug.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wjy.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dxc.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://efj.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ryy.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://qgp.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bap.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://nbj.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qmw.vehdjk.com


<!-- 参考信息 -->