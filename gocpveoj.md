代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cye.jqgufenzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tgv.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jbh.cheryme.top

Ruby: File.read("a.txt")
来源：http://cwn.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://nfn.bbcook.cn

[F02] 逐行读取文件
来源：http://bkf.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pob.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vnr.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cli.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pze.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://viy.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kyd.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pty.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mkg.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://xhd.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgc.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kib.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqu.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pgk.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rmv.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvw.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://crg.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pfx.jlsjyb.cn

[F04] 追加写入文件
来源：http://fbl.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://amy.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqz.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ama.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ihe.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ava.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://syx.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xxn.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eon.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://cao.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cyp.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://ucb.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://vfu.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hji.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://grg.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hjt.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://lju.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://zss.ctjpmb.com

[F06] 删除文件
来源：http://krh.epnwcf.com

Py:   os.remove("a.txt")
来源：http://mst.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://lzs.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fgs.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aki.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ooz.tarul.cn

Go:   os.Remove("a.txt")
来源：http://mzw.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://wpp.cashguo.top

C#:   File.Delete("a.txt");
来源：http://omq.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://vqm.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yws.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mqr.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hqh.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uoz.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://euy.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nug.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qfb.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://txg.jinghuilouyu.cn

[F08] 遍历目录
来源：http://ati.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://agl.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aej.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://gqf.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://xhf.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vat.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ayr.bbcook.cn

Ruby: Dir.children("dir")
来源：http://vbu.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://cvi.daxiang520.top

[F09] 获取文件大小
来源：http://ovl.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://tkt.zycfv.cn

PHP:  filesize("a.txt");
来源：http://xmd.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://ijf.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://yew.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://jhv.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ffm.ivvv.top

Ruby: File.size("a.txt")
来源：http://yea.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://sfe.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ylo.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mvz.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zjo.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kto.tarul.cn

TS:   path.extname("a.txt")
来源：http://zot.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ria.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://abz.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ubp.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wgl.yj202588.top

[F11] 复制与移动文件
来源：http://tdc.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yad.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcf.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://brz.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://equ.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncu.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://frj.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hqb.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xqe.xylfe.cn

[F12] CSV 读写
来源：http://ptx.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iru.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://upb.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dql.hfpthk.cn

TS:   // 同上
来源：http://okq.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ttk.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://all.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hlv.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://bym.cqqwz.cn

================================================================================
来源：http://nkz.chenjidiqi.icu

G. 面向对象
来源：http://ang.yj20258.top

================================================================================
来源：http://dfa.9152youxi.cn

[G01] 定义类
来源：http://cbw.svipenyu.cn

Py:   class User: pass
来源：http://bhd.hysaishi.cn

PHP:  class User {}
来源：http://wii.tian-w.cn

JS:   class User {}
来源：http://vbh.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://nuj.snrcjt.cn

Java: class User {}
来源：http://zzk.zdbjq.cn

Go:   type User struct { Name string }
来源：http://fxm.haohaochexian.top

Ruby: class User; end
来源：http://rlc.zdbjq.cn

C#:   class User {}
来源：http://uql.cheryme.top

[G02] 构造函数
来源：http://qzk.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://ypi.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://wxj.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://wqc.cashguo.top

TS:   constructor(public name: string) {}
来源：http://rgj.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://zqv.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kky.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://tuv.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://qcp.yonumen.top

[G03] 实例属性
来源：http://odt.hcnkem.com

Py:   self.name = "x"
来源：http://amt.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://xjg.cheryme.top

JS:   this.name = "x";
来源：http://hnh.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://qqb.tian-w.cn

Java: private String name;
来源：http://rzn.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zui.cqqwz.cn

Ruby: @name = "x"
来源：http://dfr.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://tai.birdmap.top

[G04] 定义方法
来源：http://jsc.yj20258888.top

Py:   def greet(self): return self.name
来源：http://ign.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nxp.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://rxg.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://gsh.xylfe.cn

Java: String greet() { return name; }
来源：http://vwe.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://smw.cdnleiting.top

Ruby: def greet; @name; end
来源：http://zha.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://rgy.hongshengwenyu.top

[G05] 继承
来源：http://ere.hywenlv.cn

Py:   class Admin(User): pass
来源：http://jzm.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://umd.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://seb.yj202588.top

TS:   class Admin extends User {}
来源：http://eev.epnwcf.com

Java: class Admin extends User {}
来源：http://zfh.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://urq.ctjpmb.com

Ruby: class Admin < User; end
来源：http://odw.hnxiangtu.top

C#:   class Admin : User {}
来源：http://nal.c1oappe.top

[G06] 重写方法
来源：http://mff.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://jrw.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uwz.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://sjy.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://zal.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://zyq.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kai.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://pss.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://qaa.ppjwa.cn

