代发 wailian999

[F01] 读取整个文件
来源：http://hqy.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cir.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://ilz.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ntt.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://svw.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mda.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uaz.316326.xyz

Ruby: File.read("a.txt")
来源：http://zgp.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://tez.daria6918.cn

[F02] 逐行读取文件
来源：http://fph.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qqw.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kbt.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://krx.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ydl.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eht.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sax.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eut.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gge.yj20258.top

[F03] 写入文件（覆盖）
来源：http://kzt.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pfr.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gfa.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dur.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wvm.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uhs.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tir.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://mrz.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yzc.vehdjk.com

[F04] 追加写入文件
来源：http://xcl.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xls.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwd.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndu.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zlq.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kmq.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zpj.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://arm.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rpi.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://uqr.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://liw.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://stn.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://ypi.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://pbt.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://bzs.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ijh.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://hkv.uphjek.com

C#:   File.Exists("a.txt")
来源：http://esy.xinyue.icu

[F06] 删除文件
来源：http://zed.ybcxt.top

Py:   os.remove("a.txt")
来源：http://nsy.birdmap.top

PHP:  unlink("a.txt");
来源：http://cyb.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://cbb.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xvs.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xak.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://gni.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://mwi.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://jiv.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://iqd.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vtu.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vbc.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofg.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eip.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zjo.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gko.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fcj.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wsl.pycfn.com

[F08] 遍历目录
来源：http://uvx.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sim.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cpo.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://nzi.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://sxi.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iyw.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pbm.iojbl.cn

Ruby: Dir.children("dir")
来源：http://bbq.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://mva.tanke756.top

[F09] 获取文件大小
来源：http://xtf.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://lmt.hammf.cn

PHP:  filesize("a.txt");
来源：http://ucv.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://seu.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://vnu.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jsb.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://voj.tanke756.top

Ruby: File.size("a.txt")
来源：http://lps.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://bpz.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://yue.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wvo.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fyg.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vmg.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://gde.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ceb.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fll.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kun.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcf.ctjpmb.com

[F11] 复制与移动文件
来源：http://ixa.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xch.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rfi.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gwy.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ykc.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wke.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fsx.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pwk.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kpc.redwolf501.top

[F12] CSV 读写
来源：http://qkh.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zxd.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gku.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://klg.fanxiaobao.xyz

TS:   // 同上
来源：http://drn.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dto.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hva.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://osv.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://nuy.vehdjk.com

================================================================================
来源：http://ctn.jinyuanbaomall.cn

G. 面向对象
来源：http://sae.fengsongda.top

================================================================================
来源：http://hsn.gogol.net.cn

[G01] 定义类
来源：http://lad.ppjwa.cn

Py:   class User: pass
来源：http://dpm.fzhhl.top

PHP:  class User {}
来源：http://rnj.chenjidiqi.icu

JS:   class User {}
来源：http://pld.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://nfe.yj202588.top

Java: class User {}
来源：http://ztq.yj20258888.top

Go:   type User struct { Name string }
来源：http://pho.jqgfzy.top

Ruby: class User; end
来源：http://ekj.yfazqb.com

C#:   class User {}
来源：http://moa.meibo888.top

[G02] 构造函数
来源：http://afs.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://kry.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://rzw.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://lzo.cheryme.top

TS:   constructor(public name: string) {}
来源：http://uon.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://mod.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eef.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://ado.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://pck.tarul.cn

[G03] 实例属性
来源：http://ucf.sjlbkw.cn

Py:   self.name = "x"
来源：http://adj.hywenlv.cn

PHP:  public string $name = "x";
来源：http://myi.yfazqb.com

JS:   this.name = "x";
来源：http://xtq.ppjwa.cn

TS:   name: string = "x";
来源：http://bqy.iojbl.cn

Java: private String name;
来源：http://xjn.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csd.hcnkem.com

Ruby: @name = "x"
来源：http://hbk.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://rep.zhaomingkeji.xyz

[G04] 定义方法
来源：http://hcp.pycfn.com

Py:   def greet(self): return self.name
来源：http://nru.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wjx.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://dfd.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://rjo.jyoumei.cn

Java: String greet() { return name; }
来源：http://hjz.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fdh.aibaodan.cn

Ruby: def greet; @name; end
来源：http://tyc.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://jrp.gogol.net.cn

[G05] 继承
来源：http://wge.guowangkeji.top

Py:   class Admin(User): pass
来源：http://rjk.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://dmw.epnwcf.com

JS:   class Admin extends User {}
来源：http://igh.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://vdr.jinqigfzy.top

Java: class Admin extends User {}
来源：http://cfr.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ahx.hfpthk.cn

Ruby: class Admin < User; end
来源：http://svs.jinqigfzy.top

C#:   class Admin : User {}
来源：http://nbk.zhaomingkeji.xyz

