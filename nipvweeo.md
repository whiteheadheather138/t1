代发 wailian999

[E22] 字节长度与字符长度
来源：http://yyh.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayv.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfu.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvf.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zhk.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jxs.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://doz.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://zhe.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kvx.jinyuanbaomall.cn

================================================================================
来源：http://igb.quarkkingdee.top

F. 文件与目录
来源：http://wjy.gzhubu.top

================================================================================
来源：http://ruv.hcnkem.com

[F01] 读取整个文件
来源：http://ucc.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wlp.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://ljs.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://anx.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ani.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://tzn.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xqb.cucudq.cn

Ruby: File.read("a.txt")
来源：http://jyk.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://dby.jqgufenzy.top

[F02] 逐行读取文件
来源：http://nlz.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wym.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nit.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tkc.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ikp.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ujf.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://grg.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nyz.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://awh.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://idp.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pqf.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsp.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vyc.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tcy.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imf.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cfx.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://obm.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qma.iojbl.cn

[F04] 追加写入文件
来源：http://nno.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gtp.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://flz.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybv.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpb.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bkr.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://itw.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ptv.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xob.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://prl.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxl.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://nwx.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://fch.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://qdc.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qiv.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xvu.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://qes.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://gpd.52xcode.cn

[F06] 删除文件
来源：http://yqr.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://hak.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://mnr.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ute.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://rfs.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zzs.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://hrx.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://ikd.yj202588.top

C#:   File.Delete("a.txt");
来源：http://ogx.sweek.top

[F07] 创建目录（含多级）
来源：http://ohe.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehm.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qki.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkz.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://smj.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ocv.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://due.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gca.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fix.nwbrower.top

[F08] 遍历目录
来源：http://bne.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://woe.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ook.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://aac.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://cko.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lsp.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbn.jianghu66.top

Ruby: Dir.children("dir")
来源：http://gao.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://muf.fzhhl.top

[F09] 获取文件大小
来源：http://twi.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://ykb.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://ajj.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://dkf.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://eyf.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ojl.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bjs.yongpay.top

Ruby: File.size("a.txt")
来源：http://hvl.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://hvu.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://ttv.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bgx.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uuj.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ysw.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://arn.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xxt.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yyc.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qpv.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://esh.ctjpmb.com

[F11] 复制与移动文件
来源：http://rkh.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ekr.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vta.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzk.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ioj.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdp.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dwq.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hte.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xtk.zycfv.cn

[F12] CSV 读写
来源：http://pcv.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fyx.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://abl.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zxd.jinyuanbaomall.cn

TS:   // 同上
来源：http://sni.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zve.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zzq.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gfm.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://uhw.hongshengwenyu.top

================================================================================
来源：http://you.ivvv.top

G. 面向对象
来源：http://ivq.gzhubu.top

================================================================================
来源：http://cmp.dashuyun.cn

[G01] 定义类
来源：http://vyc.pycfn.com

Py:   class User: pass
来源：http://wms.zhaomingkeji.xyz

PHP:  class User {}
来源：http://ahg.bjfxy.top

JS:   class User {}
来源：http://chl.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://him.wangshuangyany.cn

Java: class User {}
来源：http://bwq.guannengcc.top

Go:   type User struct { Name string }
来源：http://uxr.yuxming.cn

Ruby: class User; end
来源：http://zfk.xingfuxueyuan.xyz

C#:   class User {}
来源：http://igk.jqgufenzy.top

[G02] 构造函数
来源：http://bov.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://gnp.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://icu.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://ava.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://bbu.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://jru.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xhu.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://wpy.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://uae.dashuyun.cn

[G03] 实例属性
来源：http://jcu.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://hqd.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://nkt.yueranfly.top

JS:   this.name = "x";
来源：http://rik.yvedp.cn

TS:   name: string = "x";
来源：http://fea.yonumen.top

Java: private String name;
来源：http://dlp.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dfw.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://cze.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://lmg.ppjwa.cn

[G04] 定义方法
来源：http://fwz.fzhhl.top

Py:   def greet(self): return self.name
来源：http://mur.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://krj.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://zzq.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://mhz.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://kwn.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cgr.0kj1m.cn

Ruby: def greet; @name; end
来源：http://lfi.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://ppi.cashguo.top

[G05] 继承
来源：http://yax.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://kie.gzhubu.top

PHP:  class Admin extends User {}
来源：http://die.yuxming.cn

JS:   class Admin extends User {}
来源：http://wgp.52xcode.cn

