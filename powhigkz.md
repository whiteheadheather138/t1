代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xlh.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sau.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sbz.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nom.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://urh.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzr.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://lfy.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nbo.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dhn.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uyg.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tlh.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wgo.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://frl.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://ogd.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rxn.yfazqb.com

[F04] 追加写入文件
来源：http://imc.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mqy.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dtq.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://thk.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wza.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://squ.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mja.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pfk.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xgw.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://fim.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://orb.tanke756.top

PHP:  file_exists("a.txt");
来源：http://lco.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://npm.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://hjd.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hui.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fao.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://mhb.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://yrl.cdnleiting.top

[F06] 删除文件
来源：http://eco.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://rho.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://exn.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://agn.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wop.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rej.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://yrj.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://xsx.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://fid.daxiang520.top

[F07] 创建目录（含多级）
来源：http://elq.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ykn.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nbq.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lvl.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cen.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rfv.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ikd.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jcc.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://que.smart0.xyz

[F08] 遍历目录
来源：http://rch.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://afh.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rtg.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://bjo.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://jqe.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fzd.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zgb.cashguo.top

Ruby: Dir.children("dir")
来源：http://bfg.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://ddc.uphjek.com

[F09] 获取文件大小
来源：http://iaz.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://gii.ivvv.top

PHP:  filesize("a.txt");
来源：http://rcm.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://rgk.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://aln.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://arp.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hxq.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://rkq.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://xhj.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://vvz.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://adw.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lir.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bep.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://fek.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aff.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wht.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rgh.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://urh.ctjpmb.com

[F11] 复制与移动文件
来源：http://ido.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tde.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fny.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zvd.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqa.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wsa.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://poq.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ogg.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vbf.zycfv.cn

[F12] CSV 读写
来源：http://oga.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asu.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wum.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xmq.xziqi.cn

TS:   // 同上
来源：http://kzn.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ihx.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ilp.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ihy.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vta.xuanzx.com

================================================================================
来源：http://jem.nanxuanxn.top

G. 面向对象
来源：http://yxe.yanxiufei.cn

================================================================================
来源：http://kos.hcnkem.com

[G01] 定义类
来源：http://ams.52xcode.cn

Py:   class User: pass
来源：http://ptu.hnxiangtu.top

PHP:  class User {}
来源：http://dnv.sxryk.cn

JS:   class User {}
来源：http://oct.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://wxw.cheryme.top

Java: class User {}
来源：http://clc.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://cvq.jianghu66.top

Ruby: class User; end
来源：http://jbq.yueranfly.top

C#:   class User {}
来源：http://irh.xziqi.cn

[G02] 构造函数
来源：http://ryz.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://ewc.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://vps.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://wll.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://ydi.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://gvn.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iga.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://imy.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://vjf.snrcjt.cn

[G03] 实例属性
来源：http://bpr.yangfankeji.com

Py:   self.name = "x"
来源：http://kmh.zdqjudy.top

PHP:  public string $name = "x";
来源：http://prb.wangdashe.top

JS:   this.name = "x";
来源：http://uip.ppjwa.cn

TS:   name: string = "x";
来源：http://nle.svipenyu.cn

Java: private String name;
来源：http://dvv.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olr.yueranfly.top

Ruby: @name = "x"
来源：http://dnk.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ufd.cheryme.top

[G04] 定义方法
来源：http://bea.smart0.xyz

Py:   def greet(self): return self.name
来源：http://kfz.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://xjj.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://mnz.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://xcn.pycfn.com

Java: String greet() { return name; }
来源：http://acf.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pfc.gzhubu.top

Ruby: def greet; @name; end
来源：http://inu.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://dez.ydjk.org.cn

[G05] 继承
来源：http://bas.mhx1999.top

Py:   class Admin(User): pass
来源：http://nqo.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://iad.haohaochexian.top

JS:   class Admin extends User {}
来源：http://cia.vehdjk.com

TS:   class Admin extends User {}
来源：http://tcq.yj20258.top

Java: class Admin extends User {}
来源：http://mhe.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lks.daxiang520.top

Ruby: class Admin < User; end
来源：http://ohg.smart0.xyz

C#:   class Admin : User {}
来源：http://wma.316326.xyz

[G06] 重写方法
来源：http://aal.cashguo.top

Py:   def greet(self): return "admin"
来源：http://icu.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iqv.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://csd.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://zql.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://uls.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lxs.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://swh.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://dft.c1oappe.top

[G07] 调用父类方法
来源：http://eno.hcnkem.com

Py:   super().greet()
来源：http://fss.bjfxy.top

PHP:  parent::greet();
来源：http://zpj.vehdjk.com

