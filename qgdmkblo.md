代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ukt.jiagoushi.top

================================================================================
来源：http://hng.shuidangran.top

F. 文件与目录
来源：http://rlz.vqdsnc.cn

================================================================================
来源：http://rhx.jianghu66.top

[F01] 读取整个文件
来源：http://mae.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mqp.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://ffi.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zlk.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ntq.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bka.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bhh.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://bot.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://duk.ydzc1.top

[F02] 逐行读取文件
来源：http://nje.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yar.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ebm.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vml.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nxy.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jjp.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gwn.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fmr.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rfw.ivvv.top

[F03] 写入文件（覆盖）
来源：http://pbc.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://znm.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lde.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wsg.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdx.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ksf.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bsb.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://pkc.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ftu.tian-w.cn

[F04] 追加写入文件
来源：http://zfs.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwx.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://umk.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ykw.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xcd.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sbv.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pkq.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qus.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fvi.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://iiy.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tmz.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://cgu.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://pem.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://nhs.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wht.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ynh.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://sym.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://zko.hnqzz.top

[F06] 删除文件
来源：http://bfj.gzhubu.top

Py:   os.remove("a.txt")
来源：http://iar.uphjek.com

PHP:  unlink("a.txt");
来源：http://wtz.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qmi.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://jdd.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mpc.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://ajm.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://shq.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://ymc.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://yum.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jda.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wim.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vem.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlw.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rzb.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zmy.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mre.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://doq.pycfn.com

[F08] 遍历目录
来源：http://xxc.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qcg.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oeo.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://rex.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://hti.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hrr.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gsc.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://pst.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://mxm.zhixingplan.top

[F09] 获取文件大小
来源：http://sio.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://seb.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://nhh.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://yic.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://wsh.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://mww.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wji.hnqzz.top

Ruby: File.size("a.txt")
来源：http://cwf.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://gyz.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://cgo.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfk.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lkf.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://knf.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://pwi.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hxl.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gpz.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jsa.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vex.yueranfly.top

[F11] 复制与移动文件
来源：http://smm.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bae.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vmy.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://urd.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqn.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://swk.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oiq.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wpq.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jkn.xylfe.cn

[F12] CSV 读写
来源：http://ijk.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gjf.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iys.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lls.bbcook.cn

TS:   // 同上
来源：http://xtg.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://roz.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ibp.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dgo.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qxm.9152youxi.cn

================================================================================
来源：http://bpw.xingfuxueyuan.xyz

G. 面向对象
来源：http://iou.yuxming.cn

================================================================================
来源：http://ruu.gaohongyu789.top

[G01] 定义类
来源：http://lnh.hammf.cn

Py:   class User: pass
来源：http://bwu.fktsv.cn

PHP:  class User {}
来源：http://ryi.gotoacloud.top

JS:   class User {}
来源：http://mcx.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://pcq.fktsv.cn

Java: class User {}
来源：http://ddp.daxiang520.top

Go:   type User struct { Name string }
来源：http://udp.jlsjyb.cn

Ruby: class User; end
来源：http://vst.9152youxi.cn

C#:   class User {}
来源：http://xys.epnwcf.com

[G02] 构造函数
来源：http://bsk.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://cob.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ira.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://wfo.yongpay.top

TS:   constructor(public name: string) {}
来源：http://fgs.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://hze.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ghi.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://dal.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://dug.zycfv.cn

[G03] 实例属性
来源：http://ffd.dashuyun.cn

Py:   self.name = "x"
来源：http://leq.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://vcx.yj20258888.top

JS:   this.name = "x";
来源：http://cvr.nanxinkj.top

TS:   name: string = "x";
来源：http://llx.316326.xyz

Java: private String name;
来源：http://bgh.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sih.zhiwuduotai.top

Ruby: @name = "x"
来源：http://tin.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://pbo.yanxiufei.cn

[G04] 定义方法
来源：http://voa.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://jto.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxq.xziqi.cn

JS:   greet() { return this.name; }
来源：http://veb.sweek.top

TS:   greet(): string { return this.name; }
来源：http://fgx.mhx1999.top

Java: String greet() { return name; }
来源：http://vai.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://xxk.xziqi.cn

Ruby: def greet; @name; end
来源：http://phc.meibo888.top

C#:   public string Greet() => Name;
来源：http://jzi.zhoulong.xyz

[G05] 继承
来源：http://fuc.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://shn.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://cni.fzhhl.top

JS:   class Admin extends User {}
来源：http://owm.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://sjl.andypj.xyz

Java: class Admin extends User {}
来源：http://gra.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dvi.hammf.cn

Ruby: class Admin < User; end
来源：http://cdg.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://zvt.tianlin.xyz

[G06] 重写方法
来源：http://vsj.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://fwv.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xyy.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://akg.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://wjk.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://lrc.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://soo.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://zzt.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://pcn.cdnleiting.top

[G07] 调用父类方法
来源：http://eev.zhongyouzk.top

