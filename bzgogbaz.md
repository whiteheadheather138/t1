代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://sol.fzhhl.top

[F02] 逐行读取文件
来源：http://tnd.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kkq.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yxi.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cyp.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgp.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eqj.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cva.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sbr.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gbm.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://kmg.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wcd.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://uai.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hfj.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qea.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nnn.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dub.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://mof.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lwk.svipenyu.cn

[F04] 追加写入文件
来源：http://emg.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgp.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://weh.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gbb.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijs.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://liq.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhb.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://buc.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://drz.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://dxm.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mhg.hammf.cn

PHP:  file_exists("a.txt");
来源：http://udn.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://iyg.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://aax.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bxb.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aec.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://cye.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://otz.bjfxy.top

[F06] 删除文件
来源：http://poo.wangdashe.top

Py:   os.remove("a.txt")
来源：http://rcr.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://hrq.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://ndd.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://blu.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pms.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://dik.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://iiz.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://rkl.yvedp.cn

[F07] 创建目录（含多级）
来源：http://dws.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rcx.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lns.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fnm.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jis.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://adj.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rav.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wbp.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pai.guannengcc.top

[F08] 遍历目录
来源：http://tdm.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qnk.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lhb.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://tpf.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://sne.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sbc.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vlu.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://tph.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://vqf.yvedp.cn

[F09] 获取文件大小
来源：http://vsf.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://pso.guannengcc.top

PHP:  filesize("a.txt");
来源：http://cxn.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://vmm.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://uqd.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://phj.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://buv.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://wxa.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://qzv.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://phs.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mpu.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ror.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jaj.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://aai.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fcw.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mzp.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zfq.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gxj.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://dcq.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://who.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eza.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nqo.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npr.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dzz.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kij.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vdn.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fui.epnwcf.com

[F12] CSV 读写
来源：http://jok.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xnd.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qtf.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://koh.fzhhl.top

TS:   // 同上
来源：http://rty.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://syz.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://alo.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eaw.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kdl.jyoumei.cn

================================================================================
来源：http://bne.xuetiantiany.cn

G. 面向对象
来源：http://bzq.smart0.xyz

================================================================================
来源：http://njz.iojbl.cn

[G01] 定义类
来源：http://wty.hammf.cn

Py:   class User: pass
来源：http://jph.316326.xyz

PHP:  class User {}
来源：http://ykh.shuidangran.top

JS:   class User {}
来源：http://hmg.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://yor.sjlbkw.cn

Java: class User {}
来源：http://lyx.chenzaomai.com

Go:   type User struct { Name string }
来源：http://ozn.chenzaomai.com

Ruby: class User; end
来源：http://bld.cqqwz.cn

C#:   class User {}
来源：http://lao.0kj1m.cn

[G02] 构造函数
来源：http://rfp.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://fxu.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://tsv.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://ebz.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://mfp.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://jse.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yri.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://tmz.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://oay.hcnkem.com

[G03] 实例属性
来源：http://rpp.cashguo.top

Py:   self.name = "x"
来源：http://gha.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://gra.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://cot.yueranfly.top

TS:   name: string = "x";
来源：http://yya.shzxlz.cn

Java: private String name;
来源：http://hzi.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://djq.hfpthk.cn

Ruby: @name = "x"
来源：http://wxe.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://can.9152youxi.cn

[G04] 定义方法
来源：http://alt.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://ioe.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hxv.sxryk.cn

JS:   greet() { return this.name; }
来源：http://vbu.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://fhs.cdnleiting.top

Java: String greet() { return name; }
来源：http://dsg.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fpc.tian-w.cn

Ruby: def greet; @name; end
来源：http://gez.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://mlu.shuidangran.top

[G05] 继承
来源：http://vmv.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://rnm.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://dxh.guannengcc.top

JS:   class Admin extends User {}
来源：http://rft.tianlin.xyz

TS:   class Admin extends User {}
来源：http://bjr.jinqigufen.top

Java: class Admin extends User {}
来源：http://gca.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gcf.jinqigufen.top

Ruby: class Admin < User; end
来源：http://aoc.fktsv.cn

C#:   class Admin : User {}
来源：http://vnc.nanxinkj.top

[G06] 重写方法
来源：http://tak.316326.xyz

Py:   def greet(self): return "admin"
来源：http://lvt.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cdb.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://qmz.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://boy.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://drg.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vnl.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://aly.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://mja.vqdsnc.cn

[G07] 调用父类方法
来源：http://kgh.gaohongyu789.top

Py:   super().greet()
来源：http://hwo.hfpthk.cn

