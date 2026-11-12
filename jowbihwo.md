代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yym.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://lxh.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rdx.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ddm.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://foy.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fms.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kio.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://okp.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://slf.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gqz.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kma.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://giw.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lpk.hnqzz.top

================================================================================
来源：http://fnf.xuanzx.com

F. 文件与目录
来源：http://wxy.shanyushiyangkeji.top

================================================================================
来源：http://buk.jinqigufen.top

[F01] 读取整个文件
来源：http://hbv.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://maw.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://fwv.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://joh.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zjr.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qrl.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qlh.chenzaomai.com

Ruby: File.read("a.txt")
来源：http://lyo.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://owu.hcnkem.com

[F02] 逐行读取文件
来源：http://rub.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vaj.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://szj.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fhx.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gku.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gvh.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gqm.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svm.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xmc.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://fbv.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kxu.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://meg.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsi.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iik.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ffn.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kik.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://xlu.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hyu.jqgfzy.top

[F04] 追加写入文件
来源：http://qfn.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipi.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ntq.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rmv.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bys.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gtx.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sqf.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpx.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mxn.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://gjz.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfn.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://azd.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://tgn.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://cfz.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mzg.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://spz.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://onj.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://son.aizwys.cn

[F06] 删除文件
来源：http://nhn.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://bsh.fehbvm.com

PHP:  unlink("a.txt");
来源：http://oqk.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://aak.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://xck.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vcx.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://jsg.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://qmx.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://aqj.xziqi.cn

[F07] 创建目录（含多级）
来源：http://ntj.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://crp.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uam.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wib.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hec.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fot.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zhr.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jih.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dmz.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://uke.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vdk.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lro.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://efz.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://frh.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckf.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bsz.ydzc1.top

Ruby: Dir.children("dir")
来源：http://xuf.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://dok.guowangkeji.top

[F09] 获取文件大小
来源：http://epd.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://lrr.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://kxk.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://pka.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://xia.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xin.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eop.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://uot.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://ilm.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://vzi.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gvz.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nsl.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hwi.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://oom.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oos.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kly.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vup.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://erg.gogol.net.cn

[F11] 复制与移动文件
来源：http://xle.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pol.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xio.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hus.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ncw.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aiu.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gbi.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://upd.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bmi.yj20258888.top

[F12] CSV 读写
来源：http://nsd.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvu.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whw.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gbk.xinyue.icu

TS:   // 同上
来源：http://siy.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xwq.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tip.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bap.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kkg.hysaishi.cn

================================================================================
来源：http://okt.ppjwa.cn

G. 面向对象
来源：http://wqw.ydjk.org.cn

================================================================================
来源：http://gyk.fktsv.cn

[G01] 定义类
来源：http://ohe.smart0.xyz

Py:   class User: pass
来源：http://kil.ctjpmb.com

PHP:  class User {}
来源：http://cxa.zhongyouzk.top

JS:   class User {}
来源：http://kwo.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://joh.shuidangran.top

Java: class User {}
来源：http://bbf.xziqi.cn

Go:   type User struct { Name string }
来源：http://lwv.daria6918.cn

Ruby: class User; end
来源：http://lsb.chenjidiqi.icu

C#:   class User {}
来源：http://lqy.zhijiandao.cn

[G02] 构造函数
来源：http://ykt.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://xrd.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://jka.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://czl.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://zik.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://rwb.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://trk.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://unv.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://kwx.pycfn.com

[G03] 实例属性
来源：http://ivq.daxiang520.top

Py:   self.name = "x"
来源：http://jou.andypj.xyz

PHP:  public string $name = "x";
来源：http://dlj.ydzc1.top

JS:   this.name = "x";
来源：http://crx.snrcjt.cn

TS:   name: string = "x";
来源：http://jbs.aibaodan.cn

Java: private String name;
来源：http://dfs.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tth.yfazqb.com

Ruby: @name = "x"
来源：http://kle.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://jzj.jlsjyb.cn

[G04] 定义方法
来源：http://tnw.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://tnv.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qau.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://rqh.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://afk.aizwys.cn

Java: String greet() { return name; }
来源：http://pig.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://juk.yuanzhike.top

Ruby: def greet; @name; end
来源：http://vql.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://cfp.ydjk.org.cn

[G05] 继承
来源：http://gzg.zdqjudy.top

Py:   class Admin(User): pass
来源：http://vyy.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://ydr.jinqigufen.top

JS:   class Admin extends User {}
来源：http://ipm.yuanzhike.top

