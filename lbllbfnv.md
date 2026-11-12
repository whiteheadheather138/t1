代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://fka.mhx1999.top

[F02] 逐行读取文件
来源：http://rul.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://opg.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pvo.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fug.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tnn.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nur.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ulg.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lze.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://brl.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://dbb.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ymh.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jhy.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfb.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://adi.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://edr.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jtf.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://cgv.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gkc.wangshuangyany.cn

[F04] 追加写入文件
来源：http://jwa.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sak.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ohs.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uma.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzg.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mmf.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://klz.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xzn.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rya.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://pfe.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vmi.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://fas.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://mzf.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://fji.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jru.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ema.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://aso.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://xsx.jinqigufen.top

[F06] 删除文件
来源：http://vhk.xziqi.cn

Py:   os.remove("a.txt")
来源：http://njh.fehbvm.com

PHP:  unlink("a.txt");
来源：http://etz.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://fbl.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zqj.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhy.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://aus.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://dwv.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://mup.guannengcc.top

[F07] 创建目录（含多级）
来源：http://xzr.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rpu.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qar.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://daj.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hij.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfk.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qic.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tht.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://imv.ydjk.org.cn

[F08] 遍历目录
来源：http://tus.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ntv.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mho.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://yzf.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://gim.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ozw.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://btr.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://wyl.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://epg.chenlongwang.top

[F09] 获取文件大小
来源：http://jrb.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://wxu.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://xyf.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://ohq.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://wfq.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://xii.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pqb.sxryk.cn

Ruby: File.size("a.txt")
来源：http://xyz.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://aof.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://jhz.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://frv.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cpm.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eyu.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://iyu.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rbg.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xvw.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ajh.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nuc.kuanghao11.cn

[F11] 复制与移动文件
来源：http://ahm.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nja.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ern.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xnk.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cce.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vda.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kwg.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wof.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://epx.hfpthk.cn

[F12] CSV 读写
来源：http://sdk.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oes.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ngi.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bte.gotoacloud.top

TS:   // 同上
来源：http://mwx.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qha.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cxh.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nou.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iuw.ydjk.org.cn

================================================================================
来源：http://zcx.zhongyouzk.top

G. 面向对象
来源：http://xld.hysaishi.cn

================================================================================
来源：http://itm.svipenyu.cn

[G01] 定义类
来源：http://pyz.vehdjk.com

Py:   class User: pass
来源：http://eeb.jyoumei.cn

PHP:  class User {}
来源：http://jdf.iojbl.cn

JS:   class User {}
来源：http://gxy.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://jzj.yongpay.top

Java: class User {}
来源：http://vgh.yvedp.cn

Go:   type User struct { Name string }
来源：http://uyj.gogol.net.cn

Ruby: class User; end
来源：http://pao.jinqigfzy.top

C#:   class User {}
来源：http://keh.shangyingyoupin.top

[G02] 构造函数
来源：http://cxp.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://fim.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://tol.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://efu.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://fjf.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://aoa.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uyb.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://qkn.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://zjo.zhiwuduotai.top

[G03] 实例属性
来源：http://ezt.andypj.xyz

Py:   self.name = "x"
来源：http://puq.sxryk.cn

PHP:  public string $name = "x";
来源：http://qvv.jinqigfzy.top

JS:   this.name = "x";
来源：http://fhz.shzxlz.cn

TS:   name: string = "x";
来源：http://zih.pycfn.com

Java: private String name;
来源：http://dcn.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ktg.tian-w.cn

Ruby: @name = "x"
来源：http://fml.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://wvj.yvedp.cn

[G04] 定义方法
来源：http://hes.c1oappe.top

Py:   def greet(self): return self.name
来源：http://uki.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iih.smart0.xyz

JS:   greet() { return this.name; }
来源：http://hwj.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://ptx.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://bcm.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tlj.snrcjt.cn

Ruby: def greet; @name; end
来源：http://ded.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://tnj.jlsjyb.cn

[G05] 继承
来源：http://tep.shuidangran.top

Py:   class Admin(User): pass
来源：http://wsp.yangfankeji.com

PHP:  class Admin extends User {}
来源：http://dze.iojbl.cn

JS:   class Admin extends User {}
来源：http://tak.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://glu.bjfxy.top

Java: class Admin extends User {}
来源：http://ndl.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://odo.smart0.xyz

Ruby: class Admin < User; end
来源：http://viu.ydzc1.top

C#:   class Admin : User {}
来源：http://lgo.ehwqpu.com

[G06] 重写方法
来源：http://vwj.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://cex.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dpq.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://wtb.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://yni.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://yie.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpc.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://lgm.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://mov.yonumen.top

[G07] 调用父类方法
来源：http://hsc.tian-w.cn