Py:   super().greet()
来源：http://vsn.jlsjyb.cn

PHP:  parent::greet();
来源：http://alk.zhengqikj.top

JS:   super.greet();
来源：http://djc.zycfv.cn

TS:   super.greet();
来源：http://jze.yfazqb.com

Java: super.greet();
来源：http://fns.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ums.gogol.net.cn

Ruby: super
来源：http://epu.guannengcc.top

C#:   base.Greet();
来源：http://kzy.snrcjt.cn

[G08] 静态方法与属性
来源：http://buw.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hlk.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://oxx.jyoumei.cn

JS:   static f() {}
来源：http://vay.sweek.top

TS:   static f(): void {}
来源：http://kyw.vehdjk.com

Java: static void f() {}
来源：http://zxr.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tez.sxryk.cn

Ruby: def self.f; end
来源：http://ppc.c1oappe.top

C#:   public static void F() {}
来源：http://tjh.wangdashe.top

[G09] 接口 / 抽象类
来源：http://fvt.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://pbn.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://zyl.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lvc.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://pdy.yueranfly.top

Java: interface Shape { double area(); }
来源：http://wrc.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://lyp.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qtf.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://cua.cheryme.top

[G10] 访问控制
来源：http://pak.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://drv.quarkkingdee.top

PHP:  public / protected / private
来源：http://fsp.jianghu66.top

JS:   #private 字段；其余公开
来源：http://jkm.xziqi.cn

TS:   public / protected / private
来源：http://dhj.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://clt.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmt.zhijiandao.cn

Ruby: public / protected / private
来源：http://bum.ppjwa.cn

C#:   public / protected / private / internal
来源：http://vsf.ydjk.org.cn

[G11] getter / setter
来源：http://rce.zycfv.cn

Py:   @property 与 @x.setter
来源：http://gul.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://use.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://dva.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://klx.cdnleiting.top

Java: public String getName() { return name; }
来源：http://xko.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rkz.uphjek.com

Ruby: attr_accessor :name
来源：http://sfx.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://aog.gogol.net.cn

[G12] 对象转字符串
来源：http://ewn.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://lqw.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cae.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://jdn.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://npq.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://rxo.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://hud.fktsv.cn

Ruby: def to_s; @name; end
来源：http://rsi.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://osb.zdqjudy.top

[G13] 判断对象类型
来源：http://qoz.vehdjk.com

Py:   isinstance(u, User)
来源：http://tjk.gogol.net.cn

PHP:  $u instanceof User
来源：http://gjq.hywenlv.cn

JS:   u instanceof User
来源：http://jee.dianchejie.cn

TS:   u instanceof User
来源：http://kmt.316326.xyz

Java: u instanceof User
来源：http://ono.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://raj.sysykeji.top

Ruby: u.is_a?(User)
来源：http://fym.xuanzx.com

C#:   u is User
来源：http://tlz.zhixingplan.top

[G14] 数据类 / record
来源：http://gtv.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kmk.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://idf.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://vvl.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://pbz.yfazqb.com

Java: record User(String name, int age) {}
来源：http://yuz.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://msq.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rlj.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://iiq.yanxiufei.cn

[G15] 枚举
来源：http://yzl.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hic.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rxi.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://grz.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vku.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://nbz.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zzc.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://yin.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://weh.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://hfa.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jrp.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://vcn.andypj.xyz

JS:   Object.entries(obj)
来源：http://jbe.tanke756.top

TS:   Object.entries(obj)
来源：http://lkl.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://spe.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://szw.hammf.cn

Ruby: obj.instance_variables
来源：http://hgx.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://zcl.yueranfly.top

================================================================================
来源：http://gpr.zhijiandao.cn

H. 异常与错误处理
来源：http://wnc.hcnkem.com

================================================================================
来源：http://drl.jinqigfzy.top

[H01] try / catch 基础
来源：http://ppv.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dwc.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gcu.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dee.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bor.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://doj.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjj.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://trv.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dqs.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://mld.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://gcz.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwv.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zrb.daria6918.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://utg.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://gah.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tmb.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://svx.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oln.epnwcf.com

[H03] 主动抛出异常
来源：http://wpa.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://hhr.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mty.cashguo.top

JS:   throw new Error("错误信息");
来源：http://fkm.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://vrs.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wrz.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zwu.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cov.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ouy.yonumen.top

[H04] 自定义异常类型
来源：http://omh.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://ths.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://rle.cashguo.top

JS:   class MyError extends Error {}
来源：http://hjr.fzhhl.top

TS:   class MyError extends Error {}
来源：http://stu.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://uzu.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vad.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://why.yuxming.cn

C#:   class MyException : Exception {}
来源：http://awz.jlsjyb.cn

[H05] 捕获特定类型
来源：http://ilm.tian-w.cn

Py:   except ValueError as e:
来源：http://mbw.cheryme.top


<!-- 参考信息 -->