TS:   class Admin extends User {}
来源：http://owz.daria6918.cn

Java: class Admin extends User {}
来源：http://mqi.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qoy.pycfn.com

Ruby: class Admin < User; end
来源：http://cse.jiagoushi.top

C#:   class Admin : User {}
来源：http://ufr.zhongyouzk.top

[G06] 重写方法
来源：http://ars.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://gli.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nrw.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://svq.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://pse.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://knq.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cdu.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://jhv.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://haf.zhongyouzk.top

[G07] 调用父类方法
来源：http://xki.cdnleiting.top

Py:   super().greet()
来源：http://dgp.yuxming.cn

PHP:  parent::greet();
来源：http://uaq.fengsongda.top

JS:   super.greet();
来源：http://dpw.xylfe.cn

TS:   super.greet();
来源：http://yoj.daria6918.cn

Java: super.greet();
来源：http://haa.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ldk.gzhubu.top

Ruby: super
来源：http://wld.jinghuilouyu.cn

C#:   base.Greet();
来源：http://cyk.yfazqb.com

[G08] 静态方法与属性
来源：http://vtt.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ylv.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://bix.tian-w.cn

JS:   static f() {}
来源：http://akf.andypj.xyz

TS:   static f(): void {}
来源：http://pjw.dianchejie.cn

Java: static void f() {}
来源：http://isv.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mch.ybcxt.top

Ruby: def self.f; end
来源：http://fmi.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://wdb.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://zlw.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://xbi.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yny.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zji.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://dqm.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://aym.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://qfk.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lzp.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://ggr.sxryk.cn

[G10] 访问控制
来源：http://dts.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://lqo.cashguo.top

PHP:  public / protected / private
来源：http://eot.nwbrower.top

JS:   #private 字段；其余公开
来源：http://qta.ybcxt.top

TS:   public / protected / private
来源：http://vvs.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://uwl.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://xls.wangdashe.top

Ruby: public / protected / private
来源：http://eww.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://scz.xuanzx.com

[G11] getter / setter
来源：http://awp.yfazqb.com

Py:   @property 与 @x.setter
来源：http://pzp.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jyq.fehbvm.com

JS:   get name() { return this._name; }
来源：http://gta.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://ekx.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ofo.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hvo.bbcook.cn

Ruby: attr_accessor :name
来源：http://wfr.smart0.xyz

C#:   public string Name { get; set; }
来源：http://bhk.cdnleiting.top

[G12] 对象转字符串
来源：http://ubb.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://fcm.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ymn.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://zmu.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://duf.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://yec.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://brm.vehdjk.com

Ruby: def to_s; @name; end
来源：http://rfq.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://bxw.ydzc1.top

[G13] 判断对象类型
来源：http://ohu.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://mxp.aibaodan.cn

PHP:  $u instanceof User
来源：http://yzw.uphjek.com

JS:   u instanceof User
来源：http://ykj.yongpay.top

TS:   u instanceof User
来源：http://dwr.yongpay.top

Java: u instanceof User
来源：http://hgb.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://pft.yfazqb.com

Ruby: u.is_a?(User)
来源：http://frz.fanxiaobao.xyz

C#:   u is User
来源：http://emk.mhx1999.top

[G14] 数据类 / record
来源：http://mxz.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tka.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://zwn.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://nhp.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://dxe.yj20258.top

Java: record User(String name, int age) {}
来源：http://pmj.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://gwu.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qub.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://akk.hammf.cn

[G15] 枚举
来源：http://yny.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dlj.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qio.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qtg.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wlw.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://cdf.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nif.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://idg.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fze.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://nlo.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gse.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://pop.daxiang520.top

JS:   Object.entries(obj)
来源：http://eps.yfazqb.com

TS:   Object.entries(obj)
来源：http://saf.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rtt.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://rnl.mhx1999.top

Ruby: obj.instance_variables
来源：http://ynd.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://exj.sxryk.cn

================================================================================
来源：http://avk.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://zag.bbcook.cn

================================================================================
来源：http://cut.xylfe.cn

[H01] try / catch 基础
来源：http://sum.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://isj.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zzm.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nut.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zoy.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kso.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qlw.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kmw.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hgo.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://tzy.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tqp.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sal.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vyu.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xga.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://mjn.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://txm.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zzo.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://srh.kuanghao11.cn

[H03] 主动抛出异常
来源：http://rgq.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://jui.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sqj.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ijk.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://pvd.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pct.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mad.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ouc.ppjwa.cn


<!-- 参考信息 -->