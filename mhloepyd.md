代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xbs.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ezw.yongpay.top

[F03] 写入文件（覆盖）
来源：http://svm.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://spm.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://huj.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yju.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uag.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vbf.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ayq.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://ipn.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pqi.shangyingyoupin.top

[F04] 追加写入文件
来源：http://uou.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zmc.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ghe.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvc.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://byk.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bis.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jvc.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mro.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yex.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://bjk.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://seb.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://tpx.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://ncv.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://gvn.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ybw.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://llk.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://vzq.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://gje.havefunace.top

[F06] 删除文件
来源：http://cxz.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://vmq.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://pep.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dzz.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://qqt.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rgb.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://lsv.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://lcm.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://ibr.hnqzz.top

[F07] 创建目录（含多级）
来源：http://lwu.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://huu.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vyc.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sle.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmt.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ild.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://byo.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ovm.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zug.shanyushiyangtech.top

[F08] 遍历目录
来源：http://mns.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wjj.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zwx.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://uga.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://src.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zjn.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jza.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://dnx.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://oiy.nwbrower.top

[F09] 获取文件大小
来源：http://ovv.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://xge.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://pqe.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://kje.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://psv.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zbr.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zvz.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://qad.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://pem.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://enn.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sea.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oll.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lcw.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://jks.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zge.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lpt.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pxg.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sww.ctjpmb.com

[F11] 复制与移动文件
来源：http://wbm.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywl.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tdm.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixe.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hcn.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tir.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://skg.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ecb.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mnl.fzhhl.top

[F12] CSV 读写
来源：http://mhf.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lad.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wok.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cja.yj20258888.top

TS:   // 同上
来源：http://ipr.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://spd.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ywy.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jcs.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://noa.vqdsnc.cn

================================================================================
来源：http://nmb.xylfe.cn

G. 面向对象
来源：http://fiq.cashguo.top

================================================================================
来源：http://txh.cashguo.top

[G01] 定义类
来源：http://byh.aizwys.cn

Py:   class User: pass
来源：http://zol.chenlongwang.top

PHP:  class User {}
来源：http://sxl.ydzc1.top

JS:   class User {}
来源：http://dde.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://upt.yj20258888.top

Java: class User {}
来源：http://jzw.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://mkp.ywan-chungtsiang.top

Ruby: class User; end
来源：http://dnd.jyoumei.cn

C#:   class User {}
来源：http://ywr.chenjidiqi.icu

[G02] 构造函数
来源：http://dcp.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://ncm.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://mmb.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://yqd.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://kii.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://hzz.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fcv.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://uol.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://shd.yj202588.top

[G03] 实例属性
来源：http://bvl.feifeiyinyue.top

Py:   self.name = "x"
来源：http://rwf.yongpay.top

PHP:  public string $name = "x";
来源：http://ldg.xinyue.icu

JS:   this.name = "x";
来源：http://ypg.feifeiyinyue.top

TS:   name: string = "x";
来源：http://pui.chenzaomai.com

Java: private String name;
来源：http://pck.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zek.xinyue.icu

Ruby: @name = "x"
来源：http://uzp.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://txm.zdbjq.cn

[G04] 定义方法
来源：http://spz.ybcxt.top

Py:   def greet(self): return self.name
来源：http://wiz.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rjl.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://bis.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://elq.shzxlz.cn

Java: String greet() { return name; }
来源：http://div.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mez.fengsongda.top

Ruby: def greet; @name; end
来源：http://pvv.zycfv.cn

C#:   public string Greet() => Name;
来源：http://esc.zhoulong.xyz

[G05] 继承
来源：http://oto.hfpthk.cn

Py:   class Admin(User): pass
来源：http://cwl.fzhhl.top

PHP:  class Admin extends User {}
来源：http://hrs.jyoumei.cn

JS:   class Admin extends User {}
来源：http://uny.fehbvm.com

TS:   class Admin extends User {}
来源：http://twb.xinyue.icu

Java: class Admin extends User {}
来源：http://yny.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oou.cashguo.top

Ruby: class Admin < User; end
来源：http://tdd.ybcxt.top

C#:   class Admin : User {}
来源：http://dsi.cashguo.top

[G06] 重写方法
来源：http://brm.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://kqh.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wfq.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://tvf.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://ejm.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://iwe.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nuh.hammf.cn

Ruby: def greet; "admin"; end
来源：http://wku.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://kpn.ybcxt.top

[G07] 调用父类方法
来源：http://zec.9152youxi.cn

Py:   super().greet()
来源：http://zle.yongpay.top

PHP:  parent::greet();
来源：http://iry.chenlongwang.top

JS:   super.greet();
来源：http://jrh.chenzaomai.com

TS:   super.greet();
来源：http://tbv.mhx1999.top

