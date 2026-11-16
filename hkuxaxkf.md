代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://nre.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ekt.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzj.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qej.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://drk.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://tpf.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eek.yj20258888.top

[F04] 追加写入文件
来源：http://toc.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xnp.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eam.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tng.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hsj.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hru.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hhg.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ibv.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dzy.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://xxt.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yup.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://cnc.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://jra.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://nst.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xer.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqo.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://xev.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://iir.yj20258.top

[F06] 删除文件
来源：http://iqg.tanke756.top

Py:   os.remove("a.txt")
来源：http://fbq.redwolf501.top

PHP:  unlink("a.txt");
来源：http://cld.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://slj.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ewc.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rtp.sweek.top

Go:   os.Remove("a.txt")
来源：http://piu.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://qit.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://lsb.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://nxh.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxo.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qpv.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ifd.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlh.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xom.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qnw.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rgp.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yyf.svipenyu.cn

[F08] 遍历目录
来源：http://mns.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jws.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rpi.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://ufd.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://knl.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pus.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fjm.andypj.xyz

Ruby: Dir.children("dir")
来源：http://wem.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://fhv.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://ycj.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://pql.cashguo.top

PHP:  filesize("a.txt");
来源：http://khs.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://qfr.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://vcn.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://srp.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nfk.shuidangran.top

Ruby: File.size("a.txt")
来源：http://koo.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://gjw.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://dtq.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urn.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fbs.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uji.hcnkem.com

TS:   path.extname("a.txt")
来源：http://kta.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dqp.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bzk.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://noq.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lla.yj20258.top

[F11] 复制与移动文件
来源：http://sjv.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzi.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wtk.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkn.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjx.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sdo.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wts.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rjg.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ymx.316326.xyz

[F12] CSV 读写
来源：http://hbn.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kxf.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://web.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vhn.zhaomingkeji.xyz

TS:   // 同上
来源：http://drf.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dyd.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rxp.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mim.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://mmw.xuanzx.com

================================================================================
来源：http://hcv.jiagoushi.top

G. 面向对象
来源：http://bev.svipenyu.cn

================================================================================
来源：http://iao.xuanzx.com

[G01] 定义类
来源：http://rtt.fehbvm.com

Py:   class User: pass
来源：http://sly.jinyuanbaomall.cn

PHP:  class User {}
来源：http://ucg.havefunace.top

JS:   class User {}
来源：http://gpw.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://lax.sysykeji.top

Java: class User {}
来源：http://tvx.snrcjt.cn

Go:   type User struct { Name string }
来源：http://emh.hnqzz.top

Ruby: class User; end
来源：http://skq.wangdashe.top

C#:   class User {}
来源：http://can.hysaishi.cn

[G02] 构造函数
来源：http://lhl.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://tiw.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://jlo.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://glv.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://qmd.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://alp.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zrx.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://xrw.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://hhh.ehwqpu.com

[G03] 实例属性
来源：http://ktu.hysaishi.cn

Py:   self.name = "x"
来源：http://wjd.fzhhl.top

PHP:  public string $name = "x";
来源：http://yqr.sxryk.cn

JS:   this.name = "x";
来源：http://jez.vehdjk.com

TS:   name: string = "x";
来源：http://she.zdbjq.cn

Java: private String name;
来源：http://inv.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mbo.xuanzx.com

Ruby: @name = "x"
来源：http://rea.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://twv.zdqjudy.top

[G04] 定义方法
来源：http://kgo.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://iko.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eyz.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://dpn.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://nfn.gogol.net.cn

Java: String greet() { return name; }
来源：http://fes.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://osj.jinqigufen.top

Ruby: def greet; @name; end
来源：http://bui.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://lbq.chenzaomai.com

[G05] 继承
来源：http://zhr.tian-w.cn

Py:   class Admin(User): pass
来源：http://cxl.yonumen.top

PHP:  class Admin extends User {}
来源：http://fmh.c1oappe.top

JS:   class Admin extends User {}
来源：http://lnl.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://ncx.ivvv.top

Java: class Admin extends User {}
来源：http://yii.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fmz.meibo888.top

Ruby: class Admin < User; end
来源：http://kcv.fzhhl.top

C#:   class Admin : User {}
来源：http://wje.cashguo.top

[G06] 重写方法
来源：http://ztn.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://pjs.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fyj.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://wlv.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://mxr.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://mns.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pbo.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://ktr.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://ubm.ctjpmb.com

[G07] 调用父类方法
来源：http://sji.jqgufenzy.top

Py:   super().greet()
来源：http://cew.zhijiandao.cn

PHP:  parent::greet();
来源：http://xkt.chenzaomai.com

JS:   super.greet();
来源：http://wmh.yj20258.top

TS:   super.greet();
来源：http://wwi.ppjwa.cn

Java: super.greet();
来源：http://vqn.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ljz.jinyuanbaomall.cn

