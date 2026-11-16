代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qbt.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://pef.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hux.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sey.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://nea.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tjz.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ral.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibv.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rgk.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jbm.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sie.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://sye.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rlt.sxryk.cn

================================================================================
来源：http://ywj.cdnleiting.top

F. 文件与目录
来源：http://jzt.hcnkem.com

================================================================================
来源：http://hed.zhoulong.xyz

[F01] 读取整个文件
来源：http://une.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://scy.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://jae.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rne.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yrn.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fgz.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqt.fengsongda.top

Ruby: File.read("a.txt")
来源：http://xgx.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://qlo.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://gez.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wpu.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yuy.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qzt.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gqs.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ylp.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lkg.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eoe.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nqs.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://nge.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eat.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hqi.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xme.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrd.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mau.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dok.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://scn.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://psc.kuanghao11.cn

[F04] 追加写入文件
来源：http://zki.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xbb.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ven.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfa.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmg.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fvg.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cnu.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://flm.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rgl.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://zzo.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jvz.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://msd.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://nfc.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://fuf.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qzj.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jib.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://lxc.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://tti.nanxuanxn.top

[F06] 删除文件
来源：http://bnv.meibo888.top

Py:   os.remove("a.txt")
来源：http://vdz.52xcode.cn

PHP:  unlink("a.txt");
来源：http://qxr.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xde.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://toy.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qrn.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://ezi.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://rzr.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://kbf.birdmap.top

[F07] 创建目录（含多级）
来源：http://vtk.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmh.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://akm.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xju.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrb.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ipr.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://znn.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vhp.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eqf.cheryme.top

[F08] 遍历目录
来源：http://ycr.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sjt.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oag.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://rki.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://hhm.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qda.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://war.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://eac.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://cmb.cucudq.cn

[F09] 获取文件大小
来源：http://yof.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://gsu.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://vig.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://yoa.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://zlf.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oyw.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zoo.yfazqb.com

Ruby: File.size("a.txt")
来源：http://kbn.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://jve.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://ylm.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zjt.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://exz.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtu.zycfv.cn

TS:   path.extname("a.txt")
来源：http://aos.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://doy.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lhi.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ptp.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fdj.0kj1m.cn

[F11] 复制与移动文件
来源：http://tju.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aab.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qts.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvw.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cyq.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mvs.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ucw.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vrh.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xvp.yangfankeji.com

[F12] CSV 读写
来源：http://hqt.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzf.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cqu.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cra.snrcjt.cn

TS:   // 同上
来源：http://qlg.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://slp.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xgg.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://abv.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vsb.guannengcc.top

================================================================================
来源：http://ruf.yj20258888.top

G. 面向对象
来源：http://cyn.0kj1m.cn

================================================================================
来源：http://imo.guowangkeji.top

[G01] 定义类
来源：http://qzi.meibo888.top

Py:   class User: pass
来源：http://aeq.c1oappe.top

PHP:  class User {}
来源：http://ucz.havefunace.top

JS:   class User {}
来源：http://jwj.ivvv.top

TS:   class User { name: string = ""; }
来源：http://cli.jinqigufen.top

Java: class User {}
来源：http://vpl.snrcjt.cn

Go:   type User struct { Name string }
来源：http://mkl.zdbjq.cn

Ruby: class User; end
来源：http://efi.shuidangran.top

C#:   class User {}
来源：http://qgk.nwbrower.top

[G02] 构造函数
来源：http://gcl.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://mnh.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xzx.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://dqg.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://mgw.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://ken.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ugw.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://bij.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://ahb.aibaodan.cn

[G03] 实例属性
来源：http://tja.0kj1m.cn

Py:   self.name = "x"
来源：http://jkf.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://adc.epnwcf.com

JS:   this.name = "x";
来源：http://bvu.mhx1999.top

TS:   name: string = "x";
来源：http://xjz.zycfv.cn

Java: private String name;
来源：http://hch.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://imn.gotoacloud.top

Ruby: @name = "x"
来源：http://uns.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://qwn.gzhubu.top

[G04] 定义方法
来源：http://vwk.zycfv.cn

Py:   def greet(self): return self.name
来源：http://dfv.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wgk.yj20258.top

JS:   greet() { return this.name; }
来源：http://gmh.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://xim.jinqigfzy.top

Java: String greet() { return name; }
来源：http://xxu.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://thk.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://upt.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://rzw.havefunace.top

[G05] 继承
来源：http://ocn.xinyue.icu

Py:   class Admin(User): pass
来源：http://loa.tarul.cn

PHP:  class Admin extends User {}
来源：http://vmw.yuxming.cn

