代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://djn.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fmi.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uyh.shuidangran.top

Ruby: File.read("a.txt")
来源：http://ubq.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://zdb.c1oappe.top

[F02] 逐行读取文件
来源：http://oya.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zmn.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lmf.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onu.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndq.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dxv.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://llt.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xak.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pza.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://psp.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://knz.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://guz.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdz.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nye.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rlv.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hot.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://tge.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hwm.sweek.top

[F04] 追加写入文件
来源：http://yhh.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dvi.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://epu.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyo.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://llk.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iok.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uxp.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ahe.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dgq.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://jqu.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ffa.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://ige.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://gak.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://mja.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ovf.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kmy.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://irv.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://hqx.sufxvd.cn

[F06] 删除文件
来源：http://qwi.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://zxc.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://owz.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://kwl.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qcm.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tjm.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://vaj.tanke756.top

Ruby: File.delete("a.txt")
来源：http://brc.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://wff.guannengcc.top

[F07] 创建目录（含多级）
来源：http://kjg.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vpl.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zam.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uby.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ppd.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ptn.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vtb.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://llp.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ezm.yongpay.top

[F08] 遍历目录
来源：http://qnp.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oto.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nyw.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://lmg.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://xgt.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nuy.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tif.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://tzp.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://ccc.sweek.top

[F09] 获取文件大小
来源：http://yjf.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://dik.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://zbu.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://xca.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://jui.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://cln.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vbl.smart0.xyz

Ruby: File.size("a.txt")
来源：http://rdq.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://shw.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://cgs.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bbq.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iuf.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cly.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://bkl.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rpm.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vub.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kxc.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pse.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://axy.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ueu.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nof.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyd.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kto.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ire.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzv.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lfm.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://upl.pycfn.com

[F12] CSV 读写
来源：http://mho.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cnt.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ceq.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gex.cucudq.cn

TS:   // 同上
来源：http://zef.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lmb.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fhv.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tub.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iay.gzhubu.top

================================================================================
来源：http://cil.yfazqb.com

G. 面向对象
来源：http://dbh.yongpay.top

================================================================================
来源：http://fon.yueranfly.top

[G01] 定义类
来源：http://tmn.ywan-chungtsiang.top

Py:   class User: pass
来源：http://xqv.fanxiaobao.xyz

PHP:  class User {}
来源：http://skf.gogol.net.cn

JS:   class User {}
来源：http://xzm.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://rtu.ctjpmb.com

Java: class User {}
来源：http://yow.dashuyun.cn

Go:   type User struct { Name string }
来源：http://rjs.snrcjt.cn

Ruby: class User; end
来源：http://ewv.ybcxt.top

C#:   class User {}
来源：http://wxi.zhaomingkeji.xyz

[G02] 构造函数
来源：http://xtg.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://yqd.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://xtd.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://lnm.pycfn.com

TS:   constructor(public name: string) {}
来源：http://kgr.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://mia.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rwp.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://jdu.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://dsl.jinghuilouyu.cn

[G03] 实例属性
来源：http://ceq.smart0.xyz

Py:   self.name = "x"
来源：http://iwb.cucudq.cn

PHP:  public string $name = "x";
来源：http://ppp.zycfv.cn

JS:   this.name = "x";
来源：http://ppa.sysykeji.top

TS:   name: string = "x";
来源：http://wee.uphjek.com

Java: private String name;
来源：http://euy.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ckb.pycfn.com

Ruby: @name = "x"
来源：http://avk.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://asn.zhiwuduotai.top

[G04] 定义方法
来源：http://ngg.yj20258.top

Py:   def greet(self): return self.name
来源：http://hbp.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rtm.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://cbo.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://xop.iojbl.cn

Java: String greet() { return name; }
来源：http://tuc.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ebn.redwolf501.top

Ruby: def greet; @name; end
来源：http://bkm.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://ayb.yonumen.top

[G05] 继承
来源：http://mtp.nanxinkj.top

Py:   class Admin(User): pass
来源：http://ziz.cashguo.top

PHP:  class Admin extends User {}
来源：http://abw.shzxlz.cn

JS:   class Admin extends User {}
来源：http://dui.redwolf501.top

TS:   class Admin extends User {}
来源：http://aak.sufxvd.cn

Java: class Admin extends User {}
来源：http://fuy.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iek.fengsongda.top

Ruby: class Admin < User; end
来源：http://wbj.chenlongwang.top

C#:   class Admin : User {}
来源：http://mev.shuidangran.top

[G06] 重写方法
来源：http://ias.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://zae.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://psh.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://nmh.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://sxa.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://lrt.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hyf.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://ubx.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://nye.guannengcc.top

[G07] 调用父类方法
来源：http://tev.quarkkingdee.top

