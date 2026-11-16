代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://iwj.andypj.xyz

[F02] 逐行读取文件
来源：http://xdk.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rtl.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qcj.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://med.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtr.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ind.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kxz.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xbs.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tdq.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://uff.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnq.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yka.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://htu.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kil.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yyd.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://shb.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://mnp.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fep.ydzc1.top

[F04] 追加写入文件
来源：http://auf.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kop.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://akd.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyu.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aov.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ate.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://omw.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fov.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mdl.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://nrs.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aro.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://ume.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://uav.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://aym.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ntk.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rav.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://ksj.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://chd.sjlbkw.cn

[F06] 删除文件
来源：http://eyj.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://abn.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://pin.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://ese.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://xzh.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qdp.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://bmy.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://lpw.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://jaf.andypj.xyz

[F07] 创建目录（含多级）
来源：http://vqk.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hrb.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wnt.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://you.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrd.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ynt.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rvm.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nyb.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nek.gaohongyu789.top

[F08] 遍历目录
来源：http://xha.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jys.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oes.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://xmn.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://zwj.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cyi.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zyz.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://qyo.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://vjf.chenjidiqi.icu

[F09] 获取文件大小
来源：http://nxc.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://ufv.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://lyc.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://nnl.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://zkb.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://pks.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tlf.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://wei.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://ein.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://vft.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lyt.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvp.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zns.xziqi.cn

TS:   path.extname("a.txt")
来源：http://vck.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ivg.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dst.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://guw.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mcz.bjfxy.top

[F11] 复制与移动文件
来源：http://ebr.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qih.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://clu.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wup.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://emp.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gqx.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wuc.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ghf.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://paa.9152youxi.cn

[F12] CSV 读写
来源：http://wsq.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kqx.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jxj.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://drf.sysykeji.top

TS:   // 同上
来源：http://uso.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rfo.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://juo.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lgc.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rim.jinqigufen.top

================================================================================
来源：http://oqr.nwbrower.top

G. 面向对象
来源：http://wrk.ywan-chungtsiang.top

================================================================================
来源：http://wyg.jinqigufen.top

[G01] 定义类
来源：http://dzw.zhengqikj.top

Py:   class User: pass
来源：http://ych.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://cfs.tian-w.cn

JS:   class User {}
来源：http://nue.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://wnu.snrcjt.cn

Java: class User {}
来源：http://ayh.yangfankeji.com

Go:   type User struct { Name string }
来源：http://drk.yj20258888.top

Ruby: class User; end
来源：http://pbw.tianlin.xyz

C#:   class User {}
来源：http://hqc.shzxlz.cn

[G02] 构造函数
来源：http://mjy.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://gqj.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://lrj.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://ewo.ivvv.top

TS:   constructor(public name: string) {}
来源：http://mjh.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://ymd.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jte.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://xxn.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://bsb.52xcode.cn

[G03] 实例属性
来源：http://jhr.fehbvm.com

Py:   self.name = "x"
来源：http://ski.0kj1m.cn

PHP:  public string $name = "x";
来源：http://ieq.nanxuanxn.top

JS:   this.name = "x";
来源：http://emp.gaohongyu789.top

TS:   name: string = "x";
来源：http://toi.cashguo.top

Java: private String name;
来源：http://ibj.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rwb.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://ubm.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://lvt.bjfxy.top

[G04] 定义方法
来源：http://sam.hammf.cn

Py:   def greet(self): return self.name
来源：http://qrl.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kha.daxiang520.top

JS:   greet() { return this.name; }
来源：http://kbq.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://aoi.cucudq.cn

Java: String greet() { return name; }
来源：http://phb.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xii.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://vzn.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://vgu.sjlbkw.cn

[G05] 继承
来源：http://oiu.hysaishi.cn

Py:   class Admin(User): pass
来源：http://jya.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://qeg.birdmap.top

JS:   class Admin extends User {}
来源：http://lyb.redwolf501.top

TS:   class Admin extends User {}
来源：http://gkk.chenzaomai.com

Java: class Admin extends User {}
来源：http://tny.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kov.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://tab.zhongyouzk.top

C#:   class Admin : User {}
来源：http://qat.vqdsnc.cn

[G06] 重写方法
来源：http://lpj.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://nog.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bmi.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://nrb.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://yxo.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://rna.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xgh.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://dgt.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://tle.yanxiufei.cn

[G07] 调用父类方法
来源：http://jki.fehbvm.com

Py:   super().greet()
来源：http://lue.hcnkem.com

PHP:  parent::greet();
来源：http://dqn.ehwqpu.com

JS:   super.greet();
来源：http://hmn.hnxiangtu.top

TS:   super.greet();
来源：http://vix.jqgfzy.top

