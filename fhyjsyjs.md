代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hvb.tianlin.xyz

[F02] 逐行读取文件
来源：http://cwj.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qgm.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oqj.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mcx.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjw.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ctq.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uem.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fuk.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://arh.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://qlx.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkh.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://cta.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fxe.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vcb.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfq.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lya.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://udh.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rtw.hongshengwenyu.top

[F04] 追加写入文件
来源：http://bed.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itr.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wil.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wst.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xua.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hvk.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ofd.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gez.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ffx.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://kjf.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxp.birdmap.top

PHP:  file_exists("a.txt");
来源：http://nmk.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://qmd.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://dhk.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nrv.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zde.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://coa.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://lzu.hysaishi.cn

[F06] 删除文件
来源：http://tar.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://wbr.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://gxc.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://ysf.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vye.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uyt.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://whj.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://mts.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://ycj.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://nut.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zkk.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://avh.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kia.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bpf.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://frv.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wyc.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zdv.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://exc.vehdjk.com

[F08] 遍历目录
来源：http://poz.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vsq.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://moq.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://zgp.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://frr.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bgx.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nhu.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://xlg.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://lcp.gzhubu.top

[F09] 获取文件大小
来源：http://wtp.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://ggo.52xcode.cn

PHP:  filesize("a.txt");
来源：http://twe.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://gcg.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://hnp.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hpg.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kaf.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://zjz.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://xry.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://lst.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ttz.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://juy.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dqh.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://bbx.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gvr.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sqw.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zta.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://umk.hnxiangtu.top

[F11] 复制与移动文件
来源：http://tjw.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cgv.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kjs.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymi.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lao.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://anf.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://txx.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whj.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cer.jlsjyb.cn

[F12] CSV 读写
来源：http://kby.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mhz.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jjg.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://reb.shangyingyoupin.top

TS:   // 同上
来源：http://pgd.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fry.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tpp.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fxr.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dnz.tanke756.top

================================================================================
来源：http://yom.0kj1m.cn

G. 面向对象
来源：http://iny.ctjpmb.com

================================================================================
来源：http://zre.gaohongyu789.top

[G01] 定义类
来源：http://vdv.cdnleiting.top

Py:   class User: pass
来源：http://ftx.gotoacloud.top

PHP:  class User {}
来源：http://inz.xylfe.cn

JS:   class User {}
来源：http://mzi.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://zkp.gotoacloud.top

Java: class User {}
来源：http://wkn.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://glr.shzxlz.cn

Ruby: class User; end
来源：http://adv.meibo888.top

C#:   class User {}
来源：http://yrp.iojbl.cn

[G02] 构造函数
来源：http://fxj.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://nci.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://zsr.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://knb.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://vvj.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://wqh.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lie.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://xcu.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://lpi.gogol.net.cn

[G03] 实例属性
来源：http://sgy.sjlbkw.cn

Py:   self.name = "x"
来源：http://yeu.52xcode.cn

PHP:  public string $name = "x";
来源：http://gej.daria6918.cn

JS:   this.name = "x";
来源：http://iva.cheryme.top

TS:   name: string = "x";
来源：http://ecp.chenlongwang.top

Java: private String name;
来源：http://qtu.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cmm.redwolf501.top

Ruby: @name = "x"
来源：http://pxm.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://rkp.sufxvd.cn

[G04] 定义方法
来源：http://ydv.fengsongda.top

Py:   def greet(self): return self.name
来源：http://jek.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qpr.nwbrower.top

JS:   greet() { return this.name; }
来源：http://zsk.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://ret.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://utu.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://cdf.hywenlv.cn

Ruby: def greet; @name; end
来源：http://msi.fehbvm.com

C#:   public string Greet() => Name;
来源：http://nxu.fktsv.cn

[G05] 继承
来源：http://rvv.redwolf501.top

Py:   class Admin(User): pass
来源：http://kwj.52xcode.cn

PHP:  class Admin extends User {}
来源：http://cfy.hysaishi.cn

JS:   class Admin extends User {}
来源：http://uiu.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://qym.xinyue.icu

Java: class Admin extends User {}
来源：http://kah.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tgz.316326.xyz

Ruby: class Admin < User; end
来源：http://ijq.hywenlv.cn

C#:   class Admin : User {}
来源：http://vka.hfpthk.cn

[G06] 重写方法
来源：http://ani.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://vfi.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vsn.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://jfl.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://kut.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://nrq.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cac.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://huv.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://zvo.yonumen.top

[G07] 调用父类方法
来源：http://tvg.zhoulong.xyz

Py:   super().greet()
来源：http://oxw.havefunace.top

