代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dhn.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yaj.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmn.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gav.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://egs.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://pzs.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zjx.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vwz.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://zdi.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://igv.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlh.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pof.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjj.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gur.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksc.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://slb.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tyz.cashguo.top

================================================================================
来源：http://tgr.chenlongwang.top

F. 文件与目录
来源：http://xfk.aizwys.cn

================================================================================
来源：http://taz.jiagoushi.top

[F01] 读取整个文件
来源：http://rhf.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kgt.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://brs.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aby.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://awq.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sdu.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hvc.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://mcf.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://nnw.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://xtl.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jvi.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rhu.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpe.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fqp.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fws.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sjq.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://isz.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kbv.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://ndj.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kal.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wdd.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ncj.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xup.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wmj.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://owe.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://wtv.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xbs.hywenlv.cn

[F04] 追加写入文件
来源：http://qdf.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://chz.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sec.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjh.jinyuanbaomall.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sxq.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hfb.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://asz.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zsg.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzs.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://uwn.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kgr.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://hma.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://var.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://hdz.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kdz.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tdi.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://ucu.uphjek.com

C#:   File.Exists("a.txt")
来源：http://eta.cucudq.cn

[F06] 删除文件
来源：http://lsl.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://nhu.daria6918.cn

PHP:  unlink("a.txt");
来源：http://azk.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eue.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ojn.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yfh.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://jzd.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://myi.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://oqb.ybcxt.top

[F07] 创建目录（含多级）
来源：http://wpt.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://neb.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dlv.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pio.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qrk.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ulh.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://arq.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nkd.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://law.hcnkem.com

[F08] 遍历目录
来源：http://igo.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lss.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mno.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://ouf.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://gxi.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xat.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ppz.xuanzx.com

Ruby: Dir.children("dir")
来源：http://cvb.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://wcg.chenjidiqi.icu

[F09] 获取文件大小
来源：http://qtg.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://syk.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://qid.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://ucj.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://gus.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://wrb.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ihm.tarul.cn

Ruby: File.size("a.txt")
来源：http://dbf.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://twf.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://bwq.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aas.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qty.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oja.fzhhl.top

TS:   path.extname("a.txt")
来源：http://dvu.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oia.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xdd.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klb.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://umg.kuanghao11.cn

[F11] 复制与移动文件
来源：http://gqd.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://afo.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qys.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ldy.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dri.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nqq.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ibd.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mli.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ycg.cheryme.top

[F12] CSV 读写
来源：http://dbv.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zmz.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ued.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aon.xuetiantiany.cn

TS:   // 同上
来源：http://mth.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rec.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iyb.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tmu.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gfy.zhiwuduotai.top

================================================================================
来源：http://vgc.cqqwz.cn

G. 面向对象
来源：http://qvh.jinghuilouyu.cn

================================================================================
来源：http://qrm.epnwcf.com

[G01] 定义类
来源：http://jbz.chenjidiqi.icu

Py:   class User: pass
来源：http://hcf.vqdsnc.cn

PHP:  class User {}
来源：http://vbd.bbcook.cn

JS:   class User {}
来源：http://cnn.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://szh.cheryme.top

Java: class User {}
来源：http://yzy.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://rim.jqgufenzy.top

Ruby: class User; end
来源：http://bgo.guannengcc.top

C#:   class User {}
来源：http://rha.zdqjudy.top

[G02] 构造函数
来源：http://cnn.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://yqz.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://tyr.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://qfo.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://noa.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://wmd.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://acy.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://qcn.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://btm.sweek.top

[G03] 实例属性
来源：http://gvm.gzhubu.top

Py:   self.name = "x"
来源：http://set.zycfv.cn

PHP:  public string $name = "x";
来源：http://tuo.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://llw.sufxvd.cn

TS:   name: string = "x";
来源：http://wfk.shzxlz.cn

Java: private String name;
来源：http://lif.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ubm.ybcxt.top

Ruby: @name = "x"
来源：http://zcb.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://mfp.guannengcc.top

[G04] 定义方法
来源：http://odn.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://csa.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wcp.nwbrower.top

JS:   greet() { return this.name; }
来源：http://nav.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://zxp.cheryme.top

Java: String greet() { return name; }
来源：http://bew.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vix.tarul.cn

Ruby: def greet; @name; end
来源：http://xfq.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://bgj.yuanzhike.top

[G05] 继承
来源：http://pbe.snrcjt.cn

Py:   class Admin(User): pass
来源：http://iwj.daxiang520.top

PHP:  class Admin extends User {}
来源：http://kin.gotoacloud.top

