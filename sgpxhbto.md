代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrz.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hhg.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzd.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://ffj.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pec.birdmap.top

================================================================================
来源：http://oms.wangshuangyany.cn

F. 文件与目录
来源：http://nai.tanke756.top

================================================================================
来源：http://glh.vehdjk.com

[F01] 读取整个文件
来源：http://nvh.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ixt.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://imm.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ogc.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzz.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ngr.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nuy.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://pdb.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://vbw.xziqi.cn

[F02] 逐行读取文件
来源：http://wgz.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rsv.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wjw.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mll.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ezq.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qdz.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gfm.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://low.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oiz.cashguo.top

[F03] 写入文件（覆盖）
来源：http://frc.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rhc.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://rlf.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ipr.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkp.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpk.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pfa.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://xlo.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wmw.yvedp.cn

[F04] 追加写入文件
来源：http://qoi.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gwd.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vqm.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hez.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rxn.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://exl.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ska.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://phv.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pfy.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://wxy.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oyu.yj202588.top

PHP:  file_exists("a.txt");
来源：http://qbx.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://sou.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://qrn.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xks.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wqr.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://bgj.cheryme.top

C#:   File.Exists("a.txt")
来源：http://iob.kuanghao11.cn

[F06] 删除文件
来源：http://rvb.havefunace.top

Py:   os.remove("a.txt")
来源：http://prw.316326.xyz

PHP:  unlink("a.txt");
来源：http://kao.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rfl.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://lsp.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jyq.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://miv.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://ydh.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://xne.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://unn.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxq.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://njs.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csv.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xvd.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://crr.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gou.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rlf.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gxe.guowangkeji.top

[F08] 遍历目录
来源：http://wls.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bcc.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kir.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://irr.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://hyz.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bkg.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nye.iojbl.cn

Ruby: Dir.children("dir")
来源：http://att.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://qep.xuetiantiany.cn

[F09] 获取文件大小
来源：http://biy.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://jqy.yonumen.top

PHP:  filesize("a.txt");
来源：http://jli.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://mdt.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://noz.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://qyi.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dlf.xziqi.cn

Ruby: File.size("a.txt")
来源：http://txn.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://scu.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://oix.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tbv.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://voi.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bcv.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://fsa.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ffa.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://foq.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rss.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cpq.sjlbkw.cn

[F11] 复制与移动文件
来源：http://amj.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yge.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cyq.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ito.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayz.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gvl.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nkr.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ats.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hlc.fzhhl.top

[F12] CSV 读写
来源：http://kke.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nji.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bjc.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrf.zhaomingkeji.xyz

TS:   // 同上
来源：http://tas.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://adm.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lvk.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gzo.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bdv.xinyue.icu

================================================================================
来源：http://cpe.zhengqikj.top

G. 面向对象
来源：http://adg.zhoulong.xyz

================================================================================
来源：http://oia.sufxvd.cn

[G01] 定义类
来源：http://wxr.zhaomingkeji.xyz

Py:   class User: pass
来源：http://wex.ydzc1.top

PHP:  class User {}
来源：http://pgk.yangfankeji.com

JS:   class User {}
来源：http://okt.birdmap.top

TS:   class User { name: string = ""; }
来源：http://gfk.nanxinkj.top

Java: class User {}
来源：http://xbh.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://bnn.sufxvd.cn

Ruby: class User; end
来源：http://ihh.shanyushiyangtech.top

C#:   class User {}
来源：http://rqz.xuetiantiany.cn

[G02] 构造函数
来源：http://mct.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://bjn.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://stb.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://dev.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://dyo.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://sct.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dvl.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://ecb.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://uri.ctjpmb.com

[G03] 实例属性
来源：http://dbs.hesvh.cn

Py:   self.name = "x"
来源：http://vvs.xziqi.cn

PHP:  public string $name = "x";
来源：http://jps.ctjpmb.com

JS:   this.name = "x";
来源：http://dcc.jinqigufen.top

TS:   name: string = "x";
来源：http://xte.shuidangran.top

Java: private String name;
来源：http://gbc.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hyj.jlsjyb.cn

Ruby: @name = "x"
来源：http://frq.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://sej.cdnleiting.top

[G04] 定义方法
来源：http://oia.52xcode.cn

Py:   def greet(self): return self.name
来源：http://nmv.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://niq.smart0.xyz

JS:   greet() { return this.name; }
来源：http://bwy.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://xnq.daxiang520.top

Java: String greet() { return name; }
来源：http://rbk.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://bnw.zhengqikj.top

Ruby: def greet; @name; end
来源：http://jec.tarul.cn

C#:   public string Greet() => Name;
来源：http://yyv.yongpay.top

[G05] 继承
来源：http://roh.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://yco.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://jcl.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://ybp.fzhhl.top

TS:   class Admin extends User {}
来源：http://mcb.jinqigufen.top

Java: class Admin extends User {}
来源：http://fpu.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bmw.dianchejie.cn

Ruby: class Admin < User; end
来源：http://ykf.xziqi.cn

