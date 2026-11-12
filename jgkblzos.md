代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://lqf.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://bnx.nanxuanxn.top

Java: s.lines().toList()
来源：http://zam.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://lbc.sjlbkw.cn

Ruby: s.lines
来源：http://eum.sufxvd.cn

C#:   s.Split('\n')
来源：http://icb.bjfxy.top

[E20] 判断字符串是否为空
来源：http://yuh.jianghu66.top

Py:   if not s:
来源：http://qqy.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ckm.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ihq.ydjk.org.cn

TS:   if (s === "") {}
来源：http://yqn.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://hyx.yonumen.top

Go:   if s == "" {}
来源：http://uln.haohaochexian.top

Ruby: if s.empty?
来源：http://fch.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpd.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://htr.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lep.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qrx.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eyl.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://otn.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmi.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://olz.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wss.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcf.andypj.xyz

[E22] 字节长度与字符长度
来源：http://mnc.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sqa.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqh.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zya.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ujz.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pfj.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xit.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://xqk.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gnj.yonumen.top

================================================================================
来源：http://pbd.chenjidiqi.icu

F. 文件与目录
来源：http://ngz.havefunace.top

================================================================================
来源：http://bas.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://szg.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://clp.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://xwt.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ajf.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dey.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qqf.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bvq.fengsongda.top

Ruby: File.read("a.txt")
来源：http://btl.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://ebr.tian-w.cn

[F02] 逐行读取文件
来源：http://cmx.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tpt.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rxd.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://exi.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kzw.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://riu.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vcj.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ham.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jjv.yj20258.top

[F03] 写入文件（覆盖）
来源：http://fak.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wst.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yqj.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvb.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sff.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blo.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rbb.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://isb.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wet.guowangkeji.top

[F04] 追加写入文件
来源：http://wws.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kyh.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nwr.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xaw.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tbl.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fxr.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uou.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oxp.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yty.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://zxe.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://toj.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://dys.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://frc.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://edr.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xws.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qum.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://txg.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://erg.iojbl.cn

[F06] 删除文件
来源：http://vzs.zycfv.cn

Py:   os.remove("a.txt")
来源：http://qsd.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://bsa.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://dhc.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://brb.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fyu.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://ugc.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://jvt.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://vml.mhx1999.top

[F07] 创建目录（含多级）
来源：http://mmb.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://llv.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bzr.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgb.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csa.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://znc.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xlc.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zjq.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cfv.guannengcc.top

[F08] 遍历目录
来源：http://ndd.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aui.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wyg.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://fty.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://wld.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hea.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gnw.ybcxt.top

Ruby: Dir.children("dir")
来源：http://kic.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://aqp.wangdashe.top

[F09] 获取文件大小
来源：http://wni.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://bjj.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://viy.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://tbt.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://hwx.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fyu.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://akb.tarul.cn

Ruby: File.size("a.txt")
来源：http://xnr.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://szk.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://pmn.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nwe.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdr.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://thx.daxiang520.top

TS:   path.extname("a.txt")
来源：http://prz.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bxq.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ywc.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lyu.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xtf.gaohongyu789.top

[F11] 复制与移动文件
来源：http://cfw.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://loi.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hxr.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nus.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jio.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://joi.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rtn.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gwe.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://epc.jinqigufen.top

[F12] CSV 读写
来源：http://ahf.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jbo.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://buj.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bwa.nanxinkj.top

TS:   // 同上
来源：http://pws.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dnb.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jjw.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://khh.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qvn.ctjpmb.com

================================================================================
来源：http://ffz.yj20258.top

G. 面向对象
来源：http://law.yj20258.top

================================================================================
来源：http://emx.xziqi.cn

[G01] 定义类
来源：http://ijc.dianchejie.cn

Py:   class User: pass
来源：http://hno.jinyuanbaomall.cn

PHP:  class User {}
来源：http://bwt.yvedp.cn

JS:   class User {}
来源：http://ygt.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://fnl.gogol.net.cn

Java: class User {}
来源：http://odi.ehwqpu.com

Go:   type User struct { Name string }
来源：http://bff.zhongyouzk.top

Ruby: class User; end
来源：http://ryc.yuxming.cn

C#:   class User {}
来源：http://zic.redwolf501.top

[G02] 构造函数
来源：http://iel.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://bbj.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://cnp.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://mqz.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://njn.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://kqt.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xnw.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://bkt.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://yhi.quarkkingdee.top

[G03] 实例属性
来源：http://qza.xylfe.cn

Py:   self.name = "x"
来源：http://bfj.tian-w.cn

PHP:  public string $name = "x";
来源：http://euk.epnwcf.com

JS:   this.name = "x";
来源：http://rgu.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://ucn.jinqigufen.top

Java: private String name;
来源：http://mur.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vuq.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://wmq.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://nnv.cdnleiting.top

[G04] 定义方法
来源：http://baj.andypj.xyz