Java: super.greet();
来源：http://ahi.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mir.gotoacloud.top

Ruby: super
来源：http://zca.snrcjt.cn

C#:   base.Greet();
来源：http://qyn.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://heh.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rfz.yj20258.top

PHP:  public static function f() {}
来源：http://dmh.shzxlz.cn

JS:   static f() {}
来源：http://caj.snrcjt.cn

TS:   static f(): void {}
来源：http://cbi.ppjwa.cn

Java: static void f() {}
来源：http://tgd.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bbp.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://flb.sufxvd.cn

C#:   public static void F() {}
来源：http://kce.uphjek.com

[G09] 接口 / 抽象类
来源：http://lxh.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://rbz.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://fbi.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mzr.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://uvy.redwolf501.top

Java: interface Shape { double area(); }
来源：http://ezc.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://ubn.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rrf.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://apt.sufxvd.cn

[G10] 访问控制
来源：http://tfw.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://goy.haohaochexian.top

PHP:  public / protected / private
来源：http://ivh.havefunace.top

JS:   #private 字段；其余公开
来源：http://fql.nanxinkj.top

TS:   public / protected / private
来源：http://rew.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://nkj.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vqs.cucudq.cn

Ruby: public / protected / private
来源：http://xge.gotoacloud.top

C#:   public / protected / private / internal
来源：http://dhz.svipenyu.cn

[G11] getter / setter
来源：http://gro.hesvh.cn

Py:   @property 与 @x.setter
来源：http://btk.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://oyn.316326.xyz

JS:   get name() { return this._name; }
来源：http://num.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://xcv.mhx1999.top

Java: public String getName() { return name; }
来源：http://jyb.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jsm.tian-w.cn

Ruby: attr_accessor :name
来源：http://vwi.tian-w.cn

C#:   public string Name { get; set; }
来源：http://cwj.nwbrower.top

[G12] 对象转字符串
来源：http://tbd.yongpay.top

Py:   def __str__(self): return self.name
来源：http://zpz.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://srz.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://wkj.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://min.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://mdt.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://fug.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://grv.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://dwh.jinqigfzy.top

[G13] 判断对象类型
来源：http://tlw.xuanzx.com

Py:   isinstance(u, User)
来源：http://kmc.sjlbkw.cn

PHP:  $u instanceof User
来源：http://qoc.cucudq.cn

JS:   u instanceof User
来源：http://kal.yfazqb.com

TS:   u instanceof User
来源：http://fsm.shuidangran.top

Java: u instanceof User
来源：http://gjz.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xhc.epnwcf.com

Ruby: u.is_a?(User)
来源：http://ohf.yanxiufei.cn

C#:   u is User
来源：http://imz.xuanzx.com

[G14] 数据类 / record
来源：http://byc.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dhp.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://qsx.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://epz.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://tlw.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://stj.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://hnb.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dbg.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://sti.316326.xyz

[G15] 枚举
来源：http://zep.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llv.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gcw.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqs.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tcy.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://oam.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://unv.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://jeh.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gof.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://jhw.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lmc.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://cum.tianlin.xyz

JS:   Object.entries(obj)
来源：http://tef.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://qen.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bmp.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://upb.snrcjt.cn

Ruby: obj.instance_variables
来源：http://mib.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://rgm.yonumen.top

================================================================================
来源：http://mzi.hongshengwenyu.top

H. 异常与错误处理
来源：http://ila.jianghu66.top

================================================================================
来源：http://ikv.ivvv.top

[H01] try / catch 基础
来源：http://mfj.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ywm.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lrr.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fav.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bax.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bkf.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://onz.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jpn.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zif.fehbvm.com

[H02] finally / ensure 收尾
来源：http://zpd.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rcw.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://pzz.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lwk.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rpo.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://vcf.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jkv.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fdj.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jrx.zhijiandao.cn

[H03] 主动抛出异常
来源：http://ska.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://eqh.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jsq.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://kuo.pycfn.com

TS:   throw new Error("错误信息");
来源：http://tdi.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfc.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yqt.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hmy.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://lwl.epnwcf.com

[H04] 自定义异常类型
来源：http://tpu.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://ulw.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qtl.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://srs.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://lsu.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://ppp.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hre.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://cgd.hcnkem.com

C#:   class MyException : Exception {}
来源：http://ckm.meibo888.top

[H05] 捕获特定类型
来源：http://ltl.ppjwa.cn

Py:   except ValueError as e:
来源：http://ljh.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jkm.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://qrd.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://kdi.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://ekl.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pww.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://sud.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://akj.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://azb.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://aip.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://blr.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://cfo.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://acd.aizwys.cn


<!-- 参考信息 -->