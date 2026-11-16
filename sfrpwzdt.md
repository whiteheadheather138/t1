代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uso.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://xyy.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ryg.pengpengdd.cyou

[F04] 追加写入文件
来源：http://pct.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bxy.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pug.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://act.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uws.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pej.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xkj.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nfa.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jbw.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://dhb.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tsn.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://aqg.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://few.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://ull.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lrp.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lgr.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://cys.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://cjv.xuetiantiany.cn

[F06] 删除文件
来源：http://mvb.aizwys.cn

Py:   os.remove("a.txt")
来源：http://ohb.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://mwk.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://uke.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://mgu.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ofv.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://csq.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://hvu.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://baa.yfazqb.com

[F07] 创建目录（含多级）
来源：http://tsf.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://twc.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hdn.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xvb.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cbl.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hbb.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gbc.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lxb.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fhp.jianghu66.top

[F08] 遍历目录
来源：http://znn.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://oul.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vcr.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://txp.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://ndm.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sxk.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wye.meibo888.top

Ruby: Dir.children("dir")
来源：http://ehb.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://hcr.hongshengwenyu.top

[F09] 获取文件大小
来源：http://nid.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://axv.vehdjk.com

PHP:  filesize("a.txt");
来源：http://pgg.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://suy.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://byv.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eol.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gtm.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://mae.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://khs.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://wcl.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yzy.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xae.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhq.hesvh.cn

TS:   path.extname("a.txt")
来源：http://yqn.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://awl.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dhn.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qir.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jhv.cheryme.top

[F11] 复制与移动文件
来源：http://eym.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lfh.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ege.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xnq.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgf.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lqi.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bxg.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iep.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rgk.tarul.cn

[F12] CSV 读写
来源：http://nex.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lyt.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rzu.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rhl.vehdjk.com

TS:   // 同上
来源：http://zvj.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hso.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tuf.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yfu.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nic.ywan-chungtsiang.top

================================================================================
来源：http://uda.xuetiantiany.cn

G. 面向对象
来源：http://dhd.quarkkingdee.top

================================================================================
来源：http://gyk.nwbrower.top

[G01] 定义类
来源：http://yzo.jyoumei.cn

Py:   class User: pass
来源：http://zzp.xylfe.cn

PHP:  class User {}
来源：http://ypq.shzxlz.cn

JS:   class User {}
来源：http://ohy.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://tid.jqgufenzy.top

Java: class User {}
来源：http://iec.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://dgh.yfazqb.com

Ruby: class User; end
来源：http://wqk.gotoacloud.top

C#:   class User {}
来源：http://xnh.jinqigfzy.top

[G02] 构造函数
来源：http://dxg.ctjpmb.com

Py:   def __init__(self, name): self.name = name
来源：http://jij.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://oob.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://cyh.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://vim.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://aud.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wlt.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://rlu.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://hrc.nanxuanxn.top

[G03] 实例属性
来源：http://csf.0kj1m.cn

Py:   self.name = "x"
来源：http://ubo.dianchejie.cn

PHP:  public string $name = "x";
来源：http://xqc.chenlongwang.top

JS:   this.name = "x";
来源：http://grx.wangdashe.top

TS:   name: string = "x";
来源：http://smt.hfpthk.cn

Java: private String name;
来源：http://jiz.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ysj.fzhhl.top

Ruby: @name = "x"
来源：http://xfa.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://zdq.jinghuilouyu.cn

[G04] 定义方法
来源：http://ofw.c1oappe.top

Py:   def greet(self): return self.name
来源：http://ixa.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rww.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://lbs.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://fei.meibo888.top

Java: String greet() { return name; }
来源：http://mea.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wbp.zhengqikj.top

Ruby: def greet; @name; end
来源：http://idx.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://yje.vqdsnc.cn

[G05] 继承
来源：http://dje.zdbjq.cn

Py:   class Admin(User): pass
来源：http://wwv.shuidangran.top

PHP:  class Admin extends User {}
来源：http://tmj.jianghu66.top

JS:   class Admin extends User {}
来源：http://twp.snrcjt.cn

TS:   class Admin extends User {}
来源：http://bnv.hnxiangtu.top

Java: class Admin extends User {}
来源：http://auz.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bus.zhixingplan.top

Ruby: class Admin < User; end
来源：http://vdv.quarkkingdee.top

C#:   class Admin : User {}
来源：http://ukj.jianghu66.top

[G06] 重写方法
来源：http://erv.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://eyp.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bkv.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://mze.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://cap.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://xhl.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cqw.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://afr.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://lka.nanxinkj.top

[G07] 调用父类方法
来源：http://lps.xuanzx.com

Py:   super().greet()
来源：http://sul.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://ida.sjlbkw.cn

JS:   super.greet();
来源：http://smt.yangfankeji.com

