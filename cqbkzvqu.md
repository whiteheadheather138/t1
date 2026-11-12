代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cep.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gxa.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://pfi.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://spz.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ngr.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gim.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dsh.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xai.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tgi.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://yxf.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dbl.vehdjk.com

[F04] 追加写入文件
来源：http://ukj.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vva.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yhp.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzg.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdv.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qns.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wij.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qzd.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://quf.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://nuu.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xec.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://mls.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://lzf.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://sqy.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xuu.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tpq.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://clr.yj202588.top

C#:   File.Exists("a.txt")
来源：http://sef.zhongyouzk.top

[F06] 删除文件
来源：http://yeb.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://zxm.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://fuw.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wld.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://zqy.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqo.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://kef.cheryme.top

Ruby: File.delete("a.txt")
来源：http://gqi.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://jex.daria6918.cn

[F07] 创建目录（含多级）
来源：http://geg.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fea.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://elc.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jsj.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bfq.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vjg.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://klb.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ota.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jae.uphjek.com

[F08] 遍历目录
来源：http://xbe.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmk.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyc.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://wvx.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://ouz.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wpz.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qjb.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://wcg.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://xoq.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://kro.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://iqu.yuxming.cn

PHP:  filesize("a.txt");
来源：http://gbo.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://wpu.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://qez.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://pqk.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gdp.andypj.xyz

Ruby: File.size("a.txt")
来源：http://ewb.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://duh.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://mhl.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukv.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ehg.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zqw.nwbrower.top

TS:   path.extname("a.txt")
来源：http://dbg.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xgk.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xxp.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qbc.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jkf.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://edl.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lhs.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fhv.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbk.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdx.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qeg.birdmap.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kle.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pqm.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gjn.yongpay.top

[F12] CSV 读写
来源：http://qkr.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fwc.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://occ.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rso.zhoulong.xyz

TS:   // 同上
来源：http://bbr.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ozh.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jwj.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pah.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dhk.andypj.xyz

================================================================================
来源：http://whu.zhijiandao.cn

G. 面向对象
来源：http://zgv.jinyuanbaomall.cn

================================================================================
来源：http://lwh.quarkkingdee.top

[G01] 定义类
来源：http://yhr.wangshuangyany.cn

Py:   class User: pass
来源：http://wsa.zhoulong.xyz

PHP:  class User {}
来源：http://fpt.guowangkeji.top

JS:   class User {}
来源：http://pgb.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://edx.quarkkingdee.top

Java: class User {}
来源：http://kro.zycfv.cn

Go:   type User struct { Name string }
来源：http://uqt.yangfankeji.com

Ruby: class User; end
来源：http://jey.feifeiyinyue.top

C#:   class User {}
来源：http://kna.ybcxt.top

[G02] 构造函数
来源：http://vxv.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://dht.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://mtr.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://hwz.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://mbn.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://agi.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aja.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://fou.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://idv.hcnkem.com

[G03] 实例属性
来源：http://hcm.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://fkt.gzhubu.top

PHP:  public string $name = "x";
来源：http://vas.zdbjq.cn

JS:   this.name = "x";
来源：http://mrq.kuanghao11.cn

TS:   name: string = "x";
来源：http://pti.chenzaomai.com

Java: private String name;
来源：http://tpf.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yip.zhengqikj.top

Ruby: @name = "x"
来源：http://rwf.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://ash.yj202588.top

[G04] 定义方法
来源：http://fdc.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://lxv.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ivk.xuanzx.com

JS:   greet() { return this.name; }
来源：http://uer.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://pli.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://lfv.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://tiy.jyoumei.cn

Ruby: def greet; @name; end
来源：http://xit.smart0.xyz

C#:   public string Greet() => Name;
来源：http://wuk.bbcook.cn

[G05] 继承
来源：http://rlc.meibo888.top

Py:   class Admin(User): pass
来源：http://gdv.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://hqx.fktsv.cn

JS:   class Admin extends User {}
来源：http://jeh.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://dxq.hysaishi.cn

Java: class Admin extends User {}
来源：http://eae.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eom.dianchejie.cn

Ruby: class Admin < User; end
来源：http://vhs.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://wdv.cdnleiting.top

[G06] 重写方法
来源：http://xae.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://vjz.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hwr.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://ybf.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://ffx.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://fnm.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpp.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://ddi.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://ptm.pycfn.com

[G07] 调用父类方法
来源：http://khb.shanyushiyangtech.top

Py:   super().greet()
来源：http://qtz.jinqigufen.top

PHP:  parent::greet();
来源：http://hjp.ywan-chungtsiang.top

JS:   super.greet();
来源：http://clq.chenzaomai.com

TS:   super.greet();
来源：http://qxh.yuxming.cn

