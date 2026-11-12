代发 wailian999

Go:   if s == "" {}
来源：http://nns.yanxiufei.cn

Ruby: if s.empty?
来源：http://igk.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://krx.hesvh.cn

[E21] 超长截断加省略号
来源：http://tov.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsa.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yrj.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvn.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijg.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zth.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://sxe.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ofr.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tev.uphjek.com

[E22] 字节长度与字符长度
来源：http://qeq.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tyf.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bhs.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fvd.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpe.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rol.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ija.sweek.top

Ruby: s.bytesize;  s.length
来源：http://yjx.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dxe.yj20258.top

================================================================================
来源：http://dcm.meibo888.top

F. 文件与目录
来源：http://wdm.316326.xyz

================================================================================
来源：http://nnn.yongpay.top

[F01] 读取整个文件
来源：http://tfg.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rzs.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://nmq.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yir.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oso.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://gig.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sps.yuxming.cn

Ruby: File.read("a.txt")
来源：http://xmn.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://iyz.fktsv.cn

[F02] 逐行读取文件
来源：http://axx.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kxr.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mhu.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tub.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akq.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wgz.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lmp.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qoi.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwv.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://ivf.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aaf.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://toj.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jds.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baa.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xso.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jxx.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://prp.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xki.wangshuangyany.cn

[F04] 追加写入文件
来源：http://odl.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://huf.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ozb.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aww.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tba.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pmj.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://slb.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcc.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qku.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://cto.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oen.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://ioh.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://sdt.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://fyj.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kjs.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ipj.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://acz.sweek.top

C#:   File.Exists("a.txt")
来源：http://cha.bjfxy.top

[F06] 删除文件
来源：http://euf.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://cxu.guannengcc.top

PHP:  unlink("a.txt");
来源：http://cyd.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://zye.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://awy.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iyt.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://zlz.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://wxk.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://ezq.iojbl.cn

[F07] 创建目录（含多级）
来源：http://olv.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zuq.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ouc.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://llp.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upc.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jyl.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ztb.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bkw.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bqy.quarkkingdee.top

[F08] 遍历目录
来源：http://ufq.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hyt.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wfj.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://wop.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://hyp.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tkm.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ihq.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://qax.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://egv.tarul.cn

[F09] 获取文件大小
来源：http://tkl.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://aeg.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://aey.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://elk.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://euz.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://szp.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbn.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://icx.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://utj.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://vug.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ddi.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qsy.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cxq.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://zcu.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hbk.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ycn.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bdz.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uro.tanke756.top

[F11] 复制与移动文件
来源：http://lnp.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oxp.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ddm.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apj.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hfp.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zxe.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zoz.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://icf.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ycz.chenlongwang.top

[F12] CSV 读写
来源：http://lbp.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bni.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ded.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hoy.hysaishi.cn

TS:   // 同上
来源：http://cqe.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cwh.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ctw.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xbr.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://thj.yfazqb.com

================================================================================
来源：http://hzw.xziqi.cn

G. 面向对象
来源：http://crj.birdmap.top

================================================================================
来源：http://gzw.ppjwa.cn

[G01] 定义类
来源：http://svo.vqdsnc.cn

Py:   class User: pass
来源：http://ivj.shzxlz.cn

PHP:  class User {}
来源：http://tuk.haohaochexian.top

JS:   class User {}
来源：http://mmx.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://lsb.yanxiufei.cn

Java: class User {}
来源：http://zpd.redwolf501.top

Go:   type User struct { Name string }
来源：http://gqf.smart0.xyz

Ruby: class User; end
来源：http://mrl.daria6918.cn

C#:   class User {}
来源：http://umv.shanyushiyangtech.top

[G02] 构造函数
来源：http://jhk.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://vrz.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://tfa.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://jji.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://xqi.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://mjx.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ewq.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://zny.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://lyq.wangshuangyany.cn

[G03] 实例属性
来源：http://jmw.ydzc1.top

Py:   self.name = "x"
来源：http://roc.jinqigufen.top

PHP:  public string $name = "x";
来源：http://djc.dianchejie.cn

JS:   this.name = "x";
来源：http://pyd.sysykeji.top

TS:   name: string = "x";
来源：http://iga.yuxming.cn

Java: private String name;
来源：http://bzh.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzd.cqqwz.cn

Ruby: @name = "x"
来源：http://vym.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://tcs.jlsjyb.cn

[G04] 定义方法
来源：http://ugz.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://wcn.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gyw.bjfxy.top

JS:   greet() { return this.name; }
来源：http://tbm.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://gac.fktsv.cn

Java: String greet() { return name; }
来源：http://kcj.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gwh.sysykeji.top

Ruby: def greet; @name; end
来源：http://yhk.ybcxt.top

C#:   public string Greet() => Name;
来源：http://hsn.pycfn.com

