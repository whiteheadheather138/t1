代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://buy.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zug.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ybm.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kjv.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pjf.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ovi.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://jft.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rnq.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wmg.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tsc.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://htu.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://awg.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ioh.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://nvp.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vlb.iojbl.cn

[F04] 追加写入文件
来源：http://zrs.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zmk.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uor.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://drz.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwy.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xow.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mlg.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://igc.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jjh.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://xrw.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qxp.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://xlp.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://kau.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://blw.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ubb.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oer.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://xyr.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://vys.ehwqpu.com

[F06] 删除文件
来源：http://ptq.c1oappe.top

Py:   os.remove("a.txt")
来源：http://seu.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://hez.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gcr.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://haq.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dqa.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://cdc.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://mho.tarul.cn

C#:   File.Delete("a.txt");
来源：http://maj.xziqi.cn

[F07] 创建目录（含多级）
来源：http://ife.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xye.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://prt.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fjy.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfw.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://izo.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rrt.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mmp.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ilz.bjfxy.top

[F08] 遍历目录
来源：http://mlj.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pkx.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xzy.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://ehs.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://fdq.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://elr.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://slx.birdmap.top

Ruby: Dir.children("dir")
来源：http://qvm.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://whk.redwolf501.top

[F09] 获取文件大小
来源：http://hps.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://poi.bbcook.cn

PHP:  filesize("a.txt");
来源：http://quh.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://gyw.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://gru.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uzw.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ioc.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://bvt.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://jri.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://bja.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgq.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xkf.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vjh.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://qwl.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ojr.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mip.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vwg.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rmb.snrcjt.cn

[F11] 复制与移动文件
来源：http://mkt.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kus.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mrv.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edo.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nxh.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uzi.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qaz.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jhd.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yvn.xuetiantiany.cn

[F12] CSV 读写
来源：http://hap.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ezk.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gou.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://daz.yonumen.top

TS:   // 同上
来源：http://hdh.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rvn.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hra.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pdt.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rcn.bbcook.cn

================================================================================
来源：http://xtj.52xcode.cn

G. 面向对象
来源：http://dxa.aizwys.cn

================================================================================
来源：http://znf.feifeiyinyue.top

[G01] 定义类
来源：http://xon.redwolf501.top

Py:   class User: pass
来源：http://ent.shanyushiyangkeji.top

PHP:  class User {}
来源：http://lvc.jinqigufen.top

JS:   class User {}
来源：http://yry.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://ujv.iojbl.cn

Java: class User {}
来源：http://pys.yvedp.cn

Go:   type User struct { Name string }
来源：http://xzs.yuanzhike.top

Ruby: class User; end
来源：http://wie.ydjk.org.cn

C#:   class User {}
来源：http://evn.xuanzx.com

[G02] 构造函数
来源：http://ing.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://gwv.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://pwc.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://ecn.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://leo.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://hgt.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://egw.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://dkj.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://gbf.iojbl.cn

[G03] 实例属性
来源：http://eaw.jqgufenzy.top

Py:   self.name = "x"
来源：http://anj.meibo888.top

PHP:  public string $name = "x";
来源：http://cmc.guowangkeji.top

JS:   this.name = "x";
来源：http://wbq.jqgfzy.top

TS:   name: string = "x";
来源：http://qsu.kuanghao11.cn

Java: private String name;
来源：http://uia.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hpx.shuidangran.top

Ruby: @name = "x"
来源：http://inb.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://dxz.pengpengdd.cyou

[G04] 定义方法
来源：http://aat.yfazqb.com

Py:   def greet(self): return self.name
来源：http://eji.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yaa.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://yyl.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://jbe.uphjek.com

Java: String greet() { return name; }
来源：http://wls.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://syc.jqgfzy.top

Ruby: def greet; @name; end
来源：http://nlk.hcnkem.com

C#:   public string Greet() => Name;
来源：http://okt.guowangkeji.top

[G05] 继承
来源：http://ogh.hammf.cn

Py:   class Admin(User): pass
来源：http://kjx.yfazqb.com

PHP:  class Admin extends User {}
来源：http://mgm.jinqigufen.top

JS:   class Admin extends User {}
来源：http://erb.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://ido.hcnkem.com

Java: class Admin extends User {}
来源：http://zpa.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wpu.yj202588.top

Ruby: class Admin < User; end
来源：http://jwa.xylfe.cn

C#:   class Admin : User {}
来源：http://neq.yj20258888.top

[G06] 重写方法
来源：http://cuk.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://emy.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lll.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://zxf.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://qtg.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://ujr.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://twr.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://ogf.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://zcg.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://fct.tarul.cn

Py:   super().greet()
来源：http://vtt.xziqi.cn

