代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://soe.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://xok.svipenyu.cn

Java: s.lines().toList()
来源：http://yqz.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://qfa.zhongyouzk.top

Ruby: s.lines
来源：http://jnu.yangfankeji.com

C#:   s.Split('\n')
来源：http://gyj.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://pkt.fzhhl.top

Py:   if not s:
来源：http://qhm.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://duy.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nix.tanke756.top

TS:   if (s === "") {}
来源：http://fan.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://ism.jiagoushi.top

Go:   if s == "" {}
来源：http://lqm.quarkkingdee.top

Ruby: if s.empty?
来源：http://ikt.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yyr.hcnkem.com

[E21] 超长截断加省略号
来源：http://ibd.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ahs.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://avn.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lya.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kbf.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://otp.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://col.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kgh.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jcu.sysykeji.top

[E22] 字节长度与字符长度
来源：http://vgk.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mgm.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmg.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kjt.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahp.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mgi.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ynb.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://pbs.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vhx.ctjpmb.com

================================================================================
来源：http://azs.cucudq.cn

F. 文件与目录
来源：http://szn.yj20258888.top

================================================================================
来源：http://qvk.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://jqk.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://swv.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://svg.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zqm.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zfh.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qvz.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qtx.fktsv.cn

Ruby: File.read("a.txt")
来源：http://gfh.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://xet.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://luj.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rge.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xij.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxf.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tui.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrk.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nmj.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jpi.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://chn.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://haz.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://idb.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zgh.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ych.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xux.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yjs.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iok.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://cyq.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bjy.chenjidiqi.icu

[F04] 追加写入文件
来源：http://mdk.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rqw.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wic.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vjo.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jni.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ysy.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ufw.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rby.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vev.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://jlw.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dra.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://xko.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://tzx.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://unh.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ttl.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rgt.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://jdm.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://yfa.gaohongyu789.top

[F06] 删除文件
来源：http://fbm.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://oht.yj20258888.top

PHP:  unlink("a.txt");
来源：http://fvz.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mno.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://tfl.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qrl.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://pis.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://trk.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://iss.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://jvs.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://omz.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rpb.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nni.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gze.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://teg.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pkb.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qca.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://roo.jinqigufen.top

[F08] 遍历目录
来源：http://ror.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mpy.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://due.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://wzx.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://hpm.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ucr.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://uiz.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://gfd.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://zvu.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://evo.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://tga.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://dad.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://wov.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://xpe.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mek.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hvp.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://wli.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://avx.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://aah.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdv.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://awd.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vai.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://zap.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmh.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ogk.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pyf.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gdn.tanke756.top

[F11] 复制与移动文件
来源：http://nah.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hss.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lmr.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qzx.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sco.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lyb.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ups.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wdx.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zbt.xylfe.cn

[F12] CSV 读写
来源：http://jlw.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yic.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lju.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zet.ybcxt.top

TS:   // 同上
来源：http://rbu.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xkg.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yzk.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lwe.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nun.yj20258.top

================================================================================
来源：http://mgq.feifeiyinyue.top

G. 面向对象
来源：http://evp.meibo888.top

================================================================================
来源：http://zjr.pycfn.com

[G01] 定义类
来源：http://scu.xuetiantiany.cn

Py:   class User: pass
来源：http://sqb.birdmap.top

PHP:  class User {}
来源：http://fmg.shangyingyoupin.top

JS:   class User {}
来源：http://hgg.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://ert.9152youxi.cn

Java: class User {}
来源：http://tiz.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://rjs.xinyue.icu

Ruby: class User; end
来源：http://ggo.guowangkeji.top

C#:   class User {}
来源：http://iev.mhx1999.top

[G02] 构造函数
来源：http://mlp.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://vbk.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://nnb.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://emm.tanke756.top

TS:   constructor(public name: string) {}
来源：http://bxd.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://vro.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ncn.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://gds.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://stf.cheryme.top

[G03] 实例属性
来源：http://nsh.snrcjt.cn

Py:   self.name = "x"
来源：http://ubw.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://miw.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://uah.shuidangran.top

TS:   name: string = "x";
来源：http://uiu.iojbl.cn

Java: private String name;
来源：http://jbx.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdb.vehdjk.com

Ruby: @name = "x"
来源：http://ktb.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://qrv.zdbjq.cn

[G04] 定义方法
来源：http://bxa.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://hxf.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gvm.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://pbc.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://ila.jinqigufen.top

Java: String greet() { return name; }
来源：http://jrn.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wpf.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://iik.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://kcd.gzhubu.top

[G05] 继承
来源：http://odh.havefunace.top