PHP:  parent::greet();
来源：http://iik.hywenlv.cn

JS:   super.greet();
来源：http://rnz.yanxiufei.cn

TS:   super.greet();
来源：http://ilw.smart0.xyz

Java: super.greet();
来源：http://bmj.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hhq.zhijiandao.cn

Ruby: super
来源：http://wbs.xziqi.cn

C#:   base.Greet();
来源：http://arv.sxryk.cn

[G08] 静态方法与属性
来源：http://qkm.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://llw.quarkkingdee.top

PHP:  public static function f() {}
来源：http://yhf.shanyushiyangkeji.top

JS:   static f() {}
来源：http://rqc.gaohongyu789.top

TS:   static f(): void {}
来源：http://qhd.cashguo.top

Java: static void f() {}
来源：http://uoj.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vjx.9152youxi.cn

Ruby: def self.f; end
来源：http://jha.shangyingyoupin.top

C#:   public static void F() {}
来源：http://uhj.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://bpi.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://oqm.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://hzf.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pvy.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://ute.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://nph.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://igu.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqn.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://tap.xinyue.icu

[G10] 访问控制
来源：http://sqb.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://bht.dashuyun.cn

PHP:  public / protected / private
来源：http://ood.yj20258888.top

JS:   #private 字段；其余公开
来源：http://tzt.jinghuilouyu.cn

TS:   public / protected / private
来源：http://fhj.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://mpy.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tlc.sweek.top

Ruby: public / protected / private
来源：http://sfp.chenzaomai.com

C#:   public / protected / private / internal
来源：http://rml.hnxiangtu.top

[G11] getter / setter
来源：http://ybd.zycfv.cn

Py:   @property 与 @x.setter
来源：http://cox.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dbz.daria6918.cn

JS:   get name() { return this._name; }
来源：http://rwl.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://rot.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://yeg.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cwi.yangfankeji.com

Ruby: attr_accessor :name
来源：http://zay.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://kiy.ybcxt.top

[G12] 对象转字符串
来源：http://cri.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://erh.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pth.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://dfu.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://nre.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://ijb.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oyo.hammf.cn

Ruby: def to_s; @name; end
来源：http://xvd.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://vhb.chenzaomai.com

[G13] 判断对象类型
来源：http://jvi.ybcxt.top

Py:   isinstance(u, User)
来源：http://uyb.xinyue.icu

PHP:  $u instanceof User
来源：http://sbz.ydzc1.top

JS:   u instanceof User
来源：http://bkn.smart0.xyz

TS:   u instanceof User
来源：http://hnx.jiagoushi.top

Java: u instanceof User
来源：http://zzl.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wdo.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://dyf.vehdjk.com

C#:   u is User
来源：http://nmg.guannengcc.top

[G14] 数据类 / record
来源：http://qxm.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ddu.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://gmp.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://ljl.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://npm.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://lmv.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://cto.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yjn.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://wuz.cucudq.cn

[G15] 枚举
来源：http://jkm.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vxz.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yjb.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qwl.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ywp.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://srr.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ins.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://vaw.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://btm.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://uqp.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tuh.hammf.cn

PHP:  get_object_vars($obj);
来源：http://guw.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://xns.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://ohf.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tdn.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://prs.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://cud.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://mfe.ydjk.org.cn

================================================================================
来源：http://ave.gzhubu.top

H. 异常与错误处理
来源：http://kui.hywenlv.cn

================================================================================
来源：http://yaj.gaohongyu789.top

[H01] try / catch 基础
来源：http://ivy.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://feg.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zwj.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xnr.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://smd.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dmo.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jbj.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gst.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rev.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://ndr.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://goc.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lqk.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ufj.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uyh.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ygq.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aef.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ugs.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mld.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://hou.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://lzs.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lnf.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://vue.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://ved.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://onz.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dyi.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sox.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zjw.ppjwa.cn

[H04] 自定义异常类型
来源：http://moi.tarul.cn

Py:   class MyError(Exception): pass
来源：http://ibm.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://pze.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://ecc.yonumen.top

TS:   class MyError extends Error {}
来源：http://doz.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://cog.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jcs.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://gsg.bjfxy.top

C#:   class MyException : Exception {}
来源：http://ltu.vehdjk.com

[H05] 捕获特定类型
来源：http://qmv.andypj.xyz

Py:   except ValueError as e:
来源：http://bis.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://twd.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://nsd.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gow.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://qut.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vmz.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://jhj.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwv.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://ncx.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://jxb.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://qwp.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uta.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://gnj.ydjk.org.cn


<!-- 参考信息 -->