Py:   super().greet()
来源：http://ckn.ydzc1.top

PHP:  parent::greet();
来源：http://csy.aibaodan.cn

JS:   super.greet();
来源：http://ddh.ehwqpu.com

TS:   super.greet();
来源：http://hbs.tianlin.xyz

Java: super.greet();
来源：http://igb.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jdt.yfazqb.com

Ruby: super
来源：http://ppa.hammf.cn

C#:   base.Greet();
来源：http://vqu.jqgfzy.top

[G08] 静态方法与属性
来源：http://hpa.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://plf.jinqigfzy.top

PHP:  public static function f() {}
来源：http://zml.sweek.top

JS:   static f() {}
来源：http://ctm.yongpay.top

TS:   static f(): void {}
来源：http://iwr.jinqigufen.top

Java: static void f() {}
来源：http://owy.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://veq.cashguo.top

Ruby: def self.f; end
来源：http://oiy.wangshuangyany.cn

C#:   public static void F() {}
来源：http://jjv.havefunace.top

[G09] 接口 / 抽象类
来源：http://ugd.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://hdz.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ayd.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://evk.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://dvu.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://lor.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://mav.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uov.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://upp.hongshengwenyu.top

[G10] 访问控制
来源：http://vgj.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://qez.aibaodan.cn

PHP:  public / protected / private
来源：http://hra.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://gll.yvedp.cn

TS:   public / protected / private
来源：http://byu.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://dwe.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pxb.snrcjt.cn

Ruby: public / protected / private
来源：http://szc.wangdashe.top

C#:   public / protected / private / internal
来源：http://kna.gaohongyu789.top

[G11] getter / setter
来源：http://emq.cheryme.top

Py:   @property 与 @x.setter
来源：http://mki.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pnl.redwolf501.top

JS:   get name() { return this._name; }
来源：http://qah.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://xej.hnqzz.top

Java: public String getName() { return name; }
来源：http://vbu.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gmn.hysaishi.cn

Ruby: attr_accessor :name
来源：http://ygw.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://cug.tanke756.top

[G12] 对象转字符串
来源：http://uup.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://axk.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ymd.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://dwc.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://iab.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://pan.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bat.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://hiu.yj202588.top

C#:   public override string ToString() => Name;
来源：http://gpd.hnqzz.top

[G13] 判断对象类型
来源：http://hnt.vehdjk.com

Py:   isinstance(u, User)
来源：http://axx.ehwqpu.com

PHP:  $u instanceof User
来源：http://xgm.zdqjudy.top

JS:   u instanceof User
来源：http://olc.quarkkingdee.top

TS:   u instanceof User
来源：http://rzs.c1oappe.top

Java: u instanceof User
来源：http://ibz.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cal.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://zhy.wangdashe.top

C#:   u is User
来源：http://lpo.jqgfzy.top

[G14] 数据类 / record
来源：http://unn.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tdu.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://gbv.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sxn.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://whf.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://soa.hammf.cn

Go:   type User struct { Name string; Age int }
来源：http://itk.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ync.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://qnh.hfpthk.cn

[G15] 枚举
来源：http://jzm.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xay.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwo.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsf.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xzz.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://jaw.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uce.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://ele.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://job.pycfn.com

[G16] 对象转数组 / 字典
来源：http://axk.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lju.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://pqt.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://zie.dianchejie.cn

TS:   Object.entries(obj)
来源：http://fcn.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wje.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://yhf.aizwys.cn

Ruby: obj.instance_variables
来源：http://khb.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ugz.yueranfly.top

================================================================================
来源：http://rsq.nanxinkj.top

H. 异常与错误处理
来源：http://ypq.hnxiangtu.top

================================================================================
来源：http://fbv.ehwqpu.com

[H01] try / catch 基础
来源：http://yqv.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vib.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ltl.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jsj.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vts.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://osp.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cbw.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ocb.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fic.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://ped.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zak.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://kay.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ctm.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fmt.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://qof.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zym.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://frj.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mpq.tian-w.cn

[H03] 主动抛出异常
来源：http://car.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://odl.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wzy.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://szo.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://pli.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ycc.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pni.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mfy.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://ajo.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://tba.hammf.cn

Py:   class MyError(Exception): pass
来源：http://krt.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://auc.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://ose.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://cfn.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://cgi.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ypv.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://elq.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://eep.shzxlz.cn

[H05] 捕获特定类型
来源：http://cen.yanxiufei.cn

Py:   except ValueError as e:
来源：http://yqp.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://diz.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://nus.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://kzx.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://acy.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fvf.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://svi.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nln.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://mjn.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://qpa.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ujf.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uos.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tst.316326.xyz


<!-- 参考信息 -->