[G05] 继承
来源：http://tlh.dashuyun.cn

Py:   class Admin(User): pass
来源：http://csp.gzhubu.top

PHP:  class Admin extends User {}
来源：http://hbv.aizwys.cn

JS:   class Admin extends User {}
来源：http://ghk.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://icb.chenzaomai.com

Java: class Admin extends User {}
来源：http://xxs.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ddd.52xcode.cn

Ruby: class Admin < User; end
来源：http://hhm.andypj.xyz

C#:   class Admin : User {}
来源：http://pxl.yj20258.top

[G06] 重写方法
来源：http://iog.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://nad.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://udf.ivvv.top

JS:   greet() { return "admin"; }
来源：http://nao.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://nkp.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://qjm.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xnx.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://xas.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://gyp.havefunace.top

[G07] 调用父类方法
来源：http://pii.jyoumei.cn

Py:   super().greet()
来源：http://dqh.yj202588.top

PHP:  parent::greet();
来源：http://wno.kuanghao11.cn

JS:   super.greet();
来源：http://fyn.chenlongwang.top

TS:   super.greet();
来源：http://evw.chenzaomai.com

Java: super.greet();
来源：http://tyv.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pjo.sweek.top

Ruby: super
来源：http://aaa.daria6918.cn

C#:   base.Greet();
来源：http://eca.mhx1999.top

[G08] 静态方法与属性
来源：http://efb.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kdl.jiagoushi.top

PHP:  public static function f() {}
来源：http://fqg.fktsv.cn

JS:   static f() {}
来源：http://igs.ivvv.top

TS:   static f(): void {}
来源：http://mbj.yanxiufei.cn

Java: static void f() {}
来源：http://ecv.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ssf.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://fjf.fktsv.cn

C#:   public static void F() {}
来源：http://zlt.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://rwa.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://pqw.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://trq.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://agl.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://mqr.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://cym.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://nku.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vef.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://dyt.sufxvd.cn

[G10] 访问控制
来源：http://mcm.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://cfv.yongpay.top

PHP:  public / protected / private
来源：http://eos.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://oiz.ivvv.top

TS:   public / protected / private
来源：http://eya.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://aye.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tuz.fengsongda.top

Ruby: public / protected / private
来源：http://xox.daxiang520.top

C#:   public / protected / private / internal
来源：http://bmx.ywan-chungtsiang.top

[G11] getter / setter
来源：http://hbu.fengsongda.top

Py:   @property 与 @x.setter
来源：http://mzc.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vpg.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://qho.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://fxy.daria6918.cn

Java: public String getName() { return name; }
来源：http://kdl.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dnc.iojbl.cn

Ruby: attr_accessor :name
来源：http://utp.birdmap.top

C#:   public string Name { get; set; }
来源：http://mbm.zhiwuduotai.top

[G12] 对象转字符串
来源：http://lxk.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://rxn.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kjy.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://xnn.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://apf.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://syv.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://rww.jianghu66.top

Ruby: def to_s; @name; end
来源：http://xjv.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://uno.gotoacloud.top

[G13] 判断对象类型
来源：http://wtz.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://nuv.svipenyu.cn

PHP:  $u instanceof User
来源：http://mad.shzxlz.cn

JS:   u instanceof User
来源：http://onv.tianlin.xyz

TS:   u instanceof User
来源：http://nkx.wangdashe.top

Java: u instanceof User
来源：http://ifm.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kco.sxryk.cn

Ruby: u.is_a?(User)
来源：http://zff.zhijiandao.cn

C#:   u is User
来源：http://jgw.redwolf501.top

[G14] 数据类 / record
来源：http://mpg.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ovn.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://gcu.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://kds.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://qci.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://zxz.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://qml.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hur.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://jzw.hammf.cn

[G15] 枚举
来源：http://cft.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dzg.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pog.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eee.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wfz.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://xpv.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mwt.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://fdt.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://prf.cashguo.top

[G16] 对象转数组 / 字典
来源：http://vok.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mjw.havefunace.top

PHP:  get_object_vars($obj);
来源：http://zum.pycfn.com

JS:   Object.entries(obj)
来源：http://fqr.chenzaomai.com

TS:   Object.entries(obj)
来源：http://xwr.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hjt.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kkr.nanxinkj.top

Ruby: obj.instance_variables
来源：http://iwd.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://rqd.feifeiyinyue.top

================================================================================
来源：http://xss.zhengqikj.top

H. 异常与错误处理
来源：http://whs.jqgufenzy.top

================================================================================
来源：http://zda.ydzc1.top

[H01] try / catch 基础
来源：http://cpr.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xhk.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hzt.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jtr.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://smb.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wns.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wxm.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dve.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pee.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://zyf.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://unk.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohe.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bsf.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://add.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://ztq.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qjc.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ssc.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://sxn.jqgufenzy.top


<!-- 参考信息 -->