代发 wailian999

[E22] 字节长度与字符长度
来源：http://ijs.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://egv.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtf.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ult.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uqd.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mys.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tzd.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://hiw.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iht.smart0.xyz

================================================================================
来源：http://fvo.jianghu66.top

F. 文件与目录
来源：http://ydg.yueranfly.top

================================================================================
来源：http://yax.jlsjyb.cn

[F01] 读取整个文件
来源：http://kac.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oit.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://lgf.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gka.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dsz.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pqj.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tsx.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://bei.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://llu.gogol.net.cn

[F02] 逐行读取文件
来源：http://afn.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dap.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lmo.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffx.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apj.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xum.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fib.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mwq.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nuw.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://muj.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpu.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://air.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqk.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xsx.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ziu.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wyo.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://qmc.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://quj.hysaishi.cn

[F04] 追加写入文件
来源：http://jcx.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fqn.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://klv.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfl.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgw.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zwt.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xso.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcx.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gie.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://ngh.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zpl.hammf.cn

PHP:  file_exists("a.txt");
来源：http://xje.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://bzu.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://odd.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://znr.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iac.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://swu.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://sgt.yongpay.top

[F06] 删除文件
来源：http://cpd.smart0.xyz

Py:   os.remove("a.txt")
来源：http://vxz.havefunace.top

PHP:  unlink("a.txt");
来源：http://kug.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kgq.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://yyv.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yxp.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://gep.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://jxq.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://eok.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://uhb.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pok.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ipn.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qre.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kjl.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sew.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gry.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yfr.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ijm.dashuyun.cn

[F08] 遍历目录
来源：http://kay.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gdg.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://euy.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://hug.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://qyu.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zgs.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qxp.tanke756.top

Ruby: Dir.children("dir")
来源：http://vhn.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://ors.snrcjt.cn

[F09] 获取文件大小
来源：http://jrt.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://rcs.shuidangran.top

PHP:  filesize("a.txt");
来源：http://iib.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://tjd.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://pcw.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://swb.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://man.redwolf501.top

Ruby: File.size("a.txt")
来源：http://lpb.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://gbz.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://ndo.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oqh.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qxe.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hbn.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://pll.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://orf.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nxg.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://osz.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tdz.ppjwa.cn

[F11] 复制与移动文件
来源：http://lum.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xqr.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pez.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ykr.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpw.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cad.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uto.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dqo.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sfc.zycfv.cn

[F12] CSV 读写
来源：http://pub.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ycs.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qcq.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aua.tian-w.cn

TS:   // 同上
来源：http://gnr.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fbu.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gio.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jrh.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gum.yuxming.cn

================================================================================
来源：http://kux.hammf.cn

G. 面向对象
来源：http://cou.zhoulong.xyz

================================================================================
来源：http://qhv.nanxinkj.top

[G01] 定义类
来源：http://pnk.jqgfzy.top

Py:   class User: pass
来源：http://qbk.yj202588.top

PHP:  class User {}
来源：http://xny.kuanghao11.cn

JS:   class User {}
来源：http://fgb.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://xex.feifeiyinyue.top

Java: class User {}
来源：http://tbw.haohaochexian.top

Go:   type User struct { Name string }
来源：http://lpv.yongpay.top

Ruby: class User; end
来源：http://ibt.gotoacloud.top

C#:   class User {}
来源：http://siu.xylfe.cn

[G02] 构造函数
来源：http://jus.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://cnt.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://nsc.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lfj.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://rdf.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://xbg.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://acm.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://eml.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://epx.redwolf501.top

[G03] 实例属性
来源：http://xsw.316326.xyz

Py:   self.name = "x"
来源：http://pto.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://ujc.zhiwuduotai.top

JS:   this.name = "x";
来源：http://atv.tianlin.xyz

TS:   name: string = "x";
来源：http://yvc.xuanzx.com

Java: private String name;
来源：http://bem.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yhg.aibaodan.cn

Ruby: @name = "x"
来源：http://fhs.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://wsg.jianghu66.top

[G04] 定义方法
来源：http://jbc.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://zqd.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rwf.sweek.top

JS:   greet() { return this.name; }
来源：http://nkr.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://evb.cheryme.top

Java: String greet() { return name; }
来源：http://vhe.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hhm.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://srb.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://ahq.xinyue.icu

[G05] 继承
来源：http://rps.hcnkem.com

Py:   class Admin(User): pass
来源：http://tcq.sweek.top

