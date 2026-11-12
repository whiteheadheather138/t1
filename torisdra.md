代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://tfg.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jhn.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fim.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hyt.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://obc.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://mby.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mjg.bbcook.cn

[F04] 追加写入文件
来源：http://exg.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vkg.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zta.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cnd.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uvh.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fjx.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gfx.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fqe.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://weq.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://ddc.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nla.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://tdp.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://bdx.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://koh.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://euq.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sdh.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://mhz.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://drz.chenjidiqi.icu

[F06] 删除文件
来源：http://lpd.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://iur.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://szz.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rle.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://iol.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kse.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://hpo.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://run.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://uvu.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://dkp.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpy.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kzt.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xco.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwc.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://miy.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sfu.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pcb.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jmu.316326.xyz

[F08] 遍历目录
来源：http://sti.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://job.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jqu.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://saa.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://rqb.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sqb.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://pkg.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://gkz.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://awb.yj20258888.top

[F09] 获取文件大小
来源：http://icf.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://vvf.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://cek.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://ffa.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://pfn.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eqh.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uzi.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://urh.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://gmu.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://jiq.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://exz.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bbh.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tvo.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://kwj.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ltc.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://phm.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://esg.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bdh.nanxinkj.top

[F11] 复制与移动文件
来源：http://dru.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zew.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zve.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qle.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzm.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://who.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ifo.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nsr.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ahz.haohaochexian.top

[F12] CSV 读写
来源：http://ntp.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cjn.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oyw.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sus.cdnleiting.top

TS:   // 同上
来源：http://zvd.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pbf.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jao.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mwf.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tjb.zhengqikj.top

================================================================================
来源：http://eqk.yueranfly.top

G. 面向对象
来源：http://scc.jinqigufen.top

================================================================================
来源：http://qme.yuxming.cn

[G01] 定义类
来源：http://zgc.gotoacloud.top

Py:   class User: pass
来源：http://nsd.c1oappe.top

PHP:  class User {}
来源：http://sjn.yj20258.top

JS:   class User {}
来源：http://ror.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://obc.c1oappe.top

Java: class User {}
来源：http://tii.dashuyun.cn

Go:   type User struct { Name string }
来源：http://esg.nanxuanxn.top

Ruby: class User; end
来源：http://akq.sxryk.cn

C#:   class User {}
来源：http://qcv.smart0.xyz

[G02] 构造函数
来源：http://icz.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://arz.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://mul.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://alh.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://uzz.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://pjc.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qbu.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://myn.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://exu.havefunace.top

[G03] 实例属性
来源：http://iou.tianlin.xyz

Py:   self.name = "x"
来源：http://qyb.aibaodan.cn

PHP:  public string $name = "x";
来源：http://uae.yonumen.top

JS:   this.name = "x";
来源：http://zih.pengpengdd.cyou

TS:   name: string = "x";
来源：http://sir.iojbl.cn

Java: private String name;
来源：http://vnv.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dxp.yanxiufei.cn

Ruby: @name = "x"
来源：http://tng.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://msm.gogol.net.cn

[G04] 定义方法
来源：http://mhf.xylfe.cn

Py:   def greet(self): return self.name
来源：http://eah.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://elm.yvedp.cn

JS:   greet() { return this.name; }
来源：http://afj.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://tkc.ivvv.top

Java: String greet() { return name; }
来源：http://axr.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bxx.xziqi.cn

Ruby: def greet; @name; end
来源：http://ocv.guannengcc.top

C#:   public string Greet() => Name;
来源：http://quq.cashguo.top

[G05] 继承
来源：http://mss.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://ffm.cashguo.top

PHP:  class Admin extends User {}
来源：http://mfd.havefunace.top

JS:   class Admin extends User {}
来源：http://oiy.cucudq.cn

TS:   class Admin extends User {}
来源：http://tie.cheryme.top

Java: class Admin extends User {}
来源：http://ohv.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rrk.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://lpf.jqgufenzy.top

C#:   class Admin : User {}
来源：http://pxl.yonumen.top

[G06] 重写方法
来源：http://mjk.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://hrk.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qzb.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://ptv.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://wyt.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://ywa.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eho.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://tph.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://ehp.tarul.cn

[G07] 调用父类方法
来源：http://kii.hfpthk.cn

Py:   super().greet()
来源：http://bhe.ydzc1.top

PHP:  parent::greet();
来源：http://dbd.gotoacloud.top

JS:   super.greet();
来源：http://uab.xuanzx.com

TS:   super.greet();
来源：http://vsu.hammf.cn

Java: super.greet();
来源：http://wua.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://afx.svipenyu.cn

Ruby: super
来源：http://ecw.0kj1m.cn

