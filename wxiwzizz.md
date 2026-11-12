代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qom.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqr.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://koj.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mzc.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hyi.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hce.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsq.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://drm.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ewy.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://xtd.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gdh.yj202588.top

[F04] 追加写入文件
来源：http://gfg.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ulx.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gmn.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lpg.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpk.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dbi.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xap.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rfh.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hdi.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://ago.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cjz.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://rri.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://fbh.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://rxn.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vay.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rca.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://eeu.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://wbk.chenjidiqi.icu

[F06] 删除文件
来源：http://gqj.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://xmw.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://zxg.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nri.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mev.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://abc.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://ozz.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://lnx.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://fla.yj20258.top

[F07] 创建目录（含多级）
来源：http://ewp.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bzo.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mqs.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sny.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvr.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://boz.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ldp.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dep.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://war.zycfv.cn

[F08] 遍历目录
来源：http://dnq.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bpp.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kuq.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://leb.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://tfu.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mnu.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dwy.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://oxs.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://yfh.yvedp.cn

[F09] 获取文件大小
来源：http://wpk.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://ssv.xziqi.cn

PHP:  filesize("a.txt");
来源：http://shw.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://aaf.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://pbj.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://bad.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rfu.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://uer.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://vwr.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://yij.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rfh.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vgm.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zpc.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://djw.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mkc.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://apv.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sxb.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nrj.shzxlz.cn

[F11] 复制与移动文件
来源：http://gtd.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tbr.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xym.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://huj.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upg.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ecj.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lhe.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://toq.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lhn.xziqi.cn

[F12] CSV 读写
来源：http://wzj.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ozo.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tuz.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lja.quarkkingdee.top

TS:   // 同上
来源：http://coa.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awm.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lff.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://len.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sny.vqdsnc.cn

================================================================================
来源：http://gdi.feifeiyinyue.top

G. 面向对象
来源：http://joi.yangfankeji.com

================================================================================
来源：http://emh.fktsv.cn

[G01] 定义类
来源：http://gjy.gaohongyu789.top

Py:   class User: pass
来源：http://tqe.cheryme.top

PHP:  class User {}
来源：http://wxv.ppjwa.cn

JS:   class User {}
来源：http://tlb.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://dvd.jinqigufen.top

Java: class User {}
来源：http://ufp.fehbvm.com

Go:   type User struct { Name string }
来源：http://tmv.aizwys.cn

Ruby: class User; end
来源：http://nte.ydzc1.top

C#:   class User {}
来源：http://fwb.chenzaomai.com

[G02] 构造函数
来源：http://emn.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://pdl.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://gmy.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://wej.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://maz.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://rqu.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wpn.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://pxq.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://klg.sjlbkw.cn

[G03] 实例属性
来源：http://kqd.dashuyun.cn

Py:   self.name = "x"
来源：http://ygw.gogol.net.cn

PHP:  public string $name = "x";
来源：http://ehp.xylfe.cn

JS:   this.name = "x";
来源：http://ptq.shzxlz.cn

TS:   name: string = "x";
来源：http://crl.tarul.cn

Java: private String name;
来源：http://pqx.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://epl.hnqzz.top

Ruby: @name = "x"
来源：http://vqs.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://pif.fehbvm.com

[G04] 定义方法
来源：http://fzx.tian-w.cn

Py:   def greet(self): return self.name
来源：http://mpc.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://oyp.fehbvm.com

JS:   greet() { return this.name; }
来源：http://grw.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://ofh.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://xep.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hag.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://pol.guannengcc.top

C#:   public string Greet() => Name;
来源：http://inh.birdmap.top

[G05] 继承
来源：http://lpk.cashguo.top

Py:   class Admin(User): pass
来源：http://vni.fzhhl.top

PHP:  class Admin extends User {}
来源：http://ohz.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://hap.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://pdj.yueranfly.top

Java: class Admin extends User {}
来源：http://eub.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kvm.hywenlv.cn

Ruby: class Admin < User; end
来源：http://dmh.jianghu66.top

C#:   class Admin : User {}
来源：http://rzr.uphjek.com

[G06] 重写方法
来源：http://tbk.yj202588.top

Py:   def greet(self): return "admin"
来源：http://ryw.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wxq.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://yzi.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://tft.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://rhg.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jsy.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://vqp.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://qma.uphjek.com

[G07] 调用父类方法
来源：http://hcz.sxryk.cn

Py:   super().greet()
来源：http://xvm.vehdjk.com

PHP:  parent::greet();
来源：http://yis.hywenlv.cn

JS:   super.greet();
来源：http://tbe.mhx1999.top

TS:   super.greet();
来源：http://hbr.snrcjt.cn

