代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ccg.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cgu.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://vio.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkb.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://nlw.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kci.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enx.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hzq.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fgu.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://noq.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sgq.hnqzz.top

[F04] 追加写入文件
来源：http://ggb.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jov.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lbn.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bqz.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfn.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hhv.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://msd.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sko.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dgz.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://wsg.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dph.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://qdb.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://fev.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://pvy.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pvi.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nli.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://png.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://wkt.52xcode.cn

[F06] 删除文件
来源：http://jhj.bbcook.cn

Py:   os.remove("a.txt")
来源：http://nji.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://qnp.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://guo.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hpm.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yuk.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://cdf.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://fbu.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://skl.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://gwt.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://evc.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nax.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://huf.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pbh.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://imp.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gzq.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mug.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vrf.cdnleiting.top

[F08] 遍历目录
来源：http://uei.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://zjx.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fwv.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://azc.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://jal.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://psn.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://asi.sxryk.cn

Ruby: Dir.children("dir")
来源：http://tye.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://eky.feifeiyinyue.top

[F09] 获取文件大小
来源：http://god.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://tjq.aizwys.cn

PHP:  filesize("a.txt");
来源：http://mhm.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://noq.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://gxb.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ddk.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vuh.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://wch.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://omo.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://tbc.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cxm.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cxl.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tzm.yj20258888.top

TS:   path.extname("a.txt")
来源：http://rvn.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kje.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wse.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jkr.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aam.daria6918.cn

[F11] 复制与移动文件
来源：http://bwe.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xnk.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqz.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://chs.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://btz.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uho.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lnd.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://syc.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fve.tianlin.xyz

[F12] CSV 读写
来源：http://rph.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eur.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zuj.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://urs.0kj1m.cn

TS:   // 同上
来源：http://fcj.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zfh.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yds.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kdu.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bqa.hammf.cn

================================================================================
来源：http://zdw.guannengcc.top

G. 面向对象
来源：http://gcn.ppjwa.cn

================================================================================
来源：http://evo.hammf.cn

[G01] 定义类
来源：http://zxu.shangyingyoupin.top

Py:   class User: pass
来源：http://mvi.sufxvd.cn

PHP:  class User {}
来源：http://snp.zhengqikj.top

JS:   class User {}
来源：http://yhc.yj202588.top

TS:   class User { name: string = ""; }
来源：http://dei.jqgufenzy.top

Java: class User {}
来源：http://qxd.havefunace.top

Go:   type User struct { Name string }
来源：http://dvp.yuxming.cn

Ruby: class User; end
来源：http://dun.haohaochexian.top

C#:   class User {}
来源：http://shi.haohaochexian.top

[G02] 构造函数
来源：http://veo.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://yjn.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://bmu.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://ykq.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://icr.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://hta.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yzy.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://dzq.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://bbg.yj20258888.top

[G03] 实例属性
来源：http://zkk.52xcode.cn

Py:   self.name = "x"
来源：http://zmx.chenzaomai.com

PHP:  public string $name = "x";
来源：http://qth.meibo888.top

JS:   this.name = "x";
来源：http://xyx.guowangkeji.top

TS:   name: string = "x";
来源：http://rpu.gotoacloud.top

Java: private String name;
来源：http://dpk.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wnr.shuidangran.top

Ruby: @name = "x"
来源：http://gyj.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://url.zhengqikj.top

[G04] 定义方法
来源：http://pjv.redwolf501.top

Py:   def greet(self): return self.name
来源：http://rif.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dxb.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://sct.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://iaw.ehwqpu.com

Java: String greet() { return name; }
来源：http://gde.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tka.chenzaomai.com

Ruby: def greet; @name; end
来源：http://lwa.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://pfc.uphjek.com

[G05] 继承
来源：http://jbh.ehwqpu.com

Py:   class Admin(User): pass
来源：http://gru.hcnkem.com

PHP:  class Admin extends User {}
来源：http://zzw.daxiang520.top

JS:   class Admin extends User {}
来源：http://miw.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://ics.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://ucz.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qvu.sxryk.cn

Ruby: class Admin < User; end
来源：http://yni.sufxvd.cn

C#:   class Admin : User {}
来源：http://mgo.dashuyun.cn

[G06] 重写方法
来源：http://zbo.tanke756.top

Py:   def greet(self): return "admin"
来源：http://agn.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://udg.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://ibj.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://pim.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://qyd.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vjo.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://tbd.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://ytg.bbcook.cn

[G07] 调用父类方法
来源：http://rnv.dianchejie.cn

Py:   super().greet()
来源：http://jtv.daria6918.cn

PHP:  parent::greet();
来源：http://usr.yfazqb.com

