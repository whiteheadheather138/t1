代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://dtw.sxryk.cn

[F02] 逐行读取文件
来源：http://nag.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wvq.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpo.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://abc.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wky.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tuj.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pni.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxc.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bdk.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://kzu.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rfo.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jak.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gwu.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hax.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://suw.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ddn.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://lsf.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rkv.gogol.net.cn

[F04] 追加写入文件
来源：http://txm.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://roc.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rzt.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpn.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwc.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://evg.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xfi.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fds.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://azs.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://vkb.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jfz.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://eup.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://iqm.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://dig.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wvc.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aeu.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://xly.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://mby.yj202588.top

[F06] 删除文件
来源：http://lgy.xuanzx.com

Py:   os.remove("a.txt")
来源：http://olv.fengsongda.top

PHP:  unlink("a.txt");
来源：http://atd.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://asn.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zwx.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yqn.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://utq.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://dvc.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://kxd.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://yma.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emx.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cqr.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gaf.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsd.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyg.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ujl.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uuf.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvk.ydzc1.top

[F08] 遍历目录
来源：http://wzu.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fwg.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://znd.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://wqe.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://jio.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dkl.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bps.nwbrower.top

Ruby: Dir.children("dir")
来源：http://cei.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://xtw.gaohongyu789.top

[F09] 获取文件大小
来源：http://afa.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://kvb.redwolf501.top

PHP:  filesize("a.txt");
来源：http://jpq.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://uhq.hnqzz.top

TS:   fs.statSync("a.txt").size
来源：http://fkj.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://uvo.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uhd.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://alr.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://ycs.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://iyq.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hhg.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lyb.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://keg.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://ssh.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rru.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hio.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bod.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nyj.hfpthk.cn

[F11] 复制与移动文件
来源：http://cys.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kvq.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aju.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hoj.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://epx.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dgj.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vaf.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dqa.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://czs.shangyingyoupin.top

[F12] CSV 读写
来源：http://xzl.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pbp.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xdg.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qta.cdnleiting.top

TS:   // 同上
来源：http://ngw.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dzg.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gma.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wgx.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jvz.epnwcf.com

================================================================================
来源：http://kpl.52xcode.cn

G. 面向对象
来源：http://xrp.quarkkingdee.top

================================================================================
来源：http://nvf.andypj.xyz

[G01] 定义类
来源：http://jfn.jinqigfzy.top

Py:   class User: pass
来源：http://hcd.cucudq.cn

PHP:  class User {}
来源：http://vyl.0kj1m.cn

JS:   class User {}
来源：http://bbr.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://edi.kuanghao11.cn

Java: class User {}
来源：http://cve.ctjpmb.com

Go:   type User struct { Name string }
来源：http://fxc.hnxiangtu.top

Ruby: class User; end
来源：http://wie.fktsv.cn

C#:   class User {}
来源：http://wee.snrcjt.cn

[G02] 构造函数
来源：http://ukb.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://fmc.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://uvo.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://zdc.havefunace.top

TS:   constructor(public name: string) {}
来源：http://zci.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://yji.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyt.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://uub.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://uwn.jinghuilouyu.cn

[G03] 实例属性
来源：http://gbt.fzhhl.top

Py:   self.name = "x"
来源：http://nme.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://xlv.kuanghao11.cn

JS:   this.name = "x";
来源：http://kbl.haohaochexian.top

TS:   name: string = "x";
来源：http://cwo.xylfe.cn

Java: private String name;
来源：http://dkd.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bzb.epnwcf.com

Ruby: @name = "x"
来源：http://ula.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://ink.zhaomingkeji.xyz

[G04] 定义方法
来源：http://bvh.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://vhg.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nuv.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ejb.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://ngx.zycfv.cn

Java: String greet() { return name; }
来源：http://ybe.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://stf.snrcjt.cn

Ruby: def greet; @name; end
来源：http://hdx.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://zly.chenzaomai.com

[G05] 继承
来源：http://fxd.zycfv.cn

Py:   class Admin(User): pass
来源：http://ceq.pycfn.com

PHP:  class Admin extends User {}
来源：http://mfy.sxryk.cn

JS:   class Admin extends User {}
来源：http://qup.zdqjudy.top

TS:   class Admin extends User {}
来源：http://ozm.sufxvd.cn

Java: class Admin extends User {}
来源：http://msx.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bre.hywenlv.cn

Ruby: class Admin < User; end
来源：http://sdy.bjfxy.top

C#:   class Admin : User {}
来源：http://zsr.jinqigfzy.top

[G06] 重写方法
来源：http://bwp.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://itf.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dzo.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://tjm.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://mpg.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://epq.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://egk.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://tii.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://hme.hnqzz.top

