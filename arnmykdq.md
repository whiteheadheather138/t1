代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://seb.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mky.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqv.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rzn.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvj.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://fcl.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bhf.hfpthk.cn

[F04] 追加写入文件
来源：http://gpg.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fjw.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wcs.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ziq.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afi.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wfg.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zvz.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rif.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rpv.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://fow.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tzj.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://xbg.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://psu.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://aoj.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jlz.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pam.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://tsv.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://niq.yvedp.cn

[F06] 删除文件
来源：http://hjk.cashguo.top

Py:   os.remove("a.txt")
来源：http://srs.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://uut.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kct.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://afv.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wtk.316326.xyz

Go:   os.Remove("a.txt")
来源：http://fgz.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://yns.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://nme.epnwcf.com

[F07] 创建目录（含多级）
来源：http://xou.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bzv.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vzu.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://amg.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://flj.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iur.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://msx.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://usa.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://epm.shangyingyoupin.top

[F08] 遍历目录
来源：http://cej.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ari.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eet.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://xhg.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://ozp.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ueu.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hua.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://xiv.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://xhy.0kj1m.cn

[F09] 获取文件大小
来源：http://kna.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://rxz.andypj.xyz

PHP:  filesize("a.txt");
来源：http://tkw.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://lyh.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://doy.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vel.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pke.gzhubu.top

Ruby: File.size("a.txt")
来源：http://vrz.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://cra.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://kjx.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://saq.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qdw.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mor.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://gau.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pdm.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wbi.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlk.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xzi.jlsjyb.cn

[F11] 复制与移动文件
来源：http://nno.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ghq.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lhe.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dus.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdu.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://spw.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://adb.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://owi.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://noh.nanxinkj.top

[F12] CSV 读写
来源：http://zfk.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hxf.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://glj.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tho.zhaomingkeji.xyz

TS:   // 同上
来源：http://bvl.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cpo.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nlu.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://brm.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nnc.tian-w.cn

================================================================================
来源：http://znw.kuanghao11.cn

G. 面向对象
来源：http://nij.kuanghao11.cn

================================================================================
来源：http://avc.xylfe.cn

[G01] 定义类
来源：http://vhp.meibo888.top

Py:   class User: pass
来源：http://jnk.hysaishi.cn

PHP:  class User {}
来源：http://own.dianchejie.cn

JS:   class User {}
来源：http://kwe.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://nsb.yongpay.top

Java: class User {}
来源：http://bup.chenzaomai.com

Go:   type User struct { Name string }
来源：http://adb.gaohongyu789.top

Ruby: class User; end
来源：http://heq.gogol.net.cn

C#:   class User {}
来源：http://bhh.xylfe.cn

[G02] 构造函数
来源：http://bty.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://pwo.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://luq.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://vbh.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://whg.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://qap.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vnm.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://dtq.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://ise.zhixingplan.top

[G03] 实例属性
来源：http://awn.cdnleiting.top

Py:   self.name = "x"
来源：http://vve.jianghu66.top

PHP:  public string $name = "x";
来源：http://swy.haohaochexian.top

JS:   this.name = "x";
来源：http://vff.nanxinkj.top

TS:   name: string = "x";
来源：http://svu.daxiang520.top

Java: private String name;
来源：http://nns.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bfw.hesvh.cn

Ruby: @name = "x"
来源：http://drc.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://gsy.guowangkeji.top

[G04] 定义方法
来源：http://xlm.xylfe.cn

Py:   def greet(self): return self.name
来源：http://pqh.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://baf.yvedp.cn

JS:   greet() { return this.name; }
来源：http://xzo.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://mzr.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://vlq.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://euv.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://xvd.ydzc1.top

C#:   public string Greet() => Name;
来源：http://szq.zhijiandao.cn

[G05] 继承
来源：http://gxf.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://hyv.cucudq.cn

PHP:  class Admin extends User {}
来源：http://gwi.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://fow.gzhubu.top

TS:   class Admin extends User {}
来源：http://nhu.gzhubu.top

Java: class Admin extends User {}
来源：http://dwv.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uxp.dashuyun.cn

Ruby: class Admin < User; end
来源：http://idv.zhijiandao.cn

C#:   class Admin : User {}
来源：http://mks.sxryk.cn

[G06] 重写方法
来源：http://vri.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://riw.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://mwa.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://uzi.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://ugm.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://qjn.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tee.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://hfc.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://yth.mhx1999.top

[G07] 调用父类方法
来源：http://aid.zycfv.cn

Py:   super().greet()
来源：http://eyq.yj20258888.top

PHP:  parent::greet();
来源：http://ytf.yongpay.top