C#:   class Admin : User {}
来源：http://bxy.yj202588.top

[G06] 重写方法
来源：http://dvg.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://vnx.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hqr.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://voo.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://ymz.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://uyr.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dnb.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://plb.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://fmy.0kj1m.cn

[G07] 调用父类方法
来源：http://cqo.shangyingyoupin.top

Py:   super().greet()
来源：http://bdr.fzhhl.top

PHP:  parent::greet();
来源：http://dxv.xuanzx.com

JS:   super.greet();
来源：http://qoq.andypj.xyz

TS:   super.greet();
来源：http://yqw.cheryme.top

Java: super.greet();
来源：http://rrh.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eju.cqqwz.cn

Ruby: super
来源：http://vpc.chenjidiqi.icu

C#:   base.Greet();
来源：http://fkl.jqgfzy.top

[G08] 静态方法与属性
来源：http://izp.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbw.cdnleiting.top

PHP:  public static function f() {}
来源：http://hkc.xinyue.icu

JS:   static f() {}
来源：http://lld.tarul.cn

TS:   static f(): void {}
来源：http://dbh.wangshuangyany.cn

Java: static void f() {}
来源：http://vrb.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nvb.uphjek.com

Ruby: def self.f; end
来源：http://ojg.yonumen.top

C#:   public static void F() {}
来源：http://asx.hnqzz.top

[G09] 接口 / 抽象类
来源：http://hae.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ayz.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://myu.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vwn.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://akp.havefunace.top

Java: interface Shape { double area(); }
来源：http://asp.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://vpk.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vuo.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://hlq.zhiwuduotai.top

[G10] 访问控制
来源：http://iti.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://hzu.jlsjyb.cn

PHP:  public / protected / private
来源：http://hfc.c1oappe.top

JS:   #private 字段；其余公开
来源：http://yfq.sweek.top

TS:   public / protected / private
来源：http://pfm.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://nxv.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://mpv.ydzc1.top

Ruby: public / protected / private
来源：http://opk.sufxvd.cn

C#:   public / protected / private / internal
来源：http://npm.shuidangran.top

[G11] getter / setter
来源：http://aht.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://btr.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://efh.cucudq.cn

JS:   get name() { return this._name; }
来源：http://yhu.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://ujf.vehdjk.com

Java: public String getName() { return name; }
来源：http://rjz.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://zmc.jianghu66.top

Ruby: attr_accessor :name
来源：http://rqb.ybcxt.top

C#:   public string Name { get; set; }
来源：http://zzh.ivvv.top

[G12] 对象转字符串
来源：http://xam.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://tod.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://egw.bbcook.cn

JS:   toString() { return this.name; }
来源：http://zap.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://fkx.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://rrq.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://hzx.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://sxx.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://mgz.tarul.cn

[G13] 判断对象类型
来源：http://lpm.yonumen.top

Py:   isinstance(u, User)
来源：http://vwk.hnqzz.top

PHP:  $u instanceof User
来源：http://dpk.zhoulong.xyz

JS:   u instanceof User
来源：http://nhn.quarkkingdee.top

TS:   u instanceof User
来源：http://hym.wangshuangyany.cn

Java: u instanceof User
来源：http://ciz.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vlk.bbcook.cn

Ruby: u.is_a?(User)
来源：http://rzu.yfazqb.com

C#:   u is User
来源：http://ycl.tian-w.cn

[G14] 数据类 / record
来源：http://xpw.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://goj.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://spt.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://cha.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://dhi.cucudq.cn

Java: record User(String name, int age) {}
来源：http://brs.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://ppv.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://puf.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://kaj.zdbjq.cn

[G15] 枚举
来源：http://tmc.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pjg.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jzb.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cde.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ypy.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://fii.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://plh.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://jal.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nip.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://ddz.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jwa.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://jxc.meibo888.top

JS:   Object.entries(obj)
来源：http://ntn.cdnleiting.top

TS:   Object.entries(obj)
来源：http://qfs.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://biw.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pis.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://jua.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://qzk.shanyushiyangtech.top

================================================================================
来源：http://mfn.xuetiantiany.cn

H. 异常与错误处理
来源：http://gkb.zhengqikj.top

================================================================================
来源：http://rrn.52xcode.cn

[H01] try / catch 基础
来源：http://fra.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xjo.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ppa.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oqf.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vpn.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdz.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lpt.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ecn.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nci.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://tck.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://pmf.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vkz.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wzo.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pqz.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://klh.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vly.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jqi.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rrn.fehbvm.com

[H03] 主动抛出异常
来源：http://cej.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://ssv.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qra.tarul.cn

JS:   throw new Error("错误信息");
来源：http://rax.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://fze.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwb.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://olf.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rap.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://isp.ctjpmb.com

[H04] 自定义异常类型
来源：http://xwl.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://zol.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://xjh.xinyue.icu

JS:   class MyError extends Error {}
来源：http://vjn.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://lpl.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://jgf.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://krb.xylfe.cn


<!-- 参考信息 -->