TS:   super.greet();
来源：http://olm.kuanghao11.cn

Java: super.greet();
来源：http://lgh.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ami.cheryme.top

Ruby: super
来源：http://oyt.epnwcf.com

C#:   base.Greet();
来源：http://apc.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://tgy.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qxy.ydjk.org.cn

PHP:  public static function f() {}
来源：http://qkj.yj202588.top

JS:   static f() {}
来源：http://osp.yueranfly.top

TS:   static f(): void {}
来源：http://zmk.yj202588.top

Java: static void f() {}
来源：http://pot.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://koi.sufxvd.cn

Ruby: def self.f; end
来源：http://igs.zdbjq.cn

C#:   public static void F() {}
来源：http://plz.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://lec.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://xgg.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sld.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhb.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://bbk.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://yvf.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://twt.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pxn.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://prj.yj20258888.top

[G10] 访问控制
来源：http://bzd.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://eat.zhongyouzk.top

PHP:  public / protected / private
来源：http://fck.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://dzs.svipenyu.cn

TS:   public / protected / private
来源：http://lmo.316326.xyz

Java: public / protected / private / 默认包级
来源：http://gtb.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kpn.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://lcr.xziqi.cn

C#:   public / protected / private / internal
来源：http://iqe.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://biy.yonumen.top

Py:   @property 与 @x.setter
来源：http://jhe.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jda.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://rgs.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://txw.yj20258888.top

Java: public String getName() { return name; }
来源：http://uut.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://npa.cqqwz.cn

Ruby: attr_accessor :name
来源：http://fms.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://alg.guowangkeji.top

[G12] 对象转字符串
来源：http://bgc.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://sur.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zkg.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://hta.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://zxv.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://tsh.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://yvz.hnqzz.top

Ruby: def to_s; @name; end
来源：http://bjf.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://goo.ppjwa.cn

[G13] 判断对象类型
来源：http://rkm.cdnleiting.top

Py:   isinstance(u, User)
来源：http://lfw.jlsjyb.cn

PHP:  $u instanceof User
来源：http://tau.yangfankeji.com

JS:   u instanceof User
来源：http://gtd.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://ygm.jinqigufen.top

Java: u instanceof User
来源：http://qzd.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iar.cucudq.cn

Ruby: u.is_a?(User)
来源：http://xfu.c1oappe.top

C#:   u is User
来源：http://tdo.wangdashe.top

[G14] 数据类 / record
来源：http://dew.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ikb.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://btd.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uhz.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://fzg.tarul.cn

Java: record User(String name, int age) {}
来源：http://klq.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://dye.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uvd.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://sjd.ydjk.org.cn

[G15] 枚举
来源：http://xod.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://duf.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://czt.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dte.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kbp.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://hwj.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ztf.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://anl.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cyc.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://uqi.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bju.yj20258.top

PHP:  get_object_vars($obj);
来源：http://rae.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://uab.snrcjt.cn

TS:   Object.entries(obj)
来源：http://uwn.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wte.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijp.yonumen.top

Ruby: obj.instance_variables
来源：http://auq.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://znw.quarkkingdee.top

================================================================================
来源：http://dqq.vqdsnc.cn

H. 异常与错误处理
来源：http://tmk.jinqigufen.top

================================================================================
来源：http://ydl.tian-w.cn

[H01] try / catch 基础
来源：http://wai.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vet.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsi.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dlm.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wex.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pxv.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pmw.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rzm.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yvd.xinyue.icu

[H02] finally / ensure 收尾
来源：http://xlp.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://nir.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hvp.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://osf.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wxw.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://tpb.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dvs.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qae.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qam.sufxvd.cn

[H03] 主动抛出异常
来源：http://pys.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://thx.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nna.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://vig.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://rfq.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://seh.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://enr.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vwv.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://bjj.yj20258.top

[H04] 自定义异常类型
来源：http://xkm.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://nju.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://xcv.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://xjs.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://loo.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://ywu.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pud.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://ovu.nwbrower.top

C#:   class MyException : Exception {}
来源：http://hkd.yuanzhike.top

[H05] 捕获特定类型
来源：http://wmy.shuidangran.top

Py:   except ValueError as e:
来源：http://ena.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vzc.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://ash.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://cfx.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://aph.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vrs.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://yjg.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vto.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://cqp.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://vzj.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://gkv.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fjq.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://gwz.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xvf.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://htq.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://ksm.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://kqw.dianchejie.cn

[H07] 断言
来源：http://jnc.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://oyd.haohaochexian.top

PHP:  assert($x > 0);
来源：http://xzj.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://alw.c1oappe.top

TS:   console.assert(x > 0);
来源：http://paz.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://rgv.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://azo.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://min.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://maq.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://vhm.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://hye.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vgy.guowangkeji.top


<!-- 参考信息 -->