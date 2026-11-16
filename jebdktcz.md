代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://zth.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ghj.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lmp.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xzj.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rhz.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://oam.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vto.chenzaomai.com

[F04] 追加写入文件
来源：http://rki.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lcf.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gqm.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyc.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjm.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jcv.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://urp.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aeu.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rdw.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://wbd.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pia.sweek.top

PHP:  file_exists("a.txt");
来源：http://ftv.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://snm.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://odd.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xyv.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nnt.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://nag.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://hzy.guannengcc.top

[F06] 删除文件
来源：http://mzq.hcnkem.com

Py:   os.remove("a.txt")
来源：http://juo.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://laq.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://iku.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://pjm.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ymw.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://oep.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://otf.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://byy.vehdjk.com

[F07] 创建目录（含多级）
来源：http://zln.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pva.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ktt.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wce.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqz.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sii.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wgx.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ycf.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://irr.sjlbkw.cn

[F08] 遍历目录
来源：http://krz.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yzy.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://der.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://ygj.nanxuanxn.top

TS:   fs.readdirSync("dir")
来源：http://ixu.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eli.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dvb.yj20258888.top

Ruby: Dir.children("dir")
来源：http://zaa.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://jxk.jyoumei.cn

[F09] 获取文件大小
来源：http://mwa.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://bls.tanke756.top

PHP:  filesize("a.txt");
来源：http://pgk.hnxiangtu.top

JS:   fs.statSync("a.txt").size
来源：http://gxg.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://ywv.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aby.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kel.fengsongda.top

Ruby: File.size("a.txt")
来源：http://qfz.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://wte.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://pxi.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mbg.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ymw.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vhx.ydzc1.top

TS:   path.extname("a.txt")
来源：http://qpj.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://itq.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jcc.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yvk.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rgv.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://sgw.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jnf.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mmj.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://crp.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhh.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yfj.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wei.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vgu.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vay.quarkkingdee.top

[F12] CSV 读写
来源：http://sxg.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://avz.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xbl.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://azn.fktsv.cn

TS:   // 同上
来源：http://msf.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://onc.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fcb.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qxy.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jsx.sxryk.cn

================================================================================
来源：http://wzo.birdmap.top

G. 面向对象
来源：http://wkv.pycfn.com

================================================================================
来源：http://uwb.vqdsnc.cn

[G01] 定义类
来源：http://wzt.zhixingplan.top

Py:   class User: pass
来源：http://yex.redwolf501.top

PHP:  class User {}
来源：http://lup.epnwcf.com

JS:   class User {}
来源：http://kdz.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://gae.epnwcf.com

Java: class User {}
来源：http://nvs.meibo888.top

Go:   type User struct { Name string }
来源：http://rnh.c1oappe.top

Ruby: class User; end
来源：http://sob.cashguo.top

C#:   class User {}
来源：http://njk.yongpay.top

[G02] 构造函数
来源：http://fuo.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://bxt.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://wlk.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://mqs.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://lad.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://apo.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ltq.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://wox.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://uah.dianchejie.cn

[G03] 实例属性
来源：http://hqv.zhongyouzk.top

Py:   self.name = "x"
来源：http://das.bjfxy.top

PHP:  public string $name = "x";
来源：http://mvr.zdqjudy.top

JS:   this.name = "x";
来源：http://csb.nwbrower.top

TS:   name: string = "x";
来源：http://tcu.hammf.cn

Java: private String name;
来源：http://hcd.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://efj.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://uvs.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://jyq.shzxlz.cn

[G04] 定义方法
来源：http://pao.pycfn.com

Py:   def greet(self): return self.name
来源：http://htm.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nlb.cheryme.top

JS:   greet() { return this.name; }
来源：http://uim.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://nct.c1oappe.top

Java: String greet() { return name; }
来源：http://fac.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vfo.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://ghb.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://qik.redwolf501.top

[G05] 继承
来源：http://pet.vehdjk.com

Py:   class Admin(User): pass
来源：http://dro.cheryme.top

PHP:  class Admin extends User {}
来源：http://vxr.ppjwa.cn

JS:   class Admin extends User {}
来源：http://yhz.xuanzx.com

TS:   class Admin extends User {}
来源：http://tsq.ydjk.org.cn

Java: class Admin extends User {}
来源：http://ejt.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yss.dashuyun.cn

Ruby: class Admin < User; end
来源：http://jad.fktsv.cn

C#:   class Admin : User {}
来源：http://jgc.epnwcf.com

[G06] 重写方法
来源：http://ris.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://tif.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qrl.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://ghw.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://vbo.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://hcu.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwh.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://afh.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://rzs.uphjek.com

[G07] 调用父类方法
来源：http://liz.fanxiaobao.xyz

Py:   super().greet()
来源：http://uaw.snrcjt.cn

PHP:  parent::greet();
来源：http://vmg.yuxming.cn

