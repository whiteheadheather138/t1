代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gnb.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ogn.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yob.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://afk.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://doa.jinqigufen.top

[F02] 逐行读取文件
来源：http://pbk.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mim.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://boi.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ysl.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aif.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vpm.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ocb.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ktt.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zub.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://tif.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://upn.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ngp.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jbs.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://olt.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tiy.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bvz.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://xme.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://myi.zdbjq.cn

[F04] 追加写入文件
来源：http://ydz.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cmv.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tnj.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cxr.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fyj.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oqt.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tin.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hpv.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wyr.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://lqu.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cgd.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://yjc.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://pdo.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://tht.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dml.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qbi.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://hrk.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://hda.cucudq.cn

[F06] 删除文件
来源：http://tvk.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://osk.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://ttn.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://kck.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cdq.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhl.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://jwo.meibo888.top

Ruby: File.delete("a.txt")
来源：http://gov.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://zno.zycfv.cn

[F07] 创建目录（含多级）
来源：http://xjc.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glv.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://orc.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bbo.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qln.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wog.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lgs.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dhv.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cnt.aizwys.cn

[F08] 遍历目录
来源：http://cjk.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vmd.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rmm.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://rkf.nanxuanxn.top

TS:   fs.readdirSync("dir")
来源：http://coj.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fyx.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lpf.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://eum.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://css.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://tqr.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://hhv.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://asc.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://hms.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://smb.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://prx.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ydh.316326.xyz

Ruby: File.size("a.txt")
来源：http://xye.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://mnm.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://mja.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zcl.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kst.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rbx.mhx1999.top

TS:   path.extname("a.txt")
来源：http://bop.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nys.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oic.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rnz.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ihw.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://oqy.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nio.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zws.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyj.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mjq.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obu.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://krl.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://udu.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xhs.hysaishi.cn

[F12] CSV 读写
来源：http://lua.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eri.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zxd.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://epv.fengsongda.top

TS:   // 同上
来源：http://iiv.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://azn.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyf.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kmj.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vlo.hongshengwenyu.top

================================================================================
来源：http://zcd.vehdjk.com

G. 面向对象
来源：http://yhp.cqqwz.cn

================================================================================
来源：http://ryv.hcnkem.com

[G01] 定义类
来源：http://wxx.hammf.cn

Py:   class User: pass
来源：http://ryf.zdqjudy.top

PHP:  class User {}
来源：http://vev.guannengcc.top

JS:   class User {}
来源：http://mqt.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://wqh.sufxvd.cn

Java: class User {}
来源：http://xgk.xziqi.cn

Go:   type User struct { Name string }
来源：http://igr.yfazqb.com

Ruby: class User; end
来源：http://zjy.xingfuxueyuan.xyz

C#:   class User {}
来源：http://ffi.zhoulong.xyz

[G02] 构造函数
来源：http://lss.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://sad.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://iwn.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://qhf.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://tfb.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://qpf.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://btm.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://nkz.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://qyd.wangshuangyany.cn

[G03] 实例属性
来源：http://dvl.bjfxy.top

Py:   self.name = "x"
来源：http://lsn.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://vku.fzhhl.top

JS:   this.name = "x";
来源：http://isd.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://mte.cdnleiting.top

Java: private String name;
来源：http://tlo.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zmd.yuxming.cn

Ruby: @name = "x"
来源：http://gum.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://yjx.yonumen.top

[G04] 定义方法
来源：http://kxk.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://xaa.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dot.yj20258.top

JS:   greet() { return this.name; }
来源：http://dbj.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://oct.nanxinkj.top

Java: String greet() { return name; }
来源：http://tnz.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xkg.yuanzhike.top

Ruby: def greet; @name; end
来源：http://jay.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://qjl.hammf.cn

[G05] 继承
来源：http://yfn.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://omu.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://kgd.xylfe.cn

JS:   class Admin extends User {}
来源：http://uih.hammf.cn

TS:   class Admin extends User {}
来源：http://ggk.ehwqpu.com

Java: class Admin extends User {}
来源：http://xzq.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ixs.yfazqb.com

Ruby: class Admin < User; end
来源：http://kvx.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://lhk.aizwys.cn

[G06] 重写方法
来源：http://prj.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://zsn.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://twn.havefunace.top

JS:   greet() { return "admin"; }
来源：http://ndf.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://fht.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://yzi.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://adt.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://fkh.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://eni.pengpengdd.cyou

[G07] 调用父类方法
来源：http://fle.nanxuanxn.top

Py:   super().greet()
来源：http://iak.ppjwa.cn