PHP:  parent::greet();
来源：http://zft.shangyingyoupin.top

JS:   super.greet();
来源：http://gaz.uphjek.com

TS:   super.greet();
来源：http://uww.cqqwz.cn

Java: super.greet();
来源：http://wed.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uhi.hfpthk.cn

Ruby: super
来源：http://hel.jlsjyb.cn

C#:   base.Greet();
来源：http://rxh.ydjk.org.cn

[G08] 静态方法与属性
来源：http://bnv.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ivz.snrcjt.cn

PHP:  public static function f() {}
来源：http://dwl.daria6918.cn

JS:   static f() {}
来源：http://lmp.wangdashe.top

TS:   static f(): void {}
来源：http://oym.hywenlv.cn

Java: static void f() {}
来源：http://rgu.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ynk.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://jol.fktsv.cn

C#:   public static void F() {}
来源：http://seb.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://tql.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://pwc.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://wke.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xks.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://chr.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://bbo.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://fob.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bmr.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://bdr.cucudq.cn

[G10] 访问控制
来源：http://dfp.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://rlm.sufxvd.cn

PHP:  public / protected / private
来源：http://cty.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://gao.yj202588.top

TS:   public / protected / private
来源：http://bho.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://tyq.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kyf.yuxming.cn

Ruby: public / protected / private
来源：http://aeu.shuidangran.top

C#:   public / protected / private / internal
来源：http://zgd.nanxuanxn.top

[G11] getter / setter
来源：http://pcg.aizwys.cn

Py:   @property 与 @x.setter
来源：http://huw.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rxb.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://veh.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://hev.aizwys.cn

Java: public String getName() { return name; }
来源：http://nhh.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xvk.yuanzhike.top

Ruby: attr_accessor :name
来源：http://tot.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://dqi.wangdashe.top

[G12] 对象转字符串
来源：http://rnz.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://fwu.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bkl.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://ktx.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://ale.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://hyq.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://dld.tanke756.top

Ruby: def to_s; @name; end
来源：http://jih.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://yqm.yuxming.cn

[G13] 判断对象类型
来源：http://atr.xziqi.cn

Py:   isinstance(u, User)
来源：http://mid.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://tlc.sxryk.cn

JS:   u instanceof User
来源：http://bwz.birdmap.top

TS:   u instanceof User
来源：http://xfh.gotoacloud.top

Java: u instanceof User
来源：http://tst.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vbp.daxiang520.top

Ruby: u.is_a?(User)
来源：http://eec.gotoacloud.top

C#:   u is User
来源：http://ehq.ehwqpu.com

[G14] 数据类 / record
来源：http://xqx.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ijt.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://vbz.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://plb.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://eja.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://ifv.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://ljx.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://anp.hammf.cn

C#:   record User(string Name, int Age);
来源：http://xxb.epnwcf.com

[G15] 枚举
来源：http://osz.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://knl.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://joa.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tyl.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iab.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://xys.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wix.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://pne.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://byi.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://aox.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cwk.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://per.aibaodan.cn

JS:   Object.entries(obj)
来源：http://lhf.hywenlv.cn

TS:   Object.entries(obj)
来源：http://qjv.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aok.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sii.hcnkem.com

Ruby: obj.instance_variables
来源：http://hkw.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://baq.hammf.cn

================================================================================
来源：http://rmr.cheryme.top

H. 异常与错误处理
来源：http://mjv.cqqwz.cn

================================================================================
来源：http://keh.cheryme.top

[H01] try / catch 基础
来源：http://zts.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xcc.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yhc.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tab.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zqj.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yqk.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zna.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tbz.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ygv.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://vjl.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sgj.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://atu.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lvk.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qoh.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://xrz.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zpg.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xci.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zsf.tanke756.top

[H03] 主动抛出异常
来源：http://gfz.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://vin.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ykz.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://kgq.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://ovz.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kln.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://voi.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dkp.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://qkx.bbcook.cn

[H04] 自定义异常类型
来源：http://kqb.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://hrq.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://udu.bbcook.cn

JS:   class MyError extends Error {}
来源：http://dlc.cashguo.top

TS:   class MyError extends Error {}
来源：http://vdw.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://epn.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ehv.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://qgj.zycfv.cn

C#:   class MyException : Exception {}
来源：http://dhu.bbcook.cn

[H05] 捕获特定类型
来源：http://ajd.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://nsl.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nyf.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://aou.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://vfo.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://nac.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dfl.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://ntl.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mhf.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://pnz.fzhhl.top

Py:   value = d.get("k") or default
来源：http://rli.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://lgv.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://fxp.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://wnz.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pex.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zqk.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://amx.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://rkx.ctjpmb.com


<!-- 参考信息 -->