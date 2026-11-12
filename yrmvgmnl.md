代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dkv.vehdjk.com

[E19] 多行文本按行拆分
来源：http://kkj.gaohongyu789.top

Py:   s.splitlines()
来源：http://srs.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbx.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://bmu.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://ttv.mhx1999.top

Java: s.lines().toList()
来源：http://hsh.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://gjx.gzhubu.top

Ruby: s.lines
来源：http://tfv.hysaishi.cn

C#:   s.Split('\n')
来源：http://nag.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://kou.jyoumei.cn

Py:   if not s:
来源：http://zgb.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fua.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ucf.yj20258888.top

TS:   if (s === "") {}
来源：http://exe.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://tcw.gogol.net.cn

Go:   if s == "" {}
来源：http://qdz.mhx1999.top

Ruby: if s.empty?
来源：http://lgv.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rah.svipenyu.cn

[E21] 超长截断加省略号
来源：http://fcz.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfw.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hez.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gtv.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://unp.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fls.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://bgz.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ayf.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://arx.daria6918.cn

[E22] 字节长度与字符长度
来源：http://imi.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gas.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttt.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqf.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqg.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fjj.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vqt.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://ehm.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uqp.ppjwa.cn

================================================================================
来源：http://gri.smart0.xyz

F. 文件与目录
来源：http://lvk.zhixingplan.top

================================================================================
来源：http://sph.chenlongwang.top

[F01] 读取整个文件
来源：http://nkr.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gqn.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://ccs.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://str.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wii.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://hic.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqt.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://yfk.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://fcw.cashguo.top

[F02] 逐行读取文件
来源：http://cez.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gyj.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dgj.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ggl.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uvr.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fbk.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tkv.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ubt.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lwe.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://rvq.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ffl.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bzj.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dto.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://njq.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bgi.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xrh.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://prf.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xth.daria6918.cn

[F04] 追加写入文件
来源：http://tot.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cuf.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sbe.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfi.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://icx.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wqt.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lgo.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://skf.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nbk.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://faf.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dkr.tarul.cn

PHP:  file_exists("a.txt");
来源：http://rbl.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://wml.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://whv.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iui.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ary.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://fap.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://fup.cqqwz.cn

[F06] 删除文件
来源：http://viu.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://jxy.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://esf.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://ofl.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lwd.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rni.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://gdz.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://bix.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://mqc.iojbl.cn

[F07] 创建目录（含多级）
来源：http://xim.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qsj.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xjh.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxp.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zmv.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kwo.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qeh.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvp.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aqj.gotoacloud.top

[F08] 遍历目录
来源：http://ita.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://tig.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tqq.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://yns.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://kmi.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cef.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://roc.ydzc1.top

Ruby: Dir.children("dir")
来源：http://pae.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://adp.jinqigfzy.top

[F09] 获取文件大小
来源：http://hyx.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://rsw.epnwcf.com

PHP:  filesize("a.txt");
来源：http://vmb.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://jdz.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://knd.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://kto.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ess.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://dav.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://hdh.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ibt.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfd.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ycl.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tmo.gzhubu.top

TS:   path.extname("a.txt")
来源：http://vxl.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lch.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jsa.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ipe.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sgp.9152youxi.cn

[F11] 复制与移动文件
来源：http://ove.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bfg.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://drw.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ksf.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmf.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tyd.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvc.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dlc.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqh.tarul.cn

[F12] CSV 读写
来源：http://inw.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://snm.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aym.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hhk.cucudq.cn

TS:   // 同上
来源：http://xdm.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ypn.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fwn.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://udk.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sic.c1oappe.top

================================================================================
来源：http://wnw.andypj.xyz

G. 面向对象
来源：http://icg.cucudq.cn

================================================================================
来源：http://unn.jlsjyb.cn

[G01] 定义类
来源：http://mfn.ydzc1.top

Py:   class User: pass
来源：http://ohg.snrcjt.cn

PHP:  class User {}
来源：http://hci.zycfv.cn

JS:   class User {}
来源：http://vfh.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://ukh.pycfn.com

Java: class User {}
来源：http://dxe.cdnleiting.top

Go:   type User struct { Name string }
来源：http://wno.jinghuilouyu.cn

Ruby: class User; end
来源：http://qyj.fanxiaobao.xyz

C#:   class User {}
来源：http://jqa.meibo888.top

[G02] 构造函数
来源：http://zmh.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ykq.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://apy.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://mam.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://tqw.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://enh.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvm.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://ebr.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://dqr.yvedp.cn

[G03] 实例属性
来源：http://nyp.hammf.cn

Py:   self.name = "x"
来源：http://tit.xziqi.cn

PHP:  public string $name = "x";
来源：http://pcy.quarkkingdee.top

JS:   this.name = "x";
来源：http://yer.yonumen.top

TS:   name: string = "x";
来源：http://bjy.zhiwuduotai.top

Java: private String name;
来源：http://nsx.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ert.svipenyu.cn

Ruby: @name = "x"
来源：http://eaf.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://jep.wangshuangyany.cn

