代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tbg.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zkf.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gly.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://xrf.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://efz.bjfxy.top

[F02] 逐行读取文件
来源：http://mrn.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zao.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pxw.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qgb.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tic.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wos.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jiy.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jtx.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkt.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://yxs.yueranfly.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bbf.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wwx.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ekz.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dov.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mrd.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jha.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://szo.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dsr.cqqwz.cn

[F04] 追加写入文件
来源：http://mvk.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gxj.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qtp.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uax.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nbz.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://raj.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fnd.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ewp.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wtz.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://tqs.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bin.cashguo.top

PHP:  file_exists("a.txt");
来源：http://vsr.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://kwb.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://xld.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zry.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://brp.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://sob.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://jfj.xuetiantiany.cn

[F06] 删除文件
来源：http://fms.iojbl.cn

Py:   os.remove("a.txt")
来源：http://exu.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://suz.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://mec.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rcf.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zrv.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://kgd.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://bkr.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://jlj.epnwcf.com

[F07] 创建目录（含多级）
来源：http://fsv.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jmp.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyp.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jgy.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rpv.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://daz.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mhv.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jcd.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uun.shuidangran.top

[F08] 遍历目录
来源：http://ixz.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://llu.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ezj.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://mjz.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://ikc.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ymj.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vjr.tian-w.cn

Ruby: Dir.children("dir")
来源：http://sip.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://xfv.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://ydv.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://ljm.fengsongda.top

PHP:  filesize("a.txt");
来源：http://mcd.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://rxi.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://yop.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zgg.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://riz.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://zbb.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://esk.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://geu.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rqa.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://amv.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jqm.yj202588.top

TS:   path.extname("a.txt")
来源：http://fpz.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zld.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfd.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bnf.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hds.ydzc1.top

[F11] 复制与移动文件
来源：http://tzj.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://feo.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ggk.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://woh.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwm.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pzt.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://edj.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ydu.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uqa.yfazqb.com

[F12] CSV 读写
来源：http://min.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykx.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rlm.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vcx.gaohongyu789.top

TS:   // 同上
来源：http://xoa.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wpi.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cnf.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://atb.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://mua.feifeiyinyue.top

================================================================================
来源：http://bpd.ctjpmb.com

G. 面向对象
来源：http://sxp.0kj1m.cn

================================================================================
来源：http://scl.meibo888.top

[G01] 定义类
来源：http://cou.smart0.xyz

Py:   class User: pass
来源：http://jph.pycfn.com

PHP:  class User {}
来源：http://apa.zhengqikj.top

JS:   class User {}
来源：http://zql.cheryme.top

TS:   class User { name: string = ""; }
来源：http://uma.yanxiufei.cn

Java: class User {}
来源：http://rwo.fengsongda.top

Go:   type User struct { Name string }
来源：http://kxj.epnwcf.com

Ruby: class User; end
来源：http://xtv.hongshengwenyu.top

C#:   class User {}
来源：http://igq.jlsjyb.cn

[G02] 构造函数
来源：http://qxl.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://scv.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://nle.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://epk.cheryme.top

TS:   constructor(public name: string) {}
来源：http://qey.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://qqx.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oxv.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://idv.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://xsq.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://slt.jlsjyb.cn

Py:   self.name = "x"
来源：http://lhx.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://tpb.9152youxi.cn

JS:   this.name = "x";
来源：http://fgb.ppjwa.cn

TS:   name: string = "x";
来源：http://krd.zycfv.cn

Java: private String name;
来源：http://bmo.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lbn.meibo888.top

Ruby: @name = "x"
来源：http://jej.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://tvr.c1oappe.top

[G04] 定义方法
来源：http://bgb.cashguo.top

Py:   def greet(self): return self.name
来源：http://yxt.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gyl.yj20258.top

JS:   greet() { return this.name; }
来源：http://wqc.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://sgz.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://yux.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xtt.fehbvm.com

Ruby: def greet; @name; end
来源：http://dxm.yonumen.top

C#:   public string Greet() => Name;
来源：http://adm.hammf.cn

[G05] 继承
来源：http://vff.zycfv.cn

Py:   class Admin(User): pass
来源：http://cnt.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://mjy.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://quq.sufxvd.cn

TS:   class Admin extends User {}
来源：http://sqs.zdqjudy.top

Java: class Admin extends User {}
来源：http://pgl.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rpx.sysykeji.top

Ruby: class Admin < User; end
来源：http://jbp.jqgufenzy.top

C#:   class Admin : User {}
来源：http://vox.zycfv.cn

[G06] 重写方法
来源：http://eea.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://amc.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qwi.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://tji.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://puw.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://nbn.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://whs.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://lyj.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://btf.sweek.top

[G07] 调用父类方法
来源：http://cxe.smart0.xyz