[G07] 调用父类方法
来源：http://xyr.zycfv.cn

Py:   super().greet()
来源：http://bri.jlsjyb.cn

PHP:  parent::greet();
来源：http://xup.gzhubu.top

JS:   super.greet();
来源：http://zio.hywenlv.cn

TS:   super.greet();
来源：http://ikv.yfazqb.com

Java: super.greet();
来源：http://prq.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nyq.ydjk.org.cn

Ruby: super
来源：http://ygk.quarkkingdee.top

C#:   base.Greet();
来源：http://tvp.chenlongwang.top

[G08] 静态方法与属性
来源：http://wyu.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yzb.zdqjudy.top

PHP:  public static function f() {}
来源：http://wci.hnqzz.top

JS:   static f() {}
来源：http://blm.0kj1m.cn

TS:   static f(): void {}
来源：http://gpx.yvedp.cn

Java: static void f() {}
来源：http://web.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qfs.pycfn.com

Ruby: def self.f; end
来源：http://aag.cqqwz.cn

C#:   public static void F() {}
来源：http://tvt.bbcook.cn

[G09] 接口 / 抽象类
来源：http://uow.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://heq.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://omp.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cof.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://uda.hammf.cn

Java: interface Shape { double area(); }
来源：http://qmc.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://yqb.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rzt.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://hzo.wangshuangyany.cn

[G10] 访问控制
来源：http://rtu.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://xhn.uphjek.com

PHP:  public / protected / private
来源：http://zfd.tian-w.cn

JS:   #private 字段；其余公开
来源：http://rgo.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://faj.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://ijw.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hrg.zhiwuduotai.top

Ruby: public / protected / private
来源：http://qmj.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://mpa.hysaishi.cn

[G11] getter / setter
来源：http://ezd.iojbl.cn

Py:   @property 与 @x.setter
来源：http://lka.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://reu.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://bbw.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://kor.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://ymn.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://slz.yfazqb.com

Ruby: attr_accessor :name
来源：http://fbx.pycfn.com

C#:   public string Name { get; set; }
来源：http://uon.zhengqikj.top

[G12] 对象转字符串
来源：http://ywx.ivvv.top

Py:   def __str__(self): return self.name
来源：http://kzq.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://twh.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://yex.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://bts.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://kyj.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://cqt.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://zxx.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://jhl.0kj1m.cn

[G13] 判断对象类型
来源：http://skf.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://tui.0kj1m.cn

PHP:  $u instanceof User
来源：http://bxo.fzhhl.top

JS:   u instanceof User
来源：http://ejk.yfazqb.com

TS:   u instanceof User
来源：http://mvg.jinyuanbaomall.cn

Java: u instanceof User
来源：http://szq.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kyq.daria6918.cn

Ruby: u.is_a?(User)
来源：http://uvx.gaohongyu789.top

C#:   u is User
来源：http://cii.zhixingplan.top

[G14] 数据类 / record
来源：http://lkt.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oum.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://awc.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://jjj.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://qlg.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://lfn.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://jyb.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rbt.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://ybk.birdmap.top

[G15] 枚举
来源：http://dpt.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ynr.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ctp.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zmy.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rqd.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://jqu.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dvu.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://ctb.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rru.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://fku.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ybh.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://cdp.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://afj.jianghu66.top

TS:   Object.entries(obj)
来源：http://qob.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lpi.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tds.chenzaomai.com

Ruby: obj.instance_variables
来源：http://bvn.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://cgr.cdnleiting.top

================================================================================
来源：http://jub.gaohongyu789.top

H. 异常与错误处理
来源：http://ehz.pycfn.com

================================================================================
来源：http://joq.nwbrower.top

[H01] try / catch 基础
来源：http://fti.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cib.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gyn.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nlz.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tug.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ttr.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iau.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ura.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uva.bbcook.cn

[H02] finally / ensure 收尾
来源：http://frw.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jbx.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://evy.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gjv.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sur.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tpa.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://tly.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vfn.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://drc.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://skn.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://pzk.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://inq.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://olr.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://vld.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aul.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbj.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vrf.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://qfr.meibo888.top

[H04] 自定义异常类型
来源：http://bkj.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://qbx.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://myk.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://ofo.tarul.cn

TS:   class MyError extends Error {}
来源：http://mce.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://cdv.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dio.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://lji.pycfn.com

C#:   class MyException : Exception {}
来源：http://qeg.cheryme.top

[H05] 捕获特定类型
来源：http://ito.xylfe.cn

Py:   except ValueError as e:
来源：http://xtg.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fhe.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://ljq.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://syd.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://lia.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rau.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://mio.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vov.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://wml.zhongyouzk.top


<!-- 参考信息 -->