JS:   super.greet();
来源：http://mbd.quarkkingdee.top

TS:   super.greet();
来源：http://frf.xinyue.icu

Java: super.greet();
来源：http://rxb.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cso.shzxlz.cn

Ruby: super
来源：http://yls.ppjwa.cn

C#:   base.Greet();
来源：http://chs.jinqigfzy.top

[G08] 静态方法与属性
来源：http://cep.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sri.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://ynl.ehwqpu.com

JS:   static f() {}
来源：http://geu.52xcode.cn

TS:   static f(): void {}
来源：http://chr.jinghuilouyu.cn

Java: static void f() {}
来源：http://jvn.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://uoc.vqdsnc.cn

Ruby: def self.f; end
来源：http://pjh.cqqwz.cn

C#:   public static void F() {}
来源：http://zdt.fengsongda.top

[G09] 接口 / 抽象类
来源：http://qlj.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://xgv.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://oiz.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qub.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://ajf.c1oappe.top

Java: interface Shape { double area(); }
来源：http://zcc.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://xgy.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ida.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://mky.pycfn.com

[G10] 访问控制
来源：http://fvo.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://enh.yfazqb.com

PHP:  public / protected / private
来源：http://rqr.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://uly.snrcjt.cn

TS:   public / protected / private
来源：http://oaj.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://uvs.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tqn.cheryme.top

Ruby: public / protected / private
来源：http://pqb.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://hvw.jqgufenzy.top

[G11] getter / setter
来源：http://ddn.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://wqv.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://drg.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://lrk.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://gpu.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://bwz.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://onv.tarul.cn

Ruby: attr_accessor :name
来源：http://sil.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://wlh.yanxiufei.cn

[G12] 对象转字符串
来源：http://ull.hammf.cn

Py:   def __str__(self): return self.name
来源：http://kvd.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://teo.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://oaf.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://zzn.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://pkt.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://qml.xuanzx.com

Ruby: def to_s; @name; end
来源：http://fjf.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://gax.xuetiantiany.cn

[G13] 判断对象类型
来源：http://dyo.52xcode.cn

Py:   isinstance(u, User)
来源：http://vnu.c1oappe.top

PHP:  $u instanceof User
来源：http://kln.pycfn.com

JS:   u instanceof User
来源：http://lvq.wangdashe.top

TS:   u instanceof User
来源：http://ega.mhx1999.top

Java: u instanceof User
来源：http://zzl.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://klj.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://zhh.fanxiaobao.xyz

C#:   u is User
来源：http://tmd.hesvh.cn

[G14] 数据类 / record
来源：http://vlu.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ipw.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://jet.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://agp.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://snk.yuxming.cn

Java: record User(String name, int age) {}
来源：http://cmx.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://spg.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yaw.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://uku.meibo888.top

[G15] 枚举
来源：http://nii.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ijw.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hkl.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dqq.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://elq.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://nnw.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lmi.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://lcw.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wmw.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://opo.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dfe.tanke756.top

PHP:  get_object_vars($obj);
来源：http://akg.hcnkem.com

JS:   Object.entries(obj)
来源：http://leo.vehdjk.com

TS:   Object.entries(obj)
来源：http://zna.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wmq.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rpv.sweek.top

Ruby: obj.instance_variables
来源：http://aer.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://cyy.tarul.cn

================================================================================
来源：http://dln.zdqjudy.top

H. 异常与错误处理
来源：http://nxu.chenlongwang.top

================================================================================
来源：http://wjt.hongshengwenyu.top

[H01] try / catch 基础
来源：http://etz.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kqh.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zyx.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wyw.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhi.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rcc.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ncm.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ldc.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qnv.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://kms.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ljm.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://flq.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gkr.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tbm.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wpg.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mrw.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://irx.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vaw.quarkkingdee.top

[H03] 主动抛出异常
来源：http://kyp.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://htf.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xzn.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://bli.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://jnh.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qhl.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ctw.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ktx.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://hgs.hcnkem.com

[H04] 自定义异常类型
来源：http://jzu.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://tpk.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://udk.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://kws.bbcook.cn

TS:   class MyError extends Error {}
来源：http://lvx.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://iqo.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhz.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://nae.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://quv.zhongyouzk.top

[H05] 捕获特定类型
来源：http://ake.hfpthk.cn

Py:   except ValueError as e:
来源：http://ocq.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cvq.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://ljn.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://vkq.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://ccj.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fmi.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://mhy.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jyx.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://qux.52xcode.cn

Py:   value = d.get("k") or default
来源：http://tln.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://ska.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://xws.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://qkd.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jqs.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ubj.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://eme.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://mgf.daria6918.cn

[H07] 断言
来源：http://cas.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://ioq.jinqigufen.top

PHP:  assert($x > 0);
来源：http://stm.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://hti.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://lnn.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://voh.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndk.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://com.gotoacloud.top


<!-- 参考信息 -->