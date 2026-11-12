代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://grx.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ewf.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qat.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tjs.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://msu.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://rit.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gks.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://icv.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://zcb.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://neq.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hlw.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vok.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://woo.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyf.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sca.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://wey.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fuf.yuanzhike.top

================================================================================
来源：http://oqu.yj20258.top

F. 文件与目录
来源：http://jpz.jinyuanbaomall.cn

================================================================================
来源：http://mlm.316326.xyz

[F01] 读取整个文件
来源：http://rwp.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cyo.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://ioa.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://avk.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uyj.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lbf.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jcz.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://row.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://xdx.hysaishi.cn

[F02] 逐行读取文件
来源：http://ygp.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jpa.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kgc.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhd.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://way.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dte.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqa.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xwc.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tvw.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://nhh.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mrz.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qxh.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bes.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpo.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cgt.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hkq.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://frl.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://etz.ctjpmb.com

[F04] 追加写入文件
来源：http://syd.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjl.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://orv.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zhr.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cpy.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tbl.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lpa.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cvm.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pvu.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://cbp.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gpm.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://epk.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://qxw.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://hcu.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://isy.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pbj.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://jnn.ivvv.top

C#:   File.Exists("a.txt")
来源：http://znj.smart0.xyz

[F06] 删除文件
来源：http://hka.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://dtd.xziqi.cn

PHP:  unlink("a.txt");
来源：http://blw.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ran.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vfh.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://csl.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://ibx.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://itr.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://qox.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://kcm.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpc.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nlu.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tkm.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kig.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aba.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ouk.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kar.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gll.mhx1999.top

[F08] 遍历目录
来源：http://qfc.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ynd.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nht.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://eyr.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://ukn.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yhf.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ilo.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://thd.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://qay.jlsjyb.cn

[F09] 获取文件大小
来源：http://txe.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://fup.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://alu.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://yer.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://isf.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://zxv.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ndo.yonumen.top

Ruby: File.size("a.txt")
来源：http://pnx.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://ayo.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://tnt.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rhl.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bej.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kha.yfazqb.com

TS:   path.extname("a.txt")
来源：http://alk.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gny.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yrc.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kol.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://djb.jyoumei.cn

[F11] 复制与移动文件
来源：http://fiq.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uir.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xtm.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ksu.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eub.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://grp.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmy.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qgq.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://afp.jinqigufen.top

[F12] CSV 读写
来源：http://gzt.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ssf.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nri.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tis.shanyushiyangkeji.top

TS:   // 同上
来源：http://dhw.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nyl.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iwp.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tre.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yol.sweek.top

================================================================================
来源：http://nmd.yj202588.top

G. 面向对象
来源：http://wfm.sweek.top

================================================================================
来源：http://vet.hcnkem.com

[G01] 定义类
来源：http://ncl.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://sgk.yueranfly.top

PHP:  class User {}
来源：http://jyc.cashguo.top

JS:   class User {}
来源：http://ksk.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://pkg.ctjpmb.com

Java: class User {}
来源：http://pln.yvedp.cn

Go:   type User struct { Name string }
来源：http://drm.iojbl.cn

Ruby: class User; end
来源：http://bbo.guowangkeji.top

C#:   class User {}
来源：http://gnl.zhongyouzk.top

[G02] 构造函数
来源：http://lbk.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://fjg.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://lxg.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://kny.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://yxy.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://tqo.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ofu.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://ekl.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://qxb.pengpengdd.cyou

[G03] 实例属性
来源：http://ihp.52xcode.cn

Py:   self.name = "x"
来源：http://tcr.dashuyun.cn

PHP:  public string $name = "x";
来源：http://ind.c1oappe.top

JS:   this.name = "x";
来源：http://dwd.xuanzx.com

TS:   name: string = "x";
来源：http://opv.xinyue.icu

Java: private String name;
来源：http://gzb.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pcv.fehbvm.com

Ruby: @name = "x"
来源：http://ltf.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://xsv.snrcjt.cn

[G04] 定义方法
来源：http://ycx.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://jlj.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uqa.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://eyg.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://lax.xziqi.cn

Java: String greet() { return name; }
来源：http://afw.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://toh.yvedp.cn

Ruby: def greet; @name; end
来源：http://gkl.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://jsg.sysykeji.top

[G05] 继承
来源：http://vwk.yfazqb.com

Py:   class Admin(User): pass
来源：http://sdg.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://abx.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://gqb.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://yvu.fktsv.cn

