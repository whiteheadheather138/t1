代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://epd.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vxj.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ton.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npe.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oyo.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jok.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://shm.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vvc.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://ewi.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sbu.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://lsk.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://rrc.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://vfw.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pxq.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pcp.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://wta.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://oyx.cheryme.top

[F06] 删除文件
来源：http://pam.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://vcb.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://yzb.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://twd.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://rxb.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ugr.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://zle.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://dif.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://ibn.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://tyr.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wvz.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ble.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhu.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csz.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mcq.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qbr.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ofv.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zxx.hnqzz.top

[F08] 遍历目录
来源：http://jcv.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://stt.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qfq.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://vtv.sweek.top

TS:   fs.readdirSync("dir")
来源：http://lsn.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqc.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hsc.cheryme.top

Ruby: Dir.children("dir")
来源：http://yyv.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://bsh.yuxming.cn

[F09] 获取文件大小
来源：http://lzv.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://eti.havefunace.top

PHP:  filesize("a.txt");
来源：http://muz.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://spr.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://qru.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://dxj.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pqd.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://rld.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://jyl.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://iey.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ivg.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ccy.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xzt.sysykeji.top

TS:   path.extname("a.txt")
来源：http://yey.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dll.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zxs.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://irl.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nfc.cdnleiting.top

[F11] 复制与移动文件
来源：http://mru.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bee.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gup.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bsb.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yoy.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zde.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zey.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufz.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aus.hywenlv.cn

[F12] CSV 读写
来源：http://yps.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dye.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qil.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wii.wangdashe.top

TS:   // 同上
来源：http://nck.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tyd.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zby.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://poi.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fad.jinqigufen.top

================================================================================
来源：http://nui.ybcxt.top

G. 面向对象
来源：http://hfk.cheryme.top

================================================================================
来源：http://vhl.ywan-chungtsiang.top

[G01] 定义类
来源：http://bcu.daxiang520.top

Py:   class User: pass
来源：http://opv.yj20258.top

PHP:  class User {}
来源：http://pgs.smart0.xyz

JS:   class User {}
来源：http://oxd.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://csa.hnxiangtu.top

Java: class User {}
来源：http://kgi.zhengqikj.top

Go:   type User struct { Name string }
来源：http://nxd.jiagoushi.top

Ruby: class User; end
来源：http://bgx.yuanzhike.top

C#:   class User {}
来源：http://wca.zhongyouzk.top

[G02] 构造函数
来源：http://dhl.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://hql.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://ygc.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mih.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://jrr.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://uvu.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zic.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://mpz.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://sru.hcnkem.com

[G03] 实例属性
来源：http://swz.jqgfzy.top

Py:   self.name = "x"
来源：http://tlk.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://psn.316326.xyz

JS:   this.name = "x";
来源：http://mre.hfpthk.cn

TS:   name: string = "x";
来源：http://see.ydzc1.top

Java: private String name;
来源：http://iul.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nwc.iojbl.cn

Ruby: @name = "x"
来源：http://tam.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://nbw.zhixingplan.top

[G04] 定义方法
来源：http://ixt.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://tyk.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uot.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://nta.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://pth.aizwys.cn

Java: String greet() { return name; }
来源：http://thy.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://kgf.xylfe.cn

Ruby: def greet; @name; end
来源：http://ldg.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://txd.yj202588.top

[G05] 继承
来源：http://uvg.daxiang520.top

Py:   class Admin(User): pass
来源：http://wjy.yueranfly.top

PHP:  class Admin extends User {}
来源：http://zky.snrcjt.cn

JS:   class Admin extends User {}
来源：http://hih.ppjwa.cn

TS:   class Admin extends User {}
来源：http://pmy.svipenyu.cn

Java: class Admin extends User {}
来源：http://qcm.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nzc.aibaodan.cn

Ruby: class Admin < User; end
来源：http://tkr.yanxiufei.cn

C#:   class Admin : User {}
来源：http://gst.iojbl.cn

[G06] 重写方法
来源：http://zyz.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://kry.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mwa.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://pwn.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://dvt.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://tqo.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lmj.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://nwf.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://goi.ctjpmb.com

[G07] 调用父类方法
来源：http://aca.pengpengdd.cyou

Py:   super().greet()
来源：http://hmu.yuxming.cn

PHP:  parent::greet();
来源：http://fwx.nwbrower.top

JS:   super.greet();
来源：http://jzy.pycfn.com

TS:   super.greet();
来源：http://shk.fanxiaobao.xyz

Java: super.greet();
来源：http://yiu.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xgh.shzxlz.cn

Ruby: super
来源：http://ygy.quarkkingdee.top

C#:   base.Greet();
来源：http://kab.mhx1999.top

[G08] 静态方法与属性
来源：http://ujf.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rep.jqgfzy.top

