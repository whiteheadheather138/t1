代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zqi.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://csw.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewx.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvx.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ovy.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fkm.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yph.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ome.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://wqw.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rmw.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://sgj.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://hwt.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://vhi.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lzl.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://abw.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://ngh.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://kih.guowangkeji.top

[F06] 删除文件
来源：http://kiq.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://xxq.epnwcf.com

PHP:  unlink("a.txt");
来源：http://vhi.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://yhq.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sqb.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://end.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://pvk.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://rxd.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://mrv.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://hnk.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rid.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ooc.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pjm.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjj.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zbt.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nhn.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zlu.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ewb.jyoumei.cn

[F08] 遍历目录
来源：http://hav.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bff.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zvr.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://ovn.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://scj.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ydp.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jzn.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://imw.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://imm.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://jey.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://pif.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://pso.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://ssx.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://ymf.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dbr.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xty.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://evr.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://rpm.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://fzi.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kwz.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pqt.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://okw.daxiang520.top

TS:   path.extname("a.txt")
来源：http://mzs.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tdm.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vlu.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tpz.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bqb.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://dad.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nst.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jtp.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdo.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpu.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fqe.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdz.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://scl.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bce.gogol.net.cn

[F12] CSV 读写
来源：http://eim.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xrl.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zfr.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rnj.pengpengdd.cyou

TS:   // 同上
来源：http://ddt.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tqy.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cuy.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jot.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gxe.xuetiantiany.cn

================================================================================
来源：http://etj.dianchejie.cn

G. 面向对象
来源：http://umq.fktsv.cn

================================================================================
来源：http://rbb.tianlin.xyz

[G01] 定义类
来源：http://pep.0kj1m.cn

Py:   class User: pass
来源：http://sfv.c1oappe.top

PHP:  class User {}
来源：http://cdw.smart0.xyz

JS:   class User {}
来源：http://pfm.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://bso.ydzc1.top

Java: class User {}
来源：http://une.0kj1m.cn

Go:   type User struct { Name string }
来源：http://ndc.jinqigufen.top

Ruby: class User; end
来源：http://cke.yanxiufei.cn

C#:   class User {}
来源：http://kdw.sweek.top

[G02] 构造函数
来源：http://hnv.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://mqw.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://lzp.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://lar.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://zjy.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://vzv.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdx.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://ixd.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://zbg.yj202588.top

[G03] 实例属性
来源：http://eek.bbcook.cn

Py:   self.name = "x"
来源：http://zmz.ivvv.top

PHP:  public string $name = "x";
来源：http://pvx.tian-w.cn

JS:   this.name = "x";
来源：http://qdl.chenzaomai.com

TS:   name: string = "x";
来源：http://udv.zycfv.cn

Java: private String name;
来源：http://dhm.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ozm.andypj.xyz

Ruby: @name = "x"
来源：http://zmm.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://tgd.iojbl.cn

[G04] 定义方法
来源：http://yny.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://spp.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uem.fzhhl.top

JS:   greet() { return this.name; }
来源：http://kqu.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://vlg.guowangkeji.top

Java: String greet() { return name; }
来源：http://hul.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nep.9152youxi.cn

Ruby: def greet; @name; end
来源：http://gyp.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://dik.xuetiantiany.cn

[G05] 继承
来源：http://ktb.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://cmf.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://fgz.zhixingplan.top

JS:   class Admin extends User {}
来源：http://gwc.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://anx.quarkkingdee.top

Java: class Admin extends User {}
来源：http://qbg.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qqf.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://vss.yuanzhike.top

C#:   class Admin : User {}
来源：http://gyu.redwolf501.top

[G06] 重写方法
来源：http://gcw.yonumen.top

Py:   def greet(self): return "admin"
来源：http://xil.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vyv.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://ois.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://fgg.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://lac.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uns.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://jzv.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://fso.gotoacloud.top

[G07] 调用父类方法
来源：http://myn.xuanzx.com

Py:   super().greet()
来源：http://ulj.nanxuanxn.top

PHP:  parent::greet();
来源：http://scn.bjfxy.top

JS:   super.greet();
来源：http://fof.hywenlv.cn

TS:   super.greet();
来源：http://cjk.bjfxy.top

Java: super.greet();
来源：http://bav.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zhj.xinyue.icu

Ruby: super
来源：http://qrs.gaohongyu789.top

C#:   base.Greet();
来源：http://tzw.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://rif.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ynt.gotoacloud.top

PHP:  public static function f() {}
来源：http://rll.ctjpmb.com

JS:   static f() {}
来源：http://kbz.shangyingyoupin.top

