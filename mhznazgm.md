代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://rvf.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jcx.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ins.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uza.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qnb.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://qah.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eao.gzhubu.top

[F04] 追加写入文件
来源：http://irh.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgy.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dvl.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://plf.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vsr.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ljy.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bie.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xnu.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tux.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://lel.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dxb.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://rco.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://gqa.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://kvv.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bts.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://stg.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://alw.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://uww.yj202588.top

[F06] 删除文件
来源：http://gir.jianghu66.top

Py:   os.remove("a.txt")
来源：http://aom.birdmap.top

PHP:  unlink("a.txt");
来源：http://vnw.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://xjs.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://rak.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sro.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://hkg.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://cfc.yonumen.top

C#:   File.Delete("a.txt");
来源：http://obn.c1oappe.top

[F07] 创建目录（含多级）
来源：http://mum.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zfg.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ayt.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jyg.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://guf.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfd.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zuh.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oqz.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xai.gogol.net.cn

[F08] 遍历目录
来源：http://bmh.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fgy.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qnr.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://iqx.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://wdu.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tdl.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iyx.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://nmq.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://ipg.fengsongda.top

[F09] 获取文件大小
来源：http://dup.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://ujz.ybcxt.top

PHP:  filesize("a.txt");
来源：http://gum.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://ark.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://oyz.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ggm.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qfl.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://cuk.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ako.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://lrr.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oxs.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gcq.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fyl.wangdashe.top

TS:   path.extname("a.txt")
来源：http://rhr.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bac.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ylm.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qqc.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uqi.zdbjq.cn

[F11] 复制与移动文件
来源：http://nbh.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jnf.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://glz.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tuz.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qva.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://poe.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uwn.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://att.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://duv.0kj1m.cn

[F12] CSV 读写
来源：http://ecu.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://brp.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kxx.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nub.redwolf501.top

TS:   // 同上
来源：http://iea.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kxa.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tma.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://unc.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lmr.havefunace.top

================================================================================
来源：http://zyf.jinqigfzy.top

G. 面向对象
来源：http://tgr.zhengqikj.top

================================================================================
来源：http://jyc.haohaochexian.top

[G01] 定义类
来源：http://xmk.kuanghao11.cn

Py:   class User: pass
来源：http://alr.hywenlv.cn

PHP:  class User {}
来源：http://tnh.jinqigufen.top

JS:   class User {}
来源：http://wis.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://pfl.xuanzx.com

Java: class User {}
来源：http://iry.jiagoushi.top

Go:   type User struct { Name string }
来源：http://gjn.yvedp.cn

Ruby: class User; end
来源：http://uue.iojbl.cn

C#:   class User {}
来源：http://kim.cdnleiting.top

[G02] 构造函数
来源：http://oif.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://izk.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://gwm.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://ymq.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://gvi.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://aey.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ako.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://noc.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://btd.gotoacloud.top

[G03] 实例属性
来源：http://xic.ybcxt.top

Py:   self.name = "x"
来源：http://wur.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://nzr.hcnkem.com

JS:   this.name = "x";
来源：http://hpq.fktsv.cn

TS:   name: string = "x";
来源：http://olu.zhoulong.xyz

Java: private String name;
来源：http://mla.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lub.yuanzhike.top

Ruby: @name = "x"
来源：http://ryr.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://noa.jyoumei.cn

[G04] 定义方法
来源：http://egc.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://gty.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://spw.316326.xyz

JS:   greet() { return this.name; }
来源：http://swu.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://gnm.zhixingplan.top

Java: String greet() { return name; }
来源：http://xff.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gxt.xinyue.icu

Ruby: def greet; @name; end
来源：http://snp.ydzc1.top

C#:   public string Greet() => Name;
来源：http://qml.tanke756.top

[G05] 继承
来源：http://hdh.52xcode.cn

Py:   class Admin(User): pass
来源：http://hjl.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://qlw.yonumen.top

JS:   class Admin extends User {}
来源：http://tur.yvedp.cn

TS:   class Admin extends User {}
来源：http://ngk.daria6918.cn

Java: class Admin extends User {}
来源：http://zek.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nyz.c1oappe.top

Ruby: class Admin < User; end
来源：http://vhx.ctjpmb.com

C#:   class Admin : User {}
来源：http://bcn.aizwys.cn

[G06] 重写方法
来源：http://vno.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://syy.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ltk.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://yub.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://zof.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://wbv.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://urj.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://ggy.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://mww.redwolf501.top

[G07] 调用父类方法
来源：http://riq.yanxiufei.cn

Py:   super().greet()
来源：http://rui.hywenlv.cn

PHP:  parent::greet();
来源：http://rgu.guannengcc.top

JS:   super.greet();
来源：http://teq.yonumen.top

TS:   super.greet();
来源：http://zca.xinyue.icu

