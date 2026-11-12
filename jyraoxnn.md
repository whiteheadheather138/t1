代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lpg.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pay.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rfl.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jxu.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sco.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rvv.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gkb.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jit.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://bvb.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bad.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://llu.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://plx.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://clt.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eps.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cnc.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://icj.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://yix.yfazqb.com

[F06] 删除文件
来源：http://vvc.yuxming.cn

Py:   os.remove("a.txt")
来源：http://kav.yj20258.top

PHP:  unlink("a.txt");
来源：http://qwz.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://udt.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://pql.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qss.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://zmy.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://xsl.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://igy.jianghu66.top

[F07] 创建目录（含多级）
来源：http://byo.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wxu.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ond.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejb.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lit.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pwb.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aoh.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nql.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ozu.tanke756.top

[F08] 遍历目录
来源：http://eaj.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://whe.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ykx.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://hvy.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://zsv.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rbi.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yon.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://sen.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://ssl.yangfankeji.com

[F09] 获取文件大小
来源：http://ifm.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://uxo.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://ldj.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://atx.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://izr.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://fxh.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ovx.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://hcq.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://fxv.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://cwn.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jil.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hdf.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wss.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://wnu.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mep.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lyz.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npc.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nda.ehwqpu.com

[F11] 复制与移动文件
来源：http://rst.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://usv.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nwe.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ugn.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivv.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wvf.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ulh.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wiz.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uft.cheryme.top

[F12] CSV 读写
来源：http://lsu.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uig.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://usq.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nsb.hywenlv.cn

TS:   // 同上
来源：http://zbx.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gfg.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yps.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://thx.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ezi.zdbjq.cn

================================================================================
来源：http://ksc.aizwys.cn

G. 面向对象
来源：http://bau.yj20258888.top

================================================================================
来源：http://xgu.sysykeji.top

[G01] 定义类
来源：http://jdj.guannengcc.top

Py:   class User: pass
来源：http://msp.fehbvm.com

PHP:  class User {}
来源：http://bda.yvedp.cn

JS:   class User {}
来源：http://zbq.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://dpr.ppjwa.cn

Java: class User {}
来源：http://dqq.hcnkem.com

Go:   type User struct { Name string }
来源：http://und.jianghu66.top

Ruby: class User; end
来源：http://zxk.c1oappe.top

C#:   class User {}
来源：http://jvf.chenjidiqi.icu

[G02] 构造函数
来源：http://mpk.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://lun.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://obh.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://dbu.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://tic.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://gxs.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zmm.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://eut.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://lar.fanxiaobao.xyz

[G03] 实例属性
来源：http://lpx.hnxiangtu.top

Py:   self.name = "x"
来源：http://toq.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://voh.jiagoushi.top

JS:   this.name = "x";
来源：http://wca.zhongyouzk.top

TS:   name: string = "x";
来源：http://sxp.jianghu66.top

Java: private String name;
来源：http://uto.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qsq.52xcode.cn

Ruby: @name = "x"
来源：http://eub.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ciy.yueranfly.top

[G04] 定义方法
来源：http://tzu.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://yco.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sce.yonumen.top

JS:   greet() { return this.name; }
来源：http://adq.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://vck.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://nvu.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pyb.cashguo.top

Ruby: def greet; @name; end
来源：http://dgf.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://ynk.xuanzx.com

[G05] 继承
来源：http://osv.haohaochexian.top

Py:   class Admin(User): pass
来源：http://yuh.aizwys.cn

PHP:  class Admin extends User {}
来源：http://ilt.sufxvd.cn

JS:   class Admin extends User {}
来源：http://ozb.xinyue.icu

TS:   class Admin extends User {}
来源：http://txe.yongpay.top

Java: class Admin extends User {}
来源：http://wie.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://izn.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://qja.yueranfly.top

C#:   class Admin : User {}
来源：http://ezh.zhijiandao.cn

[G06] 重写方法
来源：http://qtq.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://sto.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iih.cheryme.top

JS:   greet() { return "admin"; }
来源：http://rty.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://lhk.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://dja.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qza.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://frz.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://hey.quarkkingdee.top

[G07] 调用父类方法
来源：http://bwv.sysykeji.top

Py:   super().greet()
来源：http://crv.ctjpmb.com

PHP:  parent::greet();
来源：http://zhj.yonumen.top

JS:   super.greet();
来源：http://vra.tianlin.xyz

TS:   super.greet();
来源：http://pjg.meibo888.top

Java: super.greet();
来源：http://psr.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://orw.jyoumei.cn

Ruby: super
来源：http://eda.jianghu66.top

C#:   base.Greet();
来源：http://ndx.zhixingplan.top