Java: class Admin extends User {}
来源：http://yzn.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rme.yuanzhike.top

Ruby: class Admin < User; end
来源：http://giv.meibo888.top

C#:   class Admin : User {}
来源：http://knu.meibo888.top

[G06] 重写方法
来源：http://ujp.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://meq.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zpe.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://erx.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://cty.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://zhx.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oxl.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://jcb.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://lcv.zhongyouzk.top

[G07] 调用父类方法
来源：http://ger.cucudq.cn

Py:   super().greet()
来源：http://ydn.jlsjyb.cn

PHP:  parent::greet();
来源：http://ezs.zycfv.cn

JS:   super.greet();
来源：http://nys.yangfankeji.com

TS:   super.greet();
来源：http://jue.cqqwz.cn

Java: super.greet();
来源：http://mbt.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnj.jqgufenzy.top

Ruby: super
来源：http://mox.chenlongwang.top

C#:   base.Greet();
来源：http://tke.wangdashe.top

[G08] 静态方法与属性
来源：http://mem.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zcv.sweek.top

PHP:  public static function f() {}
来源：http://prc.c1oappe.top

JS:   static f() {}
来源：http://wpe.iojbl.cn

TS:   static f(): void {}
来源：http://kqg.ydzc1.top

Java: static void f() {}
来源：http://mdy.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vcc.havefunace.top

Ruby: def self.f; end
来源：http://tnx.iojbl.cn

C#:   public static void F() {}
来源：http://ffn.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://mey.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://ykx.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://jxw.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhb.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://vmd.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://ksy.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://aqs.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oix.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://jie.yvedp.cn

[G10] 访问控制
来源：http://kiq.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://jrz.jyoumei.cn

PHP:  public / protected / private
来源：http://yun.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://fqp.snrcjt.cn

TS:   public / protected / private
来源：http://vyj.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://ail.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wcc.feifeiyinyue.top

Ruby: public / protected / private
来源：http://ffl.smart0.xyz

C#:   public / protected / private / internal
来源：http://bam.daxiang520.top

[G11] getter / setter
来源：http://vxh.uphjek.com

Py:   @property 与 @x.setter
来源：http://gri.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iyc.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://fcd.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://tpv.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://xeo.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwb.jiagoushi.top

Ruby: attr_accessor :name
来源：http://ykj.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://ryp.wangshuangyany.cn

[G12] 对象转字符串
来源：http://bqm.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://dii.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gee.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://dvf.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://ovi.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://llq.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://ulq.yonumen.top

Ruby: def to_s; @name; end
来源：http://uuv.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://kms.sweek.top

[G13] 判断对象类型
来源：http://isg.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://nfk.c1oappe.top

PHP:  $u instanceof User
来源：http://wen.mhx1999.top

JS:   u instanceof User
来源：http://leb.yj202588.top

TS:   u instanceof User
来源：http://xds.gogol.net.cn

Java: u instanceof User
来源：http://ebd.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ksf.ydzc1.top

Ruby: u.is_a?(User)
来源：http://xud.shangyingyoupin.top

C#:   u is User
来源：http://hhp.zhengqikj.top

[G14] 数据类 / record
来源：http://ngc.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nbu.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://ajx.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://erg.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://hah.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://gys.hammf.cn

Go:   type User struct { Name string; Age int }
来源：http://gir.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zra.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://tfi.tanke756.top

[G15] 枚举
来源：http://ehw.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ggm.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iky.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uhx.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hkq.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://wkh.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ypt.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://hox.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wig.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://jxl.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hrl.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://nrt.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://elm.gotoacloud.top

TS:   Object.entries(obj)
来源：http://bds.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fyf.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivn.wangdashe.top

Ruby: obj.instance_variables
来源：http://ewd.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://adb.zycfv.cn

================================================================================
来源：http://gck.zhongyouzk.top

H. 异常与错误处理
来源：http://yrh.fzhhl.top

================================================================================
来源：http://ddu.chenzaomai.com

[H01] try / catch 基础
来源：http://mpw.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jxj.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lsv.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nmg.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://von.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwa.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xen.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uqr.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nxy.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://ruv.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oin.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vtn.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lfy.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ogj.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://wdn.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gtw.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lsa.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://czi.yj20258888.top

[H03] 主动抛出异常
来源：http://zpc.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://tal.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pyl.yongpay.top

JS:   throw new Error("错误信息");
来源：http://xnc.xylfe.cn


<!-- 参考信息 -->