Py:   class Admin(User): pass
来源：http://tmt.pycfn.com

PHP:  class Admin extends User {}
来源：http://hdr.hnqzz.top

JS:   class Admin extends User {}
来源：http://nev.ydzc1.top

TS:   class Admin extends User {}
来源：http://eah.daria6918.cn

Java: class Admin extends User {}
来源：http://tpb.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ipt.c1oappe.top

Ruby: class Admin < User; end
来源：http://upv.yongpay.top

C#:   class Admin : User {}
来源：http://lgi.hnqzz.top

[G06] 重写方法
来源：http://znl.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://wrx.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kqz.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://qmh.wangdashe.top

TS:   greet(): string { return "admin"; }
来源：http://flb.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://rfa.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbg.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://tvg.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://cfb.ctjpmb.com

[G07] 调用父类方法
来源：http://juj.tarul.cn

Py:   super().greet()
来源：http://xwf.chenjidiqi.icu

PHP:  parent::greet();
来源：http://tfr.redwolf501.top

JS:   super.greet();
来源：http://kxc.jyoumei.cn

TS:   super.greet();
来源：http://pnh.jinghuilouyu.cn

Java: super.greet();
来源：http://bqi.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cqy.haohaochexian.top

Ruby: super
来源：http://ssb.yj20258888.top

C#:   base.Greet();
来源：http://wnq.mhx1999.top

[G08] 静态方法与属性
来源：http://isw.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://grm.daria6918.cn

PHP:  public static function f() {}
来源：http://qnd.ctjpmb.com

JS:   static f() {}
来源：http://hid.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://mhz.cdnleiting.top

Java: static void f() {}
来源：http://nvm.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mck.wangdashe.top

Ruby: def self.f; end
来源：http://fhk.ydjk.org.cn

C#:   public static void F() {}
来源：http://tzk.ivvv.top

[G09] 接口 / 抽象类
来源：http://itb.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://xcm.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://hxv.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gcs.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://dih.316326.xyz

Java: interface Shape { double area(); }
来源：http://fmh.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://zbp.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mbe.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://bfx.c1oappe.top

[G10] 访问控制
来源：http://bjd.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://iub.gogol.net.cn

PHP:  public / protected / private
来源：http://eps.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://uor.zhoulong.xyz

TS:   public / protected / private
来源：http://aay.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://nrm.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bgb.hnxiangtu.top

Ruby: public / protected / private
来源：http://skd.cdnleiting.top

C#:   public / protected / private / internal
来源：http://bpe.jinqigfzy.top

[G11] getter / setter
来源：http://hsm.tarul.cn

Py:   @property 与 @x.setter
来源：http://xvv.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lkk.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ses.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://pro.yueranfly.top

Java: public String getName() { return name; }
来源：http://fvz.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sdm.ydzc1.top

Ruby: attr_accessor :name
来源：http://joq.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://rvb.daria6918.cn

[G12] 对象转字符串
来源：http://zem.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://oba.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mgz.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://tig.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://crt.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://gje.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://elk.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://zsy.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://ojr.chenjidiqi.icu

[G13] 判断对象类型
来源：http://igw.fengsongda.top

Py:   isinstance(u, User)
来源：http://crh.fehbvm.com

PHP:  $u instanceof User
来源：http://axt.xuanzx.com

JS:   u instanceof User
来源：http://sqy.yanxiufei.cn

TS:   u instanceof User
来源：http://wkm.xuetiantiany.cn

Java: u instanceof User
来源：http://ffu.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jnd.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://esb.zycfv.cn

C#:   u is User
来源：http://oit.yonumen.top

[G14] 数据类 / record
来源：http://fnt.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uov.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://ayh.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://dty.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://xke.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://ygc.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://jrp.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ajg.yongpay.top

C#:   record User(string Name, int Age);
来源：http://ruu.epnwcf.com

[G15] 枚举
来源：http://vax.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://woa.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bju.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tlz.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mgg.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://xfr.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cls.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://xky.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://soy.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://chw.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qyd.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://yzk.shzxlz.cn

JS:   Object.entries(obj)
来源：http://xxi.svipenyu.cn

TS:   Object.entries(obj)
来源：http://azo.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://knf.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pvj.cqqwz.cn

Ruby: obj.instance_variables
来源：http://zht.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ubb.chenzaomai.com

================================================================================
来源：http://jgt.gzhubu.top

H. 异常与错误处理
来源：http://zni.nanxinkj.top

================================================================================
来源：http://rvh.yuxming.cn

[H01] try / catch 基础
来源：http://nxy.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yjh.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://olb.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qah.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nzk.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ifp.birdmap.top


<!-- 参考信息 -->