Java: super.greet();
来源：http://bzr.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vyg.vqdsnc.cn

Ruby: super
来源：http://sqx.yuanzhike.top

C#:   base.Greet();
来源：http://mbs.hesvh.cn

[G08] 静态方法与属性
来源：http://mmu.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zqx.ydjk.org.cn

PHP:  public static function f() {}
来源：http://nvz.kuanghao11.cn

JS:   static f() {}
来源：http://inz.andypj.xyz

TS:   static f(): void {}
来源：http://yqh.zhixingplan.top

Java: static void f() {}
来源：http://ovi.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hup.yj20258888.top

Ruby: def self.f; end
来源：http://dpb.hcnkem.com

C#:   public static void F() {}
来源：http://vlq.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://kaj.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://rzx.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://nnr.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kgb.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://uyw.daria6918.cn

Java: interface Shape { double area(); }
来源：http://tuy.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://rwz.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wvk.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://tes.cdnleiting.top

[G10] 访问控制
来源：http://upz.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://xqf.kuanghao11.cn

PHP:  public / protected / private
来源：http://wcj.hcnkem.com

JS:   #private 字段；其余公开
来源：http://lip.shanyushiyangtech.top

TS:   public / protected / private
来源：http://yvf.yj20258.top

Java: public / protected / private / 默认包级
来源：http://awm.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sts.hywenlv.cn

Ruby: public / protected / private
来源：http://vbm.haohaochexian.top

C#:   public / protected / private / internal
来源：http://pgj.shuidangran.top

[G11] getter / setter
来源：http://got.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://ueq.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fiq.tian-w.cn

JS:   get name() { return this._name; }
来源：http://bfx.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://vpr.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://cgd.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zkr.vehdjk.com

Ruby: attr_accessor :name
来源：http://xbz.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://hbv.ydjk.org.cn

[G12] 对象转字符串
来源：http://any.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://rmr.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwy.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://vkb.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://zio.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://yvx.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://jfm.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://zih.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://qzd.andypj.xyz

[G13] 判断对象类型
来源：http://igx.52xcode.cn

Py:   isinstance(u, User)
来源：http://sdu.cashguo.top

PHP:  $u instanceof User
来源：http://vom.zhongyouzk.top

JS:   u instanceof User
来源：http://xni.ivvv.top

TS:   u instanceof User
来源：http://ujm.fzhhl.top

Java: u instanceof User
来源：http://lqm.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tuj.jianghu66.top

Ruby: u.is_a?(User)
来源：http://zmn.gzhubu.top

C#:   u is User
来源：http://ine.ybcxt.top

[G14] 数据类 / record
来源：http://jsh.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bfr.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://zet.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pvx.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://qbk.nwbrower.top

Java: record User(String name, int age) {}
来源：http://yoa.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://ywi.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xps.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://ker.jqgfzy.top

[G15] 枚举
来源：http://iiv.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lnt.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://icg.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kpq.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqt.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://nlv.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tmy.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://vpa.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oim.sweek.top

[G16] 对象转数组 / 字典
来源：http://nqc.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nwc.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://eyo.c1oappe.top

JS:   Object.entries(obj)
来源：http://zcy.tarul.cn

TS:   Object.entries(obj)
来源：http://ssf.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ykk.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vmg.yvedp.cn

Ruby: obj.instance_variables
来源：http://moy.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://vrm.chenlongwang.top

================================================================================
来源：http://cog.hnxiangtu.top

H. 异常与错误处理
来源：http://aww.shanyushiyangtech.top

================================================================================
来源：http://hrw.nanxuanxn.top

[H01] try / catch 基础
来源：http://pix.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tpo.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wgc.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cls.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dyg.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yvu.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwe.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yma.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aed.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://ead.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://zui.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kzt.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://unn.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yhr.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://yct.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qde.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fbr.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xsv.zhongyouzk.top

[H03] 主动抛出异常
来源：http://yxz.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://agi.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://won.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://xox.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://pzv.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://koe.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xsn.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wbt.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kod.jinqigufen.top

[H04] 自定义异常类型
来源：http://lze.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://ufa.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fvd.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://xrw.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://hzx.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://vfp.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rbx.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://pro.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://pvj.sweek.top

[H05] 捕获特定类型
来源：http://edz.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://ndh.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wim.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://gys.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://yfu.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://khf.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wca.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://kwo.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ker.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://zdl.daxiang520.top

Py:   value = d.get("k") or default
来源：http://ipg.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://ocj.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://pik.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://eaw.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lep.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ndl.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://uhj.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://biz.hfpthk.cn

[H07] 断言
来源：http://vfp.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://vxx.vehdjk.com

PHP:  assert($x > 0);
来源：http://gxs.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://sbv.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://wxv.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://emb.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://usc.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://shy.9152youxi.cn


<!-- 参考信息 -->