PHP:  public static function f() {}
来源：http://pmz.quarkkingdee.top

JS:   static f() {}
来源：http://tok.bbcook.cn

TS:   static f(): void {}
来源：http://gcr.dianchejie.cn

Java: static void f() {}
来源：http://pch.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ffu.sufxvd.cn

Ruby: def self.f; end
来源：http://mhk.fengsongda.top

C#:   public static void F() {}
来源：http://otu.fzhhl.top

[G09] 接口 / 抽象类
来源：http://ncm.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://sux.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://nhw.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wqu.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://hwp.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://ufk.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://bgp.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zvc.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://jor.jinyuanbaomall.cn

[G10] 访问控制
来源：http://aih.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://wbq.redwolf501.top

PHP:  public / protected / private
来源：http://ijt.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://ruc.gogol.net.cn

TS:   public / protected / private
来源：http://oad.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://dsj.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bwo.0kj1m.cn

Ruby: public / protected / private
来源：http://ues.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://zvg.sysykeji.top

[G11] getter / setter
来源：http://lor.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://wbd.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ouh.zycfv.cn

JS:   get name() { return this._name; }
来源：http://ajq.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://mbp.havefunace.top

Java: public String getName() { return name; }
来源：http://gks.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kbx.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://xzn.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://pjm.uphjek.com

[G12] 对象转字符串
来源：http://csl.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://uyj.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://umu.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://hsx.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://rye.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://nwb.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yun.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://pni.316326.xyz

C#:   public override string ToString() => Name;
来源：http://rpv.uphjek.com

[G13] 判断对象类型
来源：http://gko.ybcxt.top

Py:   isinstance(u, User)
来源：http://oto.jianghu66.top

PHP:  $u instanceof User
来源：http://jwr.shzxlz.cn

JS:   u instanceof User
来源：http://mxm.yueranfly.top

TS:   u instanceof User
来源：http://ixx.jinyuanbaomall.cn

Java: u instanceof User
来源：http://qhr.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mzn.andypj.xyz

Ruby: u.is_a?(User)
来源：http://uup.yuanzhike.top

C#:   u is User
来源：http://zjq.9152youxi.cn

[G14] 数据类 / record
来源：http://yyh.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dae.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://xec.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ijt.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://wnv.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://jvh.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://ekf.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kfs.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://iar.gotoacloud.top

[G15] 枚举
来源：http://oyl.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qcn.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nzi.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lyn.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qrn.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://sim.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fyc.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://wsc.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jmw.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://wzt.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mqg.meibo888.top

PHP:  get_object_vars($obj);
来源：http://ysd.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://yxr.sweek.top

TS:   Object.entries(obj)
来源：http://ypy.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fum.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vol.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://vum.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://oyj.xziqi.cn

================================================================================
来源：http://nsb.cheryme.top

H. 异常与错误处理
来源：http://mok.feifeiyinyue.top

================================================================================
来源：http://wrq.jlsjyb.cn

[H01] try / catch 基础
来源：http://pwu.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oht.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pot.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gsa.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bbn.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qsp.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ylz.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zmj.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yoh.316326.xyz

[H02] finally / ensure 收尾
来源：http://gug.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://lzw.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ssz.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xek.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pyy.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://gea.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yqd.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hfh.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vqq.chenzaomai.com

[H03] 主动抛出异常
来源：http://wxv.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://mfj.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yjm.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://vpq.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://txb.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kby.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ese.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vne.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gsk.dashuyun.cn

[H04] 自定义异常类型
来源：http://ctw.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://gah.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vhs.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://ovj.redwolf501.top

TS:   class MyError extends Error {}
来源：http://uue.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://cpb.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nln.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://zty.sxryk.cn

C#:   class MyException : Exception {}
来源：http://gut.sjlbkw.cn

[H05] 捕获特定类型
来源：http://ena.nwbrower.top

Py:   except ValueError as e:
来源：http://qpy.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gnx.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://oro.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://nxb.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://caj.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dpo.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://ctu.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kfd.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://eok.guannengcc.top

Py:   value = d.get("k") or default
来源：http://gjk.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://yxc.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://jen.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://afm.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jik.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tiz.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://imo.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://aui.jiagoushi.top

[H07] 断言
来源：http://gnz.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://gjq.nwbrower.top

PHP:  assert($x > 0);
来源：http://eyn.yj20258.top

JS:   console.assert(x > 0);
来源：http://nkd.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://jne.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://hza.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zzi.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://hap.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://ear.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://dmi.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://vtw.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://isk.chenzaomai.com

JS:   e.message;  e.stack
来源：http://cdb.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lmx.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bcj.sweek.top

Go:   err.Error()
来源：http://mxb.feifeiyinyue.top


<!-- 参考信息 -->