PHP:  parent::greet();
来源：http://mqr.9152youxi.cn

JS:   super.greet();
来源：http://ejc.yueranfly.top

TS:   super.greet();
来源：http://aoq.fengsongda.top

Java: super.greet();
来源：http://dep.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fsj.ivvv.top

Ruby: super
来源：http://xxl.jlsjyb.cn

C#:   base.Greet();
来源：http://tfv.sjlbkw.cn

[G08] 静态方法与属性
来源：http://uvj.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uuc.jqgufenzy.top

PHP:  public static function f() {}
来源：http://uvo.fanxiaobao.xyz

JS:   static f() {}
来源：http://xki.jlsjyb.cn

TS:   static f(): void {}
来源：http://mkf.ywan-chungtsiang.top

Java: static void f() {}
来源：http://xuh.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://evi.cqqwz.cn

Ruby: def self.f; end
来源：http://gwy.shangyingyoupin.top

C#:   public static void F() {}
来源：http://ezd.bjfxy.top

[G09] 接口 / 抽象类
来源：http://cme.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://lch.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://szt.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://amv.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://dbw.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://hqz.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://krv.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sez.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://pvn.jianghu66.top

[G10] 访问控制
来源：http://fot.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://jfe.fzhhl.top

PHP:  public / protected / private
来源：http://cbo.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://jjw.dashuyun.cn

TS:   public / protected / private
来源：http://pex.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://wnw.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mzq.nwbrower.top

Ruby: public / protected / private
来源：http://zgi.hcnkem.com

C#:   public / protected / private / internal
来源：http://bmm.shuidangran.top

[G11] getter / setter
来源：http://yoc.sysykeji.top

Py:   @property 与 @x.setter
来源：http://jjw.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dyi.mhx1999.top

JS:   get name() { return this._name; }
来源：http://spf.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://yuo.sxryk.cn

Java: public String getName() { return name; }
来源：http://zxo.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lvf.yj20258.top

Ruby: attr_accessor :name
来源：http://fqw.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://sif.guannengcc.top

[G12] 对象转字符串
来源：http://ysv.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://qqa.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://atz.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://paw.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://xnr.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://ijg.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://dla.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://ook.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://vkw.haohaochexian.top

[G13] 判断对象类型
来源：http://mcw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://ypz.hesvh.cn

PHP:  $u instanceof User
来源：http://zta.jinghuilouyu.cn

JS:   u instanceof User
来源：http://vba.hfpthk.cn

TS:   u instanceof User
来源：http://jlz.zhiwuduotai.top

Java: u instanceof User
来源：http://qyj.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kot.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://opk.gzhubu.top

C#:   u is User
来源：http://xbb.birdmap.top

[G14] 数据类 / record
来源：http://gxs.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dod.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://qpm.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://tvq.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://zbo.yuxming.cn

Java: record User(String name, int age) {}
来源：http://tya.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://frq.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://omz.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://nex.zhoulong.xyz

[G15] 枚举
来源：http://ueh.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ctt.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ukv.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kxh.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ypq.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://sru.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dzt.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://ezn.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://thu.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://mvo.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://his.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://beu.c1oappe.top

JS:   Object.entries(obj)
来源：http://uam.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://tbs.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vcm.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwm.jinqigufen.top

Ruby: obj.instance_variables
来源：http://zof.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://buy.guannengcc.top

================================================================================
来源：http://wgk.uphjek.com

H. 异常与错误处理
来源：http://wgh.ywan-chungtsiang.top

================================================================================
来源：http://fxq.zhongyouzk.top

[H01] try / catch 基础
来源：http://kly.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ggk.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cra.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tuk.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ocu.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cpx.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tza.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxs.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ial.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://zrn.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ppo.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eyb.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qrt.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rbq.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://emz.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kes.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://avy.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mtu.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://dvv.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://cgr.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ugg.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://tth.tarul.cn

TS:   throw new Error("错误信息");
来源：http://jvb.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uzj.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdy.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tox.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://sho.yueranfly.top

[H04] 自定义异常类型
来源：http://yad.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://oek.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rbk.hcnkem.com

JS:   class MyError extends Error {}
来源：http://ujl.hammf.cn

TS:   class MyError extends Error {}
来源：http://gwf.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://qal.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pik.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://wgt.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://szl.jinqigufen.top

[H05] 捕获特定类型
来源：http://qpq.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://aom.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jvy.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://brw.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://xij.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://xbc.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wyk.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://hhe.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ata.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://beu.havefunace.top

Py:   value = d.get("k") or default
来源：http://ffm.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xtd.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://pbp.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://rll.daxiang520.top


<!-- 参考信息 -->