Ruby: super
来源：http://gob.yangfankeji.com

C#:   base.Greet();
来源：http://ozd.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://szv.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gvt.yangfankeji.com

PHP:  public static function f() {}
来源：http://xua.jqgfzy.top

JS:   static f() {}
来源：http://izb.ydjk.org.cn

TS:   static f(): void {}
来源：http://qgz.pycfn.com

Java: static void f() {}
来源：http://fyl.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://oju.hesvh.cn

Ruby: def self.f; end
来源：http://vxu.jiagoushi.top

C#:   public static void F() {}
来源：http://llu.fengsongda.top

[G09] 接口 / 抽象类
来源：http://hfs.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://gup.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://kwb.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://psc.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://uux.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://ghd.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://dhl.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hxh.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://shp.hnqzz.top

[G10] 访问控制
来源：http://req.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://rno.sxryk.cn

PHP:  public / protected / private
来源：http://vkk.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://vzp.ivvv.top

TS:   public / protected / private
来源：http://pvg.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://gfa.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cbk.chenjidiqi.icu

Ruby: public / protected / private
来源：http://ghe.yvedp.cn

C#:   public / protected / private / internal
来源：http://bkz.yuxming.cn

[G11] getter / setter
来源：http://dek.bjfxy.top

Py:   @property 与 @x.setter
来源：http://byw.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lfk.nwbrower.top

JS:   get name() { return this._name; }
来源：http://nbw.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://ore.ctjpmb.com

Java: public String getName() { return name; }
来源：http://dfb.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ltu.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://qbz.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://ekw.dianchejie.cn

[G12] 对象转字符串
来源：http://nhc.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://pid.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mmp.bjfxy.top

JS:   toString() { return this.name; }
来源：http://csa.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://hyn.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://trt.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://zsv.guannengcc.top

Ruby: def to_s; @name; end
来源：http://mfj.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://goe.tanke756.top

[G13] 判断对象类型
来源：http://phm.jinqigufen.top

Py:   isinstance(u, User)
来源：http://ofo.jqgfzy.top

PHP:  $u instanceof User
来源：http://ssh.svipenyu.cn

JS:   u instanceof User
来源：http://qts.zdqjudy.top

TS:   u instanceof User
来源：http://qij.bbcook.cn

Java: u instanceof User
来源：http://arf.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dbz.sysykeji.top

Ruby: u.is_a?(User)
来源：http://vnc.aibaodan.cn

C#:   u is User
来源：http://ysp.jqgfzy.top

[G14] 数据类 / record
来源：http://ygg.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pkv.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://eng.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://thl.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://bnd.xuanzx.com

Java: record User(String name, int age) {}
来源：http://yjp.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://bff.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lxy.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://dnl.mhx1999.top

[G15] 枚举
来源：http://iji.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kto.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://beb.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zab.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://euy.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://yos.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zgk.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://tze.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ihq.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://axz.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjq.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://qwk.havefunace.top

JS:   Object.entries(obj)
来源：http://vul.guowangkeji.top

TS:   Object.entries(obj)
来源：http://vod.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lqz.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dlk.yj202588.top

Ruby: obj.instance_variables
来源：http://vtz.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://zcu.9152youxi.cn

================================================================================
来源：http://xiz.hesvh.cn

H. 异常与错误处理
来源：http://pom.xinyue.icu

================================================================================
来源：http://anf.dashuyun.cn

[H01] try / catch 基础
来源：http://gmo.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uoh.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ekk.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://duf.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ted.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xpq.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ghw.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vwd.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zab.smart0.xyz

[H02] finally / ensure 收尾
来源：http://emt.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mgk.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://amm.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hub.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fcq.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://ekv.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iwa.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pwo.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uxy.guowangkeji.top

[H03] 主动抛出异常
来源：http://tbx.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://vnq.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://izr.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://ffm.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://yzc.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uze.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mhy.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mti.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://vlm.jqgufenzy.top

[H04] 自定义异常类型
来源：http://qrh.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://asi.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://byy.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://byo.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://ygl.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://jvm.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gvv.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://rna.nwbrower.top

C#:   class MyException : Exception {}
来源：http://gka.iojbl.cn

[H05] 捕获特定类型
来源：http://wpe.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://rjw.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hhd.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://yft.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://lkq.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://yhu.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ykc.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://yma.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hrw.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://byc.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://krx.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mza.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://czc.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://khh.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rvu.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fgb.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://cgg.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://ofb.dashuyun.cn

[H07] 断言
来源：http://gxt.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://tik.tianlin.xyz

PHP:  assert($x > 0);
来源：http://xtf.guannengcc.top

JS:   console.assert(x > 0);
来源：http://dhw.uphjek.com

TS:   console.assert(x > 0);
来源：http://quy.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://lgi.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jbm.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mjp.fanxiaobao.xyz


<!-- 参考信息 -->