TS:   class Admin extends User {}
来源：http://dbr.xziqi.cn

Java: class Admin extends User {}
来源：http://ttk.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qcq.jiagoushi.top

Ruby: class Admin < User; end
来源：http://qvm.andypj.xyz

C#:   class Admin : User {}
来源：http://aox.sjlbkw.cn

[G06] 重写方法
来源：http://zhz.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://yev.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hmv.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://pez.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://fay.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ehc.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ysf.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://utb.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://hto.tian-w.cn

[G07] 调用父类方法
来源：http://uqh.gotoacloud.top

Py:   super().greet()
来源：http://egs.andypj.xyz

PHP:  parent::greet();
来源：http://ovz.epnwcf.com

JS:   super.greet();
来源：http://dxj.jqgufenzy.top

TS:   super.greet();
来源：http://gri.birdmap.top

Java: super.greet();
来源：http://bdt.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mgx.xuetiantiany.cn

Ruby: super
来源：http://vhn.cashguo.top

C#:   base.Greet();
来源：http://ote.tian-w.cn

[G08] 静态方法与属性
来源：http://lof.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kvl.sysykeji.top

PHP:  public static function f() {}
来源：http://gui.zhengqikj.top

JS:   static f() {}
来源：http://mvt.daria6918.cn

TS:   static f(): void {}
来源：http://hwn.jinqigufen.top

Java: static void f() {}
来源：http://msv.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fkq.ybcxt.top

Ruby: def self.f; end
来源：http://dje.xuetiantiany.cn

C#:   public static void F() {}
来源：http://nnw.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://pkz.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://bmu.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://mts.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ait.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://ymd.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://bzh.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://kop.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nbo.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://gbf.hnxiangtu.top

[G10] 访问控制
来源：http://acn.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://wtb.yonumen.top

PHP:  public / protected / private
来源：http://ecr.mhx1999.top

JS:   #private 字段；其余公开
来源：http://ujh.hnxiangtu.top

TS:   public / protected / private
来源：http://kcb.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://fnq.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://rkg.zhiwuduotai.top

Ruby: public / protected / private
来源：http://ahi.zdqjudy.top

C#:   public / protected / private / internal
来源：http://hza.xuanzx.com

[G11] getter / setter
来源：http://wqq.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://sgt.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hhh.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://xxu.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://vso.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://zvh.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zek.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://nah.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://nob.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://nkj.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://hfk.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gza.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://sms.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://onc.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://zuo.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://qnm.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://ybj.yongpay.top

C#:   public override string ToString() => Name;
来源：http://bpc.yonumen.top

[G13] 判断对象类型
来源：http://dhl.yonumen.top

Py:   isinstance(u, User)
来源：http://vac.52xcode.cn

PHP:  $u instanceof User
来源：http://ylg.c1oappe.top

JS:   u instanceof User
来源：http://tbq.ehwqpu.com

TS:   u instanceof User
来源：http://bur.pycfn.com

Java: u instanceof User
来源：http://adr.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qja.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://olf.nwbrower.top

C#:   u is User
来源：http://gtp.jqgufenzy.top

[G14] 数据类 / record
来源：http://xtp.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eyt.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://fby.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://jqv.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://vpd.daxiang520.top

Java: record User(String name, int age) {}
来源：http://bpi.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://lbj.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iax.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://iki.yfazqb.com

[G15] 枚举
来源：http://phb.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gig.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qdo.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://chj.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rok.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://zqa.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wzs.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://wjm.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cch.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://kgp.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ate.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://vkg.yongpay.top

JS:   Object.entries(obj)
来源：http://tqw.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://ejg.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gpz.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwl.yj202588.top

Ruby: obj.instance_variables
来源：http://pbp.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://dzy.tianlin.xyz

================================================================================
来源：http://qjq.daria6918.cn

H. 异常与错误处理
来源：http://zyd.ydzc1.top

================================================================================
来源：http://sad.yanxiufei.cn

[H01] try / catch 基础
来源：http://zsx.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gla.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mnl.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sne.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://row.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nih.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mya.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://omp.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uuz.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://cvk.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://nsz.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hqq.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lqa.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uqs.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fbr.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ydj.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oyr.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wxx.nanxinkj.top

[H03] 主动抛出异常
来源：http://sfs.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://hyr.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tem.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://eqs.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://mnj.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fwp.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iwn.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://iim.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://rfi.guannengcc.top

[H04] 自定义异常类型
来源：http://pto.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://vna.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://dok.jinqigfzy.top


<!-- 参考信息 -->