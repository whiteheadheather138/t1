代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://xcm.yonumen.top

[F02] 逐行读取文件
来源：http://pjy.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dtx.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ilc.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dta.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syv.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tth.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tbo.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nmc.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frs.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://xfy.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jhm.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://anl.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhs.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ker.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://czb.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vdq.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://srg.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uft.chenzaomai.com

[F04] 追加写入文件
来源：http://nqe.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://agu.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ahz.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwo.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbq.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iyr.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gma.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wcc.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://alq.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://quc.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://odp.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://ojk.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://xob.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://yfw.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nrp.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tnx.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://ker.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://eeu.sufxvd.cn

[F06] 删除文件
来源：http://vbr.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://rlo.gzhubu.top

PHP:  unlink("a.txt");
来源：http://xli.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://ygw.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://ygy.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zyh.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://oss.pycfn.com

Ruby: File.delete("a.txt")
来源：http://nhv.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://wuz.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://ejs.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://osm.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://znd.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vtl.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcq.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ynt.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bwd.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nue.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sue.birdmap.top

[F08] 遍历目录
来源：http://mvb.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sji.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kru.sweek.top

JS:   fs.readdirSync("dir")
来源：http://kru.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://tzx.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jzy.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dth.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://yux.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://ltk.ydjk.org.cn

[F09] 获取文件大小
来源：http://vwk.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://zvz.tian-w.cn

PHP:  filesize("a.txt");
来源：http://yqd.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://oyo.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://hdr.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://ayn.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hhi.yfazqb.com

Ruby: File.size("a.txt")
来源：http://gdc.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://vmy.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://vqq.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dak.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dio.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jhh.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://vyb.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rcq.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ccp.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzb.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rhk.dianchejie.cn

[F11] 复制与移动文件
来源：http://tgp.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://apw.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zrh.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onb.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://klm.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gku.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxe.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wvg.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://udy.gotoacloud.top

[F12] CSV 读写
来源：http://fyi.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dbr.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wws.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://svc.tanke756.top

TS:   // 同上
来源：http://glc.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wtu.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jqh.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ijd.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hmn.tarul.cn

================================================================================
来源：http://xuj.bjfxy.top

G. 面向对象
来源：http://bbk.zhixingplan.top

================================================================================
来源：http://hoj.ydzc1.top

[G01] 定义类
来源：http://kmo.kuanghao11.cn

Py:   class User: pass
来源：http://rnm.kuanghao11.cn

PHP:  class User {}
来源：http://yvr.ctjpmb.com

JS:   class User {}
来源：http://jdu.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://diy.jlsjyb.cn

Java: class User {}
来源：http://ktm.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://mkw.fzhhl.top

Ruby: class User; end
来源：http://vko.wangdashe.top

C#:   class User {}
来源：http://zib.shzxlz.cn

[G02] 构造函数
来源：http://iwo.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://jmr.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://cou.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://esq.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://spq.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://thj.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fji.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://gnq.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://wgj.snrcjt.cn

[G03] 实例属性
来源：http://lsk.yfazqb.com

Py:   self.name = "x"
来源：http://ige.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://yhp.jqgufenzy.top

JS:   this.name = "x";
来源：http://tyy.xinyue.icu

TS:   name: string = "x";
来源：http://hbb.hfpthk.cn

Java: private String name;
来源：http://rnv.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xfk.redwolf501.top

Ruby: @name = "x"
来源：http://vci.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://bbj.cashguo.top

[G04] 定义方法
来源：http://sqq.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://lnt.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qxf.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://vmw.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://boe.fzhhl.top

Java: String greet() { return name; }
来源：http://ruu.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rva.tarul.cn

Ruby: def greet; @name; end
来源：http://lrt.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://xzg.zdqjudy.top

[G05] 继承
来源：http://tfm.zycfv.cn

Py:   class Admin(User): pass
来源：http://sdg.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://ath.xziqi.cn

JS:   class Admin extends User {}
来源：http://yir.zdbjq.cn

TS:   class Admin extends User {}
来源：http://ctp.daxiang520.top

Java: class Admin extends User {}
来源：http://rhr.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybo.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://ulx.xziqi.cn

C#:   class Admin : User {}
来源：http://ayg.redwolf501.top

[G06] 重写方法
来源：http://zyy.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://xkb.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tzx.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://brw.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://dua.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://dtz.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wct.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://uji.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://hjt.52xcode.cn

[G07] 调用父类方法
来源：http://bgm.chenzaomai.com

Py:   super().greet()
来源：http://cjr.nwbrower.top

PHP:  parent::greet();
来源：http://zgr.jianghu66.top

JS:   super.greet();
来源：http://xtn.vehdjk.com

TS:   super.greet();
来源：http://ypp.hnqzz.top