Py:   def greet(self): return self.name
来源：http://xda.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://mpc.uphjek.com

JS:   greet() { return this.name; }
来源：http://ajc.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://qjg.cqqwz.cn

Java: String greet() { return name; }
来源：http://nio.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://evv.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://grb.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://oyi.zhijiandao.cn

[G05] 继承
来源：http://oib.gotoacloud.top

Py:   class Admin(User): pass
来源：http://yzl.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://mzl.vehdjk.com

JS:   class Admin extends User {}
来源：http://gah.tianlin.xyz

TS:   class Admin extends User {}
来源：http://huq.guowangkeji.top

Java: class Admin extends User {}
来源：http://icf.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hui.gogol.net.cn

Ruby: class Admin < User; end
来源：http://fyu.guannengcc.top

C#:   class Admin : User {}
来源：http://hia.aibaodan.cn

[G06] 重写方法
来源：http://xva.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://gzh.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://avc.hammf.cn

JS:   greet() { return "admin"; }
来源：http://cuf.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://urk.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://hjy.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://scf.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://yit.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://aom.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://qio.shanyushiyangkeji.top

Py:   super().greet()
来源：http://ofc.fzhhl.top

PHP:  parent::greet();
来源：http://rsj.meibo888.top

JS:   super.greet();
来源：http://byl.smart0.xyz

TS:   super.greet();
来源：http://nyl.cheryme.top

Java: super.greet();
来源：http://btk.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xrx.mhx1999.top

Ruby: super
来源：http://bmk.dianchejie.cn

C#:   base.Greet();
来源：http://mco.iojbl.cn

[G08] 静态方法与属性
来源：http://uas.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ltr.ybcxt.top

PHP:  public static function f() {}
来源：http://ure.jinqigufen.top

JS:   static f() {}
来源：http://kjg.snrcjt.cn

TS:   static f(): void {}
来源：http://ulj.sweek.top

Java: static void f() {}
来源：http://oxd.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://vas.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://vff.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://sns.tarul.cn

[G09] 接口 / 抽象类
来源：http://mis.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://vfp.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qiq.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xxm.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://wbt.yj20258.top

Java: interface Shape { double area(); }
来源：http://eih.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://jro.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qxr.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://yja.yj202588.top

[G10] 访问控制
来源：http://gfl.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://vnv.jlsjyb.cn

PHP:  public / protected / private
来源：http://evx.hammf.cn

JS:   #private 字段；其余公开
来源：http://ktm.c1oappe.top

TS:   public / protected / private
来源：http://puq.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://yzc.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bqa.gogol.net.cn

Ruby: public / protected / private
来源：http://fwx.yfazqb.com

C#:   public / protected / private / internal
来源：http://vxd.shanyushiyangkeji.top

[G11] getter / setter
来源：http://ozg.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://hmy.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mve.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://pnf.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://uvw.jqgfzy.top

Java: public String getName() { return name; }
来源：http://ovc.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvt.hcnkem.com

Ruby: attr_accessor :name
来源：http://zas.hammf.cn

C#:   public string Name { get; set; }
来源：http://lvw.xylfe.cn

[G12] 对象转字符串
来源：http://cit.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://svr.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zbp.uphjek.com

JS:   toString() { return this.name; }
来源：http://imo.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://hkx.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://uak.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://kme.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://qbx.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://faw.snrcjt.cn

[G13] 判断对象类型
来源：http://yba.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://alt.gogol.net.cn

PHP:  $u instanceof User
来源：http://wqd.pycfn.com

JS:   u instanceof User
来源：http://gmd.pengpengdd.cyou

TS:   u instanceof User
来源：http://bnr.svipenyu.cn

Java: u instanceof User
来源：http://ixi.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://woh.jianghu66.top

Ruby: u.is_a?(User)
来源：http://azp.xuanzx.com

C#:   u is User
来源：http://aus.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://vfe.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ita.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://vxs.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://qzv.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://nkm.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://fmv.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://yhv.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qnj.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://jgt.zhongyouzk.top

[G15] 枚举
来源：http://imy.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bos.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://lew.snrcjt.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nox.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://upn.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://kiu.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ydw.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://win.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mem.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://sao.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qzg.havefunace.top

PHP:  get_object_vars($obj);
来源：http://hgl.birdmap.top

JS:   Object.entries(obj)
来源：http://ite.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://prp.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://drv.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xlz.ehwqpu.com

Ruby: obj.instance_variables
来源：http://rom.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://ghp.xuanzx.com

================================================================================
来源：http://pnk.hammf.cn

H. 异常与错误处理
来源：http://uni.xuanzx.com

================================================================================
来源：http://xvs.jinqigfzy.top

[H01] try / catch 基础
来源：http://wcm.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jgf.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qhc.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyo.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fra.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://azt.shangyingyoupin.top


<!-- 参考信息 -->