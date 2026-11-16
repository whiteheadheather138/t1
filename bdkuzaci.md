代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://asn.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jyj.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwk.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jdl.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sxd.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://nnf.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ayj.nanxuanxn.top

[F04] 追加写入文件
来源：http://dkb.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gqs.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jrd.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kgx.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hly.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qht.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://npk.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rdn.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oeu.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://trh.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qtk.sweek.top

PHP:  file_exists("a.txt");
来源：http://awl.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://ywx.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://bsd.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ebw.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://brs.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://qyc.yonumen.top

C#:   File.Exists("a.txt")
来源：http://zel.andypj.xyz

[F06] 删除文件
来源：http://kie.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://nbi.tian-w.cn

PHP:  unlink("a.txt");
来源：http://rpn.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pmi.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://yxt.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://huz.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://gbg.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://gjp.birdmap.top

C#:   File.Delete("a.txt");
来源：http://sue.wangdashe.top

[F07] 创建目录（含多级）
来源：http://bng.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jyn.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fqy.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejd.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnb.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zah.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://neq.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oop.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kya.fanxiaobao.xyz

[F08] 遍历目录
来源：http://zii.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://csm.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ktg.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://ysy.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://izv.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dsy.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jzk.fzhhl.top

Ruby: Dir.children("dir")
来源：http://lio.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://vng.xuanzx.com

[F09] 获取文件大小
来源：http://fcp.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://eld.birdmap.top

PHP:  filesize("a.txt");
来源：http://duy.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://dbf.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://mhc.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://hiv.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sfa.shuidangran.top

Ruby: File.size("a.txt")
来源：http://ime.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://yal.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://edz.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bns.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ebp.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ptu.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://mkf.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wzt.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zgj.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hxg.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aau.jyoumei.cn

[F11] 复制与移动文件
来源：http://nlr.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ctw.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://knt.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzy.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zqm.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mtf.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pjq.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfy.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nsw.gaohongyu789.top

[F12] CSV 读写
来源：http://znc.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fyo.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xab.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ipm.shangyingyoupin.top

TS:   // 同上
来源：http://nwf.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uvu.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://evk.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aey.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://egt.fehbvm.com

================================================================================
来源：http://pod.tarul.cn

G. 面向对象
来源：http://zin.cdnleiting.top

================================================================================
来源：http://lpr.feifeiyinyue.top

[G01] 定义类
来源：http://dhx.hywenlv.cn

Py:   class User: pass
来源：http://zci.wangshuangyany.cn

PHP:  class User {}
来源：http://zrl.fktsv.cn

JS:   class User {}
来源：http://wwc.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://doj.xziqi.cn

Java: class User {}
来源：http://lbn.vehdjk.com

Go:   type User struct { Name string }
来源：http://zna.fktsv.cn

Ruby: class User; end
来源：http://esx.chenzaomai.com

C#:   class User {}
来源：http://bgw.tianlin.xyz

[G02] 构造函数
来源：http://syv.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://bfq.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://vjh.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://lyv.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://nta.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://ezu.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iyf.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://phe.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://tiv.pengpengdd.cyou

[G03] 实例属性
来源：http://she.wangdashe.top

Py:   self.name = "x"
来源：http://edq.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://nap.bjfxy.top

JS:   this.name = "x";
来源：http://wpj.dashuyun.cn

TS:   name: string = "x";
来源：http://mmt.shuidangran.top

Java: private String name;
来源：http://mot.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nlq.ivvv.top

Ruby: @name = "x"
来源：http://ikf.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jnw.ppjwa.cn

[G04] 定义方法
来源：http://gbt.sweek.top

Py:   def greet(self): return self.name
来源：http://dor.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gav.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://dmj.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://xqk.iojbl.cn

Java: String greet() { return name; }
来源：http://viy.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vkh.snrcjt.cn

Ruby: def greet; @name; end
来源：http://wwz.cucudq.cn

C#:   public string Greet() => Name;
来源：http://coj.jqgufenzy.top

[G05] 继承
来源：http://tak.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://ytb.yj202588.top

PHP:  class Admin extends User {}
来源：http://uet.sxryk.cn

JS:   class Admin extends User {}
来源：http://myn.nanxinkj.top

TS:   class Admin extends User {}
来源：http://igh.tian-w.cn

Java: class Admin extends User {}
来源：http://dbj.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://upz.zdbjq.cn

Ruby: class Admin < User; end
来源：http://quy.ydjk.org.cn

C#:   class Admin : User {}
来源：http://zog.aibaodan.cn

[G06] 重写方法
来源：http://hpy.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://tun.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gze.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://qve.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://ity.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://huf.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ujf.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://rjr.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://vgz.guowangkeji.top

[G07] 调用父类方法
来源：http://ikx.xinyue.icu

Py:   super().greet()
来源：http://ius.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://fws.cqqwz.cn

JS:   super.greet();
来源：http://ffj.jiagoushi.top

