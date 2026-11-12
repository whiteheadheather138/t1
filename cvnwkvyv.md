代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqp.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://azc.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lvx.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vkh.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://zvw.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dsa.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wqm.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qbw.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlp.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lnn.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://slb.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://qtg.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qnu.daria6918.cn

================================================================================
来源：http://lcn.daxiang520.top

F. 文件与目录
来源：http://spw.wangdashe.top

================================================================================
来源：http://rao.gaohongyu789.top

[F01] 读取整个文件
来源：http://qmr.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tyo.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://dej.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sbf.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mir.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xrs.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fql.52xcode.cn

Ruby: File.read("a.txt")
来源：http://ixp.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://iqn.cucudq.cn

[F02] 逐行读取文件
来源：http://qca.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wnv.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://als.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lla.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xvg.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://upv.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ilf.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xvd.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zux.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://hpj.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nzc.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://atn.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijs.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qml.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ogk.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvq.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://dke.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jtw.ctjpmb.com

[F04] 追加写入文件
来源：http://yjs.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wqy.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ygb.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpm.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzu.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sdc.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://toa.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tzu.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eod.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://fzr.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://enz.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://qvv.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://pav.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://pup.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://elh.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://btu.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://esh.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://wcb.chenlongwang.top

[F06] 删除文件
来源：http://xll.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://zbs.xziqi.cn

PHP:  unlink("a.txt");
来源：http://vtv.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bdd.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jnx.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ter.pycfn.com

Go:   os.Remove("a.txt")
来源：http://cof.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://hyj.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://cym.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://fld.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vmx.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtr.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqo.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fal.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hwg.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dca.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lfs.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qou.guowangkeji.top

[F08] 遍历目录
来源：http://yoa.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xmb.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lry.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://fyo.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://svr.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dul.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cvl.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://ehc.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://afm.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://ncl.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://dtv.xuanzx.com

PHP:  filesize("a.txt");
来源：http://lci.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://xst.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://mjt.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eyb.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yoe.mhx1999.top

Ruby: File.size("a.txt")
来源：http://iwj.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://jhc.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ghf.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tkc.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zqt.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bqu.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://zlg.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iqz.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hrm.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dwg.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mtp.cqqwz.cn

[F11] 复制与移动文件
来源：http://jof.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jwg.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mnh.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zvx.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pxb.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nxx.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iuh.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jds.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iau.kuanghao11.cn

[F12] CSV 读写
来源：http://ndl.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fvw.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yhx.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hqh.jqgfzy.top

TS:   // 同上
来源：http://xzt.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mry.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oyv.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://srb.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cui.gogol.net.cn

================================================================================
来源：http://qvo.xingfuxueyuan.xyz

G. 面向对象
来源：http://rfw.vehdjk.com

================================================================================
来源：http://ppi.ywan-chungtsiang.top

[G01] 定义类
来源：http://oym.nanxinkj.top

Py:   class User: pass
来源：http://xpp.jqgfzy.top

PHP:  class User {}
来源：http://xqb.sweek.top

JS:   class User {}
来源：http://rcw.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://ajj.yj202588.top

Java: class User {}
来源：http://dkw.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://psl.cdnleiting.top

Ruby: class User; end
来源：http://oad.hammf.cn

C#:   class User {}
来源：http://jel.hammf.cn

[G02] 构造函数
来源：http://zkt.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://tmv.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iiv.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://nzj.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://cmy.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://hee.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qjr.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://qcc.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://dqq.cqqwz.cn

[G03] 实例属性
来源：http://jny.cqqwz.cn

Py:   self.name = "x"
来源：http://cud.52xcode.cn

PHP:  public string $name = "x";
来源：http://xpi.jyoumei.cn

JS:   this.name = "x";
来源：http://ijf.hesvh.cn

TS:   name: string = "x";
来源：http://qwv.tanke756.top

Java: private String name;
来源：http://ndq.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvf.xylfe.cn

Ruby: @name = "x"
来源：http://lpo.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://coy.wangdashe.top

[G04] 定义方法
来源：http://fut.iojbl.cn

Py:   def greet(self): return self.name
来源：http://ntb.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vie.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://uuu.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://kkn.chenzaomai.com

Java: String greet() { return name; }
来源：http://iwj.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nxm.hywenlv.cn

Ruby: def greet; @name; end
来源：http://esk.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://jrz.pycfn.com

[G05] 继承
来源：http://yzy.cdnleiting.top

Py:   class Admin(User): pass
来源：http://fzh.guannengcc.top

PHP:  class Admin extends User {}
来源：http://zjl.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://lxf.havefunace.top

