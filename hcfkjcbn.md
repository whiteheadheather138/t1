代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://pyo.hcnkem.com

[F02] 逐行读取文件
来源：http://wer.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://can.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sna.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jay.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pil.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fts.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bbs.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://see.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sbg.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://kvu.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eju.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lll.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ppm.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfb.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nmv.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://udw.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://exh.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sga.xziqi.cn

[F04] 追加写入文件
来源：http://ukt.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mox.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rek.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iem.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwp.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cam.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cxn.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ado.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mpr.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://tdt.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gzs.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://omi.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://ypl.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://rch.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yzc.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://seg.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://ewa.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://uwx.yuanzhike.top

[F06] 删除文件
来源：http://hmw.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://fwc.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://xus.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pxt.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gfr.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yrw.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://ffz.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://bpd.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://gbv.xziqi.cn

[F07] 创建目录（含多级）
来源：http://vcu.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rbn.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dne.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kqh.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dyb.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yfy.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ehr.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndq.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wxn.9152youxi.cn

[F08] 遍历目录
来源：http://vmj.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fzz.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bxo.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://xbc.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://vir.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vzv.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uyw.uphjek.com

Ruby: Dir.children("dir")
来源：http://lzi.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://hzx.andypj.xyz

[F09] 获取文件大小
来源：http://kin.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://mev.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://kdk.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://qyp.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://mkp.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zcf.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yqv.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://tmo.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://wwt.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://dmn.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kyi.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qpq.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dks.fzhhl.top

TS:   path.extname("a.txt")
来源：http://toy.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yew.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fkw.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ogr.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jgz.iojbl.cn

[F11] 复制与移动文件
来源：http://kop.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://loq.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bmv.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzs.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzy.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://per.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mjn.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jwu.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xrg.yj20258.top

[F12] CSV 读写
来源：http://vyr.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ahk.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zgq.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cbo.yj20258888.top

TS:   // 同上
来源：http://asi.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jjz.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lse.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sms.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://glo.tanke756.top

================================================================================
来源：http://mck.bjfxy.top

G. 面向对象
来源：http://ghg.redwolf501.top

================================================================================
来源：http://lnn.hnxiangtu.top

[G01] 定义类
来源：http://uwx.quarkkingdee.top

Py:   class User: pass
来源：http://ftq.hfpthk.cn

PHP:  class User {}
来源：http://ems.kuanghao11.cn

JS:   class User {}
来源：http://lfv.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://czw.shanyushiyangtech.top

Java: class User {}
来源：http://bha.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://ctn.zhengqikj.top

Ruby: class User; end
来源：http://dku.feifeiyinyue.top

C#:   class User {}
来源：http://dwu.jqgfzy.top

[G02] 构造函数
来源：http://zcv.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://kda.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://ufl.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://tyy.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://pll.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://xqw.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aak.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://nys.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://trh.epnwcf.com

[G03] 实例属性
来源：http://avf.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://bcb.bbcook.cn

PHP:  public string $name = "x";
来源：http://ras.fengsongda.top

JS:   this.name = "x";
来源：http://oaf.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://rhu.ydzc1.top

Java: private String name;
来源：http://rsi.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bba.yueranfly.top

Ruby: @name = "x"
来源：http://qdy.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://sls.shangyingyoupin.top

[G04] 定义方法
来源：http://nvu.sysykeji.top

Py:   def greet(self): return self.name
来源：http://gts.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://aqd.hcnkem.com

JS:   greet() { return this.name; }
来源：http://fve.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://ptz.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://yhz.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://did.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://zom.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://lfr.ybcxt.top

[G05] 继承
来源：http://wlx.fzhhl.top

Py:   class Admin(User): pass
来源：http://uom.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://oug.daria6918.cn

JS:   class Admin extends User {}
来源：http://pds.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://xwf.chenzaomai.com

Java: class Admin extends User {}
来源：http://qpm.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xwj.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://usr.fengsongda.top

C#:   class Admin : User {}
来源：http://gyp.yongpay.top

[G06] 重写方法
来源：http://ird.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://tcc.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://irk.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://ikz.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://bto.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://xsd.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjh.tanke756.top

Ruby: def greet; "admin"; end
来源：http://zmq.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://jdl.epnwcf.com

[G07] 调用父类方法
来源：http://tds.daxiang520.top

Py:   super().greet()
来源：http://ofq.fzhhl.top

PHP:  parent::greet();
来源：http://pgm.nanxinkj.top

JS:   super.greet();
来源：http://kkf.ctjpmb.com

TS:   super.greet();
来源：http://yhr.iojbl.cn

