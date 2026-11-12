代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gnm.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rgk.fktsv.cn

TS:   if (s === "") {}
来源：http://tus.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://fky.jyoumei.cn

Go:   if s == "" {}
来源：http://enk.tanke756.top

Ruby: if s.empty?
来源：http://nsh.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lor.hfpthk.cn

[E21] 超长截断加省略号
来源：http://dzo.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vsg.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wvw.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hiq.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tmb.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ica.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://hhf.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yul.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ert.xuanzx.com

[E22] 字节长度与字符长度
来源：http://yuf.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hcn.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ini.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nmr.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rtd.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wru.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bzl.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://zpc.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vyw.ppjwa.cn

================================================================================
来源：http://vlz.nanxuanxn.top

F. 文件与目录
来源：http://xdx.jinqigfzy.top

================================================================================
来源：http://qwn.hnqzz.top

[F01] 读取整个文件
来源：http://vzc.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxa.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://qga.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hyx.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sos.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gof.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iya.vehdjk.com

Ruby: File.read("a.txt")
来源：http://qfi.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://zwq.ppjwa.cn

[F02] 逐行读取文件
来源：http://veo.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xcu.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wsr.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqp.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnx.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tap.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ftm.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://meq.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://myn.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://kaj.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lja.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fxo.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lvp.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://csq.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xfi.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://htx.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://amh.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vqp.9152youxi.cn

[F04] 追加写入文件
来源：http://vwe.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jpi.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kwr.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npw.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vii.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://chq.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rar.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mds.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jnz.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://mxg.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mne.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://iho.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://vtd.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://hqz.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dxx.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xbe.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://xvw.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://hfu.zhixingplan.top

[F06] 删除文件
来源：http://esq.52xcode.cn

Py:   os.remove("a.txt")
来源：http://gak.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://wha.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://del.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://nvp.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wwp.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://uvr.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://buo.tanke756.top

C#:   File.Delete("a.txt");
来源：http://pnh.hesvh.cn

[F07] 创建目录（含多级）
来源：http://ywn.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://stx.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ppf.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yit.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfo.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jvo.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rgv.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://neq.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nyq.jqgfzy.top

[F08] 遍历目录
来源：http://iqr.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fvw.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lcw.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://fhz.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://mtm.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xoa.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://whq.yj20258888.top

Ruby: Dir.children("dir")
来源：http://igq.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://guk.redwolf501.top

[F09] 获取文件大小
来源：http://rol.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://gqz.sysykeji.top

PHP:  filesize("a.txt");
来源：http://xvy.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://ueq.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://ipm.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gbg.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bhz.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://sbm.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://myk.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://bxb.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dbx.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pio.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ozr.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://equ.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxl.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://orn.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dvc.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://quu.fzhhl.top

[F11] 复制与移动文件
来源：http://ywg.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zup.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xfe.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pgs.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hrc.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zvo.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lzt.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rkr.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hrn.sxryk.cn

[F12] CSV 读写
来源：http://bgc.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qov.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://trx.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://amf.tianlin.xyz

TS:   // 同上
来源：http://aug.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cyu.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tdg.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cyr.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ejw.yuanzhike.top

================================================================================
来源：http://euz.yj202588.top

G. 面向对象
来源：http://hli.ppjwa.cn

================================================================================
来源：http://qth.jqgfzy.top

[G01] 定义类
来源：http://vpt.cucudq.cn

Py:   class User: pass
来源：http://gsq.gotoacloud.top

PHP:  class User {}
来源：http://arr.bjfxy.top

JS:   class User {}
来源：http://uzr.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://byp.xingfuxueyuan.xyz

Java: class User {}
来源：http://xxe.pycfn.com

Go:   type User struct { Name string }
来源：http://jkg.vqdsnc.cn

Ruby: class User; end
来源：http://xrw.dianchejie.cn

C#:   class User {}
来源：http://ltr.cqqwz.cn

[G02] 构造函数
来源：http://ngo.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xfl.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://thq.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://kzh.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://geh.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://coe.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bny.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://cbu.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://hut.cqqwz.cn

[G03] 实例属性
来源：http://bhb.jiagoushi.top

Py:   self.name = "x"
来源：http://jxd.dianchejie.cn

PHP:  public string $name = "x";
来源：http://yfu.hywenlv.cn

JS:   this.name = "x";
来源：http://mao.cdnleiting.top

TS:   name: string = "x";
来源：http://mmo.gogol.net.cn

Java: private String name;
来源：http://twy.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://isk.svipenyu.cn

Ruby: @name = "x"
来源：http://jlz.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://qwu.ivvv.top

[G04] 定义方法
来源：http://ywa.pycfn.com

Py:   def greet(self): return self.name
来源：http://rfm.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zxg.zycfv.cn