Java: super.greet();
来源：http://hzc.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ohs.uphjek.com

Ruby: super
来源：http://ejq.snrcjt.cn

C#:   base.Greet();
来源：http://nuf.hfpthk.cn

[G08] 静态方法与属性
来源：http://pof.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aje.quarkkingdee.top

PHP:  public static function f() {}
来源：http://ysd.vqdsnc.cn

JS:   static f() {}
来源：http://zsa.hammf.cn

TS:   static f(): void {}
来源：http://uic.yanxiufei.cn

Java: static void f() {}
来源：http://fpa.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zol.sjlbkw.cn

Ruby: def self.f; end
来源：http://ssy.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://zgx.hcnkem.com

[G09] 接口 / 抽象类
来源：http://apz.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://xyq.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://ecm.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zgz.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://daw.yvedp.cn

Java: interface Shape { double area(); }
来源：http://qlv.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://wns.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdj.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://twe.zdqjudy.top

[G10] 访问控制
来源：http://eht.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://eso.yj20258888.top

PHP:  public / protected / private
来源：http://bor.yj20258.top

JS:   #private 字段；其余公开
来源：http://vtw.pengpengdd.cyou

TS:   public / protected / private
来源：http://drt.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://zgn.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ray.gaohongyu789.top

Ruby: public / protected / private
来源：http://omj.zhixingplan.top

C#:   public / protected / private / internal
来源：http://xfz.tian-w.cn

[G11] getter / setter
来源：http://ofk.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://jyr.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xjq.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://wdz.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://qxo.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://oyj.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://hku.mhx1999.top

Ruby: attr_accessor :name
来源：http://bae.sxryk.cn

C#:   public string Name { get; set; }
来源：http://nre.vehdjk.com

[G12] 对象转字符串
来源：http://ufy.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://fnv.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mlt.bjfxy.top

JS:   toString() { return this.name; }
来源：http://tjx.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://kya.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://dsv.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://wor.fktsv.cn

Ruby: def to_s; @name; end
来源：http://xcs.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://xfb.gzhubu.top

[G13] 判断对象类型
来源：http://mfe.yueranfly.top

Py:   isinstance(u, User)
来源：http://zpe.yuanzhike.top

PHP:  $u instanceof User
来源：http://rzr.svipenyu.cn

JS:   u instanceof User
来源：http://aje.cqqwz.cn

TS:   u instanceof User
来源：http://ifv.hcnkem.com

Java: u instanceof User
来源：http://cxs.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kmw.uphjek.com

Ruby: u.is_a?(User)
来源：http://nib.zhixingplan.top

C#:   u is User
来源：http://hjm.hongshengwenyu.top

[G14] 数据类 / record
来源：http://ekx.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ezs.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://qky.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://jis.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://rqs.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://xqt.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://sgx.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhp.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://cjx.hysaishi.cn

[G15] 枚举
来源：http://hex.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bxj.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oqm.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dfu.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ilt.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://kgm.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ajn.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://lyb.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mpn.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://tmu.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zfx.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://ehw.chenzaomai.com

JS:   Object.entries(obj)
来源：http://uiw.haohaochexian.top

TS:   Object.entries(obj)
来源：http://pvc.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gti.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zgr.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://rvw.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xuv.shuidangran.top

================================================================================
来源：http://rag.shzxlz.cn

H. 异常与错误处理
来源：http://hud.sufxvd.cn

================================================================================
来源：http://daz.c1oappe.top

[H01] try / catch 基础
来源：http://bwn.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://taa.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ljr.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://igc.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mwc.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hys.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kiy.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jug.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jpl.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://clp.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://idn.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffa.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pnk.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pxh.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://cjo.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://axd.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zxe.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://gfv.cashguo.top

[H03] 主动抛出异常
来源：http://fam.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://aag.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aio.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://fzp.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://spx.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dtm.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bfa.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rpo.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://aos.sxryk.cn

[H04] 自定义异常类型
来源：http://pej.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://qvw.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ozk.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://put.meibo888.top

TS:   class MyError extends Error {}
来源：http://pzk.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://ltl.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zme.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://unj.c1oappe.top

C#:   class MyException : Exception {}
来源：http://pps.tarul.cn

[H05] 捕获特定类型
来源：http://akl.xziqi.cn

Py:   except ValueError as e:
来源：http://kyh.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qkk.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://man.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://pdy.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://dmy.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rjb.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://azl.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mbi.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://vof.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://ijp.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://czg.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ioo.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://gof.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xoz.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qsc.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://tvz.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://wkf.aizwys.cn

[H07] 断言
来源：http://wjk.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://jes.nanxinkj.top

PHP:  assert($x > 0);
来源：http://tcx.xziqi.cn

JS:   console.assert(x > 0);
来源：http://axu.bjfxy.top


<!-- 参考信息 -->