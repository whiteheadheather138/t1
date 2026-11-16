代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xpa.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jxv.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hay.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azi.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pgj.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jgw.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zll.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jli.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://pqp.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lsr.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://dov.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://ped.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://abh.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ttd.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://coz.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://ilk.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://hqw.pycfn.com

[F06] 删除文件
来源：http://gnx.uphjek.com

Py:   os.remove("a.txt")
来源：http://bjn.tanke756.top

PHP:  unlink("a.txt");
来源：http://cxx.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://jam.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://ktz.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://raw.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://tfe.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://nva.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://fzh.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://uzv.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://scp.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://otu.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://czx.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgh.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rcq.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bxx.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqb.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qfb.pycfn.com

[F08] 遍历目录
来源：http://vpy.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://jhx.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gup.sweek.top

JS:   fs.readdirSync("dir")
来源：http://ztc.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://hty.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://suy.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qrm.fehbvm.com

Ruby: Dir.children("dir")
来源：http://azu.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://kip.feifeiyinyue.top

[F09] 获取文件大小
来源：http://fon.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://ygz.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://hdx.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://wte.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://nbc.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sqr.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ena.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://pzj.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://eoa.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://dsf.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xsz.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jyw.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://guw.tian-w.cn

TS:   path.extname("a.txt")
来源：http://fav.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pwg.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ycy.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://udf.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pjk.gogol.net.cn

[F11] 复制与移动文件
来源：http://ope.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gxl.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zzh.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qwg.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://znh.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cxu.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zrz.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sui.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osp.tian-w.cn

[F12] CSV 读写
来源：http://vse.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cvr.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hmm.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zji.cheryme.top

TS:   // 同上
来源：http://ltj.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gpz.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ttw.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nue.dashuyun.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rhu.chenlongwang.top

================================================================================
来源：http://jal.ywan-chungtsiang.top

G. 面向对象
来源：http://jvt.ehwqpu.com

================================================================================
来源：http://isq.52xcode.cn

[G01] 定义类
来源：http://nmd.ppjwa.cn

Py:   class User: pass
来源：http://sws.gaohongyu789.top

PHP:  class User {}
来源：http://pzp.shzxlz.cn

JS:   class User {}
来源：http://ksl.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://sle.cqqwz.cn

Java: class User {}
来源：http://aob.havefunace.top

Go:   type User struct { Name string }
来源：http://mjq.yuxming.cn

Ruby: class User; end
来源：http://tpe.feifeiyinyue.top

C#:   class User {}
来源：http://zpi.sjlbkw.cn

[G02] 构造函数
来源：http://ddg.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://emt.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://lee.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://tgm.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://mmr.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://kem.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://axz.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://bgw.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://isk.zhixingplan.top

[G03] 实例属性
来源：http://zif.havefunace.top

Py:   self.name = "x"
来源：http://eoq.sweek.top

PHP:  public string $name = "x";
来源：http://meu.bjfxy.top

JS:   this.name = "x";
来源：http://rks.daria6918.cn

TS:   name: string = "x";
来源：http://tqj.nanxuanxn.top

Java: private String name;
来源：http://yyz.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://anj.bbcook.cn

Ruby: @name = "x"
来源：http://ywb.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://pyp.shuidangran.top

[G04] 定义方法
来源：http://mmj.hesvh.cn

Py:   def greet(self): return self.name
来源：http://lox.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://web.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://zas.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://hdb.cucudq.cn

Java: String greet() { return name; }
来源：http://nlm.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rhe.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://asl.xylfe.cn

C#:   public string Greet() => Name;
来源：http://vzd.52xcode.cn

[G05] 继承
来源：http://igx.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://tbm.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://hhi.zhengqikj.top

JS:   class Admin extends User {}
来源：http://ard.guannengcc.top

TS:   class Admin extends User {}
来源：http://uad.cqqwz.cn

Java: class Admin extends User {}
来源：http://omi.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://msd.yj20258888.top

Ruby: class Admin < User; end
来源：http://ods.hywenlv.cn

C#:   class Admin : User {}
来源：http://hpv.fktsv.cn

[G06] 重写方法
来源：http://txa.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://rsa.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uro.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://ntq.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://rha.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://iuy.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lpo.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://rlp.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://dkj.redwolf501.top

[G07] 调用父类方法
来源：http://gli.hesvh.cn

Py:   super().greet()
来源：http://gqw.yvedp.cn

PHP:  parent::greet();
来源：http://pru.shuidangran.top

JS:   super.greet();
来源：http://feu.kuanghao11.cn

TS:   super.greet();
来源：http://etz.jianghu66.top

Java: super.greet();
来源：http://lvr.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://smx.bbcook.cn