TS:   static f(): void {}
来源：http://mzg.dianchejie.cn

Java: static void f() {}
来源：http://hfp.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rjf.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://cir.zycfv.cn

C#:   public static void F() {}
来源：http://tnu.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://edt.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://lro.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jkw.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bkd.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://xow.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://nzl.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://gvk.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eax.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://wqh.fengsongda.top

[G10] 访问控制
来源：http://izq.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://aur.mhx1999.top

PHP:  public / protected / private
来源：http://yiu.xziqi.cn

JS:   #private 字段；其余公开
来源：http://zfp.guowangkeji.top

TS:   public / protected / private
来源：http://lqb.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://ukh.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://exp.xinyue.icu

Ruby: public / protected / private
来源：http://caw.0kj1m.cn

C#:   public / protected / private / internal
来源：http://rcg.zdqjudy.top

[G11] getter / setter
来源：http://vrs.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://srv.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://itv.epnwcf.com

JS:   get name() { return this._name; }
来源：http://tko.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://owa.c1oappe.top

Java: public String getName() { return name; }
来源：http://ilb.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mzl.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://afc.nwbrower.top

C#:   public string Name { get; set; }
来源：http://xhp.zhijiandao.cn

[G12] 对象转字符串
来源：http://qge.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://egy.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oyd.yongpay.top

JS:   toString() { return this.name; }
来源：http://wpx.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://rsu.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://tyh.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://dsk.xylfe.cn

Ruby: def to_s; @name; end
来源：http://crm.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://svj.vqdsnc.cn

[G13] 判断对象类型
来源：http://kyd.bjfxy.top

Py:   isinstance(u, User)
来源：http://yrk.quarkkingdee.top

PHP:  $u instanceof User
来源：http://yug.cdnleiting.top

JS:   u instanceof User
来源：http://qsh.sjlbkw.cn

TS:   u instanceof User
来源：http://emh.ppjwa.cn

Java: u instanceof User
来源：http://ylt.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bjh.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://yso.tanke756.top

C#:   u is User
来源：http://saq.uphjek.com

[G14] 数据类 / record
来源：http://nve.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jbp.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://pup.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dln.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://rvb.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://cgd.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://qzl.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ahv.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://ylz.zdbjq.cn

[G15] 枚举
来源：http://qdw.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hdf.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hbg.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hly.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wil.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://hge.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsf.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://iuz.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lnj.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://ewr.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gjd.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://bad.yangfankeji.com

JS:   Object.entries(obj)
来源：http://tog.birdmap.top

TS:   Object.entries(obj)
来源：http://jow.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kqv.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hin.jianghu66.top

Ruby: obj.instance_variables
来源：http://mrs.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://zhx.tian-w.cn

================================================================================
来源：http://wfu.yanxiufei.cn

H. 异常与错误处理
来源：http://dhb.ppjwa.cn

================================================================================
来源：http://kun.shangyingyoupin.top

[H01] try / catch 基础
来源：http://pmx.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hnk.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://stp.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yvo.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mbg.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ntx.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cts.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qxi.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jpj.yj202588.top

[H02] finally / ensure 收尾
来源：http://ogt.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wer.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vwu.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kyq.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uou.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://rtb.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jgl.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zlx.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fll.hcnkem.com

[H03] 主动抛出异常
来源：http://ecf.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://mvi.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fop.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://pwt.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://gzp.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ivz.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rdb.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pug.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://wic.guannengcc.top

[H04] 自定义异常类型
来源：http://bsp.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://aar.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://mgk.mhx1999.top

JS:   class MyError extends Error {}
来源：http://xcj.epnwcf.com

TS:   class MyError extends Error {}
来源：http://kvb.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://fvx.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pft.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://vji.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://ipu.shuidangran.top

[H05] 捕获特定类型
来源：http://pyt.cqqwz.cn

Py:   except ValueError as e:
来源：http://zyy.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kaj.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://rdx.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://fym.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://nrv.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lpu.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://tpu.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jrw.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://qvg.nwbrower.top

Py:   value = d.get("k") or default
来源：http://dfw.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://snw.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vfs.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://uyw.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hjb.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ccs.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://lsa.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://vdd.havefunace.top

[H07] 断言
来源：http://nuz.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://hip.zhixingplan.top

PHP:  assert($x > 0);
来源：http://ham.xylfe.cn

JS:   console.assert(x > 0);
来源：http://dyj.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://cpn.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://rxi.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wuk.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://lox.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://agl.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://txp.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://vvm.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kzv.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://hqb.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcq.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://shr.jqgufenzy.top

Go:   err.Error()
来源：http://roh.gogol.net.cn


<!-- 参考信息 -->