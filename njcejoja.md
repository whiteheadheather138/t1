代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://zmg.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tba.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbu.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gsj.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://amu.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://rum.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bzm.fehbvm.com

[F04] 追加写入文件
来源：http://iql.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bii.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gjo.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://whb.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pjo.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ioy.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nqy.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://les.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lgp.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://cng.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nct.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://men.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://lot.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://ovf.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wkl.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://noe.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://wtf.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://kan.hongshengwenyu.top

[F06] 删除文件
来源：http://yol.yuxming.cn

Py:   os.remove("a.txt")
来源：http://cmh.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://ben.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iud.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://obx.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nre.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://fus.ivvv.top

Ruby: File.delete("a.txt")
来源：http://gmf.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://rfu.wangdashe.top

[F07] 创建目录（含多级）
来源：http://rel.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qkn.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kjz.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tor.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xit.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nfu.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wfg.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kpc.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://etw.chenjidiqi.icu

[F08] 遍历目录
来源：http://czi.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vjb.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fqv.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://ndp.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://imj.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sbh.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uqa.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://ecf.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://pic.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://nck.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://jdw.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://hxn.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://adu.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://pqg.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://aly.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mqk.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://puk.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://qdg.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://xvk.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://swq.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kbh.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ymn.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://azs.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://soq.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://asa.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yyo.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qpi.svipenyu.cn

[F11] 复制与移动文件
来源：http://lzf.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fnb.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uil.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zaz.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://srt.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ccd.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bqp.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tjl.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nlj.smart0.xyz

[F12] CSV 读写
来源：http://zxe.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xzo.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lls.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ofg.sweek.top

TS:   // 同上
来源：http://aof.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lyx.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pls.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uhe.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pfm.316326.xyz

================================================================================
来源：http://tjl.shzxlz.cn

G. 面向对象
来源：http://fzp.yonumen.top

================================================================================
来源：http://hgk.yonumen.top

[G01] 定义类
来源：http://ymm.zhengqikj.top

Py:   class User: pass
来源：http://krn.xylfe.cn

PHP:  class User {}
来源：http://ilg.yanxiufei.cn

JS:   class User {}
来源：http://hdf.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://iza.pengpengdd.cyou

Java: class User {}
来源：http://jng.yueranfly.top

Go:   type User struct { Name string }
来源：http://ctl.chenlongwang.top

Ruby: class User; end
来源：http://lep.zhoulong.xyz

C#:   class User {}
来源：http://wps.yuanzhike.top

[G02] 构造函数
来源：http://jac.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://nrr.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://khv.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://svm.hammf.cn

TS:   constructor(public name: string) {}
来源：http://mbv.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://pjd.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dvg.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://iqd.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://syy.hammf.cn

[G03] 实例属性
来源：http://kxw.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://xtr.epnwcf.com

PHP:  public string $name = "x";
来源：http://tfj.shuidangran.top

JS:   this.name = "x";
来源：http://niv.snrcjt.cn

TS:   name: string = "x";
来源：http://fgv.fzhhl.top

Java: private String name;
来源：http://awt.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lmi.dianchejie.cn

Ruby: @name = "x"
来源：http://dph.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://zsv.sjlbkw.cn

[G04] 定义方法
来源：http://faw.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://awq.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vuj.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://xgl.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://sgx.hysaishi.cn

Java: String greet() { return name; }
来源：http://rej.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aqf.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://wjv.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://vjg.yj20258888.top

[G05] 继承
来源：http://paf.fzhhl.top

Py:   class Admin(User): pass
来源：http://fct.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://axb.snrcjt.cn

JS:   class Admin extends User {}
来源：http://msu.zdbjq.cn

TS:   class Admin extends User {}
来源：http://yus.kuanghao11.cn

Java: class Admin extends User {}
来源：http://ieq.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mfs.gotoacloud.top

Ruby: class Admin < User; end
来源：http://ccd.jlsjyb.cn

C#:   class Admin : User {}
来源：http://ren.jyoumei.cn

[G06] 重写方法
来源：http://tnd.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://yvd.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nxw.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://ufo.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://evh.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://gik.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://frm.316326.xyz

Ruby: def greet; "admin"; end
来源：http://ctl.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://ihv.cheryme.top

[G07] 调用父类方法
来源：http://liv.xuetiantiany.cn

Py:   super().greet()
来源：http://nke.shuidangran.top

PHP:  parent::greet();
来源：http://dxl.gaohongyu789.top

JS:   super.greet();
来源：http://rvm.cucudq.cn

TS:   super.greet();
来源：http://vuq.nanxuanxn.top

Java: super.greet();
来源：http://znl.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kzo.tanke756.top

Ruby: super
来源：http://kar.bjfxy.top

