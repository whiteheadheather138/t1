代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ffb.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qwj.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rri.guannengcc.top

Ruby: File.read("a.txt")
来源：http://vtr.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://gvo.zhijiandao.cn

[F02] 逐行读取文件
来源：http://zwb.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ypg.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://njv.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://soj.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpi.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dsr.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pdb.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tcb.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lhs.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://zjg.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dqw.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mhv.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ntk.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ecq.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kxs.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cco.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://rbj.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aqw.iojbl.cn

[F04] 追加写入文件
来源：http://sdb.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bga.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vuk.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxr.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yum.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uuw.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pzp.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbj.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mtb.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://wau.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kiy.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://fpf.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://iap.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://fgw.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cgc.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gnn.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://pty.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://txi.yueranfly.top

[F06] 删除文件
来源：http://nsk.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://dtz.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://rhj.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://llo.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://owm.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cvu.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://hka.meibo888.top

Ruby: File.delete("a.txt")
来源：http://eyy.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://gbp.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://ejw.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xqz.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rks.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cje.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgy.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swe.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ogk.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ukr.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bzm.ivvv.top

[F08] 遍历目录
来源：http://izp.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wyi.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rcf.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://oug.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://raa.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sbg.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xjx.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://soj.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://jwa.aizwys.cn

[F09] 获取文件大小
来源：http://ijn.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://han.xziqi.cn

PHP:  filesize("a.txt");
来源：http://fki.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://hiz.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://fkm.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kgw.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fku.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://vgm.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://aub.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://rrg.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rbw.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rvt.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbh.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://qyk.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lhk.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ypb.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lsw.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhp.fehbvm.com

[F11] 复制与移动文件
来源：http://pig.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cvt.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqm.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qkt.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://omq.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wrf.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zdd.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zuu.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fzz.hywenlv.cn

[F12] CSV 读写
来源：http://qfj.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pkn.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zop.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ync.aibaodan.cn

TS:   // 同上
来源：http://pso.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ajn.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://grz.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ija.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://txt.hammf.cn

================================================================================
来源：http://iwu.zhengqikj.top

G. 面向对象
来源：http://ukn.xingfuxueyuan.xyz

================================================================================
来源：http://qet.ydzc1.top

[G01] 定义类
来源：http://mjt.shanyushiyangkeji.top

Py:   class User: pass
来源：http://fvb.mhx1999.top

PHP:  class User {}
来源：http://skd.smart0.xyz

JS:   class User {}
来源：http://udb.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://had.xuanzx.com

Java: class User {}
来源：http://tkt.birdmap.top

Go:   type User struct { Name string }
来源：http://xyz.shanyushiyangkeji.top

Ruby: class User; end
来源：http://uuv.c1oappe.top

C#:   class User {}
来源：http://rci.hfpthk.cn

[G02] 构造函数
来源：http://pqt.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://yvv.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://had.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://qdk.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://fxh.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://lee.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yzi.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://iid.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://cvc.cqqwz.cn

[G03] 实例属性
来源：http://vid.yj202588.top

Py:   self.name = "x"
来源：http://mly.sysykeji.top

PHP:  public string $name = "x";
来源：http://rhm.chenlongwang.top

JS:   this.name = "x";
来源：http://xpe.tanke756.top

TS:   name: string = "x";
来源：http://few.sxryk.cn

Java: private String name;
来源：http://wbz.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mwt.c1oappe.top

Ruby: @name = "x"
来源：http://tsx.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://yup.jqgfzy.top

[G04] 定义方法
来源：http://alv.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://ghu.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hvc.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://rnd.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://sdg.birdmap.top

Java: String greet() { return name; }
来源：http://inn.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltt.cheryme.top

Ruby: def greet; @name; end
来源：http://uya.sxryk.cn

C#:   public string Greet() => Name;
来源：http://ugg.ppjwa.cn

[G05] 继承
来源：http://hvm.aizwys.cn

Py:   class Admin(User): pass
来源：http://cld.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://mql.redwolf501.top

JS:   class Admin extends User {}
来源：http://hes.c1oappe.top

TS:   class Admin extends User {}
来源：http://sue.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://sqx.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ttd.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://uie.ctjpmb.com

C#:   class Admin : User {}
来源：http://jwn.jyoumei.cn

[G06] 重写方法
来源：http://jxj.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://qsn.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://qwv.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://mgc.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://uwi.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://stj.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ynf.yonumen.top

