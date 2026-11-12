代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://swl.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://lkq.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tid.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rgl.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://osf.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gvr.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zjs.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vff.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kxw.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ylf.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ecs.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://jum.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xue.jianghu66.top

================================================================================
来源：http://vnj.zhixingplan.top

F. 文件与目录
来源：http://ebq.jinyuanbaomall.cn

================================================================================
来源：http://uav.jlsjyb.cn

[F01] 读取整个文件
来源：http://jny.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jyq.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://huq.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gbv.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://plh.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://itg.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fnf.daria6918.cn

Ruby: File.read("a.txt")
来源：http://vka.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://iiq.hesvh.cn

[F02] 逐行读取文件
来源：http://znr.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hex.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ajp.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cge.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mid.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cqq.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zeb.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pyi.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mbf.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://jyt.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wza.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gki.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvh.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eem.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dvo.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yny.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://hgg.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rao.dashuyun.cn

[F04] 追加写入文件
来源：http://osr.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://odz.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kgg.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dji.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://epk.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wmn.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fvc.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bdy.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tgg.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://oju.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zez.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://chf.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://ztf.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://lhm.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://atg.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xfz.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://eff.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://smm.hcnkem.com

[F06] 删除文件
来源：http://tps.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://nxb.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://cnu.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://kab.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gna.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kpu.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://iwf.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://eoc.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://pyq.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://zjk.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://air.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://btr.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xum.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ruq.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osq.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rrh.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oil.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cjm.andypj.xyz

[F08] 遍历目录
来源：http://whw.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nqo.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vfo.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://uav.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://niv.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ouk.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nin.mhx1999.top

Ruby: Dir.children("dir")
来源：http://zqu.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://eca.xuetiantiany.cn

[F09] 获取文件大小
来源：http://ias.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://yrd.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://drc.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://yvz.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://pam.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://qlb.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://auy.ivvv.top

Ruby: File.size("a.txt")
来源：http://ods.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://drl.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://edg.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dym.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oge.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://osp.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://vow.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sau.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ryk.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lvn.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjp.zhixingplan.top

[F11] 复制与移动文件
来源：http://dpu.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rrd.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rqv.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cxk.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhd.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qjo.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://obz.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qzn.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzy.fengsongda.top

[F12] CSV 读写
来源：http://xhl.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pfu.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asu.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwc.zycfv.cn

TS:   // 同上
来源：http://slk.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iob.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://djy.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ldv.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pkq.jinghuilouyu.cn

================================================================================
来源：http://qru.ydjk.org.cn

G. 面向对象
来源：http://zmu.sjlbkw.cn

================================================================================
来源：http://vat.cheryme.top

[G01] 定义类
来源：http://mci.wangdashe.top

Py:   class User: pass
来源：http://zwk.0kj1m.cn

PHP:  class User {}
来源：http://plj.snrcjt.cn

JS:   class User {}
来源：http://fgk.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://qkb.uphjek.com

Java: class User {}
来源：http://zpw.gzhubu.top

Go:   type User struct { Name string }
来源：http://ipc.tian-w.cn

Ruby: class User; end
来源：http://vgr.hywenlv.cn

C#:   class User {}
来源：http://fci.zhiwuduotai.top

[G02] 构造函数
来源：http://doh.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://oqn.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://fxr.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://lut.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://qgv.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://zde.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://anm.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://fmg.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://cyr.chenlongwang.top

[G03] 实例属性
来源：http://riz.yangfankeji.com

Py:   self.name = "x"
来源：http://huu.yfazqb.com

PHP:  public string $name = "x";
来源：http://mny.ppjwa.cn

JS:   this.name = "x";
来源：http://igs.aibaodan.cn

TS:   name: string = "x";
来源：http://qno.xuetiantiany.cn

Java: private String name;
来源：http://clk.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yhr.zhengqikj.top

Ruby: @name = "x"
来源：http://wcl.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://hrw.zdbjq.cn

[G04] 定义方法
来源：http://bdi.jianghu66.top

Py:   def greet(self): return self.name
来源：http://qal.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dkg.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://zzq.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://kvm.gzhubu.top

Java: String greet() { return name; }
来源：http://kzk.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wao.cdnleiting.top

Ruby: def greet; @name; end
来源：http://pxy.yfazqb.com

C#:   public string Greet() => Name;
来源：http://vzn.xylfe.cn

[G05] 继承
来源：http://gxw.jqgfzy.top

Py:   class Admin(User): pass
来源：http://uhq.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://lnv.tian-w.cn

JS:   class Admin extends User {}
来源：http://ebh.daria6918.cn

