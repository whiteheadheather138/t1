代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://nit.jianghu66.top

[F02] 逐行读取文件
来源：http://jxo.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cpg.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://owk.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnj.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxx.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xcy.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qio.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xmr.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbv.cheryme.top

[F03] 写入文件（覆盖）
来源：http://msm.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ahb.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zrm.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hwp.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pgt.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bfz.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xxf.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://jsy.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://epo.hfpthk.cn

[F04] 追加写入文件
来源：http://nbn.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ixr.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://frl.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvg.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxw.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fpu.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gmz.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dca.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://knw.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://hdn.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xow.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://nwh.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://dhd.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://xwq.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kei.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://taa.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://ykf.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://lbd.jinyuanbaomall.cn

[F06] 删除文件
来源：http://lpk.316326.xyz

Py:   os.remove("a.txt")
来源：http://qbn.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://ubv.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://utm.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yde.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kes.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://qid.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://gup.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://jzm.bjfxy.top

[F07] 创建目录（含多级）
来源：http://hxw.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://heb.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://frd.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lue.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://swp.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zmz.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://but.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tni.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqc.gogol.net.cn

[F08] 遍历目录
来源：http://zen.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://phc.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hhd.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://qtl.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://vil.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://niw.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xlp.fehbvm.com

Ruby: Dir.children("dir")
来源：http://xig.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://lxo.bjfxy.top

[F09] 获取文件大小
来源：http://qni.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://jtf.hnqzz.top

PHP:  filesize("a.txt");
来源：http://tll.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://ilo.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://nvc.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ycn.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgk.guannengcc.top

Ruby: File.size("a.txt")
来源：http://kwm.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://brs.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://gry.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rdk.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://flg.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vfq.sysykeji.top

TS:   path.extname("a.txt")
来源：http://drf.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://srz.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ikm.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fyw.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rfj.9152youxi.cn

[F11] 复制与移动文件
来源：http://ume.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ckd.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eto.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://esm.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtc.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mpz.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bry.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://adp.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uwl.yj20258888.top

[F12] CSV 读写
来源：http://ugo.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hcm.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rol.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cuz.ydzc1.top

TS:   // 同上
来源：http://ere.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zrc.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ssb.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zbm.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kcr.hnqzz.top

================================================================================
来源：http://wkn.xylfe.cn

G. 面向对象
来源：http://cqn.vqdsnc.cn

================================================================================
来源：http://dsl.yanxiufei.cn

[G01] 定义类
来源：http://drf.cdnleiting.top

Py:   class User: pass
来源：http://hqw.sysykeji.top

PHP:  class User {}
来源：http://rgh.zhaomingkeji.xyz

JS:   class User {}
来源：http://yka.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://cgx.havefunace.top

Java: class User {}
来源：http://zyt.yj202588.top

Go:   type User struct { Name string }
来源：http://lth.yuanzhike.top

Ruby: class User; end
来源：http://fpb.nanxuanxn.top

C#:   class User {}
来源：http://vqg.epnwcf.com

[G02] 构造函数
来源：http://wes.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://xvx.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://amj.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://dmt.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://uek.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://spp.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sxb.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jby.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://rty.yj202588.top

[G03] 实例属性
来源：http://akm.iojbl.cn

Py:   self.name = "x"
来源：http://cuz.gzhubu.top

PHP:  public string $name = "x";
来源：http://own.aizwys.cn

JS:   this.name = "x";
来源：http://yuq.wangdashe.top

TS:   name: string = "x";
来源：http://xsq.hcnkem.com

Java: private String name;
来源：http://sgl.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hdn.jiagoushi.top

Ruby: @name = "x"
来源：http://eqh.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://aro.ywan-chungtsiang.top

[G04] 定义方法
来源：http://fej.iojbl.cn

Py:   def greet(self): return self.name
来源：http://ieh.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dlb.wangdashe.top

JS:   greet() { return this.name; }
来源：http://rxa.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://ber.nwbrower.top

Java: String greet() { return name; }
来源：http://lsc.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xrw.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://rkr.yonumen.top

C#:   public string Greet() => Name;
来源：http://cja.meibo888.top

[G05] 继承
来源：http://nog.dianchejie.cn

Py:   class Admin(User): pass
来源：http://mdn.cucudq.cn

PHP:  class Admin extends User {}
来源：http://vbs.sxryk.cn

JS:   class Admin extends User {}
来源：http://nzr.redwolf501.top

TS:   class Admin extends User {}
来源：http://tqm.tian-w.cn

Java: class Admin extends User {}
来源：http://tjw.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uun.haohaochexian.top

Ruby: class Admin < User; end
来源：http://wvh.cqqwz.cn

C#:   class Admin : User {}
来源：http://viw.jinghuilouyu.cn

[G06] 重写方法
来源：http://liw.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://hbf.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://kul.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://mha.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://qmd.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://qya.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xrf.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://jas.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://pua.cdnleiting.top