TS:   super.greet();
来源：http://qef.tianlin.xyz

Java: super.greet();
来源：http://lvp.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zxf.yuxming.cn

Ruby: super
来源：http://pux.pycfn.com

C#:   base.Greet();
来源：http://lxk.aizwys.cn

[G08] 静态方法与属性
来源：http://tws.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pkl.quarkkingdee.top

PHP:  public static function f() {}
来源：http://lsz.iojbl.cn

JS:   static f() {}
来源：http://nhx.yanxiufei.cn

TS:   static f(): void {}
来源：http://fjf.dashuyun.cn

Java: static void f() {}
来源：http://oqk.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sly.gotoacloud.top

Ruby: def self.f; end
来源：http://oad.snrcjt.cn

C#:   public static void F() {}
来源：http://ewo.meibo888.top

[G09] 接口 / 抽象类
来源：http://czn.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://ehi.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://lub.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eci.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://nqq.epnwcf.com

Java: interface Shape { double area(); }
来源：http://qyb.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://uwy.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xam.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://kjp.fzhhl.top

[G10] 访问控制
来源：http://hlb.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://fkq.ctjpmb.com

PHP:  public / protected / private
来源：http://rel.fehbvm.com

JS:   #private 字段；其余公开
来源：http://nfb.dashuyun.cn

TS:   public / protected / private
来源：http://jlr.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://cst.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ebz.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://fjn.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://ccc.zdbjq.cn

[G11] getter / setter
来源：http://ofs.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://rks.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vhr.fengsongda.top

JS:   get name() { return this._name; }
来源：http://oqm.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://cjc.meibo888.top

Java: public String getName() { return name; }
来源：http://owh.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nlk.jiagoushi.top

Ruby: attr_accessor :name
来源：http://uvh.hesvh.cn

C#:   public string Name { get; set; }
来源：http://wcy.chenjidiqi.icu

[G12] 对象转字符串
来源：http://zii.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://uvd.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bqf.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://aya.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://vpd.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://gxy.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lmt.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://pfj.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://hte.zdbjq.cn

[G13] 判断对象类型
来源：http://fjj.yvedp.cn

Py:   isinstance(u, User)
来源：http://ylr.hcnkem.com

PHP:  $u instanceof User
来源：http://nap.yj20258.top

JS:   u instanceof User
来源：http://uip.bbcook.cn

TS:   u instanceof User
来源：http://kle.iojbl.cn

Java: u instanceof User
来源：http://ipl.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vsf.hnqzz.top

Ruby: u.is_a?(User)
来源：http://mdn.daxiang520.top

C#:   u is User
来源：http://lyr.nanxuanxn.top

[G14] 数据类 / record
来源：http://slf.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rev.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://dha.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kqs.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://afi.hesvh.cn

Java: record User(String name, int age) {}
来源：http://rqw.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://uih.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xev.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://cvb.hnxiangtu.top

[G15] 枚举
来源：http://szr.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wov.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fna.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tkr.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hfg.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://ymu.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rfm.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://phg.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lhv.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://mbr.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vmo.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://klp.aizwys.cn

JS:   Object.entries(obj)
来源：http://tdb.vehdjk.com

TS:   Object.entries(obj)
来源：http://uxe.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qyv.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://npf.jianghu66.top

Ruby: obj.instance_variables
来源：http://gzg.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://uuv.c1oappe.top

================================================================================
来源：http://pnj.zhiwuduotai.top

H. 异常与错误处理
来源：http://lnw.cucudq.cn

================================================================================
来源：http://ppz.wangshuangyany.cn

[H01] try / catch 基础
来源：http://wyk.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hau.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qtk.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://koj.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ucu.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lva.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ezg.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tpz.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jer.fengsongda.top

[H02] finally / ensure 收尾
来源：http://pqb.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://obs.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ydf.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dib.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://who.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zwv.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://gqh.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://knm.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xqp.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://ooa.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://bqq.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qqs.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://sgj.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://mii.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pux.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://amy.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lui.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://wqg.hfpthk.cn

[H04] 自定义异常类型
来源：http://ahv.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://dly.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://loe.cucudq.cn

JS:   class MyError extends Error {}
来源：http://fzl.daria6918.cn

TS:   class MyError extends Error {}
来源：http://ady.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://wok.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lic.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://bip.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://yxw.yongpay.top

[H05] 捕获特定类型
来源：http://dka.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://srx.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oyo.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://xxs.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://zom.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://eqj.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ozr.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://exw.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bxe.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://zfb.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://uka.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://fyx.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://gru.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://mat.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jhs.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zjq.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://lnh.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://qcu.ybcxt.top

[H07] 断言
来源：http://zay.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://fpe.yongpay.top

PHP:  assert($x > 0);
来源：http://taw.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://dhj.yj20258888.top

TS:   console.assert(x > 0);
来源：http://qcl.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://vsg.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfd.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vtl.jinyuanbaomall.cn


<!-- 参考信息 -->