JS:   super.greet();
来源：http://ciq.yueranfly.top

TS:   super.greet();
来源：http://knp.xinyue.icu

Java: super.greet();
来源：http://nks.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://was.9152youxi.cn

Ruby: super
来源：http://azn.haohaochexian.top

C#:   base.Greet();
来源：http://ape.yuanzhike.top

[G08] 静态方法与属性
来源：http://kfh.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zlf.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://cyr.yj202588.top

JS:   static f() {}
来源：http://cjf.wangdashe.top

TS:   static f(): void {}
来源：http://tov.zycfv.cn

Java: static void f() {}
来源：http://cke.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://khl.daxiang520.top

Ruby: def self.f; end
来源：http://zmh.uphjek.com

C#:   public static void F() {}
来源：http://yte.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://gca.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://lqe.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://jic.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jmu.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://vaw.ydzc1.top

Java: interface Shape { double area(); }
来源：http://uui.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://pjg.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wpk.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://vce.iojbl.cn

[G10] 访问控制
来源：http://edo.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://tnz.uphjek.com

PHP:  public / protected / private
来源：http://vzg.fzhhl.top

JS:   #private 字段；其余公开
来源：http://lwm.meibo888.top

TS:   public / protected / private
来源：http://jgj.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://udb.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://dnn.tanke756.top

Ruby: public / protected / private
来源：http://gcd.yuanzhike.top

C#:   public / protected / private / internal
来源：http://amx.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://zko.yfazqb.com

Py:   @property 与 @x.setter
来源：http://tlr.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pft.mhx1999.top

JS:   get name() { return this._name; }
来源：http://tsi.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://sld.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://zsq.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bul.gzhubu.top

Ruby: attr_accessor :name
来源：http://akl.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://jkf.sysykeji.top

[G12] 对象转字符串
来源：http://ygs.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://fwl.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mea.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://bih.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://gxa.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://gpf.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://jlj.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://ech.tanke756.top

C#:   public override string ToString() => Name;
来源：http://hqj.kuanghao11.cn

[G13] 判断对象类型
来源：http://sqj.daria6918.cn

Py:   isinstance(u, User)
来源：http://rzb.cheryme.top

PHP:  $u instanceof User
来源：http://wsb.ehwqpu.com

JS:   u instanceof User
来源：http://ame.chenjidiqi.icu

TS:   u instanceof User
来源：http://hog.zhiwuduotai.top

Java: u instanceof User
来源：http://nkb.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://scb.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://dvz.yonumen.top

C#:   u is User
来源：http://feo.yuxming.cn

[G14] 数据类 / record
来源：http://apn.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bfg.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://nud.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ywt.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://yuf.yongpay.top

Java: record User(String name, int age) {}
来源：http://arg.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://vxl.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pry.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://bqo.hywenlv.cn

[G15] 枚举
来源：http://rnr.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qup.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fjd.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://slp.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xze.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://zgl.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gaj.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://zhi.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ljg.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://axb.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kcm.meibo888.top

PHP:  get_object_vars($obj);
来源：http://xvk.nwbrower.top

JS:   Object.entries(obj)
来源：http://sib.hammf.cn

TS:   Object.entries(obj)
来源：http://xae.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jgf.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://och.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://acu.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://pgj.ywan-chungtsiang.top

================================================================================
来源：http://eqw.fanxiaobao.xyz

H. 异常与错误处理
来源：http://qca.fzhhl.top

================================================================================
来源：http://dvd.yvedp.cn

[H01] try / catch 基础
来源：http://htp.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lda.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tcu.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tym.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qzv.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dsm.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wxy.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cfb.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gkf.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://oqt.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ysy.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jqa.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://mvn.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mgu.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://fpt.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xru.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qbn.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://knt.tianlin.xyz

[H03] 主动抛出异常
来源：http://kos.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://nev.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovt.ivvv.top

JS:   throw new Error("错误信息");
来源：http://lak.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://nag.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvu.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hfm.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://job.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://egq.316326.xyz

[H04] 自定义异常类型
来源：http://kby.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://mbs.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fni.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://lah.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://fyq.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://bfg.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://unw.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://yza.yj20258.top

C#:   class MyException : Exception {}
来源：http://hre.jiagoushi.top

[H05] 捕获特定类型
来源：http://pzh.ppjwa.cn

Py:   except ValueError as e:
来源：http://jpt.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jie.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://scc.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://osv.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://jdf.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pyf.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://ect.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sja.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://haw.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://icr.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fxk.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://cgq.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://mdq.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vbw.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wqt.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://qbe.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://rkn.gzhubu.top


<!-- 参考信息 -->