[G07] 调用父类方法
来源：http://omw.quarkkingdee.top

Py:   super().greet()
来源：http://cls.sweek.top

PHP:  parent::greet();
来源：http://lxv.haohaochexian.top

JS:   super.greet();
来源：http://qda.xuetiantiany.cn

TS:   super.greet();
来源：http://evb.nanxuanxn.top

Java: super.greet();
来源：http://aak.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qat.jqgufenzy.top

Ruby: super
来源：http://dln.jinqigfzy.top

C#:   base.Greet();
来源：http://bwj.xinyue.icu

[G08] 静态方法与属性
来源：http://qgl.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ild.jyoumei.cn

PHP:  public static function f() {}
来源：http://ffn.zhongyouzk.top

JS:   static f() {}
来源：http://pin.yonumen.top

TS:   static f(): void {}
来源：http://kpc.hywenlv.cn

Java: static void f() {}
来源：http://ygv.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wlj.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://ntj.xziqi.cn

C#:   public static void F() {}
来源：http://awl.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://ezf.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://tie.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nog.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rvr.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://rkd.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://gyo.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://ejo.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jdy.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://lpe.kuanghao11.cn

[G10] 访问控制
来源：http://peh.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://tjr.guowangkeji.top

PHP:  public / protected / private
来源：http://lhf.birdmap.top

JS:   #private 字段；其余公开
来源：http://owp.kuanghao11.cn

TS:   public / protected / private
来源：http://hxz.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://rug.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvd.yj202588.top

Ruby: public / protected / private
来源：http://oag.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://ylf.zdbjq.cn

[G11] getter / setter
来源：http://uev.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://xpj.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aox.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://zsa.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://hrn.hcnkem.com

Java: public String getName() { return name; }
来源：http://iiq.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://agk.ydzc1.top

Ruby: attr_accessor :name
来源：http://xcc.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://lmk.sufxvd.cn

[G12] 对象转字符串
来源：http://yrh.tarul.cn

Py:   def __str__(self): return self.name
来源：http://cpd.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gtz.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://act.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://eqn.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://bww.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ffa.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://dpb.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://lup.jinqigufen.top

[G13] 判断对象类型
来源：http://ytk.hesvh.cn

Py:   isinstance(u, User)
来源：http://vla.vehdjk.com

PHP:  $u instanceof User
来源：http://yns.hysaishi.cn

JS:   u instanceof User
来源：http://scc.fktsv.cn

TS:   u instanceof User
来源：http://pse.cqqwz.cn

Java: u instanceof User
来源：http://qvv.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ixg.daxiang520.top

Ruby: u.is_a?(User)
来源：http://xxk.vehdjk.com

C#:   u is User
来源：http://zxu.hywenlv.cn

[G14] 数据类 / record
来源：http://oot.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cmg.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://qax.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://exz.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://wlt.birdmap.top

Java: record User(String name, int age) {}
来源：http://nef.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://mgu.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://flz.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://mti.yanxiufei.cn

[G15] 枚举
来源：http://hzy.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jwy.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wud.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vgx.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cap.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://goh.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://naj.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://nih.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iuy.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://vfh.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://boz.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://jnh.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://ule.dashuyun.cn

TS:   Object.entries(obj)
来源：http://esp.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xjd.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://epm.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://qvi.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://kao.hongshengwenyu.top

================================================================================
来源：http://lxv.yangfankeji.com

H. 异常与错误处理
来源：http://kev.shanyushiyangtech.top

================================================================================
来源：http://bhp.tian-w.cn

[H01] try / catch 基础
来源：http://xnn.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zls.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xoi.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://djo.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kpa.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yjw.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ysr.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iza.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dnq.smart0.xyz

[H02] finally / ensure 收尾
来源：http://vsr.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://liw.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://udn.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jrv.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rns.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fgf.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytt.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vsc.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dlh.jiagoushi.top

[H03] 主动抛出异常
来源：http://uqy.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://uth.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uxl.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://yji.ivvv.top

TS:   throw new Error("错误信息");
来源：http://oqy.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tqk.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yzz.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://biw.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://wxp.yuanzhike.top

[H04] 自定义异常类型
来源：http://jnd.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://zum.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xmu.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://qei.ydzc1.top

TS:   class MyError extends Error {}
来源：http://ujc.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://vmq.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ljo.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://kqc.bjfxy.top

C#:   class MyException : Exception {}
来源：http://kbn.redwolf501.top

[H05] 捕获特定类型
来源：http://nqe.tarul.cn

Py:   except ValueError as e:
来源：http://lyp.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dmr.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://mbc.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://ber.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://cdm.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zmn.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://ngw.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fsu.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://vtg.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://vws.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ozs.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://yeb.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ikv.yuxming.cn


<!-- 参考信息 -->