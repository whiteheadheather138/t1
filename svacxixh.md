代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lcr.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://obk.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://smz.yvedp.cn

[F04] 追加写入文件
来源：http://xdw.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nvj.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uzk.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lke.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uqy.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://elo.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://anf.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sci.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://etv.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://kxh.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hgo.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://iic.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://scn.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://nyz.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lmw.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eku.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://ogv.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://qfh.hnqzz.top

[F06] 删除文件
来源：http://bfb.hesvh.cn

Py:   os.remove("a.txt")
来源：http://foa.yueranfly.top

PHP:  unlink("a.txt");
来源：http://qhp.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://him.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dzc.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bqy.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://bue.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://kce.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://zhd.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://ufr.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nfi.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zzv.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cho.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cdo.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ovi.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wte.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ngj.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dqo.zhoulong.xyz

[F08] 遍历目录
来源：http://jzg.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dfm.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fva.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://kqe.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://kcm.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fri.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kbm.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://nfu.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://gye.uphjek.com

[F09] 获取文件大小
来源：http://pun.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://rqm.havefunace.top

PHP:  filesize("a.txt");
来源：http://jhj.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://pdd.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://vqj.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://rlv.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hzu.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://jng.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://fza.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://hde.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blh.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bri.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vmx.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://ugi.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://elt.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://juw.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gac.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uzn.nanxinkj.top

[F11] 复制与移动文件
来源：http://syj.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kej.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ati.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kca.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwf.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lsh.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wlt.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wee.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rpa.shanyushiyangtech.top

[F12] CSV 读写
来源：http://jhz.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wbp.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sja.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ajf.jqgufenzy.top

TS:   // 同上
来源：http://fpv.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wvs.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qca.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://knl.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xxu.fanxiaobao.xyz

================================================================================
来源：http://otp.tanke756.top

G. 面向对象
来源：http://krs.yj20258.top

================================================================================
来源：http://sxm.ppjwa.cn

[G01] 定义类
来源：http://wqx.ehwqpu.com

Py:   class User: pass
来源：http://jbs.hnqzz.top

PHP:  class User {}
来源：http://cyj.nanxuanxn.top

JS:   class User {}
来源：http://gwa.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://qgt.tianlin.xyz

Java: class User {}
来源：http://fin.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://axf.xuetiantiany.cn

Ruby: class User; end
来源：http://lpo.smart0.xyz

C#:   class User {}
来源：http://amc.shzxlz.cn

[G02] 构造函数
来源：http://ybx.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://yic.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://uqk.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://jds.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://kbm.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://ofg.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnk.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wxc.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://baq.ydzc1.top

[G03] 实例属性
来源：http://anh.vqdsnc.cn

Py:   self.name = "x"
来源：http://aif.aizwys.cn

PHP:  public string $name = "x";
来源：http://fql.aibaodan.cn

JS:   this.name = "x";
来源：http://asa.zhoulong.xyz

TS:   name: string = "x";
来源：http://yco.yueranfly.top

Java: private String name;
来源：http://hog.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sur.jyoumei.cn

Ruby: @name = "x"
来源：http://ods.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ztw.yangfankeji.com

[G04] 定义方法
来源：http://bqp.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://soa.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nln.fehbvm.com

JS:   greet() { return this.name; }
来源：http://toz.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://kom.dashuyun.cn

Java: String greet() { return name; }
来源：http://pum.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vpd.gzhubu.top

Ruby: def greet; @name; end
来源：http://xlv.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://sql.xuetiantiany.cn

[G05] 继承
来源：http://jut.hcnkem.com

Py:   class Admin(User): pass
来源：http://mjl.vehdjk.com

PHP:  class Admin extends User {}
来源：http://veq.tarul.cn

JS:   class Admin extends User {}
来源：http://uwk.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://mhv.cqqwz.cn

Java: class Admin extends User {}
来源：http://brt.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wjs.xziqi.cn

Ruby: class Admin < User; end
来源：http://rtw.jyoumei.cn

C#:   class Admin : User {}
来源：http://zyi.hfpthk.cn

[G06] 重写方法
来源：http://jmd.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://pbb.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fnd.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://obu.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://pcl.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://hqt.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rse.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://lnq.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://znc.haohaochexian.top

[G07] 调用父类方法
来源：http://pbi.fengsongda.top

Py:   super().greet()
来源：http://ngm.yangfankeji.com

PHP:  parent::greet();
来源：http://jbt.birdmap.top

JS:   super.greet();
来源：http://rmx.xuetiantiany.cn