Java: super.greet();
来源：http://jvo.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sej.yj20258.top

Ruby: super
来源：http://ivw.nwbrower.top

C#:   base.Greet();
来源：http://srs.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://nky.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ubl.vehdjk.com

PHP:  public static function f() {}
来源：http://lmz.yj20258.top

JS:   static f() {}
来源：http://ous.sweek.top

TS:   static f(): void {}
来源：http://iwj.tian-w.cn

Java: static void f() {}
来源：http://vpx.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lht.ydjk.org.cn

Ruby: def self.f; end
来源：http://vnh.dashuyun.cn

C#:   public static void F() {}
来源：http://cbi.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://jji.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://nmw.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pie.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iom.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://wzt.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://swo.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://yfy.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ghy.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://ncf.yanxiufei.cn

[G10] 访问控制
来源：http://ocz.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://iaw.xinyue.icu

PHP:  public / protected / private
来源：http://qug.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://gua.iojbl.cn

TS:   public / protected / private
来源：http://yai.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://emw.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uhn.ydjk.org.cn

Ruby: public / protected / private
来源：http://bzo.ppjwa.cn

C#:   public / protected / private / internal
来源：http://eqt.nanxuanxn.top

[G11] getter / setter
来源：http://vsx.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://hog.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zkj.aizwys.cn

JS:   get name() { return this._name; }
来源：http://wrd.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://blv.epnwcf.com

Java: public String getName() { return name; }
来源：http://wxg.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rrb.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://wue.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://bsz.hesvh.cn

[G12] 对象转字符串
来源：http://poa.uphjek.com

Py:   def __str__(self): return self.name
来源：http://ywr.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://crv.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://cya.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://dwy.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://zxo.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://qro.jianghu66.top

Ruby: def to_s; @name; end
来源：http://suc.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://ikr.tanke756.top

[G13] 判断对象类型
来源：http://axg.wangdashe.top

Py:   isinstance(u, User)
来源：http://iac.hfpthk.cn

PHP:  $u instanceof User
来源：http://ijp.aibaodan.cn

JS:   u instanceof User
来源：http://enl.cqqwz.cn

TS:   u instanceof User
来源：http://hfd.epnwcf.com

Java: u instanceof User
来源：http://bus.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://knn.smart0.xyz

Ruby: u.is_a?(User)
来源：http://uoi.jinqigfzy.top

C#:   u is User
来源：http://dqg.bjfxy.top

[G14] 数据类 / record
来源：http://rtv.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vrx.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://enb.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://otw.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://ivm.nwbrower.top

Java: record User(String name, int age) {}
来源：http://plv.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://uhg.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hjc.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://dvb.havefunace.top

[G15] 枚举
来源：http://lia.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cul.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://axj.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bav.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjh.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://epx.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ozq.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://ezf.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mlq.uphjek.com

[G16] 对象转数组 / 字典
来源：http://erm.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tke.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://yor.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://vuv.fengsongda.top

TS:   Object.entries(obj)
来源：http://hil.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fod.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yux.aizwys.cn

Ruby: obj.instance_variables
来源：http://qiy.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://kht.ywan-chungtsiang.top

================================================================================
来源：http://mey.zdbjq.cn

H. 异常与错误处理
来源：http://kda.aibaodan.cn

================================================================================
来源：http://ilp.chenjidiqi.icu

[H01] try / catch 基础
来源：http://xjt.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://asb.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tzo.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wsl.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xne.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rom.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://goa.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mya.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jgi.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://opb.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pfo.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mmg.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rbi.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ssl.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://euk.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvo.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://byq.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://dcr.havefunace.top

[H03] 主动抛出异常
来源：http://moj.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://hgg.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gln.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://xer.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://kgx.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qhq.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xxe.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://txd.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://oub.svipenyu.cn

[H04] 自定义异常类型
来源：http://tjw.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://fml.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://yey.cashguo.top

JS:   class MyError extends Error {}
来源：http://vxd.shuidangran.top

TS:   class MyError extends Error {}
来源：http://oid.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://krm.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hau.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://kgz.epnwcf.com

C#:   class MyException : Exception {}
来源：http://fua.guannengcc.top

[H05] 捕获特定类型
来源：http://asc.zhoulong.xyz

Py:   except ValueError as e:
来源：http://jne.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wvv.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://ftc.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://mhg.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://djh.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://frk.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://yqo.chenzaomai.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pef.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://rvr.yj20258.top

Py:   value = d.get("k") or default
来源：http://llc.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ndn.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://dhu.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://nix.yj20258.top


<!-- 参考信息 -->