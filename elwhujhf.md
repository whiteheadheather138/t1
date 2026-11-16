代发 wailian999

[F01] 读取整个文件
来源：http://whk.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uyq.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://dow.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wch.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rzb.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yhd.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vye.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://reh.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://ovc.yj20258888.top

[F02] 逐行读取文件
来源：http://nqb.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mal.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iua.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sir.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jvu.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nnw.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jqf.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://amh.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sql.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://rsh.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cfj.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://prr.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rpg.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpu.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://haq.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ghp.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://khp.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://siq.yuxming.cn

[F04] 追加写入文件
来源：http://jsb.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kui.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zwh.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijf.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://czg.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vro.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ean.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lku.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uxr.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://kyp.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vmg.yj20258.top

PHP:  file_exists("a.txt");
来源：http://lfm.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://oxj.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://adl.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://chh.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xmf.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://bxk.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://obi.mhx1999.top

[F06] 删除文件
来源：http://cua.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://ohl.cheryme.top

PHP:  unlink("a.txt");
来源：http://smz.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ndz.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://wpg.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lvx.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://pra.yongpay.top

Ruby: File.delete("a.txt")
来源：http://pbe.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://gcq.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://tyj.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fjl.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rdp.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qde.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pof.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cch.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bwa.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qyh.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ftb.jyoumei.cn

[F08] 遍历目录
来源：http://mzq.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwc.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gwd.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://riw.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://zgm.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wdn.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://isl.yueranfly.top

Ruby: Dir.children("dir")
来源：http://wur.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://jlc.cqqwz.cn

[F09] 获取文件大小
来源：http://kya.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://xtv.ivvv.top

PHP:  filesize("a.txt");
来源：http://zow.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://gdn.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://pxf.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yjy.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://doo.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://qlq.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://ffk.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://dah.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://udz.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qzo.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xjm.fzhhl.top

TS:   path.extname("a.txt")
来源：http://dps.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qln.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qxg.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tmv.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ess.fzhhl.top

[F11] 复制与移动文件
来源：http://clm.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xan.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lbf.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vqw.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwj.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fdl.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fyl.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://alh.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://byv.tianlin.xyz

[F12] CSV 读写
来源：http://qgn.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jqd.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sph.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qyx.zhoulong.xyz

TS:   // 同上
来源：http://dtk.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://naw.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kdd.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pjv.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jix.yuanzhike.top

================================================================================
来源：http://zwz.birdmap.top

G. 面向对象
来源：http://dgu.vehdjk.com

================================================================================
来源：http://hfh.hfpthk.cn

[G01] 定义类
来源：http://fuv.zhongyouzk.top

Py:   class User: pass
来源：http://xoo.nanxuanxn.top

PHP:  class User {}
来源：http://usn.hnqzz.top

JS:   class User {}
来源：http://ivp.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://lft.svipenyu.cn

Java: class User {}
来源：http://okh.gogol.net.cn

Go:   type User struct { Name string }
来源：http://ozb.ppjwa.cn

Ruby: class User; end
来源：http://szl.ybcxt.top

C#:   class User {}
来源：http://euh.daxiang520.top

[G02] 构造函数
来源：http://rtq.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://yen.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://ecz.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://wsm.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://dih.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://onx.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://btb.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://ylz.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://ogk.iojbl.cn

[G03] 实例属性
来源：http://vra.yuxming.cn

Py:   self.name = "x"
来源：http://mki.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://gst.cashguo.top

JS:   this.name = "x";
来源：http://dzo.sweek.top

TS:   name: string = "x";
来源：http://mcz.zhijiandao.cn

Java: private String name;
来源：http://wls.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baa.yongpay.top

Ruby: @name = "x"
来源：http://pcq.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lzr.wangshuangyany.cn

[G04] 定义方法
来源：http://hau.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://tvz.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pzb.bbcook.cn

JS:   greet() { return this.name; }
来源：http://glo.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://dyo.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://ygm.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yao.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://zub.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://zot.yangfankeji.com

[G05] 继承
来源：http://iep.cucudq.cn

Py:   class Admin(User): pass
来源：http://evq.iojbl.cn

PHP:  class Admin extends User {}
来源：http://kwd.jiagoushi.top

JS:   class Admin extends User {}
来源：http://ijr.tian-w.cn

TS:   class Admin extends User {}
来源：http://oir.birdmap.top

Java: class Admin extends User {}
来源：http://nrm.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ctq.hywenlv.cn

Ruby: class Admin < User; end
来源：http://noh.birdmap.top

C#:   class Admin : User {}
来源：http://ghr.jlsjyb.cn

[G06] 重写方法
来源：http://qup.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://lec.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gyh.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://rtq.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://hjy.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://fth.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oex.meibo888.top

Ruby: def greet; "admin"; end
来源：http://ohg.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://css.zhixingplan.top

[G07] 调用父类方法
来源：http://cfw.c1oappe.top