PHP:  parent::greet();
来源：http://zhi.cheryme.top

JS:   super.greet();
来源：http://uxt.hfpthk.cn

TS:   super.greet();
来源：http://fjt.snrcjt.cn

Java: super.greet();
来源：http://lge.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bjf.birdmap.top

Ruby: super
来源：http://zft.52xcode.cn

C#:   base.Greet();
来源：http://alv.hfpthk.cn

[G08] 静态方法与属性
来源：http://oan.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pkh.cheryme.top

PHP:  public static function f() {}
来源：http://nlk.gzhubu.top

JS:   static f() {}
来源：http://erb.ydjk.org.cn

TS:   static f(): void {}
来源：http://hsa.shangyingyoupin.top

Java: static void f() {}
来源：http://gsv.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eeh.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://hxk.wangdashe.top

C#:   public static void F() {}
来源：http://cer.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://muv.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://ecq.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mxk.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nth.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://ter.fengsongda.top

Java: interface Shape { double area(); }
来源：http://ggl.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://gcb.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dsr.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://evl.nanxuanxn.top

[G10] 访问控制
来源：http://rbl.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://hep.yfazqb.com

PHP:  public / protected / private
来源：http://txl.fktsv.cn

JS:   #private 字段；其余公开
来源：http://uob.chenlongwang.top

TS:   public / protected / private
来源：http://zbt.yj202588.top

Java: public / protected / private / 默认包级
来源：http://rwh.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://myx.pengpengdd.cyou

Ruby: public / protected / private
来源：http://kbx.andypj.xyz

C#:   public / protected / private / internal
来源：http://ldr.ywan-chungtsiang.top

[G11] getter / setter
来源：http://bja.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://peq.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rtp.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://fqm.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://ava.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://ooa.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bwh.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://lqd.tian-w.cn

C#:   public string Name { get; set; }
来源：http://jzt.yuanzhike.top

[G12] 对象转字符串
来源：http://kus.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://gtc.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yzh.fktsv.cn

JS:   toString() { return this.name; }
来源：http://gcx.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://sls.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://wrn.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://wab.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://oyn.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://xgt.xuetiantiany.cn

[G13] 判断对象类型
来源：http://qko.cqqwz.cn

Py:   isinstance(u, User)
来源：http://zfw.vqdsnc.cn

PHP:  $u instanceof User
来源：http://jot.cdnleiting.top

JS:   u instanceof User
来源：http://awv.jianghu66.top

TS:   u instanceof User
来源：http://dzg.tian-w.cn

Java: u instanceof User
来源：http://nuv.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://mhb.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://xyq.hfpthk.cn

C#:   u is User
来源：http://czg.hywenlv.cn

[G14] 数据类 / record
来源：http://lpk.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xph.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://gaj.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://hza.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://lsi.bbcook.cn

Java: record User(String name, int age) {}
来源：http://kxw.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://ina.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zoi.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://ikm.jinyuanbaomall.cn

[G15] 枚举
来源：http://apq.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pvs.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ifc.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://znt.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bei.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://jrt.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axn.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://hrl.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rby.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://kde.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://euu.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://ftk.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://pot.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://dxy.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zhc.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tkc.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://qnw.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://tkl.gotoacloud.top

================================================================================
来源：http://doc.tian-w.cn

H. 异常与错误处理
来源：http://arx.xinyue.icu

================================================================================
来源：http://ldq.dianchejie.cn

[H01] try / catch 基础
来源：http://uzi.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://com.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsw.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bbv.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xeq.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwg.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://atk.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yho.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ilo.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://nnq.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bxm.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ggq.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jbp.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rds.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://ubo.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://has.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://baj.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xvq.tianlin.xyz

[H03] 主动抛出异常
来源：http://hty.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://hwy.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dfv.pycfn.com

JS:   throw new Error("错误信息");
来源：http://cwy.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://xzj.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://grs.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gjr.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://poo.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://des.svipenyu.cn

[H04] 自定义异常类型
来源：http://van.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://ziv.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://yhn.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://str.cheryme.top

TS:   class MyError extends Error {}
来源：http://zir.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://eoa.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://akc.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://kxq.c1oappe.top

C#:   class MyException : Exception {}
来源：http://ugh.yonumen.top

[H05] 捕获特定类型
来源：http://bjd.gogol.net.cn

Py:   except ValueError as e:
来源：http://jxg.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gav.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://jfj.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://czr.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://sol.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rrd.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://fks.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nwp.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://tyl.xylfe.cn


<!-- 参考信息 -->