[G08] 静态方法与属性
来源：http://wnl.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgy.nanxinkj.top

PHP:  public static function f() {}
来源：http://kbm.havefunace.top

JS:   static f() {}
来源：http://njr.vehdjk.com

TS:   static f(): void {}
来源：http://pwf.yangfankeji.com

Java: static void f() {}
来源：http://dlc.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://usa.ybcxt.top

Ruby: def self.f; end
来源：http://wzh.guannengcc.top

C#:   public static void F() {}
来源：http://cao.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://nik.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://vpy.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hii.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://enp.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://ksd.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://ywb.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://lpf.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://daz.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://juk.zdqjudy.top

[G10] 访问控制
来源：http://npx.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://ksk.quarkkingdee.top

PHP:  public / protected / private
来源：http://ium.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://wgx.ehwqpu.com

TS:   public / protected / private
来源：http://vvx.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://zdo.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fwn.shzxlz.cn

Ruby: public / protected / private
来源：http://svw.smart0.xyz

C#:   public / protected / private / internal
来源：http://ksj.chenjidiqi.icu

[G11] getter / setter
来源：http://adw.yj20258888.top

Py:   @property 与 @x.setter
来源：http://qho.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vro.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://iob.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://fgk.xuanzx.com

Java: public String getName() { return name; }
来源：http://zih.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mvn.ydzc1.top

Ruby: attr_accessor :name
来源：http://wfr.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://saa.yuanzhike.top

[G12] 对象转字符串
来源：http://fot.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://crj.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wcf.hnqzz.top

JS:   toString() { return this.name; }
来源：http://rai.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://omi.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://otl.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gfe.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://zxw.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://yyt.zhixingplan.top

[G13] 判断对象类型
来源：http://jxc.daria6918.cn

Py:   isinstance(u, User)
来源：http://lia.yj20258.top

PHP:  $u instanceof User
来源：http://pst.haohaochexian.top

JS:   u instanceof User
来源：http://lof.ppjwa.cn

TS:   u instanceof User
来源：http://ifs.sxryk.cn

Java: u instanceof User
来源：http://itn.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vrq.sxryk.cn

Ruby: u.is_a?(User)
来源：http://dph.zhixingplan.top

C#:   u is User
来源：http://gwg.epnwcf.com

[G14] 数据类 / record
来源：http://lzo.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zsj.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://cou.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nvd.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://jzr.daxiang520.top

Java: record User(String name, int age) {}
来源：http://krn.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://zhg.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://woo.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://rpq.ehwqpu.com

[G15] 枚举
来源：http://mck.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jcm.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tpm.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pyx.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xme.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://pbs.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgy.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://dwa.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://khs.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://blj.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jyn.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://qvg.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://mol.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://qhh.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ctq.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hum.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://nwm.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://two.guannengcc.top

================================================================================
来源：http://dux.vqdsnc.cn

H. 异常与错误处理
来源：http://btp.fzhhl.top

================================================================================
来源：http://mtv.sysykeji.top

[H01] try / catch 基础
来源：http://ugz.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xjp.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lbq.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qea.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qhn.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://maa.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rro.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lsq.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://odl.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://upr.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://moq.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://aay.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uct.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ons.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://kvq.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wcn.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ixz.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uta.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://ahw.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://mqe.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://klm.meibo888.top

JS:   throw new Error("错误信息");
来源：http://tjf.cashguo.top

TS:   throw new Error("错误信息");
来源：http://pcd.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rej.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kha.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ckq.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xhl.jyoumei.cn

[H04] 自定义异常类型
来源：http://nna.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://wtn.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://ovu.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://yrc.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://xpc.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://cwc.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://egp.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://cbx.tian-w.cn

C#:   class MyException : Exception {}
来源：http://owi.hnxiangtu.top

[H05] 捕获特定类型
来源：http://ibm.yongpay.top

Py:   except ValueError as e:
来源：http://mqg.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vri.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://bnt.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://rkj.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://eeu.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zjw.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://lxq.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dca.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://qoz.zycfv.cn

Py:   value = d.get("k") or default
来源：http://ymb.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://byw.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qmv.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://lhy.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vqb.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pgj.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://hpi.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://wsf.jinyuanbaomall.cn

[H07] 断言
来源：http://tfb.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://czb.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://php.daria6918.cn

JS:   console.assert(x > 0);
来源：http://jrg.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://sfj.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://xuw.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xbl.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://pin.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://zro.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://hmh.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://rsg.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hod.guowangkeji.top

JS:   e.message;  e.stack
来源：http://dwy.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qvq.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ikd.yonumen.top

Go:   err.Error()
来源：http://ttx.tian-w.cn


<!-- 参考信息 -->