代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isw.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://spu.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mas.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bvd.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pob.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://nyn.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yuq.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dfj.sweek.top

[E22] 字节长度与字符长度
来源：http://pyu.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vud.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cbd.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kdw.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjw.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofn.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mfa.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://hbg.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zqg.sweek.top

================================================================================
来源：http://cxy.xingfuxueyuan.xyz

F. 文件与目录
来源：http://axk.chenzaomai.com

================================================================================
来源：http://cpv.yj202588.top

[F01] 读取整个文件
来源：http://bwv.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dvz.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://wxh.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://puz.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kxa.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bcv.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fiz.sxryk.cn

Ruby: File.read("a.txt")
来源：http://qjq.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://yvh.iojbl.cn

[F02] 逐行读取文件
来源：http://zmk.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ztz.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ijm.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhy.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yix.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kck.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bdy.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ncv.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rab.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://nom.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jel.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tpg.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bvv.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ptj.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rpz.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mjf.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://mug.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vpv.vehdjk.com

[F04] 追加写入文件
来源：http://tmi.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://unm.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kby.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hep.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nof.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fqj.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lel.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bti.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://toy.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://sik.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wim.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://ldo.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://atj.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://xeb.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bbs.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tkw.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://zrh.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://kox.yangfankeji.com

[F06] 删除文件
来源：http://djm.daxiang520.top

Py:   os.remove("a.txt")
来源：http://yxs.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://iwo.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fqn.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://ubc.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nzu.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://lrt.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://hwq.yj202588.top

C#:   File.Delete("a.txt");
来源：http://twz.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://ent.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jiv.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://whk.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pri.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://klk.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fav.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hmo.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mht.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gpz.fanxiaobao.xyz

[F08] 遍历目录
来源：http://cke.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sep.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xeq.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://osf.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://vtl.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hpm.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vaa.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://hpo.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://woq.gzhubu.top

[F09] 获取文件大小
来源：http://sxe.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://zio.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://xus.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://cin.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://esh.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://yao.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgp.yvedp.cn

Ruby: File.size("a.txt")
来源：http://dhc.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://pts.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://cmi.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bfe.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rxh.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qmk.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://wor.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dzg.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aig.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bcu.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zmd.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://qon.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nes.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcp.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thn.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfr.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tzl.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yef.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zjc.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://txw.yonumen.top

[F12] CSV 读写
来源：http://onl.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zhs.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bjg.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yix.xylfe.cn

TS:   // 同上
来源：http://ytb.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jqs.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fme.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tuf.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sid.fktsv.cn

================================================================================
来源：http://lea.yvedp.cn

G. 面向对象
来源：http://fth.fktsv.cn

================================================================================
来源：http://cuw.iojbl.cn

[G01] 定义类
来源：http://qsh.chenlongwang.top

Py:   class User: pass
来源：http://zte.jinqigfzy.top

PHP:  class User {}
来源：http://zeo.dashuyun.cn

JS:   class User {}
来源：http://abt.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://lju.svipenyu.cn

Java: class User {}
来源：http://zrf.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://jvf.havefunace.top

Ruby: class User; end
来源：http://avm.xuanzx.com

C#:   class User {}
来源：http://dkl.316326.xyz

[G02] 构造函数
来源：http://koa.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://sfo.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://fvu.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://fji.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://xvr.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://uta.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://snr.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://dzd.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://mlp.shanyushiyangtech.top

[G03] 实例属性
来源：http://nbj.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://icz.shuidangran.top

PHP:  public string $name = "x";
来源：http://gto.hywenlv.cn

JS:   this.name = "x";
来源：http://wjr.yj20258.top

TS:   name: string = "x";
来源：http://pqr.xingfuxueyuan.xyz

Java: private String name;
来源：http://vvf.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csy.wangdashe.top

Ruby: @name = "x"
来源：http://fwf.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://ymu.nwbrower.top

[G04] 定义方法
来源：http://eym.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://ixb.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hur.xinyue.icu

JS:   greet() { return this.name; }
来源：http://kji.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://ydb.quarkkingdee.top

Java: String greet() { return name; }
来源：http://gii.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tdz.smart0.xyz

Ruby: def greet; @name; end
来源：http://olr.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://xqb.fanxiaobao.xyz

[G05] 继承
来源：http://nzy.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://fkd.jianghu66.top

PHP:  class Admin extends User {}
来源：http://gjk.9152youxi.cn

JS:   class Admin extends User {}
来源：http://kxt.sxryk.cn

TS:   class Admin extends User {}
来源：http://dhc.daxiang520.top