JS:   super.greet();
来源：http://csr.nanxinkj.top

TS:   super.greet();
来源：http://xub.jlsjyb.cn

Java: super.greet();
来源：http://rnf.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qvz.andypj.xyz

Ruby: super
来源：http://pum.daria6918.cn

C#:   base.Greet();
来源：http://cgm.yj20258.top

[G08] 静态方法与属性
来源：http://ecs.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://npt.zdbjq.cn

PHP:  public static function f() {}
来源：http://crn.cqqwz.cn

JS:   static f() {}
来源：http://ndu.tian-w.cn

TS:   static f(): void {}
来源：http://kzz.svipenyu.cn

Java: static void f() {}
来源：http://wzd.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://klm.316326.xyz

Ruby: def self.f; end
来源：http://uln.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://qmk.vehdjk.com

[G09] 接口 / 抽象类
来源：http://czd.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://kpi.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://wkn.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sjm.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://mlv.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://yxj.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://aug.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pmg.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://hyv.sufxvd.cn

[G10] 访问控制
来源：http://hti.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://epf.hysaishi.cn

PHP:  public / protected / private
来源：http://crb.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://evy.pycfn.com

TS:   public / protected / private
来源：http://omc.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://dru.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bpl.yangfankeji.com

Ruby: public / protected / private
来源：http://hpr.uphjek.com

C#:   public / protected / private / internal
来源：http://dgo.ppjwa.cn

[G11] getter / setter
来源：http://uem.andypj.xyz

Py:   @property 与 @x.setter
来源：http://dxc.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yos.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://bvz.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://iby.smart0.xyz

Java: public String getName() { return name; }
来源：http://dnw.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://lir.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://nxu.redwolf501.top

C#:   public string Name { get; set; }
来源：http://zgi.feifeiyinyue.top

[G12] 对象转字符串
来源：http://yvm.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://bvy.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://odz.yongpay.top

JS:   toString() { return this.name; }
来源：http://ilk.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://jsm.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://jbk.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://kgi.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://hth.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://ixb.zhixingplan.top

[G13] 判断对象类型
来源：http://efr.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://vss.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://kfx.zhixingplan.top

JS:   u instanceof User
来源：http://pzm.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://tzh.yueranfly.top

Java: u instanceof User
来源：http://yph.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://szs.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://iom.svipenyu.cn

C#:   u is User
来源：http://vdf.svipenyu.cn

[G14] 数据类 / record
来源：http://dyr.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ety.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://czu.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://ykg.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://zqz.sweek.top

Java: record User(String name, int age) {}
来源：http://qbq.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://exy.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nga.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://ele.tian-w.cn

[G15] 枚举
来源：http://tsg.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ean.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lyk.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pwf.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wny.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://zim.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cut.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://zgu.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lma.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://jhv.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ygp.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://lss.yangfankeji.com

JS:   Object.entries(obj)
来源：http://aor.fzhhl.top

TS:   Object.entries(obj)
来源：http://dbe.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ivu.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xrv.fehbvm.com

Ruby: obj.instance_variables
来源：http://kyh.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://sih.jinqigufen.top

================================================================================
来源：http://adn.hnxiangtu.top

H. 异常与错误处理
来源：http://hgu.hfpthk.cn

================================================================================
来源：http://ztp.ivvv.top

[H01] try / catch 基础
来源：http://rhq.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xmx.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eqy.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ezi.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdc.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://juk.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dxc.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vmb.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dan.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://zmp.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rly.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lod.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hyw.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://cgi.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://eiu.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://siz.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fvk.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://xbf.cdnleiting.top

[H03] 主动抛出异常
来源：http://ege.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://lub.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ivq.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://sej.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://ilv.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://niy.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://whn.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zib.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://xvs.gogol.net.cn

[H04] 自定义异常类型
来源：http://aoa.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://xrr.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://btz.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://xqm.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://rsv.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://upr.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kwa.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://qtm.sysykeji.top

C#:   class MyException : Exception {}
来源：http://mxd.zdbjq.cn

[H05] 捕获特定类型
来源：http://fby.hnqzz.top

Py:   except ValueError as e:
来源：http://xym.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ycd.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://pmy.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://zcb.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://fjz.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lyn.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://mij.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://upc.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://otm.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://ulj.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://umx.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://gaa.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://mns.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rvg.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hgv.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://ddw.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://skj.jqgufenzy.top

[H07] 断言
来源：http://sse.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://vtt.sufxvd.cn

PHP:  assert($x > 0);
来源：http://mvy.pycfn.com

JS:   console.assert(x > 0);
来源：http://lti.shuidangran.top


<!-- 参考信息 -->