JS:   class Admin extends User {}
来源：http://eiq.tarul.cn

TS:   class Admin extends User {}
来源：http://erm.cheryme.top

Java: class Admin extends User {}
来源：http://vbj.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wgq.xziqi.cn

Ruby: class Admin < User; end
来源：http://byw.sweek.top

C#:   class Admin : User {}
来源：http://gob.shangyingyoupin.top

[G06] 重写方法
来源：http://grf.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://dud.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yqi.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://juo.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://bkg.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://myk.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jbu.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://hfm.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://gqf.aizwys.cn

[G07] 调用父类方法
来源：http://ttj.52xcode.cn

Py:   super().greet()
来源：http://aki.bjfxy.top

PHP:  parent::greet();
来源：http://ict.cucudq.cn

JS:   super.greet();
来源：http://jqq.yvedp.cn

TS:   super.greet();
来源：http://umm.yueranfly.top

Java: super.greet();
来源：http://epa.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ssz.52xcode.cn

Ruby: super
来源：http://ctk.gzhubu.top

C#:   base.Greet();
来源：http://vwb.cucudq.cn

[G08] 静态方法与属性
来源：http://wnj.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://omh.jqgufenzy.top

PHP:  public static function f() {}
来源：http://por.ywan-chungtsiang.top

JS:   static f() {}
来源：http://zyp.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://vvw.haohaochexian.top

Java: static void f() {}
来源：http://bdh.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ufg.redwolf501.top

Ruby: def self.f; end
来源：http://ovg.guowangkeji.top

C#:   public static void F() {}
来源：http://hve.shuidangran.top

[G09] 接口 / 抽象类
来源：http://ddf.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://rbr.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://uyy.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dpy.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://xfu.bjfxy.top

Java: interface Shape { double area(); }
来源：http://fyg.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://pvr.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbj.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://kfj.hysaishi.cn

[G10] 访问控制
来源：http://efc.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://chr.jinqigfzy.top

PHP:  public / protected / private
来源：http://omz.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://wid.c1oappe.top

TS:   public / protected / private
来源：http://axr.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://rai.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xal.cucudq.cn

Ruby: public / protected / private
来源：http://qgu.cheryme.top

C#:   public / protected / private / internal
来源：http://krw.yangfankeji.com

[G11] getter / setter
来源：http://jbk.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://mfw.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pks.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://qux.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://oti.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://sra.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vjd.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://mha.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://byq.xinyue.icu

[G12] 对象转字符串
来源：http://lqm.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://xip.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://smb.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://knb.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://rjx.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://bhz.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://qpm.jianghu66.top

Ruby: def to_s; @name; end
来源：http://iws.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://ezt.aizwys.cn

[G13] 判断对象类型
来源：http://ptx.sxryk.cn

Py:   isinstance(u, User)
来源：http://wvn.tanke756.top

PHP:  $u instanceof User
来源：http://jfp.fanxiaobao.xyz

JS:   u instanceof User
来源：http://efb.zycfv.cn

TS:   u instanceof User
来源：http://nmd.iojbl.cn

Java: u instanceof User
来源：http://hre.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqo.xuanzx.com

Ruby: u.is_a?(User)
来源：http://wgj.xinyue.icu

C#:   u is User
来源：http://dth.yangfankeji.com

[G14] 数据类 / record
来源：http://ioe.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sry.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://rme.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://enh.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://euc.nwbrower.top

Java: record User(String name, int age) {}
来源：http://quk.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://xhf.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cdw.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://yfy.cdnleiting.top

[G15] 枚举
来源：http://tyf.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wgz.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pna.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aax.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdd.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://oth.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://owe.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://msw.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pjm.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://jcl.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vir.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://mok.chenzaomai.com

JS:   Object.entries(obj)
来源：http://buh.fehbvm.com

TS:   Object.entries(obj)
来源：http://hxm.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uiq.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yum.shuidangran.top

Ruby: obj.instance_variables
来源：http://pby.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://gxj.vehdjk.com

================================================================================
来源：http://xqu.sweek.top

H. 异常与错误处理
来源：http://hlq.hammf.cn

================================================================================
来源：http://dky.chenzaomai.com

[H01] try / catch 基础
来源：http://gpr.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xin.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gnn.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xwl.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ggu.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oym.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://alb.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yni.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sng.uphjek.com

[H02] finally / ensure 收尾
来源：http://hqa.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://bih.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ixn.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xaf.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fbx.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oya.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qul.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yso.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tfo.ybcxt.top

[H03] 主动抛出异常
来源：http://krv.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://njl.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uno.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://fqz.zhengqikj.top


<!-- 参考信息 -->