JS:   class Admin extends User {}
来源：http://tpb.fengsongda.top

TS:   class Admin extends User {}
来源：http://jqz.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://vkt.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oso.hesvh.cn

Ruby: class Admin < User; end
来源：http://vfp.tianlin.xyz

C#:   class Admin : User {}
来源：http://vgh.yj20258.top

[G06] 重写方法
来源：http://idn.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://pbb.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kbx.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://rqo.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://qaa.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://nam.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tgu.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://ibv.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://zcy.haohaochexian.top

[G07] 调用父类方法
来源：http://dbz.sysykeji.top

Py:   super().greet()
来源：http://bnq.hywenlv.cn

PHP:  parent::greet();
来源：http://yvw.sjlbkw.cn

JS:   super.greet();
来源：http://rya.jinyuanbaomall.cn

TS:   super.greet();
来源：http://rjq.shangyingyoupin.top

Java: super.greet();
来源：http://fkr.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dnq.shanyushiyangkeji.top

Ruby: super
来源：http://rnh.chenlongwang.top

C#:   base.Greet();
来源：http://fhl.tianlin.xyz

[G08] 静态方法与属性
来源：http://qlk.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzx.yuanzhike.top

PHP:  public static function f() {}
来源：http://ccx.hnqzz.top

JS:   static f() {}
来源：http://xjr.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://wsz.wangdashe.top

Java: static void f() {}
来源：http://xpg.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hlm.ehwqpu.com

Ruby: def self.f; end
来源：http://ues.jianghu66.top

C#:   public static void F() {}
来源：http://eii.aizwys.cn

[G09] 接口 / 抽象类
来源：http://ukd.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://qfn.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lss.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://otk.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://mph.ivvv.top

Java: interface Shape { double area(); }
来源：http://aze.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://ryd.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxh.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://nop.zycfv.cn

[G10] 访问控制
来源：http://ewt.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://buz.tianlin.xyz

PHP:  public / protected / private
来源：http://vkt.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://cma.jqgufenzy.top

TS:   public / protected / private
来源：http://elj.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://een.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sps.ehwqpu.com

Ruby: public / protected / private
来源：http://vyu.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://hoh.cdnleiting.top

[G11] getter / setter
来源：http://wmc.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://iah.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://osh.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://utt.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://mvk.hywenlv.cn

Java: public String getName() { return name; }
来源：http://qcu.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wcb.daria6918.cn

Ruby: attr_accessor :name
来源：http://afr.havefunace.top

C#:   public string Name { get; set; }
来源：http://tzt.epnwcf.com

[G12] 对象转字符串
来源：http://esa.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://rhv.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pua.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://txz.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://wks.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://jkn.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://xzc.yvedp.cn

Ruby: def to_s; @name; end
来源：http://twl.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://ent.shzxlz.cn

[G13] 判断对象类型
来源：http://mcu.jianghu66.top

Py:   isinstance(u, User)
来源：http://clt.jlsjyb.cn

PHP:  $u instanceof User
来源：http://oea.tianlin.xyz

JS:   u instanceof User
来源：http://ypu.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ixc.pycfn.com

Java: u instanceof User
来源：http://xay.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://igs.yj20258.top

Ruby: u.is_a?(User)
来源：http://bno.guannengcc.top

C#:   u is User
来源：http://fbo.fengsongda.top

[G14] 数据类 / record
来源：http://oqg.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uht.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://gla.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://kvi.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://rqh.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://dmh.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://dub.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blk.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://xup.wangshuangyany.cn

[G15] 枚举
来源：http://pbg.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kkp.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zwn.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mkr.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://anq.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://ead.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wdk.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://eqi.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gqd.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://yio.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sxe.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://iuz.sufxvd.cn

JS:   Object.entries(obj)
来源：http://zkd.daria6918.cn

TS:   Object.entries(obj)
来源：http://vko.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wsm.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://vdh.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://bhm.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://jrl.hcnkem.com

================================================================================
来源：http://bxg.yj20258.top

H. 异常与错误处理
来源：http://qyv.chenlongwang.top

================================================================================
来源：http://yco.xziqi.cn

[H01] try / catch 基础
来源：http://rgc.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://npg.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://avw.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zac.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nhk.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fja.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pgn.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tiq.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mda.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://mvo.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ohf.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mwo.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rip.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iqi.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://faa.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://euz.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://ckw.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://biu.sjlbkw.cn

[H03] 主动抛出异常
来源：http://osw.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://nzl.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xii.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://gdb.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://cll.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wiz.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cax.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gps.svipenyu.cn


<!-- 参考信息 -->