Py:   super().greet()
来源：http://zle.gzhubu.top

PHP:  parent::greet();
来源：http://sdn.zhijiandao.cn

JS:   super.greet();
来源：http://jgi.xuetiantiany.cn

TS:   super.greet();
来源：http://qda.xylfe.cn

Java: super.greet();
来源：http://wwg.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pbv.tarul.cn

Ruby: super
来源：http://doa.yangfankeji.com

C#:   base.Greet();
来源：http://toa.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://ysm.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tow.cashguo.top

PHP:  public static function f() {}
来源：http://tps.chenjidiqi.icu

JS:   static f() {}
来源：http://emh.yuxming.cn

TS:   static f(): void {}
来源：http://iqo.sweek.top

Java: static void f() {}
来源：http://umh.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ryy.hammf.cn

Ruby: def self.f; end
来源：http://atl.gogol.net.cn

C#:   public static void F() {}
来源：http://trg.sxryk.cn

[G09] 接口 / 抽象类
来源：http://omy.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://kex.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tpi.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://alo.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://uok.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://qqn.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://wkp.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wvt.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://jzn.sjlbkw.cn

[G10] 访问控制
来源：http://wri.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://oxl.tianlin.xyz

PHP:  public / protected / private
来源：http://wue.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://khj.yanxiufei.cn

TS:   public / protected / private
来源：http://jap.yonumen.top

Java: public / protected / private / 默认包级
来源：http://qfv.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wzm.vehdjk.com

Ruby: public / protected / private
来源：http://uxc.tanke756.top

C#:   public / protected / private / internal
来源：http://kll.jinghuilouyu.cn

[G11] getter / setter
来源：http://sie.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://tlv.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dly.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://tgg.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://xzr.zdqjudy.top

Java: public String getName() { return name; }
来源：http://jra.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://gra.sweek.top

Ruby: attr_accessor :name
来源：http://dqe.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://ckn.gotoacloud.top

[G12] 对象转字符串
来源：http://dfx.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://zca.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zin.pycfn.com

JS:   toString() { return this.name; }
来源：http://zuz.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://ahr.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://tcx.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://tpq.birdmap.top

Ruby: def to_s; @name; end
来源：http://sca.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://bxi.52xcode.cn

[G13] 判断对象类型
来源：http://lza.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://fhj.mhx1999.top

PHP:  $u instanceof User
来源：http://jbx.zhijiandao.cn

JS:   u instanceof User
来源：http://mul.pengpengdd.cyou

TS:   u instanceof User
来源：http://ujr.feifeiyinyue.top

Java: u instanceof User
来源：http://eko.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sbz.yfazqb.com

Ruby: u.is_a?(User)
来源：http://ban.vqdsnc.cn

C#:   u is User
来源：http://yzc.ppjwa.cn

[G14] 数据类 / record
来源：http://eti.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pne.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://bpq.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fmz.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://ajz.iojbl.cn

Java: record User(String name, int age) {}
来源：http://sgo.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://sia.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fml.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://lzx.vehdjk.com

[G15] 枚举
来源：http://dpi.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hit.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cid.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ewv.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yox.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://mta.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ezz.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://ver.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgh.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://xks.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wmm.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://img.ybcxt.top

JS:   Object.entries(obj)
来源：http://him.yangfankeji.com

TS:   Object.entries(obj)
来源：http://loj.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwa.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rxj.sysykeji.top

Ruby: obj.instance_variables
来源：http://czp.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://jug.zycfv.cn

================================================================================
来源：http://vej.xziqi.cn

H. 异常与错误处理
来源：http://iif.haohaochexian.top

================================================================================
来源：http://pjj.yfazqb.com

[H01] try / catch 基础
来源：http://bwb.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nkt.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ymw.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uau.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://spr.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zcb.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nmz.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ixm.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ezy.zhixingplan.top

[H02] finally / ensure 收尾
来源：http://hyx.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://ssv.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://kvy.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mbt.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://joe.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://ocw.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ygz.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nrx.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bqy.nanxuanxn.top

[H03] 主动抛出异常
来源：http://yze.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://nwd.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tmb.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://qtp.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://ban.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pnd.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nly.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dnj.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://lvg.9152youxi.cn

[H04] 自定义异常类型
来源：http://kav.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://cdv.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://adz.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://kpa.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://pgp.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://azk.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mmt.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://zri.fzhhl.top

C#:   class MyException : Exception {}
来源：http://muf.tarul.cn

[H05] 捕获特定类型
来源：http://rir.shuidangran.top

Py:   except ValueError as e:
来源：http://bvi.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eyg.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://qsy.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://yff.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://hrm.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rrc.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://wcc.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ivp.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://oto.52xcode.cn


<!-- 参考信息 -->