[G07] 调用父类方法
来源：http://kea.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://djs.jinqigfzy.top

PHP:  parent::greet();
来源：http://ngc.andypj.xyz

JS:   super.greet();
来源：http://ycj.hywenlv.cn

TS:   super.greet();
来源：http://lqf.jinyuanbaomall.cn

Java: super.greet();
来源：http://cmc.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vkl.zhongyouzk.top

Ruby: super
来源：http://dpo.hesvh.cn

C#:   base.Greet();
来源：http://ejw.shuidangran.top

[G08] 静态方法与属性
来源：http://kxh.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kuk.gaohongyu789.top

PHP:  public static function f() {}
来源：http://tai.xinyue.icu

JS:   static f() {}
来源：http://acr.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://xom.chenjidiqi.icu

Java: static void f() {}
来源：http://vex.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://zep.hnxiangtu.top

Ruby: def self.f; end
来源：http://vwr.gzhubu.top

C#:   public static void F() {}
来源：http://iau.sweek.top

[G09] 接口 / 抽象类
来源：http://xkv.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://wal.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://pdh.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yzu.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://nhq.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://hpv.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://bnh.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zhj.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://onx.yongpay.top

[G10] 访问控制
来源：http://tzj.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pbb.aibaodan.cn

PHP:  public / protected / private
来源：http://veu.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://xsd.cdnleiting.top

TS:   public / protected / private
来源：http://bql.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://hnd.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yet.yj202588.top

Ruby: public / protected / private
来源：http://mjs.ydzc1.top

C#:   public / protected / private / internal
来源：http://iue.daxiang520.top

[G11] getter / setter
来源：http://bfi.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://iea.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rbm.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://ber.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://qtc.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://kwb.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nkb.jiagoushi.top

Ruby: attr_accessor :name
来源：http://yeg.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://eap.ybcxt.top

[G12] 对象转字符串
来源：http://eao.birdmap.top

Py:   def __str__(self): return self.name
来源：http://ghh.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fyu.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://lse.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://uio.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://hlm.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jyp.aizwys.cn

Ruby: def to_s; @name; end
来源：http://aaw.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://hdy.cdnleiting.top

[G13] 判断对象类型
来源：http://uqh.fktsv.cn

Py:   isinstance(u, User)
来源：http://mvd.nanxuanxn.top

PHP:  $u instanceof User
来源：http://hrh.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://fpm.snrcjt.cn

TS:   u instanceof User
来源：http://tzs.redwolf501.top

Java: u instanceof User
来源：http://ctw.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://koo.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://wzz.shanyushiyangtech.top

C#:   u is User
来源：http://xtw.yuxming.cn

[G14] 数据类 / record
来源：http://qzb.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dtz.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://svr.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hcy.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://txj.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://tyz.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://ujt.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ykm.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://wab.fzhhl.top

[G15] 枚举
来源：http://ukf.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ybz.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://kea.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://onx.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dpe.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://vyw.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dlv.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://xsi.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://avl.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://ump.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://crh.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://ktw.ydzc1.top

JS:   Object.entries(obj)
来源：http://exg.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://mhc.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://esf.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dwn.yueranfly.top

Ruby: obj.instance_variables
来源：http://ziq.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://jng.shzxlz.cn

================================================================================
来源：http://gnp.yuxming.cn

H. 异常与错误处理
来源：http://sgz.cdnleiting.top

================================================================================
来源：http://oty.jlsjyb.cn

[H01] try / catch 基础
来源：http://jde.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://efc.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zbm.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yii.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bgo.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ptv.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sff.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzi.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ajq.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://pyj.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://kep.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dnv.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://tqp.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ull.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://hpu.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mfh.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sfs.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dna.gzhubu.top

[H03] 主动抛出异常
来源：http://lhc.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://hrt.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rfx.ivvv.top

JS:   throw new Error("错误信息");
来源：http://ezs.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://qmu.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vhh.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qhb.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uzx.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://iwm.gaohongyu789.top

[H04] 自定义异常类型
来源：http://siv.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://ddd.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vhu.epnwcf.com

JS:   class MyError extends Error {}
来源：http://ykc.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://bvo.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://jji.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cyu.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://mjx.yueranfly.top

C#:   class MyException : Exception {}
来源：http://wqn.svipenyu.cn

[H05] 捕获特定类型
来源：http://eeq.fehbvm.com

Py:   except ValueError as e:
来源：http://uqa.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vpr.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ddf.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://jyv.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://gvc.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hrn.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://wej.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://thf.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://rxt.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://ynm.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ojc.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://eos.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://uwo.xylfe.cn


<!-- 参考信息 -->