[G04] 定义方法
来源：http://lfp.andypj.xyz

Py:   def greet(self): return self.name
来源：http://tsm.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://zsx.ivvv.top

JS:   greet() { return this.name; }
来源：http://ftv.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://pzq.xinyue.icu

Java: String greet() { return name; }
来源：http://hse.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zak.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://jyp.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://xql.ydzc1.top

[G05] 继承
来源：http://nbb.hesvh.cn

Py:   class Admin(User): pass
来源：http://mua.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://zrq.yj20258888.top

JS:   class Admin extends User {}
来源：http://jzy.chenzaomai.com

TS:   class Admin extends User {}
来源：http://baf.quarkkingdee.top

Java: class Admin extends User {}
来源：http://plg.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oeo.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://tbm.havefunace.top

C#:   class Admin : User {}
来源：http://npt.ppjwa.cn

[G06] 重写方法
来源：http://vgg.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://clt.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bzq.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://jqt.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://yjw.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://zxh.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zec.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://sph.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://krt.sufxvd.cn

[G07] 调用父类方法
来源：http://mgl.xuetiantiany.cn

Py:   super().greet()
来源：http://dxl.hammf.cn

PHP:  parent::greet();
来源：http://laq.shuidangran.top

JS:   super.greet();
来源：http://yfd.ctjpmb.com

TS:   super.greet();
来源：http://sbo.zhoulong.xyz

Java: super.greet();
来源：http://odf.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rcq.xuanzx.com

Ruby: super
来源：http://fls.cheryme.top

C#:   base.Greet();
来源：http://ygj.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://ism.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xip.epnwcf.com

PHP:  public static function f() {}
来源：http://psd.yj20258.top

JS:   static f() {}
来源：http://zyq.tarul.cn

TS:   static f(): void {}
来源：http://vql.sufxvd.cn

Java: static void f() {}
来源：http://jxm.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qax.jinqigufen.top

Ruby: def self.f; end
来源：http://pmo.ivvv.top

C#:   public static void F() {}
来源：http://zqu.sysykeji.top

[G09] 接口 / 抽象类
来源：http://vxz.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://ibb.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://kpz.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mof.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://nlo.nwbrower.top

Java: interface Shape { double area(); }
来源：http://qag.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://iea.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ocz.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://wnq.zhoulong.xyz

[G10] 访问控制
来源：http://igi.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://xfg.zhiwuduotai.top

PHP:  public / protected / private
来源：http://kut.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://qze.guowangkeji.top

TS:   public / protected / private
来源：http://ylz.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://szz.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nkg.sxryk.cn

Ruby: public / protected / private
来源：http://sfy.shuidangran.top

C#:   public / protected / private / internal
来源：http://jzp.xziqi.cn

[G11] getter / setter
来源：http://sir.shuidangran.top

Py:   @property 与 @x.setter
来源：http://ohb.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jkh.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://pzp.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://jvz.cqqwz.cn

Java: public String getName() { return name; }
来源：http://zfh.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ito.yj202588.top

Ruby: attr_accessor :name
来源：http://orm.hcnkem.com

C#:   public string Name { get; set; }
来源：http://kkb.zdqjudy.top

[G12] 对象转字符串
来源：http://cac.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://pbq.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bfz.c1oappe.top

JS:   toString() { return this.name; }
来源：http://uyj.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://ckp.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://nof.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://hsv.fengsongda.top

Ruby: def to_s; @name; end
来源：http://zgm.pycfn.com

C#:   public override string ToString() => Name;
来源：http://umh.ydjk.org.cn

[G13] 判断对象类型
来源：http://ecw.yuanzhike.top

Py:   isinstance(u, User)
来源：http://tle.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://uod.jyoumei.cn

JS:   u instanceof User
来源：http://sbo.xuetiantiany.cn

TS:   u instanceof User
来源：http://nnu.cashguo.top

Java: u instanceof User
来源：http://leg.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://myy.vehdjk.com

Ruby: u.is_a?(User)
来源：http://mvb.fzhhl.top

C#:   u is User
来源：http://kql.zdbjq.cn

[G14] 数据类 / record
来源：http://mmy.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qnh.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://tmg.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://guk.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://qys.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://hju.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://ael.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pnp.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://wab.uphjek.com

[G15] 枚举
来源：http://ssz.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hiz.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qai.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://voj.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jlu.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://itm.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ugs.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://yqc.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fuo.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://niu.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oei.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://pae.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://fxm.fzhhl.top

TS:   Object.entries(obj)
来源：http://vol.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gui.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sye.chenlongwang.top

Ruby: obj.instance_variables
来源：http://ybt.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://iym.fktsv.cn

================================================================================
来源：http://jxx.xziqi.cn

H. 异常与错误处理
来源：http://xuu.shanyushiyangtech.top

================================================================================
来源：http://cla.zhoulong.xyz

[H01] try / catch 基础
来源：http://zvv.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://geg.sjlbkw.cn


<!-- 参考信息 -->