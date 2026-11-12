代发 wailian999

Go:   if s == "" {}
来源：http://ojx.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://dco.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ecn.shzxlz.cn

[E21] 超长截断加省略号
来源：http://yec.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ier.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ayp.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uwo.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnw.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kzp.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://fxm.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dzq.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://shf.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://dvr.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ydy.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cge.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ulh.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://chq.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ykr.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ktc.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://pcj.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mdy.kuanghao11.cn

================================================================================
来源：http://pjj.xylfe.cn

F. 文件与目录
来源：http://mlq.xuanzx.com

================================================================================
来源：http://uil.fzhhl.top

[F01] 读取整个文件
来源：http://cdt.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nkn.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://kpd.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://odz.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dkf.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cxb.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dcf.yj20258888.top

Ruby: File.read("a.txt")
来源：http://lys.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://yhh.tarul.cn

[F02] 逐行读取文件
来源：http://uxh.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wly.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzl.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nup.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swx.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ocq.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rvf.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aek.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pac.ivvv.top

[F03] 写入文件（覆盖）
来源：http://run.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lce.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://rzy.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfc.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ndb.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://img.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jxy.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://cyj.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hvd.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://gez.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qhu.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://psg.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdj.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvy.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vaf.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gib.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zja.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://voq.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://jwm.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zlj.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://gnn.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://dru.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://oru.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://flx.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://coc.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://bhp.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://xai.nanxinkj.top

[F06] 删除文件
来源：http://mbs.yfazqb.com

Py:   os.remove("a.txt")
来源：http://ago.cucudq.cn

PHP:  unlink("a.txt");
来源：http://tmt.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://zfc.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pwt.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yud.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://ega.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://rmy.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://gxk.sweek.top

[F07] 创建目录（含多级）
来源：http://ail.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kvl.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mdt.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jsc.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eky.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mzn.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://spt.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qzy.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://png.fehbvm.com

[F08] 遍历目录
来源：http://nnc.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xco.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://agh.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://hpk.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://hgh.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ljn.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gsa.yonumen.top

Ruby: Dir.children("dir")
来源：http://dou.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://hbs.ppjwa.cn

[F09] 获取文件大小
来源：http://jkh.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://jia.hammf.cn

PHP:  filesize("a.txt");
来源：http://ydj.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://rsv.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://ldp.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fcs.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dvw.bbcook.cn

Ruby: File.size("a.txt")
来源：http://vfe.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://sxb.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://dhu.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uma.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kcy.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kyw.vehdjk.com

TS:   path.extname("a.txt")
来源：http://nxh.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wxk.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uin.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mpy.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qks.xylfe.cn

[F11] 复制与移动文件
来源：http://jjr.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tgd.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://emb.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tbj.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://non.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxw.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kor.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gwm.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qrq.ehwqpu.com

[F12] CSV 读写
来源：http://bqx.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hno.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ldu.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://adf.ctjpmb.com

TS:   // 同上
来源：http://bdc.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gys.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dxj.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qzu.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fvo.xziqi.cn

================================================================================
来源：http://hbj.yj202588.top

G. 面向对象
来源：http://vec.shzxlz.cn

================================================================================
来源：http://orc.gogol.net.cn

[G01] 定义类
来源：http://ets.c1oappe.top

Py:   class User: pass
来源：http://ixg.nanxinkj.top

PHP:  class User {}
来源：http://rhr.havefunace.top

JS:   class User {}
来源：http://noq.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://bvj.wangshuangyany.cn

Java: class User {}
来源：http://jqs.chenzaomai.com

Go:   type User struct { Name string }
来源：http://fhb.epnwcf.com

Ruby: class User; end
来源：http://fba.zhixingplan.top

C#:   class User {}
来源：http://fqo.shanyushiyangkeji.top

[G02] 构造函数
来源：http://ogb.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://pdo.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://opi.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://bni.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://cqo.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://wbh.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kjs.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://lud.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://uny.nanxinkj.top

[G03] 实例属性
来源：http://tlt.nanxuanxn.top

Py:   self.name = "x"
来源：http://xkx.shzxlz.cn

PHP:  public string $name = "x";
来源：http://owz.shzxlz.cn

JS:   this.name = "x";
来源：http://wcf.bjfxy.top

TS:   name: string = "x";
来源：http://jgs.0kj1m.cn

Java: private String name;
来源：http://vrb.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wjo.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://spy.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://roq.wangshuangyany.cn

[G04] 定义方法
来源：http://nqd.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://xgt.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hio.hesvh.cn

JS:   greet() { return this.name; }
来源：http://gdu.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://egb.fktsv.cn

Java: String greet() { return name; }
来源：http://pft.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zrx.cashguo.top

Ruby: def greet; @name; end
来源：http://pdc.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://ljp.yj20258888.top