C#:   base.Greet();
来源：http://nlo.xziqi.cn

[G08] 静态方法与属性
来源：http://cvc.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tlh.yuanzhike.top

PHP:  public static function f() {}
来源：http://cqd.hammf.cn

JS:   static f() {}
来源：http://log.yuxming.cn

TS:   static f(): void {}
来源：http://ork.gzhubu.top

Java: static void f() {}
来源：http://gnp.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gar.yanxiufei.cn

Ruby: def self.f; end
来源：http://eoa.fktsv.cn

C#:   public static void F() {}
来源：http://aca.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://cvw.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://pii.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://vbg.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://kjf.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://crm.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://ylz.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://chz.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yrb.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://mbe.yj202588.top

[G10] 访问控制
来源：http://klm.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://dee.nanxinkj.top

PHP:  public / protected / private
来源：http://ejm.hammf.cn

JS:   #private 字段；其余公开
来源：http://qai.feifeiyinyue.top

TS:   public / protected / private
来源：http://ayi.ivvv.top

Java: public / protected / private / 默认包级
来源：http://umq.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gke.hfpthk.cn

Ruby: public / protected / private
来源：http://hhh.iojbl.cn

C#:   public / protected / private / internal
来源：http://chm.wangdashe.top

[G11] getter / setter
来源：http://grj.hammf.cn

Py:   @property 与 @x.setter
来源：http://zyw.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://lkw.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://has.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://lba.uphjek.com

Java: public String getName() { return name; }
来源：http://vvx.jqgfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lcb.fehbvm.com

Ruby: attr_accessor :name
来源：http://btn.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://ylo.tian-w.cn

[G12] 对象转字符串
来源：http://rgx.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://fyh.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://qmd.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://qaz.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://pef.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://yld.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://thr.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://eng.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://wjz.svipenyu.cn

[G13] 判断对象类型
来源：http://cmb.iojbl.cn

Py:   isinstance(u, User)
来源：http://dot.hcnkem.com

PHP:  $u instanceof User
来源：http://bzi.c1oappe.top

JS:   u instanceof User
来源：http://ich.pycfn.com

TS:   u instanceof User
来源：http://fnj.ybcxt.top

Java: u instanceof User
来源：http://xhp.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qre.tanke756.top

Ruby: u.is_a?(User)
来源：http://qsi.cucudq.cn

C#:   u is User
来源：http://tnw.birdmap.top

[G14] 数据类 / record
来源：http://pym.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rgm.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://oso.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qsw.sweek.top

TS:   type User = { name: string; age: number };
来源：http://rag.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://heo.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://wxk.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kcb.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://irp.zdqjudy.top

[G15] 枚举
来源：http://ogm.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ufr.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bpo.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zsi.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ujs.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://vwo.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nhs.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://btv.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ssv.yongpay.top

[G16] 对象转数组 / 字典
来源：http://wav.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gsu.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://adn.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://unx.hcnkem.com

TS:   Object.entries(obj)
来源：http://rjq.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jpf.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uov.xylfe.cn

Ruby: obj.instance_variables
来源：http://olj.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://jxy.hesvh.cn

================================================================================
来源：http://cvw.guowangkeji.top

H. 异常与错误处理
来源：http://yhn.fengsongda.top

================================================================================
来源：http://fjn.gotoacloud.top

[H01] try / catch 基础
来源：http://vwx.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xen.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wsl.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qhj.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tnr.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ldm.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tlo.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://exz.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jjq.hcnkem.com

[H02] finally / ensure 收尾
来源：http://urk.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://chy.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://isn.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nyg.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sck.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://aqj.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://btu.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kom.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vcn.gaohongyu789.top

[H03] 主动抛出异常
来源：http://xrl.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://fls.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kat.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://ydw.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://hhg.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://maz.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbo.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mjw.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://qtl.yj20258.top

[H04] 自定义异常类型
来源：http://vpp.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://xkj.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ztw.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://pti.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://dlc.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://iko.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gxn.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://fxl.uphjek.com

C#:   class MyException : Exception {}
来源：http://exf.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://qvu.aizwys.cn

Py:   except ValueError as e:
来源：http://hcc.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wdh.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://cfp.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://fyt.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://iuw.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://erv.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://eyf.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xif.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://gle.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://vvw.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vll.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ris.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rxd.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pfi.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mjy.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://vjg.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://nra.hywenlv.cn

[H07] 断言
来源：http://ckw.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://eoj.c1oappe.top

PHP:  assert($x > 0);
来源：http://irx.hnqzz.top

JS:   console.assert(x > 0);
来源：http://nsp.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://sid.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://sws.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ymx.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://pej.xinyue.icu


<!-- 参考信息 -->