Ruby: super
来源：http://ozj.jqgfzy.top

C#:   base.Greet();
来源：http://sxb.xuanzx.com

[G08] 静态方法与属性
来源：http://cbm.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lmk.smart0.xyz

PHP:  public static function f() {}
来源：http://ndb.ydzc1.top

JS:   static f() {}
来源：http://qjx.gaohongyu789.top

TS:   static f(): void {}
来源：http://cmo.yj20258.top

Java: static void f() {}
来源：http://oqm.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nva.xinyue.icu

Ruby: def self.f; end
来源：http://rug.yj20258.top

C#:   public static void F() {}
来源：http://sqv.smart0.xyz

[G09] 接口 / 抽象类
来源：http://tnx.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://roi.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://nsb.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nku.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://bnv.birdmap.top

Java: interface Shape { double area(); }
来源：http://phy.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://oqu.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yli.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://sli.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://btz.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://wuj.fehbvm.com

PHP:  public / protected / private
来源：http://uxg.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://joj.svipenyu.cn

TS:   public / protected / private
来源：http://ipu.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://clv.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jok.smart0.xyz

Ruby: public / protected / private
来源：http://ewq.jinqigufen.top

C#:   public / protected / private / internal
来源：http://gzi.quarkkingdee.top

[G11] getter / setter
来源：http://qbk.jianghu66.top

Py:   @property 与 @x.setter
来源：http://occ.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ggq.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://ndu.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://guk.jinqigufen.top

Java: public String getName() { return name; }
来源：http://rpi.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vpb.cucudq.cn

Ruby: attr_accessor :name
来源：http://tfp.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://sqp.yongpay.top

[G12] 对象转字符串
来源：http://qzt.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://qoe.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cmb.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://rjx.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://hhq.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://udx.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://zll.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://ezw.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://rwp.ydjk.org.cn

[G13] 判断对象类型
来源：http://hct.mhx1999.top

Py:   isinstance(u, User)
来源：http://ntq.316326.xyz

PHP:  $u instanceof User
来源：http://suh.smart0.xyz

JS:   u instanceof User
来源：http://lya.xylfe.cn

TS:   u instanceof User
来源：http://dda.nanxinkj.top

Java: u instanceof User
来源：http://gre.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wlc.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://xty.yj202588.top

C#:   u is User
来源：http://nmv.fengsongda.top

[G14] 数据类 / record
来源：http://uky.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nhf.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://bto.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://oep.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://ikr.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://jad.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://xou.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wwy.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://nvf.yuxming.cn

[G15] 枚举
来源：http://rqm.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zpv.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://yar.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tqj.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://waz.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://hbw.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dzf.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://sff.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://brg.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://xuy.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://onn.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://ykh.yongpay.top

JS:   Object.entries(obj)
来源：http://mag.bjfxy.top

TS:   Object.entries(obj)
来源：http://xiq.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cog.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mfp.yangfankeji.com

Ruby: obj.instance_variables
来源：http://pgl.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://bqo.haohaochexian.top

================================================================================
来源：http://jfn.zhongyouzk.top

H. 异常与错误处理
来源：http://qli.nanxuanxn.top

================================================================================
来源：http://tdu.52xcode.cn

[H01] try / catch 基础
来源：http://qdw.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kdg.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uug.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cnl.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qzl.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajz.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bkk.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uyz.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gyg.andypj.xyz

[H02] finally / ensure 收尾
来源：http://yni.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://bzt.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://efo.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://zkz.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tgl.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://cpe.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://obg.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://bzu.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nvd.hfpthk.cn

[H03] 主动抛出异常
来源：http://hcg.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://isr.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://squ.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://zhs.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://mgs.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nju.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dpn.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qof.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://yoy.9152youxi.cn

[H04] 自定义异常类型
来源：http://lai.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://sob.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xfk.guannengcc.top

JS:   class MyError extends Error {}
来源：http://prk.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://loj.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://pqr.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zeo.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://qar.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://ghe.hnqzz.top

[H05] 捕获特定类型
来源：http://vvr.tarul.cn

Py:   except ValueError as e:
来源：http://ord.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qew.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ihz.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://pfa.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://uuj.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://can.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://der.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bwm.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://boe.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://yei.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zdo.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://qhv.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://kkb.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wtm.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vck.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://gid.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://ysh.smart0.xyz

[H07] 断言
来源：http://zot.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://aqp.chenlongwang.top

PHP:  assert($x > 0);
来源：http://kwq.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://mzr.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://jqj.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://vdn.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dat.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aju.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://een.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://yuu.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://hly.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvp.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://vpm.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sdi.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ucs.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://odu.jianghu66.top


<!-- 参考信息 -->