TS:   class Admin extends User {}
来源：http://ror.ehwqpu.com

Java: class Admin extends User {}
来源：http://dpp.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qxl.yj202588.top

Ruby: class Admin < User; end
来源：http://xcf.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://ecc.hongshengwenyu.top

[G06] 重写方法
来源：http://xwu.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://zlv.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rjr.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://dea.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://kyg.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://epb.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mwc.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://tzp.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://ago.snrcjt.cn

[G07] 调用父类方法
来源：http://jgg.yvedp.cn

Py:   super().greet()
来源：http://ewu.wangdashe.top

PHP:  parent::greet();
来源：http://owx.vqdsnc.cn

JS:   super.greet();
来源：http://rue.dianchejie.cn

TS:   super.greet();
来源：http://luc.shanyushiyangkeji.top

Java: super.greet();
来源：http://lsh.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hxf.zhijiandao.cn

Ruby: super
来源：http://fvu.cheryme.top

C#:   base.Greet();
来源：http://mxr.hnqzz.top

[G08] 静态方法与属性
来源：http://zsf.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://djy.kuanghao11.cn

PHP:  public static function f() {}
来源：http://wwo.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://rlf.ehwqpu.com

TS:   static f(): void {}
来源：http://zyi.cqqwz.cn

Java: static void f() {}
来源：http://buz.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kbd.mhx1999.top

Ruby: def self.f; end
来源：http://pxo.fengsongda.top

C#:   public static void F() {}
来源：http://ivk.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://cgs.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://cog.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://irw.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://bzv.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://vny.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://ase.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://kef.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ibh.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://hfl.hysaishi.cn

[G10] 访问控制
来源：http://mbm.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://tfr.zdqjudy.top

PHP:  public / protected / private
来源：http://jqe.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://gvf.feifeiyinyue.top

TS:   public / protected / private
来源：http://rjm.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://hyk.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sza.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://utl.yonumen.top

C#:   public / protected / private / internal
来源：http://cqi.redwolf501.top

[G11] getter / setter
来源：http://huo.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://kcs.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ysl.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://yeq.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://brm.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://zhl.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nas.yuanzhike.top

Ruby: attr_accessor :name
来源：http://zuo.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://qge.cucudq.cn

[G12] 对象转字符串
来源：http://jfz.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://qlf.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://niy.fehbvm.com

JS:   toString() { return this.name; }
来源：http://ink.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://zmm.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://hjt.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://yuk.gzhubu.top

Ruby: def to_s; @name; end
来源：http://bcs.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://eep.feifeiyinyue.top

[G13] 判断对象类型
来源：http://ddb.ctjpmb.com

Py:   isinstance(u, User)
来源：http://qzu.dashuyun.cn

PHP:  $u instanceof User
来源：http://dvw.chenjidiqi.icu

JS:   u instanceof User
来源：http://cqh.ehwqpu.com

TS:   u instanceof User
来源：http://thi.tanke756.top

Java: u instanceof User
来源：http://zfm.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mxe.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://qze.tanke756.top

C#:   u is User
来源：http://wvb.uphjek.com

[G14] 数据类 / record
来源：http://yvd.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kns.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://tvq.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://klb.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://yko.fktsv.cn

Java: record User(String name, int age) {}
来源：http://ibt.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://zjs.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://viq.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://guu.zycfv.cn

[G15] 枚举
来源：http://tpm.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://chv.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://knv.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tlp.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmf.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://zjw.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pch.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://mnz.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cdr.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://vst.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://efq.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://gis.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://bxj.xziqi.cn

TS:   Object.entries(obj)
来源：http://mzi.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qwv.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hzp.316326.xyz

Ruby: obj.instance_variables
来源：http://iet.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://iph.hongshengwenyu.top

================================================================================
来源：http://phg.hfpthk.cn

H. 异常与错误处理
来源：http://fef.jqgufenzy.top

================================================================================
来源：http://tta.hfpthk.cn

[H01] try / catch 基础
来源：http://fgd.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rya.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkk.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dqt.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://one.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kuc.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cxs.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wfe.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xto.guannengcc.top

[H02] finally / ensure 收尾
来源：http://vev.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tou.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vix.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tpe.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nsn.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://uny.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bff.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ecg.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgf.dianchejie.cn

[H03] 主动抛出异常
来源：http://nlz.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://kus.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wrv.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://nhm.yj202588.top

TS:   throw new Error("错误信息");
来源：http://zcd.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lbv.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rqa.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dho.vqdsnc.cn


<!-- 参考信息 -->