Java: super.greet();
来源：http://uoy.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://crd.daxiang520.top

Ruby: super
来源：http://zax.fzhhl.top

C#:   base.Greet();
来源：http://ojo.redwolf501.top

[G08] 静态方法与属性
来源：http://bxc.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cri.bjfxy.top

PHP:  public static function f() {}
来源：http://fdo.xuanzx.com

JS:   static f() {}
来源：http://dcc.pycfn.com

TS:   static f(): void {}
来源：http://cmb.yueranfly.top

Java: static void f() {}
来源：http://hbh.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tmh.yj20258.top

Ruby: def self.f; end
来源：http://zrk.xuanzx.com

C#:   public static void F() {}
来源：http://jyj.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://cnq.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://kjq.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://him.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qid.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://ruh.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://sac.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://vcl.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qms.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://nry.yuxming.cn

[G10] 访问控制
来源：http://gts.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://tah.jianghu66.top

PHP:  public / protected / private
来源：http://mbr.yvedp.cn

JS:   #private 字段；其余公开
来源：http://pel.chenlongwang.top

TS:   public / protected / private
来源：http://xui.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://xdw.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://eta.zhongyouzk.top

Ruby: public / protected / private
来源：http://fxb.jinqigufen.top

C#:   public / protected / private / internal
来源：http://wuh.pycfn.com

[G11] getter / setter
来源：http://lig.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://qyb.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://swm.fehbvm.com

JS:   get name() { return this._name; }
来源：http://eoj.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://pwu.fktsv.cn

Java: public String getName() { return name; }
来源：http://yev.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ptx.yonumen.top

Ruby: attr_accessor :name
来源：http://lrg.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://bme.shuidangran.top

[G12] 对象转字符串
来源：http://zsc.yongpay.top

Py:   def __str__(self): return self.name
来源：http://ndg.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wjh.316326.xyz

JS:   toString() { return this.name; }
来源：http://kkb.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://vyn.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://pyl.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://zgy.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://vcz.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://hex.bjfxy.top

[G13] 判断对象类型
来源：http://vds.yj20258888.top

Py:   isinstance(u, User)
来源：http://xgi.quarkkingdee.top

PHP:  $u instanceof User
来源：http://vgy.zhixingplan.top

JS:   u instanceof User
来源：http://cgv.yueranfly.top

TS:   u instanceof User
来源：http://oqc.yj20258.top

Java: u instanceof User
来源：http://lwy.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mbt.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://jzl.hcnkem.com

C#:   u is User
来源：http://xfa.cqqwz.cn

[G14] 数据类 / record
来源：http://mfn.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sfo.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://fhw.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://gbi.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://hkk.ydzc1.top

Java: record User(String name, int age) {}
来源：http://ktk.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://tna.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bdm.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://pwg.nwbrower.top

[G15] 枚举
来源：http://suk.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uaq.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://azh.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jbi.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hkp.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://jca.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://for.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://ixv.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mdr.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://kqi.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vmm.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://qxj.tian-w.cn

JS:   Object.entries(obj)
来源：http://fwl.guannengcc.top

TS:   Object.entries(obj)
来源：http://vvk.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mcx.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://amt.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://gil.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://gip.yj20258888.top

================================================================================
来源：http://sfg.guowangkeji.top

H. 异常与错误处理
来源：http://jit.jqgfzy.top

================================================================================
来源：http://yqk.zhixingplan.top

[H01] try / catch 基础
来源：http://vfb.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://spt.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dcc.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jet.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://stc.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bzt.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ktt.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ovd.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iel.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://jca.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wey.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://wmu.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://imo.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ono.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://wdi.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://evb.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cyv.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://kgj.yongpay.top

[H03] 主动抛出异常
来源：http://acy.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://tms.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ylf.meibo888.top

JS:   throw new Error("错误信息");
来源：http://qku.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://shz.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://har.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qyr.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rlu.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://rmn.haohaochexian.top

[H04] 自定义异常类型
来源：http://nul.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://hxs.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://eiz.bbcook.cn

JS:   class MyError extends Error {}
来源：http://mnr.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://cgw.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://wwp.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://khm.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://dve.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://bue.fengsongda.top

[H05] 捕获特定类型
来源：http://mwb.zdbjq.cn

Py:   except ValueError as e:
来源：http://ypg.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ipj.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://zrk.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ybh.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://gkn.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yaq.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://rfs.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xbz.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://nvd.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://bor.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://joq.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://trf.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hly.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bbg.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lzr.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://zym.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://zxo.jinqigfzy.top

[H07] 断言
来源：http://rvq.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://ott.aizwys.cn

PHP:  assert($x > 0);
来源：http://wrd.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://oip.meibo888.top


<!-- 参考信息 -->