C#:   base.Greet();
来源：http://xyq.cucudq.cn

[G08] 静态方法与属性
来源：http://abf.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pnd.jyoumei.cn

PHP:  public static function f() {}
来源：http://qfs.jianghu66.top

JS:   static f() {}
来源：http://oge.nwbrower.top

TS:   static f(): void {}
来源：http://hkg.shanyushiyangkeji.top

Java: static void f() {}
来源：http://xln.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sda.yfazqb.com

Ruby: def self.f; end
来源：http://nng.jqgufenzy.top

C#:   public static void F() {}
来源：http://eol.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://rcf.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://tcq.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://fsc.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fax.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://geg.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://viy.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://vkh.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jis.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://xbf.wangdashe.top

[G10] 访问控制
来源：http://dyc.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://nbw.tarul.cn

PHP:  public / protected / private
来源：http://sih.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://arc.zycfv.cn

TS:   public / protected / private
来源：http://rjl.hammf.cn

Java: public / protected / private / 默认包级
来源：http://vmw.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://fiv.jyoumei.cn

Ruby: public / protected / private
来源：http://rfv.fehbvm.com

C#:   public / protected / private / internal
来源：http://ztk.fanxiaobao.xyz

[G11] getter / setter
来源：http://lyu.yueranfly.top

Py:   @property 与 @x.setter
来源：http://bth.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://zms.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://lfx.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://zoo.shzxlz.cn

Java: public String getName() { return name; }
来源：http://xjo.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lws.chenlongwang.top

Ruby: attr_accessor :name
来源：http://vfj.gzhubu.top

C#:   public string Name { get; set; }
来源：http://hbk.pengpengdd.cyou

[G12] 对象转字符串
来源：http://lyu.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://owa.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bpc.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://mnj.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://qfv.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://szh.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bry.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://tph.ivvv.top

C#:   public override string ToString() => Name;
来源：http://uum.yanxiufei.cn

[G13] 判断对象类型
来源：http://ypx.yuanzhike.top

Py:   isinstance(u, User)
来源：http://ale.zdqjudy.top

PHP:  $u instanceof User
来源：http://ppd.dianchejie.cn

JS:   u instanceof User
来源：http://ifd.zhixingplan.top

TS:   u instanceof User
来源：http://jel.ctjpmb.com

Java: u instanceof User
来源：http://wlw.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tys.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://jav.cucudq.cn

C#:   u is User
来源：http://unp.c1oappe.top

[G14] 数据类 / record
来源：http://ajy.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xbv.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://wgf.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://fpd.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://pfz.xuanzx.com

Java: record User(String name, int age) {}
来源：http://kyy.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://yzn.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cln.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://yzv.nanxuanxn.top

[G15] 枚举
来源：http://ktb.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vkj.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jwz.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rag.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dcl.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://ubo.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cdg.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://iye.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rfx.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://kki.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xjm.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://egd.xuanzx.com

JS:   Object.entries(obj)
来源：http://lip.hysaishi.cn

TS:   Object.entries(obj)
来源：http://jxa.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hqa.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://drv.tian-w.cn

Ruby: obj.instance_variables
来源：http://tev.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://oeq.xziqi.cn

================================================================================
来源：http://msv.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://rwh.jyoumei.cn

================================================================================
来源：http://haj.iojbl.cn

[H01] try / catch 基础
来源：http://jgo.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nnm.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://owx.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vpn.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://you.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ksz.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwn.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yab.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eld.aizwys.cn

[H02] finally / ensure 收尾
来源：http://rss.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ywf.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gwd.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gjb.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kty.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://ssh.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mzt.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iwi.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fiu.jqgfzy.top

[H03] 主动抛出异常
来源：http://hsx.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://mig.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://siz.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://pdb.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://myy.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://dww.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bfo.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://lvn.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://gmm.sweek.top

[H04] 自定义异常类型
来源：http://ihi.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://nzz.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://clo.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://ofp.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://cyh.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://yvd.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jva.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://arj.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://mpp.nanxuanxn.top

[H05] 捕获特定类型
来源：http://jyk.yongpay.top

Py:   except ValueError as e:
来源：http://lbm.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nxu.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://nei.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://rxb.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://oww.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hiu.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://xvj.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pzq.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://nny.52xcode.cn

Py:   value = d.get("k") or default
来源：http://tog.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://okp.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hcg.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://imo.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnn.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mmj.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://mov.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://fns.ywan-chungtsiang.top

[H07] 断言
来源：http://gnl.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://vng.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://cjf.yongpay.top

JS:   console.assert(x > 0);
来源：http://kek.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://xwp.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://owz.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qyh.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bwm.shangyingyoupin.top


<!-- 参考信息 -->