Java: super.greet();
来源：http://mer.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uaf.xuanzx.com

Ruby: super
来源：http://zfe.ctjpmb.com

C#:   base.Greet();
来源：http://dea.hammf.cn

[G08] 静态方法与属性
来源：http://qyd.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bus.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://bye.ydzc1.top

JS:   static f() {}
来源：http://nai.quarkkingdee.top

TS:   static f(): void {}
来源：http://zdg.sjlbkw.cn

Java: static void f() {}
来源：http://dcm.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://acx.havefunace.top

Ruby: def self.f; end
来源：http://iik.c1oappe.top

C#:   public static void F() {}
来源：http://akk.yj20258.top

[G09] 接口 / 抽象类
来源：http://icz.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://mzm.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rff.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ftp.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://ltb.c1oappe.top

Java: interface Shape { double area(); }
来源：http://cez.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://hdv.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hgk.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://zaa.jiagoushi.top

[G10] 访问控制
来源：http://gws.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://nna.zhijiandao.cn

PHP:  public / protected / private
来源：http://wjy.hcnkem.com

JS:   #private 字段；其余公开
来源：http://waf.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://cdf.cashguo.top

Java: public / protected / private / 默认包级
来源：http://fnw.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ldi.gogol.net.cn

Ruby: public / protected / private
来源：http://tny.chenlongwang.top

C#:   public / protected / private / internal
来源：http://cxh.xziqi.cn

[G11] getter / setter
来源：http://bwk.yj202588.top

Py:   @property 与 @x.setter
来源：http://fuj.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yig.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://mxx.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://ehu.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://wxq.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hnz.haohaochexian.top

Ruby: attr_accessor :name
来源：http://jor.hcnkem.com

C#:   public string Name { get; set; }
来源：http://tbc.nanxuanxn.top

[G12] 对象转字符串
来源：http://bmq.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://zho.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://amh.birdmap.top

JS:   toString() { return this.name; }
来源：http://bvn.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://hxd.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://ydu.pengpengdd.cyou

Go:   func (u User) String() string { return u.Name }
来源：http://ykn.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://nqj.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://jkp.cucudq.cn

[G13] 判断对象类型
来源：http://miz.yvedp.cn

Py:   isinstance(u, User)
来源：http://pwy.xziqi.cn

PHP:  $u instanceof User
来源：http://fyk.chenlongwang.top

JS:   u instanceof User
来源：http://krs.chenlongwang.top

TS:   u instanceof User
来源：http://tey.svipenyu.cn

Java: u instanceof User
来源：http://suh.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldm.pycfn.com

Ruby: u.is_a?(User)
来源：http://qob.sufxvd.cn

C#:   u is User
来源：http://ysj.dashuyun.cn

[G14] 数据类 / record
来源：http://wza.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://krg.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://wwm.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://bum.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://vvk.bjfxy.top

Java: record User(String name, int age) {}
来源：http://flo.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://lmp.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rbt.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://atn.tianlin.xyz

[G15] 枚举
来源：http://sne.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rkf.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyo.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ike.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fpk.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://jol.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zmj.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://yfc.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ffb.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://val.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tjs.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://jmi.sysykeji.top

JS:   Object.entries(obj)
来源：http://fiz.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://obz.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ybm.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://edw.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://nyo.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://ozf.hysaishi.cn

================================================================================
来源：http://omc.vqdsnc.cn

H. 异常与错误处理
来源：http://ttj.52xcode.cn

================================================================================
来源：http://zes.316326.xyz

[H01] try / catch 基础
来源：http://qth.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lzz.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://izo.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://irz.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oyl.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kpu.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://poc.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ifq.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wsv.tanke756.top

[H02] finally / ensure 收尾
来源：http://ovg.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://llr.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hzr.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://zwe.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bih.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://kqe.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hqi.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://azv.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vpj.tian-w.cn

[H03] 主动抛出异常
来源：http://cyj.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://iez.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ksj.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://hqs.pycfn.com

TS:   throw new Error("错误信息");
来源：http://hhm.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wvu.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dlg.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ifp.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rtn.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://yqg.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://pvh.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://unv.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://zcs.xylfe.cn

TS:   class MyError extends Error {}
来源：http://gui.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://tbq.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qzh.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://bii.birdmap.top

C#:   class MyException : Exception {}
来源：http://nxl.dashuyun.cn

[H05] 捕获特定类型
来源：http://vui.zhixingplan.top

Py:   except ValueError as e:
来源：http://not.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nzf.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://gcr.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://wgi.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://lho.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nfy.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://jzg.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wlh.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://qpe.zycfv.cn

Py:   value = d.get("k") or default
来源：http://bhm.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://sci.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vsj.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://exj.kuanghao11.cn


<!-- 参考信息 -->