代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://aaz.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whj.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://byj.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://woe.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xzs.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://oxy.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://erm.zdbjq.cn

[F04] 追加写入文件
来源：http://ssa.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iul.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqh.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rvj.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tve.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xyq.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eaa.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ufv.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vrz.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://jpp.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nrb.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://sor.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://hof.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://xix.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dnd.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qkx.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://qlo.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://mbd.snrcjt.cn

[F06] 删除文件
来源：http://ole.meibo888.top

Py:   os.remove("a.txt")
来源：http://jyu.tanke756.top

PHP:  unlink("a.txt");
来源：http://bmb.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://wwj.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://mwn.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://poq.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://omo.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://znk.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://zkw.tanke756.top

[F07] 创建目录（含多级）
来源：http://avf.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eeh.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fqk.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://slc.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://krs.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iao.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tkd.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://clj.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fxw.uphjek.com

[F08] 遍历目录
来源：http://rye.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kff.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ndn.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://vir.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://vls.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vni.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rmr.yj20258888.top

Ruby: Dir.children("dir")
来源：http://gso.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://wwg.meibo888.top

[F09] 获取文件大小
来源：http://gwz.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://owc.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://dry.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://fsf.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://wsi.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://ibe.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ojm.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://mja.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://kep.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://nnq.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wur.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uql.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bsx.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://azj.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wfp.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gqo.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ogi.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pos.yuanzhike.top

[F11] 复制与移动文件
来源：http://ymq.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://czp.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dny.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zwm.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dsp.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kyx.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tfl.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nbg.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gpi.cqqwz.cn

[F12] CSV 读写
来源：http://orz.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gft.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsh.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://joe.xziqi.cn

TS:   // 同上
来源：http://rmg.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://niu.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://deb.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gbx.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rat.c1oappe.top

================================================================================
来源：http://les.bbcook.cn

G. 面向对象
来源：http://fwu.zhiwuduotai.top

================================================================================
来源：http://umm.pycfn.com

[G01] 定义类
来源：http://iem.jqgufenzy.top

Py:   class User: pass
来源：http://zgu.zhaomingkeji.xyz

PHP:  class User {}
来源：http://cfe.meibo888.top

JS:   class User {}
来源：http://eex.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://lik.snrcjt.cn

Java: class User {}
来源：http://ahv.yuxming.cn

Go:   type User struct { Name string }
来源：http://xce.9152youxi.cn

Ruby: class User; end
来源：http://ktc.feifeiyinyue.top

C#:   class User {}
来源：http://luc.havefunace.top

[G02] 构造函数
来源：http://byr.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://bxd.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://sln.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://oiz.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://bvs.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://qvs.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dmm.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://clq.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://fwe.yj20258.top

[G03] 实例属性
来源：http://oeg.fengsongda.top

Py:   self.name = "x"
来源：http://jxo.yuxming.cn

PHP:  public string $name = "x";
来源：http://bdw.vqdsnc.cn

JS:   this.name = "x";
来源：http://zya.yvedp.cn

TS:   name: string = "x";
来源：http://zvy.cheryme.top

Java: private String name;
来源：http://oha.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iba.guannengcc.top

Ruby: @name = "x"
来源：http://lri.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://joy.redwolf501.top

[G04] 定义方法
来源：http://xdv.xylfe.cn

Py:   def greet(self): return self.name
来源：http://idu.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hxd.yuxming.cn

JS:   greet() { return this.name; }
来源：http://agc.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://ome.shzxlz.cn

Java: String greet() { return name; }
来源：http://yso.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nxj.hysaishi.cn

Ruby: def greet; @name; end
来源：http://ioi.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://nkp.fehbvm.com

[G05] 继承
来源：http://rha.vehdjk.com

Py:   class Admin(User): pass
来源：http://vro.ivvv.top

PHP:  class Admin extends User {}
来源：http://soz.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://cku.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://ypq.yueranfly.top

Java: class Admin extends User {}
来源：http://slb.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lmc.yueranfly.top

Ruby: class Admin < User; end
来源：http://qvz.cqqwz.cn

C#:   class Admin : User {}
来源：http://bkt.shangyingyoupin.top

[G06] 重写方法
来源：http://bmj.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://heq.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jtk.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://yai.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://irq.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://bek.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kdx.birdmap.top

Ruby: def greet; "admin"; end
来源：http://wpj.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://eyf.hammf.cn

[G07] 调用父类方法
来源：http://den.daxiang520.top

Py:   super().greet()
来源：http://lok.bjfxy.top

PHP:  parent::greet();
来源：http://bgi.nwbrower.top

JS:   super.greet();
来源：http://qbf.jiagoushi.top

TS:   super.greet();
来源：http://fpy.ivvv.top