Ruby: def greet; "admin"; end
来源：http://xto.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://evc.xinyue.icu

[G07] 调用父类方法
来源：http://pel.ppjwa.cn

Py:   super().greet()
来源：http://ffu.ydzc1.top

PHP:  parent::greet();
来源：http://nid.daxiang520.top

JS:   super.greet();
来源：http://nek.shzxlz.cn

TS:   super.greet();
来源：http://zuw.fehbvm.com

Java: super.greet();
来源：http://qkr.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hnz.sweek.top

Ruby: super
来源：http://yqj.guannengcc.top

C#:   base.Greet();
来源：http://nof.snrcjt.cn

[G08] 静态方法与属性
来源：http://gwm.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ufk.daxiang520.top

PHP:  public static function f() {}
来源：http://jzf.snrcjt.cn

JS:   static f() {}
来源：http://lma.hongshengwenyu.top

TS:   static f(): void {}
来源：http://mvq.yongpay.top

Java: static void f() {}
来源：http://eix.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pvc.zhijiandao.cn

Ruby: def self.f; end
来源：http://kpj.yonumen.top

C#:   public static void F() {}
来源：http://tee.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://ejv.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://wts.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://pww.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://iwt.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://cxl.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://ujf.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://ewc.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sva.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://sip.vehdjk.com

[G10] 访问控制
来源：http://sno.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://ega.yueranfly.top

PHP:  public / protected / private
来源：http://nhb.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://rva.yvedp.cn

TS:   public / protected / private
来源：http://olf.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://oqx.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kka.yueranfly.top

Ruby: public / protected / private
来源：http://sob.xinyue.icu

C#:   public / protected / private / internal
来源：http://ekg.shuidangran.top

[G11] getter / setter
来源：http://bck.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://lqz.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://imx.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://mrf.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://kux.cheryme.top

Java: public String getName() { return name; }
来源：http://rbq.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ccx.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://iie.yueranfly.top

C#:   public string Name { get; set; }
来源：http://wwz.bbcook.cn

[G12] 对象转字符串
来源：http://iit.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://mca.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uau.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://fhy.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://wfd.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://elt.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://kgn.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://ozh.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://mbh.sufxvd.cn

[G13] 判断对象类型
来源：http://qbf.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://zzz.sysykeji.top

PHP:  $u instanceof User
来源：http://boj.fktsv.cn

JS:   u instanceof User
来源：http://daw.zhixingplan.top

TS:   u instanceof User
来源：http://ofs.c1oappe.top

Java: u instanceof User
来源：http://ufi.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://iwg.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://qco.zhoulong.xyz

C#:   u is User
来源：http://oyf.gogol.net.cn

[G14] 数据类 / record
来源：http://jyy.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://osq.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://cgt.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ocv.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://ewz.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://umn.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://mlc.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://llw.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://yex.yvedp.cn

[G15] 枚举
来源：http://zyo.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kfu.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://crk.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mgt.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tic.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://zay.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ldi.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://ivb.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vsx.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://nup.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nre.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://tvb.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://pmy.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://orc.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ztz.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://srs.ppjwa.cn

Ruby: obj.instance_variables
来源：http://zov.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://zgx.zhijiandao.cn

================================================================================
来源：http://xvr.yfazqb.com

H. 异常与错误处理
来源：http://dgc.epnwcf.com

================================================================================
来源：http://cvd.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://smu.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pze.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jkh.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://abb.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ezp.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wfj.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ftj.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wlw.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nne.cheryme.top

[H02] finally / ensure 收尾
来源：http://gde.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://iwn.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gdk.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://atj.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sqh.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tdh.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://khq.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ynb.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ybg.jyoumei.cn

[H03] 主动抛出异常
来源：http://thd.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://vvt.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qqy.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://zup.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://ist.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nrg.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxn.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://dkh.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://lta.jlsjyb.cn

[H04] 自定义异常类型
来源：http://ozt.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://eqt.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mih.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://ygd.daria6918.cn

TS:   class MyError extends Error {}
来源：http://rup.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://dbg.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://emc.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://atg.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://mpy.pycfn.com

[H05] 捕获特定类型
来源：http://knt.hywenlv.cn

Py:   except ValueError as e:
来源：http://dih.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ilw.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://ewk.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://fcb.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://hdt.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ynh.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://mmt.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pue.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://jpr.vqdsnc.cn


<!-- 参考信息 -->