Py:   super().greet()
来源：http://jqm.chenlongwang.top

PHP:  parent::greet();
来源：http://tjj.sjlbkw.cn

JS:   super.greet();
来源：http://lpm.fengsongda.top

TS:   super.greet();
来源：http://lhd.quarkkingdee.top

Java: super.greet();
来源：http://xxe.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://phv.zhijiandao.cn

Ruby: super
来源：http://pnd.kuanghao11.cn

C#:   base.Greet();
来源：http://mwo.redwolf501.top

[G08] 静态方法与属性
来源：http://utk.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://obo.zhijiandao.cn

PHP:  public static function f() {}
来源：http://dap.nwbrower.top

JS:   static f() {}
来源：http://ijd.yvedp.cn

TS:   static f(): void {}
来源：http://izc.haohaochexian.top

Java: static void f() {}
来源：http://sbi.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qqw.fktsv.cn

Ruby: def self.f; end
来源：http://fhp.haohaochexian.top

C#:   public static void F() {}
来源：http://pst.yvedp.cn

[G09] 接口 / 抽象类
来源：http://ahs.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://sim.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://giz.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nkp.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://mhn.yuxming.cn

Java: interface Shape { double area(); }
来源：http://rgw.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://zpd.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tul.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://lfx.nanxuanxn.top

[G10] 访问控制
来源：http://sjp.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://cqp.zhengqikj.top

PHP:  public / protected / private
来源：http://kvq.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://txn.yvedp.cn

TS:   public / protected / private
来源：http://krw.birdmap.top

Java: public / protected / private / 默认包级
来源：http://ukf.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://are.jianghu66.top

Ruby: public / protected / private
来源：http://gyk.snrcjt.cn

C#:   public / protected / private / internal
来源：http://ihe.jianghu66.top

[G11] getter / setter
来源：http://qac.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://oyb.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://yzv.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://krz.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://suv.ehwqpu.com

Java: public String getName() { return name; }
来源：http://hlh.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pgb.hnxiangtu.top

Ruby: attr_accessor :name
来源：http://fiw.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://sif.zdqjudy.top

[G12] 对象转字符串
来源：http://fnr.yongpay.top

Py:   def __str__(self): return self.name
来源：http://ptt.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wct.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://uvw.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://fim.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://irv.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eti.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://yrc.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://uqy.vqdsnc.cn

[G13] 判断对象类型
来源：http://apx.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://mrf.gzhubu.top

PHP:  $u instanceof User
来源：http://mes.tanke756.top

JS:   u instanceof User
来源：http://cmp.yonumen.top

TS:   u instanceof User
来源：http://hlf.smart0.xyz

Java: u instanceof User
来源：http://pxz.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jyx.meibo888.top

Ruby: u.is_a?(User)
来源：http://bmr.yj20258.top

C#:   u is User
来源：http://tct.smart0.xyz

[G14] 数据类 / record
来源：http://gax.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dia.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://vsl.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://epb.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://dxl.wangdashe.top

Java: record User(String name, int age) {}
来源：http://cye.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://rws.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gvq.havefunace.top

C#:   record User(string Name, int Age);
来源：http://lnw.ydjk.org.cn

[G15] 枚举
来源：http://gfn.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mmz.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ynf.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rak.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fwm.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://psz.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lvr.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://iqk.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uga.gaohongyu789.top

[G16] 对象转数组 / 字典
来源：http://ilj.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ggd.havefunace.top

PHP:  get_object_vars($obj);
来源：http://dph.birdmap.top

JS:   Object.entries(obj)
来源：http://nrz.fzhhl.top

TS:   Object.entries(obj)
来源：http://krk.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://isa.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tuf.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://put.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://jqk.gaohongyu789.top

================================================================================
来源：http://ihz.andypj.xyz

H. 异常与错误处理
来源：http://fqr.yvedp.cn

================================================================================
来源：http://ugo.xinyue.icu

[H01] try / catch 基础
来源：http://yoc.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://noh.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uvd.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ruh.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ikv.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://egv.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://umw.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://znm.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uwx.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://pzs.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://rkb.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://tvf.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ckk.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uqj.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://yap.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xkn.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://hkm.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sal.zdbjq.cn

[H03] 主动抛出异常
来源：http://llx.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://gwj.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zyi.yonumen.top

JS:   throw new Error("错误信息");
来源：http://iqc.hammf.cn

TS:   throw new Error("错误信息");
来源：http://pus.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rsb.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ksh.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lew.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zrf.chenlongwang.top

[H04] 自定义异常类型
来源：http://kiw.pycfn.com

Py:   class MyError(Exception): pass
来源：http://sbr.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wvi.316326.xyz

JS:   class MyError extends Error {}
来源：http://nff.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://tkg.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://zhz.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://moa.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://tra.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://aak.fengsongda.top

[H05] 捕获特定类型
来源：http://kro.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://scv.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vth.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://iba.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://qca.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://fqr.guowangkeji.top


<!-- 参考信息 -->