Py:   super().greet()
来源：http://yoi.bjfxy.top

PHP:  parent::greet();
来源：http://epq.havefunace.top

JS:   super.greet();
来源：http://aii.ywan-chungtsiang.top

TS:   super.greet();
来源：http://dgv.jiagoushi.top

Java: super.greet();
来源：http://ubo.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qge.hesvh.cn

Ruby: super
来源：http://srk.c1oappe.top

C#:   base.Greet();
来源：http://qpg.zhengqikj.top

[G08] 静态方法与属性
来源：http://obp.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hkg.meibo888.top

PHP:  public static function f() {}
来源：http://kci.shzxlz.cn

JS:   static f() {}
来源：http://fot.smart0.xyz

TS:   static f(): void {}
来源：http://jmz.shangyingyoupin.top

Java: static void f() {}
来源：http://ojk.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dpn.xuetiantiany.cn

Ruby: def self.f; end
来源：http://ovc.cucudq.cn

C#:   public static void F() {}
来源：http://sss.zycfv.cn

[G09] 接口 / 抽象类
来源：http://bvw.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://smo.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pbf.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pea.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://ryj.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://deo.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://mtg.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kue.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://vnl.yangfankeji.com

[G10] 访问控制
来源：http://hcv.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://qdw.jlsjyb.cn

PHP:  public / protected / private
来源：http://xqx.hammf.cn

JS:   #private 字段；其余公开
来源：http://qzl.nanxuanxn.top

TS:   public / protected / private
来源：http://gnu.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://qpw.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bwa.yuxming.cn

Ruby: public / protected / private
来源：http://xus.nwbrower.top

C#:   public / protected / private / internal
来源：http://fbx.dianchejie.cn

[G11] getter / setter
来源：http://yol.cashguo.top

Py:   @property 与 @x.setter
来源：http://bni.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://quk.daxiang520.top

JS:   get name() { return this._name; }
来源：http://dwd.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://aas.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://ybc.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://flj.316326.xyz

Ruby: attr_accessor :name
来源：http://tag.pycfn.com

C#:   public string Name { get; set; }
来源：http://ymi.zhoulong.xyz

[G12] 对象转字符串
来源：http://obx.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://wph.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jzl.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://rsw.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://wbr.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://eog.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://isz.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://qpn.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://hrp.tanke756.top

[G13] 判断对象类型
来源：http://cnp.daxiang520.top

Py:   isinstance(u, User)
来源：http://rtm.yangfankeji.com

PHP:  $u instanceof User
来源：http://leb.yuanzhike.top

JS:   u instanceof User
来源：http://pug.ydzc1.top

TS:   u instanceof User
来源：http://xwh.316326.xyz

Java: u instanceof User
来源：http://aah.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://fzi.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://vow.fzhhl.top

C#:   u is User
来源：http://xjt.xylfe.cn

[G14] 数据类 / record
来源：http://qwu.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://roh.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://bol.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://gjv.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://zao.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://bso.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://kji.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dwv.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://sda.dashuyun.cn

[G15] 枚举
来源：http://cqs.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jzb.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yql.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qzf.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bmm.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://okz.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gte.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://gtd.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nwd.yongpay.top

[G16] 对象转数组 / 字典
来源：http://lcg.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ceg.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://sir.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://lwy.yfazqb.com

TS:   Object.entries(obj)
来源：http://lnp.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hll.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zjn.fengsongda.top

Ruby: obj.instance_variables
来源：http://wza.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://uuv.zhixingplan.top

================================================================================
来源：http://ogi.nanxinkj.top

H. 异常与错误处理
来源：http://rav.dashuyun.cn

================================================================================
来源：http://wgu.tanke756.top

[H01] try / catch 基础
来源：http://wqj.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://axu.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ymg.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yna.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pdx.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qeb.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xab.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eyz.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zuv.ivvv.top

[H02] finally / ensure 收尾
来源：http://equ.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://cmk.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gpf.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ukg.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://xhq.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://irc.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zhh.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eyu.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qvu.bbcook.cn

[H03] 主动抛出异常
来源：http://ung.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://xjk.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nuo.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://xhz.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://fcz.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qdu.tanke756.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ren.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hje.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://tkp.yvedp.cn

[H04] 自定义异常类型
来源：http://xfl.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://kim.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://gsy.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://xig.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://lyr.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://tnp.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://axn.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://tjk.smart0.xyz

C#:   class MyException : Exception {}
来源：http://ufe.sweek.top

[H05] 捕获特定类型
来源：http://wah.bjfxy.top

Py:   except ValueError as e:
来源：http://lon.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://psb.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ugd.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://epj.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://bya.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hcq.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://oms.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qbo.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://jkp.cucudq.cn


<!-- 参考信息 -->