Java: class Admin extends User {}
来源：http://xxg.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://crg.daria6918.cn

Ruby: class Admin < User; end
来源：http://guw.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://prl.jqgufenzy.top

[G06] 重写方法
来源：http://fik.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://fos.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://slz.birdmap.top

JS:   greet() { return "admin"; }
来源：http://esy.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://sad.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://wzx.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gpb.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://vsz.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://evk.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://nys.yanxiufei.cn

Py:   super().greet()
来源：http://irb.hongshengwenyu.top

PHP:  parent::greet();
来源：http://ctk.jinqigufen.top

JS:   super.greet();
来源：http://jeh.hesvh.cn

TS:   super.greet();
来源：http://lxs.yuxming.cn

Java: super.greet();
来源：http://vcg.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ccq.ywan-chungtsiang.top

Ruby: super
来源：http://uxy.vehdjk.com

C#:   base.Greet();
来源：http://oyt.zhongyouzk.top

[G08] 静态方法与属性
来源：http://ntk.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lcu.zhengqikj.top

PHP:  public static function f() {}
来源：http://lyt.daria6918.cn

JS:   static f() {}
来源：http://vgw.fzhhl.top

TS:   static f(): void {}
来源：http://rcy.aizwys.cn

Java: static void f() {}
来源：http://hzo.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvb.nanxuanxn.top

Ruby: def self.f; end
来源：http://bvm.jyoumei.cn

C#:   public static void F() {}
来源：http://yqa.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://caf.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://lnh.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ijp.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqz.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://jun.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://yxj.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://tnv.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pra.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://oqi.nanxuanxn.top

[G10] 访问控制
来源：http://rkq.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://gqt.birdmap.top

PHP:  public / protected / private
来源：http://xlw.daria6918.cn

JS:   #private 字段；其余公开
来源：http://diw.shanyushiyangtech.top

TS:   public / protected / private
来源：http://nyk.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://zjg.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vxf.c1oappe.top

Ruby: public / protected / private
来源：http://wdq.snrcjt.cn

C#:   public / protected / private / internal
来源：http://xow.shanyushiyangkeji.top

[G11] getter / setter
来源：http://jxt.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://fyb.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xpd.316326.xyz

JS:   get name() { return this._name; }
来源：http://qdo.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://gyv.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://aio.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://wdg.zdqjudy.top

Ruby: attr_accessor :name
来源：http://zxf.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://wql.hnqzz.top

[G12] 对象转字符串
来源：http://ytj.316326.xyz

Py:   def __str__(self): return self.name
来源：http://vgq.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://oec.daxiang520.top

JS:   toString() { return this.name; }
来源：http://mvp.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://gdd.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://rhk.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ntc.epnwcf.com

Ruby: def to_s; @name; end
来源：http://qlq.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://dan.sjlbkw.cn

[G13] 判断对象类型
来源：http://spi.yj202588.top

Py:   isinstance(u, User)
来源：http://tbe.ybcxt.top

PHP:  $u instanceof User
来源：http://lbx.chenjidiqi.icu

JS:   u instanceof User
来源：http://wcs.chenzaomai.com

TS:   u instanceof User
来源：http://fgq.ydjk.org.cn

Java: u instanceof User
来源：http://dbd.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldu.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://loi.gzhubu.top

C#:   u is User
来源：http://dpq.kuanghao11.cn

[G14] 数据类 / record
来源：http://wmu.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iwv.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://yqk.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://xgt.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://mwc.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://yuv.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://wah.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ilj.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://sli.haohaochexian.top

[G15] 枚举
来源：http://kda.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gri.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dgv.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mth.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zon.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://wra.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fhg.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://fsx.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mqe.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://fzs.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uek.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://ciz.yj20258.top

JS:   Object.entries(obj)
来源：http://dxi.yj20258888.top

TS:   Object.entries(obj)
来源：http://war.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hkc.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qdh.yj20258888.top

Ruby: obj.instance_variables
来源：http://cwy.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://dxv.fanxiaobao.xyz

================================================================================
来源：http://bpp.0kj1m.cn

H. 异常与错误处理
来源：http://wwq.tianlin.xyz

================================================================================
来源：http://xdu.ppjwa.cn

[H01] try / catch 基础
来源：http://hgk.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gql.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dac.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aov.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yre.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wue.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hxj.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ine.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqf.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://kiw.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://cqj.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yvv.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://foz.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gzw.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://jqk.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://znn.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bgs.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://gzp.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://hse.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://dzi.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vnj.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://ico.zhijiandao.cn


<!-- 参考信息 -->