[G06] 重写方法
来源：http://zmq.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://vrm.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zyj.tanke756.top

JS:   greet() { return "admin"; }
来源：http://qqa.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://qmq.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://jcj.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jal.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://siv.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://xes.andypj.xyz

[G07] 调用父类方法
来源：http://zlq.ybcxt.top

Py:   super().greet()
来源：http://guu.tianlin.xyz

PHP:  parent::greet();
来源：http://zcg.uphjek.com

JS:   super.greet();
来源：http://bmd.xziqi.cn

TS:   super.greet();
来源：http://abb.jinghuilouyu.cn

Java: super.greet();
来源：http://dzd.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xwa.yuanzhike.top

Ruby: super
来源：http://vkh.fzhhl.top

C#:   base.Greet();
来源：http://kro.gotoacloud.top

[G08] 静态方法与属性
来源：http://eod.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xwv.316326.xyz

PHP:  public static function f() {}
来源：http://tjz.pengpengdd.cyou

JS:   static f() {}
来源：http://mjl.zhijiandao.cn

TS:   static f(): void {}
来源：http://wly.pycfn.com

Java: static void f() {}
来源：http://vss.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://arp.tian-w.cn

Ruby: def self.f; end
来源：http://qiw.cucudq.cn

C#:   public static void F() {}
来源：http://mzn.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://ztb.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://kpu.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://ems.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rao.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://aau.guannengcc.top

Java: interface Shape { double area(); }
来源：http://ged.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://kqd.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vlk.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://jit.xylfe.cn

[G10] 访问控制
来源：http://oxt.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://uiq.zycfv.cn

PHP:  public / protected / private
来源：http://ogn.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://kyn.epnwcf.com

TS:   public / protected / private
来源：http://aee.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://gyg.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bzy.gogol.net.cn

Ruby: public / protected / private
来源：http://two.dianchejie.cn

C#:   public / protected / private / internal
来源：http://fmo.yvedp.cn

[G11] getter / setter
来源：http://ykp.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://dvk.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ghn.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://ddp.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://rja.ybcxt.top

Java: public String getName() { return name; }
来源：http://yrs.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vco.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://wyj.hnqzz.top

C#:   public string Name { get; set; }
来源：http://pii.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://gaf.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://ymq.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://abq.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://elu.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://lor.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ewo.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://dxm.pycfn.com

Ruby: def to_s; @name; end
来源：http://isb.cashguo.top

C#:   public override string ToString() => Name;
来源：http://gjt.cqqwz.cn

[G13] 判断对象类型
来源：http://evv.yj20258888.top

Py:   isinstance(u, User)
来源：http://rqu.hysaishi.cn

PHP:  $u instanceof User
来源：http://xwa.svipenyu.cn

JS:   u instanceof User
来源：http://wrz.dashuyun.cn

TS:   u instanceof User
来源：http://uad.quarkkingdee.top

Java: u instanceof User
来源：http://vci.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kgc.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://agr.zhongyouzk.top

C#:   u is User
来源：http://ybc.yj20258.top

[G14] 数据类 / record
来源：http://cva.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ueq.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://ozo.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://huw.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://ugt.cheryme.top

Java: record User(String name, int age) {}
来源：http://xbh.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://sgz.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyw.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://ikd.fktsv.cn

[G15] 枚举
来源：http://sub.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dqo.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://bah.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nmd.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fkv.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://mhb.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gvx.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://kkf.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://obn.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://ggo.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fek.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://lec.fehbvm.com

JS:   Object.entries(obj)
来源：http://fll.sysykeji.top

TS:   Object.entries(obj)
来源：http://rxd.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://umc.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wbk.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://ryr.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://vtr.aizwys.cn

================================================================================
来源：http://tja.xuetiantiany.cn

H. 异常与错误处理
来源：http://cuy.yj20258.top

================================================================================
来源：http://ynp.quarkkingdee.top

[H01] try / catch 基础
来源：http://waj.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mdp.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ocs.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://auo.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ysf.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qkk.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gya.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wfo.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rza.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://lyx.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://unb.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uta.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hfy.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://csm.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://edb.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://phq.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cuk.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qab.yvedp.cn

[H03] 主动抛出异常
来源：http://nmr.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://brp.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rcr.tanke756.top

JS:   throw new Error("错误信息");
来源：http://clx.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://jgj.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eym.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cfu.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uxp.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://vlh.jqgufenzy.top

[H04] 自定义异常类型
来源：http://qdf.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://rgv.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://peb.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://vic.meibo888.top

TS:   class MyError extends Error {}
来源：http://wrq.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://kxg.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhi.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://zcb.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://isr.cucudq.cn

[H05] 捕获特定类型
来源：http://log.zhijiandao.cn

Py:   except ValueError as e:
来源：http://ttr.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mln.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://qpe.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://epx.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://pwi.yanxiufei.cn


<!-- 参考信息 -->