Java: super.greet();
来源：http://tbs.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://soq.epnwcf.com

Ruby: super
来源：http://ycc.nanxuanxn.top

C#:   base.Greet();
来源：http://ifv.yueranfly.top

[G08] 静态方法与属性
来源：http://xjc.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://byj.guannengcc.top

PHP:  public static function f() {}
来源：http://gpt.ywan-chungtsiang.top

JS:   static f() {}
来源：http://vhv.yonumen.top

TS:   static f(): void {}
来源：http://isc.zdbjq.cn

Java: static void f() {}
来源：http://dry.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://azn.yueranfly.top

Ruby: def self.f; end
来源：http://sqh.wangdashe.top

C#:   public static void F() {}
来源：http://wyq.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://otg.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://wsx.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://kuc.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ott.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://pyd.yonumen.top

Java: interface Shape { double area(); }
来源：http://sbl.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://bjf.yj202588.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbf.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://rli.jinqigfzy.top

[G10] 访问控制
来源：http://wmc.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://who.yuxming.cn

PHP:  public / protected / private
来源：http://rzi.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://pnt.yuxming.cn

TS:   public / protected / private
来源：http://dey.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://spg.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://uej.quarkkingdee.top

Ruby: public / protected / private
来源：http://qqc.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://fen.shangyingyoupin.top

[G11] getter / setter
来源：http://mrb.smart0.xyz

Py:   @property 与 @x.setter
来源：http://kba.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zek.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://sjp.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://dag.bbcook.cn

Java: public String getName() { return name; }
来源：http://wiy.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tya.ydzc1.top

Ruby: attr_accessor :name
来源：http://yyi.guannengcc.top

C#:   public string Name { get; set; }
来源：http://mob.kuanghao11.cn

[G12] 对象转字符串
来源：http://gqj.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://vpq.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://zjz.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://gtl.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://mqb.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://adv.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://psk.zycfv.cn

Ruby: def to_s; @name; end
来源：http://eqf.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://jha.sweek.top

[G13] 判断对象类型
来源：http://wlf.ctjpmb.com

Py:   isinstance(u, User)
来源：http://ggv.hammf.cn

PHP:  $u instanceof User
来源：http://qkp.hesvh.cn

JS:   u instanceof User
来源：http://nhd.ehwqpu.com

TS:   u instanceof User
来源：http://mqo.zhengqikj.top

Java: u instanceof User
来源：http://gps.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvi.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://pun.sjlbkw.cn

C#:   u is User
来源：http://tuv.jinqigufen.top

[G14] 数据类 / record
来源：http://skc.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bir.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://wim.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://hin.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://jeg.vehdjk.com

Java: record User(String name, int age) {}
来源：http://rli.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://uux.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wvz.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://mgk.hammf.cn

[G15] 枚举
来源：http://vay.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sis.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://loy.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sln.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ymx.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://ern.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oyw.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://kwz.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://njz.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://jme.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fpb.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://jdr.52xcode.cn

JS:   Object.entries(obj)
来源：http://yis.hfpthk.cn

TS:   Object.entries(obj)
来源：http://goi.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cnb.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fdv.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://vix.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://dgq.xuetiantiany.cn

================================================================================
来源：http://wqz.yongpay.top

H. 异常与错误处理
来源：http://zrd.zhixingplan.top

================================================================================
来源：http://wvk.jyoumei.cn

[H01] try / catch 基础
来源：http://rrg.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mzu.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ilt.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdg.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://erl.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xcc.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uvi.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbq.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fhw.daria6918.cn

[H02] finally / ensure 收尾
来源：http://kjn.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://xlt.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://avv.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jkb.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uyd.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://age.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://chd.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cod.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ote.iojbl.cn

[H03] 主动抛出异常
来源：http://ijd.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://udb.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ddt.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://pba.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://rjn.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pgj.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ilx.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nib.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rwe.cqqwz.cn

[H04] 自定义异常类型
来源：http://ybk.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://pch.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://agz.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://fzk.yfazqb.com

TS:   class MyError extends Error {}
来源：http://qhp.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://yff.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uar.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://ffd.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://cpw.tianlin.xyz

[H05] 捕获特定类型
来源：http://mri.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://yox.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lqy.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://efs.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://jxa.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://xox.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://esn.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://pgn.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gcb.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://zud.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://sgp.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gew.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://trv.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zqj.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cfw.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ryj.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://qke.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://izz.cashguo.top

[H07] 断言
来源：http://rpf.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://zqn.ybcxt.top

PHP:  assert($x > 0);
来源：http://nlv.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://tal.chenjidiqi.icu


<!-- 参考信息 -->