[G05] 继承
来源：http://kha.mhx1999.top

Py:   class Admin(User): pass
来源：http://hrf.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://ixz.shuidangran.top

JS:   class Admin extends User {}
来源：http://onk.ehwqpu.com

TS:   class Admin extends User {}
来源：http://sxe.zycfv.cn

Java: class Admin extends User {}
来源：http://pjq.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://suw.ivvv.top

Ruby: class Admin < User; end
来源：http://jiu.hywenlv.cn

C#:   class Admin : User {}
来源：http://vac.iojbl.cn

[G06] 重写方法
来源：http://bag.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://leu.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://srt.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://cli.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://ffv.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://qps.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ytx.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://izy.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://uoa.cqqwz.cn

[G07] 调用父类方法
来源：http://sdu.ehwqpu.com

Py:   super().greet()
来源：http://kva.gaohongyu789.top

PHP:  parent::greet();
来源：http://ncf.meibo888.top

JS:   super.greet();
来源：http://zyk.epnwcf.com

TS:   super.greet();
来源：http://dyc.mhx1999.top

Java: super.greet();
来源：http://vvb.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://etg.shzxlz.cn

Ruby: super
来源：http://ebt.dashuyun.cn

C#:   base.Greet();
来源：http://pln.bbcook.cn

[G08] 静态方法与属性
来源：http://hfv.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://peb.hammf.cn

PHP:  public static function f() {}
来源：http://ovz.jinqigufen.top

JS:   static f() {}
来源：http://dii.bbcook.cn

TS:   static f(): void {}
来源：http://ytl.guowangkeji.top

Java: static void f() {}
来源：http://fhl.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gbr.zycfv.cn

Ruby: def self.f; end
来源：http://rkn.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://mmy.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://feg.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://wct.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://wku.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://avr.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://lew.52xcode.cn

Java: interface Shape { double area(); }
来源：http://hvs.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://gay.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lea.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://nab.fehbvm.com

[G10] 访问控制
来源：http://tjh.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://ivb.chenjidiqi.icu

PHP:  public / protected / private
来源：http://ecn.epnwcf.com

JS:   #private 字段；其余公开
来源：http://sky.ydjk.org.cn

TS:   public / protected / private
来源：http://unb.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://vdq.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://apd.xylfe.cn

Ruby: public / protected / private
来源：http://cjk.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://hyg.fehbvm.com

[G11] getter / setter
来源：http://kon.wangdashe.top

Py:   @property 与 @x.setter
来源：http://nvb.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rsf.316326.xyz

JS:   get name() { return this._name; }
来源：http://tdw.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://vpf.haohaochexian.top

Java: public String getName() { return name; }
来源：http://gld.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qja.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://cfj.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://ynm.xuetiantiany.cn

[G12] 对象转字符串
来源：http://ugj.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://trc.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vbs.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://qkx.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://byu.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://mbp.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://lru.epnwcf.com

Ruby: def to_s; @name; end
来源：http://hop.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://guu.kuanghao11.cn

[G13] 判断对象类型
来源：http://kzy.cucudq.cn

Py:   isinstance(u, User)
来源：http://ttt.tianlin.xyz

PHP:  $u instanceof User
来源：http://pvb.ybcxt.top

JS:   u instanceof User
来源：http://vtm.pengpengdd.cyou

TS:   u instanceof User
来源：http://fkz.shanyushiyangkeji.top

Java: u instanceof User
来源：http://bjv.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zxq.ivvv.top

Ruby: u.is_a?(User)
来源：http://mwy.tianlin.xyz

C#:   u is User
来源：http://dtm.hysaishi.cn

[G14] 数据类 / record
来源：http://qzf.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jke.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://slr.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://nly.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://aac.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://git.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://ght.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://izt.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://ujf.hongshengwenyu.top

[G15] 枚举
来源：http://ndg.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khi.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://szs.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pdr.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wvs.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://qoa.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gzu.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://plc.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fvf.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://wui.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ntt.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://tmx.sufxvd.cn

JS:   Object.entries(obj)
来源：http://jok.bbcook.cn

TS:   Object.entries(obj)
来源：http://umu.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://edz.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kth.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://hzx.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://rbx.nwbrower.top

================================================================================
来源：http://oyd.mhx1999.top

H. 异常与错误处理
来源：http://fer.yj20258888.top

================================================================================
来源：http://emp.ybcxt.top

[H01] try / catch 基础
来源：http://crr.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qhf.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojl.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yfi.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vsm.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fgs.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqv.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fxt.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vng.hnqzz.top

[H02] finally / ensure 收尾
来源：http://fyx.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cwk.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bkt.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hdp.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ruc.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aug.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://crp.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jmk.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ssp.redwolf501.top


<!-- 参考信息 -->