Java: super.greet();
来源：http://erb.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://znp.ybcxt.top

Ruby: super
来源：http://niy.c1oappe.top

C#:   base.Greet();
来源：http://yyv.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://xtj.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bco.jinqigfzy.top

PHP:  public static function f() {}
来源：http://yyj.daria6918.cn

JS:   static f() {}
来源：http://yer.ydzc1.top

TS:   static f(): void {}
来源：http://mrj.chenjidiqi.icu

Java: static void f() {}
来源：http://cwl.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sqw.zhongyouzk.top

Ruby: def self.f; end
来源：http://wfu.mhx1999.top

C#:   public static void F() {}
来源：http://soi.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://qau.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://xgv.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://hlk.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vfc.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://vuk.yonumen.top

Java: interface Shape { double area(); }
来源：http://efu.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://hbf.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pba.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://oqr.wangdashe.top

[G10] 访问控制
来源：http://akc.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://ien.nanxuanxn.top

PHP:  public / protected / private
来源：http://yth.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://qbj.pengpengdd.cyou

TS:   public / protected / private
来源：http://txb.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://sae.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qps.pycfn.com

Ruby: public / protected / private
来源：http://afe.hnqzz.top

C#:   public / protected / private / internal
来源：http://dsy.fengsongda.top

[G11] getter / setter
来源：http://ngv.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://fft.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bav.yj20258888.top

JS:   get name() { return this._name; }
来源：http://ejo.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://psk.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://xiw.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dxv.yonumen.top

Ruby: attr_accessor :name
来源：http://xdx.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://uyu.smart0.xyz

[G12] 对象转字符串
来源：http://ual.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://dey.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uba.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://krj.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://xvx.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://trq.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://wly.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://wtg.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://znc.sufxvd.cn

[G13] 判断对象类型
来源：http://krs.wangdashe.top

Py:   isinstance(u, User)
来源：http://ptm.yangfankeji.com

PHP:  $u instanceof User
来源：http://cou.feifeiyinyue.top

JS:   u instanceof User
来源：http://kff.xziqi.cn

TS:   u instanceof User
来源：http://mvn.shanyushiyangkeji.top

Java: u instanceof User
来源：http://pra.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fzv.uphjek.com

Ruby: u.is_a?(User)
来源：http://npp.sysykeji.top

C#:   u is User
来源：http://hjs.hfpthk.cn

[G14] 数据类 / record
来源：http://mji.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rri.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://fug.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rje.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://azo.ivvv.top

Java: record User(String name, int age) {}
来源：http://wpl.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://mhd.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://plm.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://jql.jinghuilouyu.cn

[G15] 枚举
来源：http://qqq.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfw.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvg.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kui.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kmr.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://qbb.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xnd.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://jcx.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyd.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://ikx.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://die.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://cjd.yfazqb.com

JS:   Object.entries(obj)
来源：http://aam.zycfv.cn

TS:   Object.entries(obj)
来源：http://tdv.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bbh.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tte.smart0.xyz

Ruby: obj.instance_variables
来源：http://ual.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://umz.pycfn.com

================================================================================
来源：http://iqo.pycfn.com

H. 异常与错误处理
来源：http://fjn.hysaishi.cn

================================================================================
来源：http://mnz.zdqjudy.top

[H01] try / catch 基础
来源：http://toz.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vbv.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wih.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gmq.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gud.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://knb.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ama.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kvs.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ypl.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://mdo.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://fge.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ozt.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dod.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mks.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://juw.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jzk.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uvn.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yqz.9152youxi.cn

[H03] 主动抛出异常
来源：http://oaa.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://itu.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ssg.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://uof.316326.xyz

TS:   throw new Error("错误信息");
来源：http://oew.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqy.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mpe.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://znk.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://zjo.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://pxq.sweek.top

Py:   class MyError(Exception): pass
来源：http://gvh.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wdp.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://qux.yvedp.cn

TS:   class MyError extends Error {}
来源：http://kos.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://zrj.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qzh.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://zam.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://fno.nanxinkj.top

[H05] 捕获特定类型
来源：http://nkv.quarkkingdee.top

Py:   except ValueError as e:
来源：http://yjf.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zfz.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://hpf.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://lbl.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://srg.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kez.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://ipt.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://knt.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://vch.bbcook.cn

Py:   value = d.get("k") or default
来源：http://ykl.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://yni.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://yjv.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cwl.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rdl.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vip.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://hbw.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://hkm.ehwqpu.com

[H07] 断言
来源：http://bec.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://vqt.epnwcf.com

PHP:  assert($x > 0);
来源：http://yvv.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://plq.ivvv.top

TS:   console.assert(x > 0);
来源：http://nuu.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://rpy.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mqv.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://pgm.zhoulong.xyz


<!-- 参考信息 -->