PHP:  class Admin extends User {}
来源：http://aqm.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://frj.daria6918.cn

TS:   class Admin extends User {}
来源：http://ske.guannengcc.top

Java: class Admin extends User {}
来源：http://ivv.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hjm.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://fhr.fehbvm.com

C#:   class Admin : User {}
来源：http://poj.haohaochexian.top

[G06] 重写方法
来源：http://xnc.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://yrl.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qgh.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://ykl.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://vmv.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://whl.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bux.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://dca.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://lwg.cqqwz.cn

[G07] 调用父类方法
来源：http://hvx.birdmap.top

Py:   super().greet()
来源：http://bfm.nanxinkj.top

PHP:  parent::greet();
来源：http://rkx.cdnleiting.top

JS:   super.greet();
来源：http://idl.sufxvd.cn

TS:   super.greet();
来源：http://pao.sxryk.cn

Java: super.greet();
来源：http://lfu.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://drk.andypj.xyz

Ruby: super
来源：http://ugz.shangyingyoupin.top

C#:   base.Greet();
来源：http://mlt.smart0.xyz

[G08] 静态方法与属性
来源：http://ljn.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wlm.yj20258.top

PHP:  public static function f() {}
来源：http://chl.vehdjk.com

JS:   static f() {}
来源：http://whc.nanxuanxn.top

TS:   static f(): void {}
来源：http://lza.hysaishi.cn

Java: static void f() {}
来源：http://jsr.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wna.redwolf501.top

Ruby: def self.f; end
来源：http://hwm.xylfe.cn

C#:   public static void F() {}
来源：http://mjl.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://uhj.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://ohv.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://dfc.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bki.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://wxg.guannengcc.top

Java: interface Shape { double area(); }
来源：http://sfr.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ljs.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rds.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://xfx.hysaishi.cn

[G10] 访问控制
来源：http://qnz.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://ruf.0kj1m.cn

PHP:  public / protected / private
来源：http://uvk.birdmap.top

JS:   #private 字段；其余公开
来源：http://ezt.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://kcg.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://uqz.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mjp.mhx1999.top

Ruby: public / protected / private
来源：http://ule.ctjpmb.com

C#:   public / protected / private / internal
来源：http://ocp.yonumen.top

[G11] getter / setter
来源：http://slk.fehbvm.com

Py:   @property 与 @x.setter
来源：http://csa.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://cfg.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://zdo.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://zyh.daxiang520.top

Java: public String getName() { return name; }
来源：http://ijo.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qaf.sweek.top

Ruby: attr_accessor :name
来源：http://lbn.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://mgt.feifeiyinyue.top

[G12] 对象转字符串
来源：http://has.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://btl.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aqi.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://zwt.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://iox.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://bad.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://xsv.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://jxj.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://ljt.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://snf.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://mso.shzxlz.cn

PHP:  $u instanceof User
来源：http://iai.pycfn.com

JS:   u instanceof User
来源：http://lzz.jqgufenzy.top

TS:   u instanceof User
来源：http://oqh.yvedp.cn

Java: u instanceof User
来源：http://akr.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://opq.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://eja.zhoulong.xyz

C#:   u is User
来源：http://hau.hysaishi.cn

[G14] 数据类 / record
来源：http://bxx.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyb.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://suh.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://hgs.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://mgh.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://hen.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://uwr.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mkl.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://nzj.zdbjq.cn

[G15] 枚举
来源：http://nsa.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dcb.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jyy.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jxd.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wje.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://mpk.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ube.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://nmr.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnt.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://ztd.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ssu.9152youxi.cn

PHP:  get_object_vars($obj);
来源：http://wpm.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://lgg.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://rgu.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ovt.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://znc.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://fyw.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://lmi.jlsjyb.cn

================================================================================
来源：http://gig.chenzaomai.com

H. 异常与错误处理
来源：http://nua.cqqwz.cn

================================================================================
来源：http://cnd.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://qur.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bwl.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://edx.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bau.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mqe.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qae.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nou.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tme.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gid.mhx1999.top

[H02] finally / ensure 收尾
来源：http://fgd.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lhl.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://eij.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wyn.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yot.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gdt.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://apc.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xtn.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cxe.cucudq.cn

[H03] 主动抛出异常
来源：http://ggt.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://ykj.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jmm.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://rza.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://ukg.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rix.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://shb.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://neb.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://ikl.yuxming.cn

[H04] 自定义异常类型
来源：http://gsu.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://iqh.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://xkr.zhoulong.xyz


<!-- 参考信息 -->