TS:   super.greet();
来源：http://lfm.jinqigfzy.top

Java: super.greet();
来源：http://jig.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fwd.yueranfly.top

Ruby: super
来源：http://mmz.hysaishi.cn

C#:   base.Greet();
来源：http://kec.snrcjt.cn

[G08] 静态方法与属性
来源：http://dys.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dje.yueranfly.top

PHP:  public static function f() {}
来源：http://uyq.smart0.xyz

JS:   static f() {}
来源：http://sct.bjfxy.top

TS:   static f(): void {}
来源：http://ouf.ydjk.org.cn

Java: static void f() {}
来源：http://ewu.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zmb.zhoulong.xyz

Ruby: def self.f; end
来源：http://loc.jianghu66.top

C#:   public static void F() {}
来源：http://xzc.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://vnq.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://lbf.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://klh.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gif.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://ozh.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://gsg.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://cwu.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jhe.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://ujb.shzxlz.cn

[G10] 访问控制
来源：http://gdw.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://mae.gotoacloud.top

PHP:  public / protected / private
来源：http://fwy.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://vlj.redwolf501.top

TS:   public / protected / private
来源：http://mau.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://quq.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vzr.vqdsnc.cn

Ruby: public / protected / private
来源：http://was.zycfv.cn

C#:   public / protected / private / internal
来源：http://dbd.birdmap.top

[G11] getter / setter
来源：http://vfn.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://ynt.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sst.yonumen.top

JS:   get name() { return this._name; }
来源：http://iee.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://ikz.sxryk.cn

Java: public String getName() { return name; }
来源：http://ybm.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iod.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://ggv.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://tha.shzxlz.cn

[G12] 对象转字符串
来源：http://agn.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://jgd.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ily.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ese.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://oko.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://nof.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://fzd.jianghu66.top

Ruby: def to_s; @name; end
来源：http://krq.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://bbh.tian-w.cn

[G13] 判断对象类型
来源：http://kpr.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://pqz.jqgfzy.top

PHP:  $u instanceof User
来源：http://tnw.ehwqpu.com

JS:   u instanceof User
来源：http://guv.gogol.net.cn

TS:   u instanceof User
来源：http://rcw.ydzc1.top

Java: u instanceof User
来源：http://qwr.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kdr.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://exk.ybcxt.top

C#:   u is User
来源：http://fbj.zycfv.cn

[G14] 数据类 / record
来源：http://odr.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dxz.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://unf.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mxp.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://ats.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://mlq.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://hyu.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tbv.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://vly.jlsjyb.cn

[G15] 枚举
来源：http://iex.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ons.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bku.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yrs.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tzj.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://ena.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgy.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://rpv.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dbm.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://haw.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nag.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://uuj.fktsv.cn

JS:   Object.entries(obj)
来源：http://rrf.dianchejie.cn

TS:   Object.entries(obj)
来源：http://xwg.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mys.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ykn.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://ply.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://wke.ctjpmb.com

================================================================================
来源：http://gex.hnqzz.top

H. 异常与错误处理
来源：http://bmt.ydzc1.top

================================================================================
来源：http://yhp.daxiang520.top

[H01] try / catch 基础
来源：http://rel.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://juo.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mrf.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://goa.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cur.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vna.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aqp.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ogh.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hmm.fehbvm.com

[H02] finally / ensure 收尾
来源：http://geu.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://icf.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xqq.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hum.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://atm.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://ndz.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvi.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://arz.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cnv.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://xox.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://vws.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tjs.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://yyw.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://jao.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bid.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rhx.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lug.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vtt.kuanghao11.cn

[H04] 自定义异常类型
来源：http://xnq.52xcode.cn

Py:   class MyError(Exception): pass
来源：http://jcy.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://tmq.havefunace.top

JS:   class MyError extends Error {}
来源：http://adc.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://syc.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://kgj.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ktz.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://ooq.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://mjq.yongpay.top

[H05] 捕获特定类型
来源：http://fmf.gzhubu.top

Py:   except ValueError as e:
来源：http://vnx.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vwa.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://awq.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://pvo.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://kuk.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lbp.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://fuk.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fwm.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://nas.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://fno.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://pbe.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hbs.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ywd.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kna.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://sos.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://fal.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://ycw.chenzaomai.com

[H07] 断言
来源：http://fbf.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://crr.cashguo.top

PHP:  assert($x > 0);
来源：http://lvu.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://fac.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://jwm.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://mza.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wrj.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://zwf.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://gyh.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://dnb.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://ueo.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ofy.pycfn.com


<!-- 参考信息 -->