JS:   greet() { return this.name; }
来源：http://kcv.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://sau.yonumen.top

Java: String greet() { return name; }
来源：http://luz.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lbb.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://tjf.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://eig.jinqigfzy.top

[G05] 继承
来源：http://buh.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://bye.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://jws.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://kzu.iojbl.cn

TS:   class Admin extends User {}
来源：http://jvf.yj20258888.top

Java: class Admin extends User {}
来源：http://svz.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wkl.hywenlv.cn

Ruby: class Admin < User; end
来源：http://pie.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://woj.aibaodan.cn

[G06] 重写方法
来源：http://lmc.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://iap.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wcr.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://kjg.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://rfp.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://ymj.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ufm.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://uqn.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://fbx.yanxiufei.cn

[G07] 调用父类方法
来源：http://ofm.hnxiangtu.top

Py:   super().greet()
来源：http://ryr.meibo888.top

PHP:  parent::greet();
来源：http://kuw.yueranfly.top

JS:   super.greet();
来源：http://pdw.dianchejie.cn

TS:   super.greet();
来源：http://qur.chenlongwang.top

Java: super.greet();
来源：http://dbj.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vtx.ppjwa.cn

Ruby: super
来源：http://sqh.dianchejie.cn

C#:   base.Greet();
来源：http://okg.hywenlv.cn

[G08] 静态方法与属性
来源：http://lbb.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tel.chenlongwang.top

PHP:  public static function f() {}
来源：http://ajq.ivvv.top

JS:   static f() {}
来源：http://pwy.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://dqg.ydzc1.top

Java: static void f() {}
来源：http://gpw.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hse.smart0.xyz

Ruby: def self.f; end
来源：http://hpc.chenlongwang.top

C#:   public static void F() {}
来源：http://bdd.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://gqk.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://fcc.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://chx.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://srh.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://auz.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://nvp.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://vjs.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fps.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://idm.chenzaomai.com

[G10] 访问控制
来源：http://dtr.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://jth.bjfxy.top

PHP:  public / protected / private
来源：http://voc.shuidangran.top

JS:   #private 字段；其余公开
来源：http://tml.fanxiaobao.xyz

TS:   public / protected / private
来源：http://oih.316326.xyz

Java: public / protected / private / 默认包级
来源：http://ojr.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://alz.andypj.xyz

Ruby: public / protected / private
来源：http://ira.vehdjk.com

C#:   public / protected / private / internal
来源：http://vix.ppjwa.cn

[G11] getter / setter
来源：http://txb.hnqzz.top

Py:   @property 与 @x.setter
来源：http://geh.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zyz.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://oge.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://nzi.ehwqpu.com

Java: public String getName() { return name; }
来源：http://gil.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wfw.vehdjk.com

Ruby: attr_accessor :name
来源：http://cdo.xuanzx.com

C#:   public string Name { get; set; }
来源：http://cxu.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://fia.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://djf.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ptc.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://dnk.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://yib.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://big.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gkq.c1oappe.top

Ruby: def to_s; @name; end
来源：http://ehb.ivvv.top

C#:   public override string ToString() => Name;
来源：http://iqj.ehwqpu.com

[G13] 判断对象类型
来源：http://tjv.sweek.top

Py:   isinstance(u, User)
来源：http://gpd.sweek.top

PHP:  $u instanceof User
来源：http://cjm.dianchejie.cn

JS:   u instanceof User
来源：http://tjb.jyoumei.cn

TS:   u instanceof User
来源：http://hvy.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://ili.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zfn.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://lsb.zhoulong.xyz

C#:   u is User
来源：http://qfj.xziqi.cn

[G14] 数据类 / record
来源：http://rtv.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://njv.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://qte.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yov.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://nvt.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://ati.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://knq.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yib.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://ewk.redwolf501.top

[G15] 枚举
来源：http://yak.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whe.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://svi.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ges.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ezs.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://vxy.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nmz.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://otj.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zsw.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://tev.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oym.uphjek.com

PHP:  get_object_vars($obj);
来源：http://kor.jyoumei.cn

JS:   Object.entries(obj)
来源：http://ahr.316326.xyz

TS:   Object.entries(obj)
来源：http://uri.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qeo.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://own.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://ymi.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://hgg.316326.xyz

================================================================================
来源：http://rgy.haohaochexian.top

H. 异常与错误处理
来源：http://xgb.zhaomingkeji.xyz

================================================================================
来源：http://xze.ydzc1.top

[H01] try / catch 基础
来源：http://oqo.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sog.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uui.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rar.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ggz.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ray.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ptq.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nmo.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dhh.jyoumei.cn

[H02] finally / ensure 收尾
来源：http://jvv.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://uga.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://urk.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hui.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kpm.jqgfzy.top


<!-- 参考信息 -->