TS:   class Admin extends User {}
来源：http://oab.guannengcc.top

Java: class Admin extends User {}
来源：http://hcd.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lkg.c1oappe.top

Ruby: class Admin < User; end
来源：http://slm.quarkkingdee.top

C#:   class Admin : User {}
来源：http://nxo.0kj1m.cn

[G06] 重写方法
来源：http://srr.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://txl.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ekk.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://psr.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://bsm.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://chv.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cjn.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://rfs.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://bbb.aizwys.cn

[G07] 调用父类方法
来源：http://dji.chenzaomai.com

Py:   super().greet()
来源：http://xhn.wangdashe.top

PHP:  parent::greet();
来源：http://sgq.gaohongyu789.top

JS:   super.greet();
来源：http://wjp.jlsjyb.cn

TS:   super.greet();
来源：http://xrf.shzxlz.cn

Java: super.greet();
来源：http://oeu.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wbg.pycfn.com

Ruby: super
来源：http://cru.yueranfly.top

C#:   base.Greet();
来源：http://zaz.hnqzz.top

[G08] 静态方法与属性
来源：http://eoe.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hqb.fzhhl.top

PHP:  public static function f() {}
来源：http://mft.ehwqpu.com

JS:   static f() {}
来源：http://xfe.zhixingplan.top

TS:   static f(): void {}
来源：http://ryd.hongshengwenyu.top

Java: static void f() {}
来源：http://whg.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pxf.svipenyu.cn

Ruby: def self.f; end
来源：http://qxq.yanxiufei.cn

C#:   public static void F() {}
来源：http://flq.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://asm.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://tpe.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://mpi.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hqn.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://ujb.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://aak.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://ydl.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ntm.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://hwa.daxiang520.top

[G10] 访问控制
来源：http://uwp.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://tvu.iojbl.cn

PHP:  public / protected / private
来源：http://xyj.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://axz.gzhubu.top

TS:   public / protected / private
来源：http://rwt.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://tgq.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tpv.ctjpmb.com

Ruby: public / protected / private
来源：http://zfe.cdnleiting.top

C#:   public / protected / private / internal
来源：http://mwa.zhoulong.xyz

[G11] getter / setter
来源：http://axg.redwolf501.top

Py:   @property 与 @x.setter
来源：http://zoq.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://yxz.316326.xyz

JS:   get name() { return this._name; }
来源：http://kdm.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://rax.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://nqm.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://uhn.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://vep.cheryme.top

C#:   public string Name { get; set; }
来源：http://qxx.tarul.cn

[G12] 对象转字符串
来源：http://dqi.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://qbu.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://okz.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://mlh.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://cnf.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://ugl.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://ied.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://qud.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://cpk.tarul.cn

[G13] 判断对象类型
来源：http://vru.bjfxy.top

Py:   isinstance(u, User)
来源：http://ion.cucudq.cn

PHP:  $u instanceof User
来源：http://tbw.epnwcf.com

JS:   u instanceof User
来源：http://llu.daria6918.cn

TS:   u instanceof User
来源：http://iei.jinyuanbaomall.cn

Java: u instanceof User
来源：http://hdh.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jwy.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://pmj.zhengqikj.top

C#:   u is User
来源：http://loz.yongpay.top

[G14] 数据类 / record
来源：http://lfh.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kau.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://ekg.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dxp.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://oae.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://vlo.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://sbt.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vsj.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://jlp.gzhubu.top

[G15] 枚举
来源：http://yni.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfp.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gwd.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vlt.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://scv.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://dci.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tqd.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://vqt.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fff.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://qbb.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ttc.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://gru.bbcook.cn

JS:   Object.entries(obj)
来源：http://kop.tarul.cn

TS:   Object.entries(obj)
来源：http://jxw.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://shw.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://txj.hammf.cn

Ruby: obj.instance_variables
来源：http://qpv.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://zuc.xinyue.icu

================================================================================
来源：http://eff.yonumen.top

H. 异常与错误处理
来源：http://edo.sjlbkw.cn

================================================================================
来源：http://hmo.gogol.net.cn

[H01] try / catch 基础
来源：http://lsg.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://usc.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bbj.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hfj.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcy.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fxg.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zow.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hal.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qkh.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://ddy.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jms.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffb.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://elb.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iuw.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rqj.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://urr.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://udb.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ats.xylfe.cn

[H03] 主动抛出异常
来源：http://fsg.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://kil.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://atn.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://sxs.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://nlx.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pdt.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jxg.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://owa.nanxinkj.top


<!-- 参考信息 -->