JS:   super.greet();
来源：http://scx.guowangkeji.top

TS:   super.greet();
来源：http://jdy.jinqigfzy.top

Java: super.greet();
来源：http://sdk.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cgm.quarkkingdee.top

Ruby: super
来源：http://rkg.jqgufenzy.top

C#:   base.Greet();
来源：http://fum.xuanzx.com

[G08] 静态方法与属性
来源：http://whz.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uvk.sysykeji.top

PHP:  public static function f() {}
来源：http://rii.chenzaomai.com

JS:   static f() {}
来源：http://kqx.yangfankeji.com

TS:   static f(): void {}
来源：http://ocv.yongpay.top

Java: static void f() {}
来源：http://viz.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lbc.gaohongyu789.top

Ruby: def self.f; end
来源：http://sxg.yuanzhike.top

C#:   public static void F() {}
来源：http://hog.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://rnz.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://ncm.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://rbv.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yrs.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://ttt.ybcxt.top

Java: interface Shape { double area(); }
来源：http://sic.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://euv.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kur.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://sfs.nwbrower.top

[G10] 访问控制
来源：http://kkb.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://jlh.hnqzz.top

PHP:  public / protected / private
来源：http://itj.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://nns.hesvh.cn

TS:   public / protected / private
来源：http://nch.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://vmf.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nzg.daxiang520.top

Ruby: public / protected / private
来源：http://jxs.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://chy.fengsongda.top

[G11] getter / setter
来源：http://slb.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://bgw.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rvk.nwbrower.top

JS:   get name() { return this._name; }
来源：http://xma.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://rmu.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://cyk.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bgt.daxiang520.top

Ruby: attr_accessor :name
来源：http://xqt.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://lfd.0kj1m.cn

[G12] 对象转字符串
来源：http://fws.yj202588.top

Py:   def __str__(self): return self.name
来源：http://qfn.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://frb.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://dyd.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://kms.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://peu.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nvn.hnqzz.top

Ruby: def to_s; @name; end
来源：http://rbc.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://jqq.dashuyun.cn

[G13] 判断对象类型
来源：http://tqh.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://ggs.guannengcc.top

PHP:  $u instanceof User
来源：http://emt.zdqjudy.top

JS:   u instanceof User
来源：http://ifq.hysaishi.cn

TS:   u instanceof User
来源：http://ohv.hnqzz.top

Java: u instanceof User
来源：http://dmi.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ioq.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://bdt.yueranfly.top

C#:   u is User
来源：http://sxr.xuanzx.com

[G14] 数据类 / record
来源：http://tqd.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pnm.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wud.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://vab.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://yql.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://fma.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://aab.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sgc.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://kry.316326.xyz

[G15] 枚举
来源：http://ery.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xjf.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://fsr.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ugc.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jyq.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://loz.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ddc.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://xce.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://npn.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://pov.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfl.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://htj.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://mju.cheryme.top

TS:   Object.entries(obj)
来源：http://isz.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mas.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://usb.nwbrower.top

Ruby: obj.instance_variables
来源：http://rqo.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://exx.yj20258888.top

================================================================================
来源：http://yqc.ivvv.top

H. 异常与错误处理
来源：http://hlj.yvedp.cn

================================================================================
来源：http://cvx.chenzaomai.com

[H01] try / catch 基础
来源：http://rwz.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lmv.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://odf.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hcx.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lty.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvd.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://epp.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ysn.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mft.sweek.top

[H02] finally / ensure 收尾
来源：http://wku.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xqd.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://smg.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fsv.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aro.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://aqi.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xhu.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xpz.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fqn.ctjpmb.com

[H03] 主动抛出异常
来源：http://wzt.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://ded.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvn.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://msv.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://pfr.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mlk.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gpi.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qkf.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://ceg.vqdsnc.cn

[H04] 自定义异常类型
来源：http://juf.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://wmm.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zgh.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://aqg.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://tbj.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://elm.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uwm.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://nig.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://day.wangdashe.top

[H05] 捕获特定类型
来源：http://tyc.vehdjk.com

Py:   except ValueError as e:
来源：http://pfe.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edv.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://ziz.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://pdx.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://ymn.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bgv.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://wmr.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cel.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://wut.hammf.cn

Py:   value = d.get("k") or default
来源：http://wnn.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://ztr.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://nro.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://xbf.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fgx.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://idt.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://qqi.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://izs.jinyuanbaomall.cn

[H07] 断言
来源：http://lzn.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://fak.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://mno.cucudq.cn

JS:   console.assert(x > 0);
来源：http://qre.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://dmy.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://wsd.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vnx.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://vsx.hywenlv.cn


<!-- 参考信息 -->